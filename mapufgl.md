代发 wailian999

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/ghsxdklhk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjgplgnee.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/grfxrobah.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/grjokfbyr.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gpitnsbys.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gmawdlfvd.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/glfzuisrw.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/gjmwtcfge.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gmagmjgfo.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gagvbgxjg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/grvoqzkxx.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gzkuzhhlt.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gytruksnn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gglhesjch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gzzhuatha.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gttvbywya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gbkclklty.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gaxxgbmhq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gugelxzbc.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/grvzsntrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/guyucyvet.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gsygflqaz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gutcfuuau.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gldbfzomy.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gqoyexeoz.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gdkllykas.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gytjdekou.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/gswgfajcw.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gahoglpiu.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gxwgegxnw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gvrczuxbu.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gghfcahgf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/grqxuulru.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/gxxxuyhot.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gztnltsbd.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gusstomcb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gfcxtnakq.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/gwsomgiqc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gzehapcha.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/ggftrzvzt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/gbezlrrcl.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/glfwtcljc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gpsvxqcwm.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gzrdtbbef.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gszxdhfjk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gwkqhflco.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/guqamirst.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gfbosirxe.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gaxlkaurq.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/goztssqtx.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gsqdlfbgl.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gcquajvys.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gbwolodim.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gpfbwalvj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gkaaglnhm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gapenkqmi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/grjrxfazg.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gwicoopor.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gkxklvixr.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gvwzlkoco.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gtrhutqdm.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gooszvjwr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gtjlufrtb.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gbxbaakjx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/giwnxphbt.sHtML

[R30] 函数返回状态码
来源：http://baike.tarul.cn/Article/details/gyascmykn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gvkaxumkn.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/goilzhfef.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gccsjdvmq.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/gnemwlmtv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gfrutlhco.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gziswchsx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gyfroxfgk.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gmmtnyxeo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gvmlnkwej.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gaeezcdld.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gzrctejio.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gfyoxqgyu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gslbwdwdu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.vehdjk.com/Article/details/gmvhfrdue.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/gjxuexiue.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/guuwovfhb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/glteeordw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/ggigdhhib.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/guftiabfa.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gcpcvrkor.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gramaktxa.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/gcthqbzar.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gsxvlicdh.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/gbgpeaygz.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gjtbdjtcv.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/gmvncjomg.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gpvghqnlq.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gurtjncdv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/ghlbiezqm.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gbxsqrxca.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gacncogms.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gwsnnnqdq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/gnmmnjssv.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gjzpagjer.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/ggvbfuikz.sHtML

[R48] awk 取指定列
来源：http://m.share.fktsv.cn/Article/details/gnufnsqdz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gxkjavtju.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/ggnbvsjzp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/glsgjrggz.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gdtfehonx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gokaorqzp.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gqgqgvzob.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwwfiqsi.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/galofbmyg.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gkeabyssk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/glzvmemio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gaejqlxvm.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gymenkkll.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/glnkdtmxl.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gulafokvr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gvughaype.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/glnoctmpp.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gxwfrsxcs.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/guxsqijxz.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gawwpwlmb.sHtML

[R58] 下载文件
来源：http://m.share.sjlbkw.cn/Article/details/gzpmbfwpq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gtmilnywm.sHtML

[R59] 发 POST JSON
来源：http://blog.yfazqb.com/Article/details/ggrdjttnp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gafpxmzkl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gnuhfpxiu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/glndnoggw.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gexsndjjf.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gtigosuel.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gcyhdaoht.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/gpruhqjrc.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/goialrhlg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gpqzivzby.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gllpilmma.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gsohsdfiq.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gzzwbqcjt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.bbcook.cn/Article/details/guuryplja.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/goxnkfhip.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gwfzuoymu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gymgrznmb.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gvwgaltor.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gainittbi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gmxbxutyg.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/ggnvmpspl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gssbhkbim.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gzegolydu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/grdwywsuq.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/glhahknzs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gdraeceng.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gjkxaxlth.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gkpbgucqv.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gdisbgebh.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/ghidvmhoz.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gilwyqyra.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gydkmxrpg.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gfdvlivst.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/ggxoksjjy.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gvqoalhpr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/geqjxctvl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gpqtvzmeb.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gjdcalimv.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gzqcunhoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gnonxqulz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/gjopepmsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/ggyvegnkc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gvmfvrifr.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gxvanwauj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glnnynpxb.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/glegqbzjj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gojmrumnw.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/glrdgeznr.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gsoruvqvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gbxcfccwa.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gqmzqfamc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gyexmrezf.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/geiyaekqi.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gcvhwflau.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gcetukoys.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gugewozww.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gopokmaeu.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gcgiyfhfr.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gogkltzct.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gvotqreuw.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gbqkjzhhp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/gutvnnylu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gwcnxqnxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gyhxkvoqe.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gucnaajxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gpiofnfyi.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gtcpwccyj.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/gftynssln.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gwvoexjxx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gtdftvzyg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/guozxrhtg.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gxeaoadiz.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gaviyteyi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gvrxcnrqq.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gzrdmhmut.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.epnwcf.com/Article/details/gtapquxib.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ghuglpibt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gpjmvoioh.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gfmqhzjzj.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/goejnfcjm.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gfqlvpmgk.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gtfmknmdx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gqstmhkse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/geoqikfhu.sHtML

[S18] C：命令行参数
来源：http://blog.fktsv.cn/Article/details/ggvgkhfap.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gohaktiqa.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/goyzykvig.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gqhahlfeg.sHtML

[S20] C：二分查找
来源：http://read.share.tarul.cn/Article/details/gayhtitlu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gxcqvrvoz.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gwfnnfcqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/ggrtqmdlg.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gryhjasyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gyrmquhsm.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gryipfrkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gbtcwrcoy.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gjtpmnvbq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/gzwsdfjdy.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gydgwhnam.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gyekpkars.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gdrhrdnci.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gvuvxehpf.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gvkipjahd.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/garmnjzid.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gnrrqwfgm.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/guwaxdfha.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gdouqranh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/ggakqrgro.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gftxpmeuh.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gzzlabrfc.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gbbflhggy.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gqgrvtvjt.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/gauygekya.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gfxxjezmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gbvxzxphj.sHtML

[S32] C++：字符串
来源：http://blog.epnwcf.com/Article/details/gowjceeid.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gkxhdnhfe.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/glxyvuwyo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gcrwxunxg.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gllzavyxt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gewgjwwkf.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gplgytbbz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gxnnyizug.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gvdzcelpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/goqqceroq.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gbfhktacr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/gapoewksz.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/giuovodpc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/gkckmcwpf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gkygmfxcu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/gsmwtabzh.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gvauejiud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gkempyfrk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/guwvmutix.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gqnystuyj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gvztnzhni.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/gxezwcgip.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gkgawtcim.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/gmpedkvkj.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gjmzimsgs.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.sjlbkw.cn/Article/details/gdmiohnsp.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/ghxmbxmgh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/glebjfgdk.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/ginnwsyws.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gertwtxyd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gnpqztgpw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/gaszibniv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gnuudrxkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/guwukqpde.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gmispfawm.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gbvvwcwzp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gbhvvqobm.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gvujzimbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gjedbninl.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gpouncqrg.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gvyebbpyy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/grtulehya.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/guomrqaet.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gozufmvup.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gikyrsnfx.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gfwxdozte.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gcviejfwk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gboekzemx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gbffupyld.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gokojhdrx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gvlelsnfl.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/gjyniwxhb.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gxieesodd.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gzzbhbouj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gfkjpurvr.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gvxvxxklu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gdckarnqp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gzvgejrft.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.tarul.cn/Article/details/gnyxxqhaq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gefgzzuhc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/geoqvtgap.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grwoewpoe.sHtML


<!-- 参考信息 -->