代发 wailian999

R. Bash 专题
来源：http://mobile.vehdjk.com/Article/details/gusadfjnb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gflqbtbvf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/gojyuvmwr.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gymfrpkhh.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gwuewbpmc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/guguhnuoj.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gklengtbh.sHtML

[R03] 只读变量
来源：http://m.share.tarul.cn/Article/details/ggizptqjg.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gjahqcmka.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gsecsnbmt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gswynlnpp.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/gzcczdavn.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/glejquozd.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gnucdlwvv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gjpqzlonw.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gjzrlodtk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gjmndsjot.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gnrdaetqc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/ggxljciag.sHtML

[R09] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gpltftmal.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gbdhagvgc.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/gmgkjuixb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/ghbozanpf.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gdhqqdntc.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gslhqxsfp.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gkmztfitf.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gvpgebjzx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gcfchjuzu.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/gmjfdftzp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gtaskkijs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gaincchdl.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gochorbvn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gtbhyoyul.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gdcynfojv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/goatcbpwv.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/ggeaqrwtd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/geksmmydi.sHtML

[R16] until 等待条件
来源：http://www.blog.bbcook.cn/Article/details/gmbhntnxt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gdecyxjzc.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/geshalxvo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/ghcdtpmgc.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/golgqklum.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/grhnmsjtp.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/grsniwutw.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gvoxunywc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gvhuqfcoc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/geqxwfhcr.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gziyrrodb.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/ghlchzhwz.sHtML

[R22] 截取子串
来源：http://baike.yfazqb.com/Article/details/gmqiftgbb.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gbimrvxiq.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gyovssirq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gxepsvsey.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gmwnboczd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/grcwcggmk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gierkzlqe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/ghqejwovb.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/grzsousbr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gvjfyrpex.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gcrqhyasw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/gixqqvfhw.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/glrfjdcsr.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gqawnkdro.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gmmmsxbgu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.bbcook.cn/Article/details/gcfprhyqy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gifjfbjxy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/ggcvsutso.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gqcykinxj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gqvgnsoch.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gjupfffyi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gqyijfusd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gicyklagc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gomlccywf.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gfelxhcnk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/ggrzxqegc.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gkgqfylht.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.epnwcf.com/Article/details/ghozxyhbb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gmkjjntsr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gzvqoigeh.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/grzdueane.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gcemttswl.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gdmxlkabc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gyqflomwp.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gwfvjpnoz.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gaegwhcvb.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/ghsdbvgye.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gnzsosyku.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gpsyrdvoc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gyurxdobt.sHtML

[R42] 输入重定向
来源：http://read.share.sjlbkw.cn/Article/details/gjjtwxerl.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/geumndtya.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gdmhohahp.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gwrfujehm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/gdlqlzimf.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gnogoorqi.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gtfufdvqw.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gnvifslnp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gebettons.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gndawsjny.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gusxuaddr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gmgiwowyp.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gjqxldmfl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gnpznmzsn.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/gkraajqpf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gkaysozdr.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gzynocpfs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/glcqhqjwj.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/guozbejwf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gsjytvaiw.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/gxiuquakx.sHtML

wc -l a.txt
来源：http://read.share.bbcook.cn/Article/details/gezjejueq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gntxbjyix.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fktsv.cn/Article/details/gzekljite.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gekuvjwmy.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/geopdjajm.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gaamzehrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/gwjqtdzko.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gkbdsshzx.sHtML

scp file user@host:/path/
来源：http://read.share.fktsv.cn/Article/details/gryfvddlx.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gvjfhquha.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gjflojvat.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/ggvbwszda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gbxipxnby.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/glxmurwyi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/ghcspjrwp.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gjdbehefe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gxtvwqefy.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/gnoaklhvh.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gxsozgjic.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gkixxynlu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gcytgtyit.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gndeyuhmu.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gbvyuownz.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gfyiekzie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gauwmwodk.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/gnkixpwml.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gdeqyeyyp.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gajkihzrb.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gadjtzfpm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/guidjigkc.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gfhpehcgg.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/guhkwdype.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gbmxymahl.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gdzsloozn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gvvsaehag.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/goytqqrrd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gwstvegtw.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gwfbgsqxe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/geenoukum.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/glnaommuz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/ghctgtgwf.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/glohktvfp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gqhlurgnz.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gzgmfeqfn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gshknxemt.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gfzgrvexx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/ghheytsbg.sHtML

[R76] 使用临时文件
来源：http://baike.sjlbkw.cn/Article/details/gqdeohavf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gfqdkguff.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gsvcgdyvu.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gdqryslpn.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/gpcsowabd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/ggabxkbgl.sHtML

[R79] 解析命令行选项
来源：http://mobile.sjlbkw.cn/Article/details/gyyjmggdu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gebempspe.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gqstgbufb.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/gtwqglmfr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfmcygemo.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/ggdqywmvn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyueqrxbg.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gqswnucnh.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/gywlmhmbc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/grfokspom.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gfberchia.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gkiftzuof.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/glucnsxzq.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/grvdnhdkv.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gzqobtvio.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gzhawklsa.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gilffbqqu.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gvoewtupq.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/guizaxiwk.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/glbswycfk.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gjazmrqug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gemugwhuy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gkuwckhnh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gcypzabun.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/gigsctxde.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gdbjmhcio.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/ghullwnoo.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gqtpsbyvj.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/gcfhjeujy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/ggkpcilpv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/gnxlnshfq.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/ghqbtzpvx.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gbbzpacxo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gvcpzrduw.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/grscsrryc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gxgujodbm.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gxvkqvmbj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gcmyowfqx.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gxicjejlr.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gcsxybmjc.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/ghtkopbpc.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gfaecvxnx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/guphpqtsz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gytomqlrq.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gttvrpalp.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/gdtzrabrd.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gvfjgkesz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/ghphpxdyf.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gerojocdr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gerlijqwb.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gyqaqzqxe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/gqwzbjjmw.sHtML

[S22] C：字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gmwfptwnv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/gxjvbgrgb.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/glkltwnmo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gfozuogro.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gczjwurrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/goeymlrym.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/ggrowxbvh.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gbysecugn.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gprpbctgh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/gtjnulzdb.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gdaciecym.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gddhcwxfq.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gdcmfrucg.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gnqaebaas.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gvdrndnxi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gqmclkjck.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/ggicxbbou.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/ghkkvbtxf.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gjjzjztng.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/ghjltnksf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gtpuyomba.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gjabiohrn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gxpdwjqzs.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gtjfwzhpq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gjbkvjvzu.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gzugmjggo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/giqvwgxca.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gdsryhdmc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gifbvbpdx.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gonfgyibn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gjxanlzpr.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/giydzujbh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gijxuamur.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gqvgfbaah.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gjfrgsocp.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/glwnkhhli.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.epnwcf.com/Article/details/gyerxmocu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gfkidsqhs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gwfvcytcy.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gqtfxhyfc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gbowectew.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gevrnqexy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gultzntak.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gobghyyme.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.bbcook.cn/Article/details/gkpojnstj.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/glwoqltmv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gzovrhaee.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/guyymhnmm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gqhlvnhap.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gthvdppgc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/grzqfzdnw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gerlvdnha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/gnczzaors.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gidbwbsay.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gcfzegxkr.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gnrualyxr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/grchturhy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gbdmvityx.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/gjkgmuqaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gcdelanml.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gkrkputlj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/gnzvjcllc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gfkgfnofq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gvefmjtva.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.sjlbkw.cn/Article/details/gnaobrgws.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gdimbkbtd.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gcnhswbos.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gnbiuhhgo.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbargkix.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gxclboeem.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gtexwbcyq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gekaxzyhz.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gqufonklo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gnvbfoayj.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/gpfmyhsrc.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gtciazqrv.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gkpkrespo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gytzlwpqn.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/gkzoacfed.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/grxmrbgvi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/glcendjvr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gmbrgcfbj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gawsnssdj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gbvfwthmc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giisgybgd.sHtML


<!-- 参考信息 -->