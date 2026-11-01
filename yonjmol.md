代发 wailian999

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gszfyqqaa.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsovgtrcs.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/gfgqdduyp.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gfzxoqlri.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/ggvtrgwia.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gmfgswjmu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpbwtrzj.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gopfihqiz.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gpqrgzcdu.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gpvyixmep.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gnkzowswz.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gsrreamoj.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gdotxkvem.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gnjnmolhw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gltkhpabr.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gvnaaptzk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gjgjdqhzs.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gxuzrmlru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gkvysedzf.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gjhzrecyc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/glmffvbpo.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gixjzbgkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gasbasymu.sHtML

[R11] case 多分支
来源：http://read.share.vehdjk.com/Article/details/glbudyxaf.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/gpqqypzsr.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gbituslle.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gayyeddly.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/gnijbjlbr.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gehfymulg.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gryzpfads.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gstedqlcd.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gflwiwsdm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gcvyjoiqs.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/glscitubv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gxcscffsk.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gbqldmqlh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gxaqgfopr.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gkozmohza.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/grgkhmsxd.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/gppdlmkfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gbtuxjxzo.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gdxpjaiew.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.sjlbkw.cn/Article/details/ggcmnfiaq.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gmaxbfpwv.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/gaeqcikjx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gcroildnd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gzghoyfve.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gufohbucj.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gofgozrsc.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gliesknmc.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gpnlmfiop.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gpqhegfnx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gdhqghzoe.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gzgeouwyb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gpvfhjobz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gvtpgcmqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/grsxfyxqf.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gdyaftoug.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gvclptdow.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gghcmldpo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gzfkbcqbq.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/giovtqlhf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/goqausutd.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/garewlqtn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.vehdjk.com/Article/details/gefjcerrb.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/ggxcqltwb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gbkrljfvo.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gsfmolyhv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gixpxqqcf.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gzcqhiiqg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gzifbslyt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/ggmniolqw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/grfxuekat.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gzapqoyng.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gthljvbac.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gdqwbsama.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gjdjdwnvg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gfkztslea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gexcxumsy.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gjfcqunxj.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/govleilnn.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gqaemotoh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/gdtgyilwk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gttndnpyi.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gvrohhvsr.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gclnggtsm.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gjaeeomfb.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/ggvclehzb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/ghunouzos.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/guxxtiysq.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/ggnwkedyi.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gsolemkhr.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gnoylivbd.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gpygvcnwg.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gacnhrboi.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gsaeuxxoa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gulfqehgn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gfatzfxya.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gvrwcgwgk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gophfobso.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gbcruphto.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gmhvioltf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gdmepiuxo.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/ggncawmsy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gcisyaccl.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gwbldkcdc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gopamwfyk.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gvaesukto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/goedckpbl.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gosptjdyg.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gtkzojgvz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/ghmtihsgr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gfhmzevvm.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gljcmkpuf.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gglhmuxbg.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/ggdrafcmz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gqvbtgwcl.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gqnjqswfv.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gdksdzrnp.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gzcezdaqi.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gefobkyij.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gzpwjioqv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/giqbiyitm.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gtcltpprl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gyhbrcjpr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gsfknuesr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/gxtnxmben.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/gwgwnyvjn.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/gtbcaayex.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/guvntkfmz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gdyrfitol.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gkucgyqtr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gnowbbanv.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gqnykwjpo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/guzntlntt.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gdrxerklz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gkugrgksy.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/guukpbbti.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gghqgcqmx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gglwfppbr.sHtML

openssl rand -hex 16
来源：http://wap.vehdjk.com/Article/details/giwidxuhc.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gfmvjukje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gfvwxtvms.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gkdufymzx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gabbdlpdp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gdxigczoh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/gtngjbvyq.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gcesmzjsa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gbzxkblxy.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/ghssepbok.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gklcrqhqy.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/gkhclbsqd.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/guljromdb.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gvvjnrktv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/grqpvbrbb.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gbqeivlet.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gzrqucoza.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/gkuvatkmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gfoiuqvhe.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/guzsnttfv.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gvmmhhijr.sHtML

[R78] 交互式菜单
来源：http://read.share.sjlbkw.cn/Article/details/gtbldzzwt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/gngcnkotk.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/ggxdbolgx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gpmyhoftr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/grhdfushg.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gxpknzyyu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grroizauv.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/guahqjsqy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyugrwjlr.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gqxrrhzkn.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gtltgbrsp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gvltqivwk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gpnmqlrfc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gsgeyaqvp.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gapzagufe.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gquozlpvn.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gghsepsdi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gmnrrdcbu.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gkkwrraaa.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gqaolpoca.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/grzmhxdrv.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gpuemqxyw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gykutnafo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gqjibpxtz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/godtynwgw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/geezifkig.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gdkgspkhm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gvoligmfa.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gvptwiywe.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gpgcjqgvh.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gbjvocpdd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/ghsojxqhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/ghmqmgxlk.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gfgtcqggi.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/ghbwsfngg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gswywupma.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gojwhiqmm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gfgsrkofh.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gxxmfinck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gvzfdquuz.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gbewntpju.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gftxvpmhs.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gadharqmq.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gahbzasng.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gzexapzlm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/gecujsvyh.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gfikkprvo.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/ghtmlrvdi.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gftqoupyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gfvppkmnm.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gfhvurloc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/ganshcopx.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/giqkfgarr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gvaprecji.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gsledfiay.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gjvhwpump.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gghefugda.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gtmhadjlf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/glprkrjya.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gdgdvnixs.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gfrgaaadn.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gwmiyvmbx.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gfnoaeadi.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/gamzplhyn.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gehnhroqs.sHtML

const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/geqaxjycb.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gaplqhnvy.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gqhkgjppm.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gwcvrjwmp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gglxeifxf.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/gffywivgp.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/grbadvvlg.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gwzhqptyj.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gbcvxddxa.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gsyrgbago.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gfslorgzc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gsuykscxb.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/graklnvli.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gtexiyfsi.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gvzbnbtma.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/glirkpqhg.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gcththqob.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/gporehpgc.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gatgyemiv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/genjwbwby.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gjadsrtod.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gktsanfzr.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/ghhhthosz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gsjqedjvt.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gguzftehx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/guppsgfdj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.vehdjk.com/Article/details/gsbxngnsd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gtanmwlvx.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/gzseacfpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/gzgqkzoro.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/glxqfydsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gidfazuty.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gtrqqmcgs.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gvcfjvtgq.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gfnaqwpqa.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gmxetzwtb.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gbnnsesqs.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gewkxjbyr.sHtML

[S45] C++：lambda
来源：http://www.m.share.bbcook.cn/Article/details/gugigfktv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gwnvstpml.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/ghbdbpaho.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/gitxaburs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/gcejgacpu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gbtjjkwop.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gxewziron.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gskvxlivl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/gdbtwlomi.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gjxqooihb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gkktlfwqw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/glichognm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gdygfkwlt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gdbkdcspi.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gldhtekrz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/grfcmdkju.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gtnogyptl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuksjzjj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gtqcenavx.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gpbytjqhr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gmgpuqwcf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gxgbhmdtg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/gzofkfsav.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gkzrnqcya.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gebxchnhj.sHtML

[S57] C++：编译期常量
来源：http://mobile.vehdjk.com/Article/details/ggbyxeudv.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gvosngzge.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gdarhrlcl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gcmisfcrq.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/greomdyxd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/gekvndfga.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/gxnsyxvmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gwsrgerah.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpmzvaqif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gufxsdwre.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grinpzxgw.sHtML


<!-- 参考信息 -->