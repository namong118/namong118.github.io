---
title: "Particle Simulation"
excerpt: "Houdini SOP+DOP 파이프라인 기반 파티클 이펙트 시뮬레이션"
collection: portfolio
---

`Houdini`

Houdini SOP + DOP 파이프라인을 활용한 파티클 기반 비주얼 이펙트입니다. 커스텀 VEX 로직으로 파티클 속도·색상·수명을 세밀하게 제어했습니다.

<video controls width="100%">
  <source src="/images/portfolio/particle-simulation/particle.mp4" type="video/mp4">
</video>

<video controls width="100%">
  <source src="/images/portfolio/particle-simulation/particle-assignment.mp4" type="video/mp4">
</video>

---

### 주요 기술

- **SOP:** scatter로 소스 포인트 분산, attribute wrangle로 초기 속도/크기/수명 설정
- **DOP/POP:** pop source → pop force (Gravity / Drag / Turbulence) → pop wrangle (VEX)
- **수명 기반 색상:** `ratio = life / lifespan`으로 흰색 → 주황 → 빨강 → 투명 그라디언트
- **렌더:** Principled Shader + Emission 채널로 자체 발광 표현
