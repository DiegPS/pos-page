<template>
  <label>
    <input class="toggle-checkbox" type="checkbox" />
    <div class="toggle-slot">
      <div class="sun-icon-wrapper">
        <div class="iconify sun-icon" data-icon="feather-sun" data-inline="false"></div>
      </div>
      <div class="toggle-button"></div>
      <div class="moon-icon-wrapper">
        <div class="iconify moon-icon" data-icon="feather-moon" data-inline="false"></div>
      </div>
    </div>
  </label>
</template>
<style scoped>
label {
  padding-left: 0.3rem;
}
.toggle-checkbox {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
}

.toggle-slot {
  font-size: 10px;
  position: relative;
  height: 1rem;
  width: 2rem;
  border: 0px solid transparent;
  border-radius: 10em;
  background-color: #999999;
  transition: background-color 250ms;
}

.toggle-checkbox:checked ~ .toggle-slot {
  background-color: #374151;
}

.toggle-button {
  transform: translate(0.15em, 0.125em);
  position: absolute;
  height: 1.5em;
  width: 1.5em;
  border-radius: 50%;
  background-color: #ffeccf;
  box-shadow: inset 0px 0px 0px 0.375em #ffbb52;
  transition:
    background-color 250ms,
    border-color 250ms,
    transform 500ms cubic-bezier(0.26, 2, 0.46, 0.71);
}
.toggle-checkbox:checked ~ .toggle-slot .toggle-button {
  background-color: #485367;
  box-shadow: inset 0px 0px 0px 0.75em white;
  transform: translate(1.65em, 0.25em);
}

.sun-icon {
  position: absolute;
  height: 6em;
  width: 6em;
  color: #ffbb52;
}

.sun-icon-wrapper {
  position: absolute;
  height: 6em;
  width: 6em;
  opacity: 1;
  transform: translate(2em, 2em) rotate(15deg);
  transform-origin: 50% 50%;
  transition:
    opacity 150ms,
    transform 500ms cubic-bezier(0.26, 2, 0.46, 0.71);
}

.toggle-checkbox:checked ~ .toggle-slot .sun-icon-wrapper {
  opacity: 0;
  transform: translate(3em, 2em) rotate(0deg);
}

.moon-icon {
  position: absolute;
  height: 6em;
  width: 6em;
  color: white;
}

.moon-icon-wrapper {
  position: absolute;
  height: 6em;
  width: 6em;
  opacity: 0;
  transform: translate(11em, 2em) rotate(0deg);
  transform-origin: 50% 50%;
  transition:
    opacity 150ms,
    transform 500ms cubic-bezier(0.26, 2.5, 0.46, 0.71);
}

.toggle-checkbox:checked ~ .toggle-slot .moon-icon-wrapper {
  opacity: 1;
  transform: translate(2em, 2em) rotate(-15deg);
}
</style>
