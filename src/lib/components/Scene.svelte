<script lang="ts">
	import { T, useTask } from '@threlte/core';
	import { GLTF, OrbitControls } from '@threlte/extras';
</script>

<T.PerspectiveCamera makeDefault fov={5} position={[10, 40, 20]}>
	<OrbitControls />
</T.PerspectiveCamera>

<T.AmbientLight color="blue" intensity={4} />
<T.PointLight intensity={2} position.y={0.6} />
<T.DirectionalLight color="blue" position.y={-0.6} />
<T.DirectionalLight position.y={-0.6} />

<GLTF url="/models/scene.glb" />
