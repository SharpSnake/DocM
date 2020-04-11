# C++ Core Guidelines [![](https://img.shields.io/badge/C++_Core_Guidelines-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+CjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiIHdpZHRoPSI0NnB4IiBoZWlnaHQ9IjUycHgiIHZpZXdCb3g9IjAgMCA0NiA1MiIgZW5hYmxlLWJhY2tncm91bmQ9Im5ldyAwIDAgNDYgNTIiIHhtbDpzcGFjZT0icHJlc2VydmUiPiAgPGltYWdlIGlkPSJpbWFnZTAiIHdpZHRoPSI0NiIgaGVpZ2h0PSI1MiIgeD0iMCIgeT0iMCIKICAgIGhyZWY9ImRhdGE6aW1hZ2UvcG5nO2Jhc2U2NCxpVkJPUncwS0dnb0FBQUFOU1VoRVVnQUFBQzRBQUFBMENBWUFBQUQxOUFyS0FBQUFCR2RCVFVFQUFMR1BDL3hoQlFBQUFDQmpTRkpOCkFBQjZKZ0FBZ0lRQUFQb0FBQUNBNkFBQWRUQUFBT3BnQUFBNm1BQUFGM0NjdWxFOEFBQUFCbUpMUjBRQS93RC9BUCtndmFlVEFBQUEKQ1hCSVdYTUFBQkowQUFBU2RBSGVaaDk0QUFBQUIzUkpUVVVINUFRTEFpd2IwMUNrMlFBQURSaEpSRUZVYU43Tm1ubVVsY1daaDUrcQorcGE3OXUwR0Y2Q0JabE5FTVVFVWwxRTA0NkFqb3c0elF4YmpSRDBlaFFTTnl6amtIR1NpUVRObUlKSGpuTVFsUnBHSkVqMHpyb21LCmlBc0JGVWxRWkpGdXRnWWFvYUUzdXZ2ZXZ0dTMxZnp4TmMzVzNiZVZudVU5NS83M1ZiMVB2ZlhXcjk2cXVrSnJUWC9hYll0M25pZHMKODA0M241bU9EcFFWVGI2RzBQLys2UFVqMXZTbkg5RmY0RDlZWER0R0tqRlhhLzhtdzRySVlqWU5hS3hZa3NEM1FmTkMwUzArdE9pVwpjWnYvWDREUFhQQnVtVEZrekcxQzZMdVZZWjFhekxZVCtCNElFWDZnTlVJcEl2RnlmTGQ0VUF2NXkweGI0NitlKytINUIvL1B3SC80ClhOMC9hS0h2VTZZMXdjMTM0RG1GdzhESG10WW95OGFLSnZIZFlqVmFQdlRZRFZYUC82K0N6M3htMi9tbWJjOFZNRTNyQUNmZjhhWGEKbTVFNDBqQUpndUF0NGZzUFBYYmpxSS8rUjhGblBMV3gwb3FVemZaOWQ1WnBSKzFpdGcwZEJEMUh1VWZUQ0NHeDRpbDhwK2dpZU1Zcgordk9mbWpGMmQ3K0NYM1huVW12a3BETnVGZkFqdzRxTUtHYlRCSjd6RllDUDVkZEl3OFNPcC9EYzRqNFFDOU1IMnA5Y012dnJ1Uk1HCnYyM0pyaXVra1BkSlpVejJuRHh1SVhmaXdOME13TENqR0pFWWdldXUxVkkrK1BqMXc5LzRTdUN6RnRXY0plM0l2UnI5ajFJb2lybFEKM3FDZm9ZOHhPNVpFaDU1ZTFMNzdzeWR1UEcxOW44QnZlTFptUUZ6WWR3ay91TXVNUkZPRmJCdmE5MHRHV1FPZXIvSDhnRUREb1c2RgowRWdoTUpURVVLTDBzQS9KWnl5RjYrU3pRcXJIbkdKMjRkTzNudDNZSS9qdHorNzZIa3JNVVlaMWxwUEw0THZGWG9FRjRQcWFnaHVnCkpGVEVMVTRxTXhtWXNJamJDZ0ZraXo0dEhRNU5hWmUybklQclE5U1VtRXJRYTVKcWpUSXRyRmdabnV0c2x3UUxOdTU0OWo5V3padm4KZDRIZi90dnFNNFdaZUJpWUd2Z2ViaUhiYTFBRTRBZWFiTkVuRlRNNVowUVpFMGVXY2ZxZ0JNbW9Rc21qQnh0b1RTYm5zNzBoeTdyZAphZGJ0YXFjdDZ4S3pGWVlzUFFBekVrZFpOam9JM2cvYzNJOGV2K21NZGVMR0p6NGJra2lrL21SWWthRzVkQXVVa0RjQjVKMEFLZUd5CmNRTzU2dXNuTWFRaVVpb0JqcklEN1VXV2IyeG14ZVlXWEQ4Z1pxbmU0VHZYVnJ6c0pBUitVOXpLWHloK3NIajdRaXVldUNmYjJvZ28Ka2NjQ3lCUThLZ2RFdUdueVVNNGVudnhTd01kYXpiNE9mdnZCUG5ZMzVVaEdqRjc5MnFhSjQ3bHNPMWhrL1piYXhlTFdwejV2bFZLVQpCNzVmMGxHbTRERitXSkxicGxReElHR2VFSFJYbjNtUFg3KzNoMDkydGxNV1BSN2VNaFJDQ09vYUQvTEo5ajBjT0pnR1E3bFNTRkVlCitGN0pTSGNVUE1ZUFRYTFAxSkg5QmcyUWpCcmNQWFVFNTQxSzBWSHd1bFJIU1VuVU1tbnR5UFBPWjF0NFkrMW1EclNsd1RKQUtWTnEKMzZlVU51ZmRnRUhsTnJkZldVWE1WdjBHZmNoTUpabDFSUlZWSjBmSk93RlJ5OFQxZlQ3ZXNvdVhWNjluMjk0R1VCS016aG5SQWJKVQpwMEduWE41ODJUQXE0djBYNldNdFlTdithZXBveXVNV20rcjI4K3JIRy9oa1d4MU9FSUJsSGljWVJxa09zd1dmeThjUDVHdDlYSWliCjkzWlFzeTlEYzhaRkF3T1RKdU9HSkRocmFBSlpZdkhYTlJ4azlhWWExdFUyZ0tsQzRCNnNWM0EvMENTaUJsZFBPS1VrOEk2R0xQLzUKY1FPYjkyaDhuVVBLY04wRUdrd2xPSDF3Z205ZE1JaHhsWW5qMnU1dXpQQ0xWOWJ6OUxzMU9INEFVYXVrdjE3QjgyN0FSV1BLcVJ6UQp1MDcvdWJhTko5N1poNnViR1Z5NWxrenJGWGp1UUpTUlJnaE5FSVRTOTI5L3FHWEc1Y09ZUEhaQU9KdEZqOGZmMnN6RHI2Mm5zVEVECkNUdU1jaDhxN1Y3QkJacHpSNlY2N1dCWFk0NG4zOTJENjV1VXhSU25EdjAxQTA1NWxhYjZtYVJiTDBXZ2tTcExNcUlvZUFGTFB0alAKb0ZTVTJ2b21mdkw4V3Y1Y3N4OGlKcFJId3c3N2VEdzRBbHpnZTBsQ2hkRjRQcFRaa3ZHVkZUMjMxdkM3RDNPa3N3bVNrUml1NitONwo1VVRqMnhnNmVpNlp0a3RwcXIrSmZNZFptR2FCOHJqSHZ1WU0wK1l2WSt2ZVJnSTNnTEpvWncyaElWc0VRMEhNT3FKS0EzSXVlSDQ0CkkxS0E3Z1RYV3FGVWxnR1ZMeUpsRHJUQ0N5QVpWYXhyTGtPMEhCOElLU0NUOTBrYmFVYU5BWUZDcWp4U0Z2QzlGRm9MeWlyZUo1NWMKUzN2TDMxUC94VGY1OEpNaTJ3N1U0bnNGTU0xUWt6WGcrQ1RqTm5PK05aSE5lOXQ0ZnRWMnNGUklYWEQ1OXVReG5ETnlJQXRlMzBSYgp1Z0NXNm95NFZnaFpZT0NnSlJoR0sxcWJDQVNCMXF6YUc0RHVmZ2FsaEZNcUphSnpsa0RpZXdtMERsWFc5OG9Sd3VIa3djOWl4dC9oCjgvMFg0KytiQktSQTVRNlg5NTVQZWRSazdqY25zblRkSHA1ZlhnTm1wMUlYUEw1OThXaW1YemlTUmU5dm82MGxDNVpDM1BxYmpWb0gKRm9iVlJOWFlPekNNZHJRK2xFRjlPVFRvSTc3dE9VRU53OEUyUGVycWg3RjA1Vit4dWZZMGtCNDRIcithY1FsWFRoaks2WU5UcFBNdQpkVTBaN2xuOE1ZN3I4K2pNU3hoK1VvSlV6R0w3L25aV2JLN24rMDk4VUVySHY4eUpwMmRvclFXZ2tOSWhHZXNnYWhlTytyd3NacEdLCmhSSm9La0ZGd2laaVNvVFdWTVJ0VENPTWZ1cUk3NDZJZUNPanpyd1p3d3hUSlhRWUhnUjZNaWtFVVVzaXBjQXlUVUNTejF0ZDYwcHIKVUVvVGl4Wm83MGl3NmsrWHNITE5oZVR6VVlqbXUvcXhQWjlSZzFOVS8vSTdMTit3bCtrUHZFbkJOdEJBTk8reFpPNVZURHUvaW5QdQplWWt0ZXc1U01BL2x1QWpRMnFhdCtXcVV5cUsxUVJCb1lyYkJlU1BpSUk2UHBoQ0Nqb0xQNTNzTFlmVzJweDdIeXpCKy9GNU0wME5yClFUeGV4UGNscTFlUDQrMTNKdEhjUGhvcURJZ2N5dTl3Tm91K1ptOTdua1h2YmVIVG5jMTArRUc0Y3dub0NBSmUvN1NPMW80Q2RhMDUKQ3I0R3N6UGloM0kwOE9OZE0rajVta1RFWU1GM2g1T005WkFDQWR6NTlEWmVXTHFhbGdNSFVja01jKzk5bVZOUGJnZXAyYmExa3VWTAp6Mk5MelhCUUhsZ09TQXNqVlk0WHFQRFFFdTNjMWdNTk9RZVVncWh4OU5JcGVLRWNScTFRempoS3h6VlNIYjZSa2dyYTh6N1Y5U2t1CkdOUDlKaVFrWER0QjhPaWlMU0JqeEJJZXlXU08xclk0eTk2Y3hKbzFaK0M3Q21LRkVLQVlnSlBoZDNQL0ZsOUZtTHRrRGJ1L2FJVzQKRmRZbWNmdjQ1YUlCMndoL1I1aWFlTzJzZWQxQ0FVVlBZNXVTODNyWlBVZFhEbVRvb0FxV3JxekdFVG0wanZMaWYxM0s5dXJoYU5zRAp1N1BXenhZUXJzOGo5MXpMTFZkUDVPeXFBVnczZVF4Q0NUYldOdU4wRkVQdGxuMFRneDdCRHkyKzVvekRSV01IRUxONnJvQW5qaDNDCmhETXJxYTVwWWZXN0NZcVpBSXdjdUI3a0hTZzZuRG5pVkI2Yk00MWJyam0zcTEwaVluTGxoR0ZjTTZtS3B2WThOYnRid3J4WEphdnQKSTNQOGVET1VJdWRvTGg0VFkrYVVrU1U3eStRZDN2eG9LMy84dEpaZHpSbTBocXFCQ2I0eGNSUi9jL0ZZS2hLOUYydHZmRkxIN1UrdQpaRStiRTI1QXZkeXlkYXZqUWdnaXRrVTJsMmZEcGhwZWUya0g0MDY1Z2NsZnErclZjVEpxY2QyVXM3bHV5dGtsQjltZG5UVWtTYkdoCkhod0Y1UldnREFpNmwrUGo1c1MyTEF5bHFONWF5eXR2TG1mRHhzOUpaN0xjdnZCMVdqdnlKWjEvVmNzVlhhNS84Q1VhR3RQZzVhQzEKQVhMcE1IWEU4YWtqaFpSb3JURU5nMGpFcHY1QUE2OHZYOEY3cXo2aUxkMEJFUnRTY1RaVjcrUG1uNzZDNHdYOURoMW96WXo1cjdIbQowNTJkMWFJRTM0ZDBLN1EyZ2xNSUM2TkRKeWdoTUtRUTJXZzhGai9ZMnNabkc2dXAyYkdUd1BQQnNnL3Y5bHBEZVl6ZnY3ZUo2NlZnCjBYM1RTY1hzZm9FdXVoNHpmL1lxejcveEthUmlSK2kzQ0g5dUVkcWFJQktEZUJrWUZ1Z0FOV0hhSFZWYmR0ZWYrKzc3ZjZTK2ZqL2EKTU1BMHVpOVJvaFkxMVh0NWYvMXVKcHcybU1xVHkwNEllc09PQTN4djNvdjhmc1hua0lwM2Y0UFdOUUFIQ2xtdzRpRE5GNFU1NWNFeApiaURYWXBqbEJNWFMzb1NBVEk1VUlzcmQzL2tMWmsyL2dGTXJFcVhiSFdFdDZSeS9lWFV0QzEvNGtKYldiSmdlZlRFakNvR2Z4M2ZPCkYxcHJ4T1gvT2hrN3VoQXBKK0VYd1hmb3RTb1VBaHdQc2dXcWhwL0U5TDhjejk5TlBvUHhvd2YxS0hsdDJTS2JkemJ3aHcrMjhOS0sKVGV5c2F3NjNjTnZzVmZaQWd6VEJpSUFPTmxETXp0SHYzYitzNjVwWmZPTW5jZXo0OXhGNk5zb2NqRnNBN1ZHeXJDMjZVSEFoWmpGbQpjQVZuVkozTXNNRVZET2djUUd1MnlCZjdEN0sxcnBsdDlhMlFMUndHN3RVMENBVm1GQUtuQlNFWGtzMDlybGZPYTRkdUx2YkZsUGtqCmtmcGVwTHdKYVZpNGVmcDBnZzEwT0F1dUh4WlBSNW9VaCs5SityaWxoOENCRHp5SDl1YnJ0K2R1UFlxenA2Y1VjZlhDaXdpQyt4SHkKS3JRUFhoL3l2ejlNV1dGcWFIOEYybjlBTDV1enNsdStVbzlYNHEvbjM0QlVjNURHbVhnRkNGejYveDFJZ3pUQ1BQYTlIWWpnNTJTWApQcU5YcmVyeEZOT241MEp4MmJ5QlJLTjNBSGVoekhMY2ZGaU05NGNKQVdZTVBDZUxsSThpY28vb3BmTWFTamI3TWcrMFlzcjg4Umh5Ckx2QmRwQUMzY0dMUVJwY0N2WXgySHRMTC91V3pQck44bFNkeE1mVVhWNEM0SHlFdklYREJML0tsRHRYS0FtV0Q3NjFGaUFmMVc3UGYKNkdQakV3TUhFRmZkYWFFclp5REZiS1E1QWkvZll5VjN1SkVNMHlMdzlrSHdDSDdURTNyNXd5VmZrZnNWdkt1RHFRc3EwZXFmMGQ0cwpsQm5CeTNlem9ZaFEzbnpYUThxbjhaMEZldm1QZDUrUTMvNzZvNDJZdXVBQ0VEOUd5R3ZRd1dINVZGYW9HSUYrbThCN1NDK2Y4MEcvCitPdnZ2emFKcVQrL0hNVDlCTjVsQUVpMUJpRWYwRXRuTCt0UFAvOE5UcVRZUXRwS2wyZ0FBQUFIZEVWWWRFRjFkR2h2Y2dDcHJzeEkKQUFBQUNIUkZXSFJEYjIxdFpXNTBBUGJNbHI4QUFBQUtkRVZZZEVOdmNIbHlhV2RvZEFDc0Q4dzZBQUFBRG5SRldIUkRjbVZoZEdsdgpiaUIwYVcxbEFEWDNEd2tBQUFBbGRFVllkR1JoZEdVNlkzSmxZWFJsQURJd01qQXRNRFF0TVRGVU1ESTZORFE2TWpZck1EQTZNREEwCm9XVTJBQUFBSlhSRldIUmtZWFJsT20xdlpHbG1lUUF5TURJd0xUQTBMVEV4VkRBeU9qUTBPakkyS3pBd09qQXdSZnpkaWdBQUFBeDAKUlZoMFJHVnpZM0pwY0hScGIyNEFFd2toSXdBQUFBdDBSVmgwUkdselkyeGhhVzFsY2dDM3dMU1BBQUFBQ1hSRldIUlRiMlowZDJGeQpaUUJkY1A4NkFBQUFCM1JGV0hSVGIzVnlZMlVBOWYrRDZ3QUFBQVowUlZoMFZHbDBiR1VBcU83U0p3QUFBQWgwUlZoMFYyRnlibWx1Clp3REFHK2FIQUFBQUFFbEZUa1N1UW1DQyIgLz4KPC9zdmc+Cg==&labelColor=CED8F6&logoWidth=30&style=flat "C++ Core Guidelines")](https://github.com/isocpp/CppCoreGuidelines)

- [Per.19: Access memory predictably](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md#per19-access-memory-predictably)

  关于临近内存访问性能的问题，官方给出的例子有待商榷，只能说此例在大多数情况下具有代表性和合理性，因为C++二维数组是行主续存储的，那么逐行遍历应该是性能最好的。

  早些年做Matlab开发时，也有一个核心原则，其大意是：如果有嵌套循环，则应该尽量把繁忙的循环放到内层。例如当一个二维数组的行数远大于列数时，这时逐列遍历程序会有更好的性能。
  
  如果从更底层的角度去思考或许可以这样解释：相对于内存访问，机器指令频繁跳转的消耗已经占了主导（_我并不会汇编语言，这里只是打个比方_）。
  
  经过测试（MSVC 2017开启/O2优化）这个原则同样适用于C++，按照Per.19中的示例，当二维数组为200000行、2列，此时按逐列遍历的性能是逐行遍历的1.5倍左右。

  那么对于这条原则**我的建议是**：官方示例具有一定的指导意义，但仍然需要特殊情况特殊对待。更好的一个解释可以参考[MODERNES C++](http://www.modernescpp.com/index.php/c-core-guidelines-the-remaining-rules-to-performance)这篇文章中对这条原则的分析，即用std::vector和std::deque做对比。🌄




- to do