# Copyright lowRISC contributors.
# Licensed under the Apache License, Version 2.0, see LICENSE for details.
# SPDX-License-Identifier: Apache-2.0

# UART DIF library (dif_uart)
dif_uart = declare_dependency(
  link_with: static_library(
    'uart_ot',
    sources: [
      hw_ip_uart_reg_h,
      'dif_uart.c',
    ],
    dependencies: [
      sw_lib_mmio,
    ],
  )
)

# PLIC DIF library (dif_plic)
dif_plic = declare_dependency(
  link_with: static_library(
    'dif_plic_ot',
    sources: [
      hw_top_earlgrey_rv_plic_reg_h,
      'dif_plic.c',
    ],
    dependencies: [
      sw_lib_mmio,
    ],
  )
)

# GPIO DIF library
sw_lib_dif_gpio = declare_dependency(
  link_with: static_library(
    'sw_lib_dif_gpio',
    sources: [
      hw_ip_gpio_reg_h,
      'dif_gpio.c',
    ],
    dependencies: [
      sw_lib_mmio,
    ],
  )
)

# SPI DIF library
sw_lib_dif_spi_device = declare_dependency(
  link_with: static_library(
    'sw_lib_dif_spi_device',
    sources: [
      hw_ip_spi_device_reg_h,
      'dif_spi_device.c',
    ],
    dependencies: [sw_lib_mmio],
  )
)

# RISC-V Timer DIF library (dif_rv_timer)
dif_rv_timer = declare_dependency(
  link_with: static_library(
    'dif_rv_timer_ot',
    sources: [
      hw_ip_rv_timer_reg_h,
      'dif_rv_timer.c',
    ],
    dependencies: [
      sw_lib_mmio
    ],
  )
)

# I2C DIF library
sw_lib_dif_i2c = declare_dependency(
  link_with: static_library(
    'sw_lib_dif_i2c',
    sources: [
      hw_ip_i2c_reg_h,
      'dif_i2c.c',
    ],
    dependencies: [
      sw_lib_mmio,
    ],
  )
)

# USBDEV DIF library (dif_usbdev)
sw_lib_dif_usbdev = declare_dependency(
  link_with: static_library(
    'sw_lib_dif_usbdev',
    sources: [
      hw_ip_usbdev_reg_h,
      'dif_usbdev.c',
    ],
    dependencies: [
      sw_lib_mmio,
      sw_lib_bitfield,
    ],
  )
)

# HMAC device DIF library
sw_dif_hmac = declare_dependency(
  link_with: static_library(
    'sw_dif_hmac',
    sources: [
      hw_ip_hmac_reg_h,
      'dif_hmac.c'
    ],
    dependencies: [
      sw_lib_bitfield,
      sw_lib_mmio,
    ],
  )
)

