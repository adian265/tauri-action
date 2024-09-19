@echo off
if "%1" == "h" goto begin
mshta vbscript:createobject("wscript.shell").run("""%~nx0"" h",0)(window.close)&&exit
:begin
REM
tasklist | findstr "modbuswebpro" > nul
if %errorlevel% equ 0 (
    echo 进程已经在运行
) else (
    echo 进程未运行
    ModbusWebPro.exe
)


