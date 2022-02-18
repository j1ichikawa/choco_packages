# 除外指定して残り全てをアップグレードする場合

## 下段の要領で除隊指定対応が可能らしい
choco upgrade all --except="'skype,conemu'"

## choco 自身ののアップグレード
choco upgrade chocolatey -y

## アップグレード後、デスクトップにショートカットが出現するのがウザい
del C:\Users\Public\Desktop\*.lnk

## タスクスケジューラでの実行部

    <Exec>
        <Command>C:\ProgramData\chocolatey\bin\choco.exe</Command>
        <Arguments>upgrade all -y</Arguments>
    </Exec>
    <Exec>
        <Command>C:\ProgramData\chocolatey\bin\choco.exe</Command>
        <Arguments>upgrade chocolatey -y</Arguments>
    </Exec>

