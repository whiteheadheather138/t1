代发 wailian999

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gerujbblc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gagsohnhv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fktsv.cn/Article/details/gfpvnaxqp.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gwgbidbeq.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/guwilfgod.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/ghhvtnuyt.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gpmccagyt.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gxbgtpidp.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gatcghqty.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/gtzdiydhu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/giymoqjvp.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/glkowklzx.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/ghiyvhzrb.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/grohfyupi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/ghvrbpzvi.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/grhizhnoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/gormkjmyb.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/grqjpdvwh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/ggzcwecks.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gtfebqpwn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/grbitsrcs.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gwjdtrfyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/geblsdbnr.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gffmyfjtt.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gpslsxxbf.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/gqlbnwikd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtckeozrx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/gvpwabqzl.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gzxwpjtht.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gbvgrtvqw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtdevxlm.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gvtqndkcx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gxdcfcxqs.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gjgawyxqh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gnpjwswix.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gafibplym.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gdfwbbrxk.sHtML

[R16] until 等待条件
来源：http://baike.sjlbkw.cn/Article/details/gddxjwpie.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gfsuhbrfv.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gjzvjwdmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/gjhkxmvoo.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/gkjpxdmqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gtqgdwwrr.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/guqvusqll.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gcwaklehq.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/ghxovjeup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gscdafwxf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gnqmqosye.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gnjjpyczu.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gcrcprzoj.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/geepyagvu.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gqtelktqz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gvflylluj.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gwfvzraos.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gdlaxjfbw.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/ghdxrnohj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gopewoteb.sHtML

[R26] 命令替换
来源：http://mobile.fktsv.cn/Article/details/gyrzlxbvk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gqsculxcy.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gypmqbwra.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gdyrencue.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gdkoyeobd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gjkdpozwm.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/guyffxqaf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gzyhobhxa.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gsbrxhdlj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gvrmhrqfu.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gimpmsnig.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/goscdwkvj.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gxkcuauuh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gmgejaqgh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gcecccvxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gqqghnzit.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/ghqdkmzju.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gukeknwbr.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/gtwwtfxeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gfiyeftrv.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gyzrdoods.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gporzwkgp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gfxpnwsse.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gyxxddeaj.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gfpdaorjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/glhgiayny.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gmnxuhkyu.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gioynjkzs.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/gqjrhlwvh.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gmcfhcdhf.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gqwcduuao.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gidbhapwg.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gjmpoxaob.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gcnexrvix.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gqhlgabnh.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/ggfepnmwq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gsyseteax.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gjwictnil.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gkriamdxw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gpavspblw.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gvaxxmxai.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gmvpqnlpx.sHtML

[R47] sed 单行替换
来源：http://m.share.yfazqb.com/Article/details/gmbbpvnao.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gciiycppw.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gseglpako.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gxwkuknfo.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gwvyslgvg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gtjlwyyis.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/ggdgwurnb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gumwuonsn.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gvazpaynk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gmkqgpynu.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gpgowcvkv.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gswpqjedj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.bbcook.cn/Article/details/gwqogqhvv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gxmgaskxa.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gbcprgvej.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gwhjuwicz.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gkjbxuxjq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gztxaqajv.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gijjclhct.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkcbchvu.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gvvncqzyx.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gyxjqrdwb.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gwwlajxfv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gbzbzxpiu.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gbvgwwqre.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gldowwvlo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/ghhfvhoqy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.bbcook.cn/Article/details/gnofmyoad.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gorcayged.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gjdrgyybp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/grmxgtcbv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gsjldfvhl.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gzlgrsmtw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gkdekdjfy.sHtML

[R64] 结束进程
来源：http://3g.bbcook.cn/Article/details/gqmrxldxn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gbcwqmwqh.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/gnhylxpad.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.bbcook.cn/Article/details/gkfsvizps.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gxboblagh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gwmseoeyp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gycsqriek.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gdpljcwty.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gmthhbbzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gutumwtkb.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gminkmzig.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gmrihmwog.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/gznfytdym.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gkijdpyff.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gdkvyozxh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/glpvwgfox.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gjtbjhffn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/ghvmqebta.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gapwyfaqb.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gqgiowzmv.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gcnoinuoz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.vehdjk.com/Article/details/gmpviahby.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/grxtpwbut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/glvirdypg.sHtML

[R76] 使用临时文件
来源：http://wap.yfazqb.com/Article/details/gvooevnyp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gafofkgeq.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gtubpdukp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/grhkejimo.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gdxhfvile.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/glgsxmarv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/ghfadauqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gbrmdhrbi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gorvohlsz.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gwrchblvs.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gipfcjjxz.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/ghlpvcbbg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwsgkkyay.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gaevtymwo.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gypdipxan.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gnmlujook.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gspkjnpum.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gypwcrwsc.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gybfifcou.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gsbeljrlx.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gnkbdnbrx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gkiwosqnz.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gmmkmkzei.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/gkectklzd.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gedsiewjz.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gvuotdefi.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gjmpvqgvc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpzytbkj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/guwxibotv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gchpribwh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gqjilbagc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gmdasyquc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gkplpabib.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gwyrzzazb.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gzpuolpun.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gwfahypbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gekbzraiw.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gjporxidb.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gutttfyre.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/gbfvopmms.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/glyyftinb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gozxxonwj.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gucidabpy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.tarul.cn/Article/details/gnveplaod.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gywsmtlpo.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/ghsizwupl.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/glyfhfiak.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gshoahapb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gofetlmwr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/ghxojfcgv.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/gilyvzuwk.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gsrxlycno.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gyexplaob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/grwruvcun.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gfpwlenjf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gfucumohk.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gmdjcgqpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/govfufuqt.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gyyjpctqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gufzwffjn.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gjwaijylr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gdupsjglp.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gbyjbewck.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/glgmvlvam.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gkalqdzln.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gvnblgkub.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gmcwqblyz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gzzsowqiy.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/guiwolqmj.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/guzkowwoc.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/ghvlpiiuj.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/gquvjrfxd.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/grgcjzest.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gnqgggjjm.sHtML

[S30] C：头文件保护
来源：http://blog.sjlbkw.cn/Article/details/gbhznarqp.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/grdembfyz.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gzayvticu.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gxngjseis.sHtML

[S31] C++：Hello World
来源：http://www.share.bbcook.cn/Article/details/grjrxmxmr.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gxxfdqicz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guahziwsz.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/goqoqnbwx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gdeearpyh.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/guafunlyt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/ggkqwuynt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/glojfdxzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/gwepmfqeo.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/gmumzlqzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/grnhngkdk.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/gelakfrvx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gixkmnone.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gokcydqbs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gejplyvbv.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/ghxrjhfis.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gvniqrqym.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gxorcvsdb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/gobvymsad.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gewycoqvw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gceegsalj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/ggwikheza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/goclulupn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/garramako.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gbfctgjra.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gnrowqqqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gtspfesjj.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/gxggsbrrc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gdkvrpwpi.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gaylkyftc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gafrgbxzt.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gzgypguzo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gscuhhvyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/ggmiudgjy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.epnwcf.com/Article/details/guflexvcs.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gukgwzubb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gkbzpfqww.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gwzhdpnxc.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gfkrewpge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gxbgbzssq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gzcagoykc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gxbtkfgcl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gqdbgovnf.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/gziivwpfh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/glrxlrdfx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/gdzrxrdvh.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gppaieili.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gbnfwbufz.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gxdpphjbu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gjugoswhw.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gzyomsgiv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/grzhtpksa.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gcpazidog.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gfhtpokmd.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gjqyyyxyt.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gizpiulkt.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/guoingtzj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzmvaprs.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxchzipw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gnrdgtdco.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.bbcook.cn/Article/details/ghdfqphgm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/geojcalij.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfzagecew.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gwclntaew.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggammjoda.sHtML


<!-- 参考信息 -->