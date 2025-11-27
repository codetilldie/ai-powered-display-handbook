# VRR 可变刷新率 (G-Sync, FreeSync)

VRR (Variable Refresh Rate) 技术允许显示器的刷新率**实时**跟随显卡的帧率变化。

## 为什么需要 VRR？

在游戏中，显卡渲染画面的速度是不稳定的（比如这一秒 60帧，下一秒 45帧）。
如果显示器固定 60Hz 刷新，就会出现两个问题：
1.  **画面撕裂 (Tearing)**：显卡渲染太快，显示器还在扫描上一帧，显卡就送来了下一帧，导致屏幕上部是旧画面，下部是新画面，中间有错位。
2.  **卡顿 (Stuttering)**：开启垂直同步 (V-Sync) 强制锁定帧率，当显卡渲染慢了，显示器只能重复显示上一帧，导致视觉卡顿和输入延迟增加。

**VRR 的作用**：显卡渲染一帧，显示器就刷新一帧。显卡慢，显示器就等。彻底解决了撕裂和卡顿问题。

## 三大阵营

### 1. NVIDIA G-Sync
*   **G-Sync Ultimate**：最高标准。显示器内置 NVIDIA 专用硬件芯片。支持 HDR，极宽的刷新率范围，经过极其严格的认证。价格昂贵。
*   **G-Sync**：内置 NVIDIA 芯片。性能优秀，价格较贵。
*   **G-Sync Compatible (兼容模式)**：**最常见**。显示器没有 NVIDIA 芯片，利用通用的 Adaptive-Sync 协议实现，但通过了 NVIDIA 的认证测试，保证无闪屏等问题。

### 2. AMD FreeSync
*   **FreeSync Premium Pro**：最高标准。支持 HDR，低帧率补偿 (LFC)。
*   **FreeSync Premium**：要求至少 120Hz，支持 LFC。
*   **FreeSync**：基础标准。

### 3. VESA Adaptive-Sync
*   **性质**：DisplayPort 接口的通用标准协议。FreeSync 其实就是基于此协议开发的。
*   **现状**：现在几乎所有支持 FreeSync 的显示器都默认支持 Adaptive-Sync，也就意味着**N卡也可以开启兼容模式**。

## 选购建议

1.  **必须有**：现在 VRR 已经是电竞显示器的标配，甚至是办公显示器的加分项。
2.  **N卡用户**：不一定要买带 G-Sync 芯片的（太贵）。购买支持 **FreeSync / Adaptive-Sync** 的显示器，通常都能在驱动里开启 "G-Sync Compatible" 模式，体验 95% 是一样的。
3.  **主机用户**：
    *   **Xbox**：支持 FreeSync。
    *   **PS5**：支持 **HDMI 2.1 VRR**。需要显示器配备 HDMI 2.1 接口。

## 注意事项

*   **闪屏问题**：部分低端 VA 面板在开启 VRR 且帧率波动剧烈时，可能会出现亮度闪烁。
*   **VRR 范围**：留意 VRR 的生效范围（如 48-144Hz）。如果帧率低于 48，可能会失效（除非支持 LFC 低帧率补偿）。
