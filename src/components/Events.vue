<template>
    <div>
        <!-- The template code here -->
         <!-- The button below will only be clickable once -->
         <button @click.once="doThis">Submit just once</button>
         
         <!-- The click event propagation will be stopped -->
         <a @click.stop="doThis">Stop the click event propagation</a>

         <!-- The Submit event will no longer reload the page -->
         <form @submit.prevent="onSubmit">The Submit event will not reload page</form>

          <!-- The Modifier can be chained -->
         <a @click.stop.prevent="doSomeThing">Modifier can be chained</a>


         <!-- Keys can be used to listen to specific keys -->
          <!-- Also call the Onsubmit when the 'key' is 'Enter' -->
          <input @keyup.enter="onSubmit">
           
          <!-- Combining with the system keys modifiers -->

          <!-- Alt + Enter will clear the input field -->
           <input @keyup.alt.enter="clear">


           <!-- Ctrl + Click  -->
            <div @click.ctrl="doSomeThing">Do Something</div>
    </div>
</template>