<template>
  <div class="skill-bar-container">
    <div class="skill-icon"><i :class="icon"></i></div>
    <span class="skill-label">{{ label }}</span>
    <div class="skill-bar">
      <div class="skill-bar-fill" :style="{ width: percentage + '%' }">
        <span>{{ percentage }}%</span>
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
  display: flex;
  align-items: center;
  margin: 0.5rem 0;
}

.skill-icon {
  font-size: 1.5rem;
  margin-right: 0.5rem;
  color: #6c7a89; /* Color of icons */
}

.skill-label {
  flex: 1;
  text-align: left;
  margin-right: 1rem;
}

.skill-bar {
  background-color: #333;
  border-radius: 0.25rem;
  flex-grow: 1;
  height: 1rem;
  overflow: hidden;
}

.skill-bar-fill {
  background-color: #6c7a89;
  border-radius: 0.25rem;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  height: 100%;
  padding-right: 0.5rem;
  color: #fff;
  font-weight: bold;
  transition: width 1s ease-in-out;
}
</style>