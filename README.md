# React-Three-Fiber 예제

- vite
- React
- vercel
- react-three-fiber
- react-three-drei

사용 

## vite 프로젝트 만들기
```bash
// npm 
npm create vite@latest
// yarn 
yarn create vite
```

```bash
javascript
React 
```
javascript, React 선택

### 설치
```bash
yarn add three @types/three @react-three/fiber @react-three/drei
```

참고
https://docs.pmnd.rs/react-three-fiber/getting-started/introduction
https://github.com/pmndrs/drei

## models 다운로드

https://market.pmnd.rs/ 
위 사이트에서 3d 객체 파일 다운로드

노트북으로 다운로드 

```
<OrbitControls />
// 3d 컨트롤러 움직일 수 있다

<PresentationControls global 
      config={{mass: 4, tension: 400}}  
      snap={{mass: 4, tension: 300}} 
>
// 움직일 수 있지만 다시 기본상태로 돌아옴
```

```
// 3d 모델 불러오기
const macbook = useGLTF("https://vazxmixjsiawhamofees.supabase.co/storage/v1/object/public/models/macbook/model.gltf")
<primitive object={macbook.scene} position={[-2.4, -1.3, 0.2]} scale={[2,2,2]}>
    </primitive> 
```

```
 <Float rotationIntensity={1.5}></Float>
// 둥둥뜨는 효과

 <ContactShadows  scale={7} blur={2.4} opacity={0.7} position-y={-2.0} />
// 그림자 효과
```

```
// 노트북 화면 빛 효과
<rectAreaLight 
        color={"#0021a7"} 
        intensity={55} 
        rotation={[0.1, Math.PI, 0]} 
        width={2.0}
        height={1.65}
        position={[0,0,-1]}
    />
```






