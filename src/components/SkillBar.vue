<template>
  <div class="skill-bar-container">
    <!-- Skill Label -->
    <div class="skill-label">{{ label }}</div>
    
    <!-- Skill Bar with Icon -->
    <div class="skill-progress-container">
      <div class="skill-icon"><i :class="icon"></i></div>
      <div class="skill-bar">
        <div class="skill-bar-fill" :style="{ width: percentage + '%' }"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SkillBar',
  props: {
    label: String,
    percentage: Number,
    icon: String
  }
};
</script>

<style scoped>
.skill-bar-container {
  margin: 0.5rem 0;
}

.skill-label {
  font-size: 0.85rem;
  margin-bottom: 0.25rem; /* Space between label and bar */
}

.skill-progress-container {
  display: flex;
  align-items: center;
  width: 100%;
}

.skill-icon {
  font-size: 1.5rem;
  margin-right: 0.5rem;
  color: #6c7a89; /* Color of icons */
}

.skill-bar {
  background-color: #333;
  border-radius: 0.25rem;
  flex-grow: 1;
  height: 1rem;
  overflow: hidden;
  width: 300px;
}

.skill-bar-fill {
  background-color: #6c7a89;
  border-radius: 0.25rem;
  height: 100%;
  transition: width 1s ease-in-out;
}
</style>
