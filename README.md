# Presentation Vue.js
***
#### slide №1
## About Vue.js
Today I want to tell about js framework VUE
***
#### slide №2
The Creator Of Vue.js is Evan You, an employee of Google. 
He began to develop the framework in 2013, and in February 2014 the first public release took place.
At the end of September 2016 was released Vue.js 2.0
The latest version of the program to date 2.6.10
***
#### slide №3
## Simple example
- creates a new view instance via new Vue 
- in el, we define which element is monitored by the view 
- in data, we have a state object

in html we have an element with the selector 
we need data from the state 
we associate the input with the message value of the state object using the v-model Directive
***
#### slide №4
## The Concept Of Vue.js
- Constructor
- Components
- Directives
- Transitions
***
#### slide №5-6
## Constructor
Working with Vue.js begins by creating a new instance of new Vue. In el, we have an element that is monitored by Vue. In template selected (or registered inline) element where Vue will render. Data stores the current state of the instance, and the calculated method provides us with calculated properties.
#### slide №7-8
Vue lifecycle methods
The following custom methods and Vue lifecycle methods can be distinguished in methods: 
1.	beforeCreate — looking data and initialisere events 
2.	created — see if there is an el or template. If there is, render in them; if not, look for the render method 
3.	beforeMount — creates a vm.$el and replaces it with el 
4.	mounted — element rendered 
When the state changes: 
5.	beforeUpdate — again renders VDOM and compares it with the real DOM, applies changes 
6.	updated — changes are rendered 
7.	beforeDestroy — the complete dismantling of the watcher, the internal components and event listeners 
8.	destroyed — called when the operation is stopped
***
#### slide №9-10
## Components
Components help extend basic html elements and embed reusable code. Essentially, components are reusable parts of the UI. 
During the design phase, we break our application into independent parts and obtain a tree structure of the components.
***
#### slide №11
## Directives 
Directives — special attributes to add additional functionality to html elements. 
All Vue directives are prefixed with “v-”. A state value is passed to the Directive, and html attributes or events can be arguments.
Consider some built-in directives (who worked with Angular, to they seem very familiar):
-	V-bind — dynamically binds to one or more attributes. 
-	v-if — condition for element rendering 
-	V-for — loops an array of objects The V-model associates a condition with input element 
-	V-on — connects the event listener to the element 
-	V-show — toggles element visibility by changing the CSS display property 
***
#### slide №12
## Transitions
Vue provides different ways to apply animation effects when items are rendered, updated, or removed from the DOM. 
They include tools for: 
1.	automatically apply classes to CSS transitions and animations 
2.	integration of third-party libraries for CSS animations such as Animate.css 
3.	using JavaScript to manipulate the DOM 
4.	integration of third-party JavaScript libraries for animations such as Velocity.js
***
#### slide №13
## AJAX
There is a Vue-resource plugin to work with Ajax requests. It provides the ability to create web requests and process responses using XMLHttpRequest or JSONP. Another feature of the plugin is support for Promise API and URI templates.
***
#### slide №14
## Vuex
Vuex is a pattern and state management library for applications on Vue.js. 
It provides a centralized common state for all components in the application and rules to ensure predictable state changes. 
The image below shows an application on Vue+Vuex with the following parts:
1. State, which is the only data source for components. 
2. Vue-components (Vue-components), which are essentially only declarative status display.
3. Actions (Actions), which catch the event that occurred, gather data from external API, and trigger a needed mutation. 
4. Mutations are the only part that can change the state and, having received data from Actions, applies them to the state.
***
#### slide №15
## Vue-devtools 
For debugging in the browser there is a Vue-devtools (unfortunately, only for Chrome), which allows you to see what components are in our application and their current status.
It also works great with Vuex and allows you to perform so-called time-travel debugging: in the browser, we can see the status history and switch between them.
***
#### slide №16-17
## Arguments
It is very easy to start working with it, even if you have never worked with JavaScript frameworks. It's the perfect combination of convenience and power. Consider a few more arguments in his favor: 
1. It's even smaller now. Runtime Vue Assembly.js 2.0 weighs only 16kb, and together with the vue-router and vuex — 26kb (about as the kernel of the first version).
2. He's faster. In Vue.js has always paid great attention to performance.
3. Vue 2.0 supports server-side rendering. This is the module Vue-server-renderer supports other tools of the ecosystem Vue (vue-router and vuex).
***
#### slide №18
## End
