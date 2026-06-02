---
title: "Unreal Engine Shaders"
excerpt: "Unreal Engine 머티리얼 에디터를 활용한 셰이더 스터디 모음"
collection: portfolio
---

Unreal Engine 머티리얼 에디터 및 포스트 프로세스를 활용한 셰이더 구현 작업들입니다.

---

### Fresnel Function Shader
`Shader` `Unreal`

유리 소재의 물리적 특성 — 프레넬 반사, 굴절, 투명도의 각도 의존성 — 을 Unreal Engine 머티리얼 에디터로 재현하는 것을 목표로 작업했습니다.

---

### Water Depth Fade Shader
`Shader` `Unreal`

단순한 투명 평면이 아닌 깊이에 따른 색상 변화, 엣지 페이드, 물결 노멀맵을 조합해 실제감 있는 수면을 구현했습니다.

---

### Ocean Shader
`Shader` `Unreal`

실제 바다의 잔물결과 너울을 별도 레이어로 나눠 겹치는 방식으로 구현했습니다. 파도 거품과 수면 굴곡(버텍스 변위)까지 포함한 풀 파이프라인을 구성했습니다.

---

### Varnished Wood Floor Shader
`Shader` `Unreal`

니스가 칠해진 원목 바닥재를 재현한 머티리얼 스터디입니다. 나무 표면 자체와 코팅(니스) 레이어를 분리하여 표현했으며, UE5의 Clear Coat 셰이딩 모델을 활용해 두 레이어가 물리적으로 올바르게 반응하도록 구현했습니다.

---

### Toon Shader
`Shader` `Unreal`

포스트 프로세스 방식으로 구현한 셀 셰이딩 머티리얼입니다. 씬 전체에 적용되는 포스트 프로세스이기 때문에 개별 오브젝트 머티리얼을 변경하지 않고도 애니메이션풍 렌더링을 적용할 수 있습니다. 외곽선(Outline), 툰 조명(Toon Lighting), 그림자 밴드(Light Band) 세 가지 시스템이 조합되어 동작합니다.
