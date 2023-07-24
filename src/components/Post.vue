<script setup>
  import { ref } from 'vue';
  
  const posts = ref([
    {
      id: 1,
      title: 'Rambo: First Blood',
      description: 'First Blood (also known as Rambo: First Blood) is a 1982 American action film directed by Ted Kotcheff and co-written by and starring Sylvester Stallone as Vietnam War veteran John Rambo. It co-stars Richard Crenna as Rambos mentor Sam Trautman and Brian Dennehy as Sheriff Will Teasle. It is the first installment in the Rambo franchise, followed by Rambo: First Blood Part II.',
      content: 'The film is based on the 1972 novel First Blood by David Morrell, which many directors and studios had unsuccessfully attempted to adapt in the 1970s. In the film, Rambo is a troubled and misunderstood Vietnam veteran who must rely on his combat and survival skills when a series of brutal events results in him having to survive a massive manhunt by police and government troops near the fictional small town of Hope, Washington.',
    },
    {
      id: 2,
      title: 'Rambo: First Blood Part II',
      description: ' is a 1985 American action film directed by George P. Cosmatos and co-written by Sylvester Stallone, who also reprises his role as Vietnam War veteran John Rambo. A sequel to First Blood (1982), it is the second installment in the Rambo franchise, followed by Rambo III. It co-stars Richard Crenna, who reprises his role as Colonel Sam Trautman, along with Charles Napier, Julia Nickson, and Steven Berkoff.',
      content: 'The films plot is inspired by the Vietnam War POW MIA issue. In the movie, Rambo gets released from prison in a deal with the United States government to document the possible existence of missing POWs in Vietnam, but is given strict orders not to rescue any. When Rambo defies his orders, he is abandoned and forced once again to rely on his own brutal combat skills to save the POWs.',
    },
    {
      id: 3,
      title: 'Rambo III',
      description: ' is a 1988 American action film directed by Peter MacDonald and co-written by Sylvester Stallone, who also reprises his role as Vietnam War veteran John Rambo. A sequel to Rambo: First Blood Part II (1985), it is the third installment in the Rambo franchise.',
      content: 'The film depicts fictional events during the Soviet–Afghan War. In the film, Rambo sets out on a dangerous journey to Afghanistan in order to rescue his former commander and his longtime best friend, Col. Sam Trautman, from the hands of an extremely powerful and ruthless Soviet Army colonel who is bent on killing both Trautman and Rambo, while helping a local band of Afghan rebels fight against Soviet forces threatening to destroy their village.',
    },
  ]);
  </script>
<template>
    <div>
      <h2>Post List</h2>
      <ul class="posts">
        <li class="post-lines" v-for="post in posts" :key="post.id">
          <h3>{{ post.title }}</h3>
          <p>{{ post.description }}</p>
          <div>{{ post.content }}</div>
        </li>
      </ul>
    </div>
  </template>

  <style>
  .posts {
    list-style-type: none;
    padding: 0;
    text-align: center;
  }
  
  .post-lines {
    margin-bottom: 20px;
    border: 1px solid #000000;
    padding: 10px
  
  }
  </style>
  