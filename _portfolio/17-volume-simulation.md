---
title: "Volume Simulation"
excerpt: "Houdini Pyro/VDB 기반 볼류메트릭 연기/유체 시뮬레이션"
collection: portfolio
---

`Houdini`

Houdini SOP + DOP + VDB 파이프라인을 활용한 볼류메트릭 연기 시뮬레이션입니다. 밀도·온도·속도장을 VEX로 세밀하게 제어했습니다.

<video controls width="100%">
  <source src="/images/portfolio/volume-simulation/volume.mp4" type="video/mp4">
</video>

---

### 주요 기술

- **DOP:** Pyro Solver — Gas Buoyancy(온도 기반 상승) + Gas Turbulence(자연스러운 흐트러짐) + Gas Dissipate(소멸)
- **VEX — 커스텀 바람:** `sin(@Time * 1.2 + P.y * 0.5)`로 사인파 옆바람 적용
- **VEX — 밀도 색상 매핑:** density/temperature 값으로 연한 회색 → 짙은 회색 + 오렌지 발광 표현
- **VDB 후처리:** vdbsmooth → vdbresize로 볼륨 정리 및 최적화
- **렌더:** Mantra/Karma — Volume Step Size 0.05~0.1, Emission 채널 연결
