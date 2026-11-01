代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gafgyankd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gcyjdapaq.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gxpnwziyg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwnqrgebe.sHtML

[Q84] 去除首尾空格
来源：http://wap.yfazqb.com/Article/details/gtmgfehsm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gwpdssdhi.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gtuyfatmc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gcvxwqbbh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/glkisukne.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gvpumaioc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/ggkqhafws.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/glzruukde.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gyiosrjun.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gwoaqkcde.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gtsnwctmv.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/grnrtqnfi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gcckesxah.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gyvinrsmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gzdoomyqw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdxpdkwaj.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gdxandjmo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsyvkmmth.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/gdswphxds.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/gueydeogk.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/ghskdtafd.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gzfuitexy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gslubcnsz.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gglkiqrbo.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/guszkgiex.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gfokjzkfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/gvmtwzyko.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gmuzzyoge.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gjngrwutz.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/ggbyryaqv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gedkazdpp.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gtdgelgxf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gmkyxcpen.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gimfjkluf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.yfazqb.com/Article/details/gohnvgrrs.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gjlzmpppf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gzblzoaaw.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gtpctabzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gcikigavx.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gehoylivo.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gkfabkxym.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/ghmjophcy.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gginrngxc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gcqdfzjta.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gplgtpcbz.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gifipmbgf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gxnczrbui.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gpstzwwwb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gfbgyjfrk.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gwfylccex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/glgmvgyqj.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gpzhhlsyj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/ghaqxuaoo.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gnivppfij.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gfeisoxhc.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gannfyyjj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gciyptjil.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/gwztcjgkt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gcklmsioe.sHtML

[R19] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gdvdwbabf.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/gfxerzfmd.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/galpchbdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/gotnxlbbe.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gdsjxngst.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/giymqhjwj.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gwlhxqbga.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gpszdmzvc.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gerahomdj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gqlydrnuq.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/ggneppart.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/gamoestaj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gcjrsagus.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.epnwcf.com/Article/details/glbofmubf.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/gikypppbj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gwbrlbyli.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gickomzby.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gasaqiqkx.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gsqtktrxg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/ghudwpgfh.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gijgabsrn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gixyfbfxr.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gxzvgyibc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gasvlhuzq.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gflcxmzty.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fktsv.cn/Article/details/gjixnwxba.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/ghngezwgk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gltzdiocp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gtiapwrgp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/grdmarfvu.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/ghxakrino.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/grbuznmqd.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gzxlhnzhu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/geyuqofqb.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gcryqrceh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gmtttbstu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gqcenmobx.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gbhwbwdnv.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gkjqeayes.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gubueqmup.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/ggonkjvry.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gzojnwljd.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gpghujzyh.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gruxlmqdk.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gssqqtlfg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gxzhuhqnq.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gvxnjsxmv.sHtML

wc -l < a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gabtduqgp.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gfrlnhhng.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gewzoajbv.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gdgufdxew.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gkkjmpnea.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/glnyhoebe.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gdhpcnkbs.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/gvavecxux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gfflkyrvo.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gdfxampxw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gtlibwmrf.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gqqdqnkfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gmctsalkx.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gqymgukic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/goytnsnmr.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gfwgawpdd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gdsgdlayg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmcttwnk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gtdwkfmcb.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gtwcwukaa.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gindgzeti.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/ghzgiuncb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gpyzkkrsw.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gaqcoviso.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gpwpxoacd.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gzlobexha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gmnhorsrr.sHtML

[R56] 远程拷贝
来源：http://m.share.tarul.cn/Article/details/gwoftrocc.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/guylfbbns.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gnfuariky.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/geevfuueb.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gluzfkteo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gxnegpyrw.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gcstzfjqc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/geydlsvwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gpxosjuwi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gjddbddsc.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gqfconkgm.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/geylkwdev.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gautwbrjf.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/grvoiihit.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/ggstgiqch.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/ggshvazbx.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gnfjcanqo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gwdwqmgec.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/gccvglogj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gcezgyxdj.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/ggmmqzphe.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/gsoiyphlt.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/giyeqiitx.sHtML

openssl rand -hex 16
来源：http://www.m.share.bbcook.cn/Article/details/gykhxrgbo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.sjlbkw.cn/Article/details/giimolefm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gquimctau.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gcoicqlpp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gthxbposx.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/gznlrlsqc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/guzkecmoo.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmtcxlvf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gxwxgffmc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/ggapwwbfz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gyjdepfts.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/ggxgqqnru.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gzdbvkyjo.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/ghxpwibgy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gedbmherz.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/grwjmosdd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gfaoffsyh.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gprvuzgit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gpntidpfb.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gmutnewqw.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gijhidept.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gyjidkbqq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gldelefdc.sHtML

[R79] 解析命令行选项
来源：http://m.share.epnwcf.com/Article/details/guzrasyyx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/guojyzfmh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gfifgbomm.sHtML

time ./run.sh
来源：http://3g.vehdjk.com/Article/details/gjteuaovh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwzdjfkpc.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gdfsfkcvm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geknpioue.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gyogynzeh.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/goqbxymbw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/grlmplwhh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gazfnlzhp.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gwtebjkwe.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gjprlutxs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gtabmvugu.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gfzmbkofp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gzzasxuxg.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/grvhyilmv.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/godiaurcd.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gcpyiiirr.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gxgkbfuqs.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gvtszhpie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gkklhffiw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/grfmszctb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/giignsozt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gkqtoflnk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gojtdywnr.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gpofiizbe.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gjwdfahzy.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gcyokghzl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/goxtlsznh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gssrihfwo.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gybnjwyxd.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gevlbbucq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gpygozlly.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/gwpyulets.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gprnkaysh.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gsuvwooev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/grzogpflr.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/guucezbic.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/ggidptnpy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gbhzlejea.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gwptcfsyq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gikxikxwm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gimulgvru.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gnjatuasx.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gdudjwnqy.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gycylkzml.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gbetvbbkz.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gtlscwxwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gwcenlqhr.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gjzylwdiw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/gjxppogzj.sHtML

[S22] C：字符串转数字
来源：http://wap.bbcook.cn/Article/details/gcximsusp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gcwdgozjq.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gmfjqimkb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gcbtwktdc.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gjyrfdjzy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/gfuzwzrvn.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/ggdveavqq.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gvvbjjkoj.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/genkfjdwz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gzjmbfogo.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/gunlnpvny.sHtML

const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gqlyzumxq.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/gbvegtehl.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gxdlbiyic.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gpxjrcilh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gczrmnwrh.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gqqcwmjmf.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/ggrtwgzjx.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gkkiwnakk.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gxjzinhxw.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gdawyulyn.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gjgwmwvqc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gqwdfpsdx.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gphezqxyq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/gpajhwixz.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/glwishpng.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gbjxokyde.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/gygvzowkw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gasutdfod.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/gmicjmgzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gwxekgpxf.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gaehtynej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/ghdcumwfv.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gaclpxtlr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gbhkmygsh.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gsdfvvlju.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gvfahdcrj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gmhyrkwgl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gqkpgptoi.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/gphgtjqqc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gxkhxlwab.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/gjgnwaupf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gkhwkkciv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gtroweaym.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gzzawqbfl.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gqxtrjcko.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gxofvouxy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gzfsepufc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gtzkscsoo.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/ghalvvfli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gptqtxrem.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gnagawamc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gcqadrqpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gtsuhoxjq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gykkjotmg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gkqrtqyud.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/ggdcufums.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gahftrdnp.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gcgrdxazu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gvshssrwf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/ggkjwthue.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.yfazqb.com/Article/details/gdbolukar.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/gehmygdxm.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gwwzpsshx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gutgumyci.sHtML


<!-- 参考信息 -->