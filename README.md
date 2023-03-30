# EXPERIMENT--02-INTEFACING-A-DIGITAL-INPUT-TO-ARM-DEVELOPMENT-BOARD
## Aim: To Interface a Digital Input  (userpush button  ) to ARM   development board and write a  program to obtain  the data and flash the led  
## Components required: STM32 CUBE IDE, ARM IOT development board,  STM programmer tool.
## Theory 
The full form of an ARM is an advanced reduced instruction set computer (RISC) machine, and it is a 32-bit processor architecture expanded by ARM holdings. The applications of an ARM processor include several microcontrollers as well as processors. The architecture of an ARM processor was licensed by many corporations for designing ARM processor-based SoC products and CPUs. This allows the corporations to manufacture their products using ARM architecture. Likewise, all main semiconductor companies will make ARM-based SOCs such as Samsung, Atmel, TI etc.

 
  
## Procedure:
 1. click on STM 32 CUBE IDE, the following screen will appear 
 ![image](https://user-images.githubusercontent.com/36288975/226189166-ac10578c-c059-40e7-8b80-9f84f64bf088.png)

 2. click on FILE, click on new stm 32 project 
 ![image](https://user-images.githubusercontent.com/36288975/226189215-2d13ebfb-507f-44fc-b772-02232e97c0e3.png)
![image](https://user-images.githubusercontent.com/36288975/226189230-bf2d90dd-9695-4aaf-b2a6-6d66454e81fc.png)
3. select the target to be programmed  as shown below and click on next 

![image](https://user-images.githubusercontent.com/36288975/226189280-ed5dcf1d-dd8d-43ae-815d-491085f4863b.png)

4.select the program name 
![image](https://user-images.githubusercontent.com/36288975/226189316-09832a30-4d1a-4d4f-b8ad-2dc28f137711.png)


5. corresponding ioc file will be generated automatically 
![image](https://user-images.githubusercontent.com/36288975/226189378-3abbdee2-0df6-470f-a3cd-79c74e3d3ad8.png)

6.select the appropriate pins as gipo, in or out, USART or required options and configure 
![image](https://user-images.githubusercontent.com/36288975/226189403-f7179f1a-3eae-4637-826b-ab4ec35ba1e1.png)
![image](https://user-images.githubusercontent.com/36288975/226189425-2b2414ce-49b3-4b61-a260-c658cb2e4152.png)


7.click on cntrl+S , automaticall C program will be generated 
![image](https://user-images.githubusercontent.com/36288975/226189443-8b43451d-0b14-47e4-a20b-cc09c6ad8458.png)
![image](https://user-images.githubusercontent.com/36288975/226189450-85ffa969-2ffb-4788-81e5-72d60fdda0f1.png)
8. edit the program and as per required 
![image](https://user-images.githubusercontent.com/36288975/226189461-a573e62f-a109-4631-a250-a20925758fe0.png)

9. use project and build all 
![image](https://user-images.githubusercontent.com/36288975/226189554-3f7101ac-3f41-48fc-abc7-480bd6218dec.png)
10. once the project is bulild 
![image](https://user-images.githubusercontent.com/36288975/226189577-c61cc1eb-3990-4968-8aa6-aefffc766b70.png)

11. click on debug option 
![image](https://user-images.githubusercontent.com/36288975/226189625-37daa9a3-62e9-42b5-a5ce-2ac63345905b.png)

12. connect the  ARM board to power supply and usb 


13. check for execution of the output using run option 



## STM 32 CUBE PROGRAM :
```
/* USER CODE BEGIN Header */
/**
  **************************
  * @file           : main.c
  * @brief          : Main program body
  **************************
  * @attention
  *
  * Copyright (c) 2023 STMicroelectronics.
  * All rights reserved./* USER CODE BEGIN Header */
  *
/**
  * This software is licensed under terms that can be found in the LICENSE file
  **************************
  * in the root directory of this software component.
  * @file           : main.c
  * If no LICENSE file comes with this software, it is provided AS-IS.
  * @brief          : Main program body
  *
  **************************
  **************************
  * @attention
  */
  *
/* USER CODE END Header */
  * Copyright (c) 2023 STMicroelectronics.
/* Includes ------------------------------------------------------------------*/
  * All rights reserved.
#include "main.h"
  *
#include <stdbool.h>
  * This software is licensed under terms that can be found in the LICENSE file
/* Private includes ----------------------------------------------------------*/
  * in the root directory of this software component.
/* USER CODE BEGIN Includes */
  * If no LICENSE file comes with this software, it is provided AS-IS.

  *
/* USER CODE END Includes */
  **************************

  */
/* Private typedef -----------------------------------------------------------*/
/* USER CODE END Header */
/* USER CODE BEGIN PTD */
/* Includes ------------------------------------------------------------------*/

#include "main.h"
/* USER CODE END PTD */
#include <stdbool.h>

/* Private includes ----------------------------------------------------------*/
/* Private define ------------------------------------------------------------*/
/* USER CODE BEGIN Includes */
/* USER CODE BEGIN PD */

/* USER CODE END PD */
/* USER CODE END Includes */


/* Private macro -------------------------------------------------------------*/
/* Private typedef -----------------------------------------------------------*/
/* USER CODE BEGIN PM */
/* USER CODE BEGIN PTD */


/* USER CODE END PM */
/* USER CODE END PTD */


/* Private variables ---------------------------------------------------------*/
/* Private define ------------------------------------------------------------*/

/* USER CODE BEGIN PD */
/* USER CODE BEGIN PV */
/* USER CODE END PD */


/* USER CODE END PV */
/* Private macro -------------------------------------------------------------*/

/* USER CODE BEGIN PM */
/* Private function prototypes -----------------------------------------------*/

void SystemClock_Config(void);
/* USER CODE END PM */
static void MX_GPIO_Init(void);

void push_button();
/* Private variables ---------------------------------------------------------*/
bool button_status;

/* USER CODE BEGIN PFP */
/* USER CODE BEGIN PV */


/* USER CODE END PFP */
/* USER CODE END PV */


/* Private user code ---------------------------------------------------------*/
/* Private function prototypes -----------------------------------------------*/
/* USER CODE BEGIN 0 */
void SystemClock_Config(void);

static void MX_GPIO_Init(void);
/* USER CODE END 0 */
void push_button();

bool button_status;
/**
/* USER CODE BEGIN PFP */
  * @brief  The application entry point.

  * @retval int
/* USER CODE END PFP */
  */

int main(void)
/* Private user code ---------------------------------------------------------*/
{
/* USER CODE BEGIN 0 */
  /* USER CODE BEGIN 1 */


/* USER CODE END 0 */
  /* USER CODE END 1 */


/**
  /* MCU Configuration--------------------------------------------------------*/
  * @brief  The application entry point.

  * @retval int
  /* Reset of all peripherals, Initializes the Flash interface and the Systick. */
  */
  HAL_Init();
int main(void)

{
  /* USER CODE BEGIN Init */
  /* USER CODE BEGIN 1 */


  /* USER CODE END Init */
  /* USER CODE END 1 */


  /* Configure the system clock */
  /* MCU Configuration--------------------------------------------------------*/
  SystemClock_Config();


  /* Reset of all peripherals, Initializes the Flash interface and the Systick. */
  /* USER CODE BEGIN SysInit */
  HAL_Init();


  /* USER CODE END SysInit */
  /* USER CODE BEGIN Init */


  /* Initialize all configured peripherals */
  /* USER CODE END Init */
  MX_GPIO_Init();

  /* USER CODE BEGIN 2 */
  /* Configure the system clock */

  SystemClock_Config();
  /* USER CODE END 2 */


  /* USER CODE BEGIN SysInit */
  /* Infinite loop */

  /* USER CODE BEGIN WHILE */
  /* USER CODE END SysInit */
  while (1)

  {
  /* Initialize all configured peripherals */
    /* USER CODE END WHILE */
  MX_GPIO_Init();
	  push_button();
  /* USER CODE BEGIN 2 */
    /* USER CODE BEGIN 3 */

  }
  /* USER CODE END 2 */
  /* USER CODE END 3 */

}
  /* Infinite loop */

  /* USER CODE BEGIN WHILE */
/**
  while (1)
  * @brief System Clock Configuration
  {
  * @retval None
    /* USER CODE END WHILE */
  */
	  push_button();
void push_button()
    /* USER CODE BEGIN 3 */
{
  }
	button_status=HAL_GPIO_ReadPin(GPIOC,GPIO_PIN_13);
  /* USER CODE END 3 */
	if(button_status==0)
}
	{

		HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_SET);
/**
	}
  * @brief System Clock Configuration
	else
  * @retval None
	{
  */
		HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_RESET);
void push_button()
	}
{
}
	button_status=HAL_GPIO_ReadPin(GPIOC,GPIO_PIN_13);
void SystemClock_Config(void)
	if(button_status==0)
{
	{
  RCC_OscInitTypeDef RCC_OscInitStruct = {0};
		HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_SET);
  RCC_ClkInitTypeDef RCC_ClkInitStruct = {0};
	}

	else
  /** Configure the main internal regulator output voltage
	{
  */
		HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_RESET);
  HAL_PWREx_ControlVoltageScaling(PWR_REGULATOR_VOLTAGE_SCALE1);
	}
  /** Initializes the RCC Oscillators according to the specified parameters
}
  * in the RCC_OscInitTypeDef structure.
void SystemClock_Config(void)
  */
{
  RCC_OscInitStruct.OscillatorType = RCC_OSCILLATORTYPE_HSI;
  RCC_OscInitTypeDef RCC_OscInitStruct = {0};
  RCC_OscInitStruct.HSIState = RCC_HSI_ON;
  RCC_ClkInitTypeDef RCC_ClkInitStruct = {0};
  RCC_OscInitStruct.HSIDiv = RCC_HSI_DIV1;

  RCC_OscInitStruct.HSICalibrationValue = RCC_HSICALIBRATION_DEFAULT;
  /** Configure the main internal regulator output voltage
  RCC_OscInitStruct.PLL.PLLState = RCC_PLL_NONE;
  */
  if (HAL_RCC_OscConfig(&RCC_OscInitStruct) != HAL_OK)
  HAL_PWREx_ControlVoltageScaling(PWR_REGULATOR_VOLTAGE_SCALE1);
  {
  /** Initializes the RCC Oscillators according to the specified parameters
    Error_Handler();
  * in the RCC_OscInitTypeDef structure.
  }
  */
  /** Initializes the CPU, AHB and APB buses clocks
  RCC_OscInitStruct.OscillatorType = RCC_OSCILLATORTYPE_HSI;
  */
  RCC_OscInitStruct.HSIState = RCC_HSI_ON;
  RCC_ClkInitStruct.ClockType = RCC_CLOCKTYPE_HCLK|RCC_CLOCKTYPE_SYSCLK
  RCC_OscInitStruct.HSIDiv = RCC_HSI_DIV1;
                              |RCC_CLOCKTYPE_PCLK1;
  RCC_OscInitStruct.HSICalibrationValue = RCC_HSICALIBRATION_DEFAULT;
  RCC_ClkInitStruct.SYSCLKSource = RCC_SYSCLKSOURCE_HSI;
  RCC_OscInitStruct.PLL.PLLState = RCC_PLL_NONE;
  RCC_ClkInitStruct.AHBCLKDivider = RCC_SYSCLK_DIV1;
  if (HAL_RCC_OscConfig(&RCC_OscInitStruct) != HAL_OK)
  RCC_ClkInitStruct.APB1CLKDivider = RCC_HCLK_DIV1;
  {

    Error_Handler();
  if (HAL_RCC_ClockConfig(&RCC_ClkInitStruct, FLASH_LATENCY_0) != HAL_OK)
  }
  {
  /** Initializes the CPU, AHB and APB buses clocks
    Error_Handler();
  */
  }
  RCC_ClkInitStruct.ClockType = RCC_CLOCKTYPE_HCLK|RCC_CLOCKTYPE_SYSCLK
}
                              |RCC_CLOCKTYPE_PCLK1;

  RCC_ClkInitStruct.SYSCLKSource = RCC_SYSCLKSOURCE_HSI;
/**
  RCC_ClkInitStruct.AHBCLKDivider = RCC_SYSCLK_DIV1;
  * @brief GPIO Initialization Function
  RCC_ClkInitStruct.APB1CLKDivider = RCC_HCLK_DIV1;
  * @param None

  * @retval None
  if (HAL_RCC_ClockConfig(&RCC_ClkInitStruct, FLASH_LATENCY_0) != HAL_OK)
  */
  {
static void MX_GPIO_Init(void)
    Error_Handler();
{
  }
  GPIO_InitTypeDef GPIO_InitStruct = {0};
}


  /* GPIO Ports Clock Enable */
/**
  __HAL_RCC_GPIOC_CLK_ENABLE();
  * @brief GPIO Initialization Function
  __HAL_RCC_GPIOA_CLK_ENABLE();
  * @param None

  * @retval None
  /*Configure GPIO pin Output Level */
  */
  HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_RESET);
static void MX_GPIO_Init(void)

{
  /*Configure GPIO pin : PC13 */
  GPIO_InitTypeDef GPIO_InitStruct = {0};
  GPIO_InitStruct.Pin = GPIO_PIN_13;

  GPIO_InitStruct.Mode = GPIO_MODE_INPUT;
  /* GPIO Ports Clock Enable */
  GPIO_InitStruct.Pull = GPIO_PULLUP;
  __HAL_RCC_GPIOC_CLK_ENABLE();
  HAL_GPIO_Init(GPIOC, &GPIO_InitStruct);
  __HAL_RCC_GPIOA_CLK_ENABLE();


  /*Configure GPIO pin : PA5 */
  /*Configure GPIO pin Output Level */
  GPIO_InitStruct.Pin = GPIO_PIN_5;
  HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, GPIO_PIN_RESET);
  GPIO_InitStruct.Mode = GPIO_MODE_OUTPUT_PP;

  GPIO_InitStruct.Pull = GPIO_PULLUP;
  /*Configure GPIO pin : PC13 */
  GPIO_InitStruct.Speed = GPIO_SPEED_FREQ_LOW;
  GPIO_InitStruct.Pin = GPIO_PIN_13;
  HAL_GPIO_Init(GPIOA, &GPIO_InitStruct);
  GPIO_InitStruct.Mode = GPIO_MODE_INPUT;

  GPIO_InitStruct.Pull = GPIO_PULLUP;
}
  HAL_GPIO_Init(GPIOC, &GPIO_InitStruct);


/* USER CODE BEGIN 4 */
  /*Configure GPIO pin : PA5 */

  GPIO_InitStruct.Pin = GPIO_PIN_5;
/* USER CODE END 4 */
  GPIO_InitStruct.Mode = GPIO_MODE_OUTPUT_PP;

  GPIO_InitStruct.Pull = GPIO_PULLUP;
/**
  GPIO_InitStruct.Speed = GPIO_SPEED_FREQ_LOW;
  * @brief  This function is executed in case of error occurrence.
  HAL_GPIO_Init(GPIOA, &GPIO_InitStruct);
  * @retval None

  */
}
void Error_Handler(void)

{
/* USER CODE BEGIN 4 */
  /* USER CODE BEGIN Error_Handler_Debug */

  /* User can add his own implementation to report the HAL error return state */
/* USER CODE END 4 */
  __disable_irq();

  while (1)
/**
  {
  * @brief  This function is executed in case of error occurrence.
  }
  * @retval None
  /* USER CODE END Error_Handler_Debug */
  */
}
void Error_Handler(void)

{
#ifdef  USE_FULL_ASSERT
  /* USER CODE BEGIN Error_Handler_Debug */
/**
  /* User can add his own implementation to report the HAL error return state */
  * @brief  Reports the name of the source file and the source line number
  __disable_irq();
  *         where the assert_param error has occurred.
  while (1)
  * @param  file: pointer to the source file name
  {
  * @param  line: assert_param error line source number
  }
  * @retval None
  /* USER CODE END Error_Handler_Debug */
  */
}
void assert_failed(uint8_t *file, uint32_t line)

{
#ifdef  USE_FULL_ASSERT
  /* USER CODE BEGIN 6 */
/**
  /* User can add his own implementation to report the file name and line number,
  * @brief  Reports the name of the source file and the source line number
     ex: printf("Wrong parameters value: file %s on line %d\r\n", file, line) */
  *         where the assert_param error has occurred.
  /* USER CODE END 6 */
  * @param  file: pointer to the source file name
}
  * @param  line: assert_param error line source number
#endif /* USE_FULL_ASSERT */
  * @retval None
  */
void assert_failed(uint8_t *file, uint32_t line)
{
  /* USER CODE BEGIN 6 */
  /* User can add his own implementation to report the file name and line number,
     ex: printf("Wrong parameters value: file %s on line %d\r\n", file, line) */
  /* USER CODE END 6 */
}
#endif /* USE_FULL_ASSERT */
```


## Output  :

![exp2mic2](https://user-images.githubusercontent.com/119557910/228872932-e25bde58-2624-4a31-91b8-b52033a19ea6.jpeg)

![exp2mic](https://user-images.githubusercontent.com/119557910/228873060-b93cb548-1546-430e-a7a5-7548765ade94.jpeg)

## Result :
Interfacing a digital Input (Pushbutton ) with ARM microcontroller based IOT development is executed and the results are verified.
