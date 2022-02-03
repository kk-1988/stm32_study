## 概念

## 时钟系统
> 时钟源相关介绍
1. 高速内部RC振荡器(HSI RC)
2. 高速外部时钟源(HSE OSC)
3. 低速外部时钟源(LSE OSC,32.768KHz，一般给RTC时钟)
4. 低速内置RC振荡器(LSI RC,约等于40KHz)  
5. MCO（PA8）是时钟输出引脚（可以选择PLL的2分频，HSI,HSE，或者系统时钟）
6. 任何外设使用前，必须使能其相应时钟
7. stm32有5个时钟源：HSI,HSE,LSI,LSE,PLL(倍频器)

> 系统时钟(sysclk)
1. sysclk之后有个AHB分频器，AHB有一个HCLK的时钟(一般就是72M(F1芯片))
2. AHB的AHB1分频器，PCLK1最高36Mhz(低速外设，通用定时器)
3. AHB的AHB2分频器，PCLK2最高72Mhz()
4. 可来源于三个时钟源：HSI振荡器的，HSE振荡器的，PLL时钟(PLLCLK)

>  


## 中断系统
> 
> 
> 