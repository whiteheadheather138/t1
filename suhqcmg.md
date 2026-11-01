代发 wailian999

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gwibgufhs.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkeholywi.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gqakdobhe.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gcguroxxs.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gdcwyupev.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/gupafkejk.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/ghqidmcth.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gvprtkmwi.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gouykhplb.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gofbftcsa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.sjlbkw.cn/Article/details/gsanaaiul.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gvhzpjyqq.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/ghywnopht.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gqlxdasri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gbtkqzjeu.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gavcsgxns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gyuxxtajv.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gheekgpiy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/glfihfwew.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/ggkcidxja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/geqdmziui.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/gdyvrpfjw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/grgeadcnf.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gfcmmahht.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/ghqaltuof.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gvnawhcox.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gdtfofogu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gkrbbjwng.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gttdvqqpi.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gtxhiaqpq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gkqgsxiix.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gnhvweqgn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/geebwavgl.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/gjdbezoqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/grkzvhcwf.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gidvvuqkl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/gjapengig.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gwjqzklxp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gtkyodlhj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gpxxuespo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gssteknrs.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gsqnhtorp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/gxqxkphsu.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gtwuguytt.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gjyvrtbrp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/glrpyqaia.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/gedcbitwi.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gwjtvzxev.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gguelnotl.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gawzrorqq.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gpwguyrcj.sHtML

[R23] 字符串替换
来源：http://wap.tarul.cn/Article/details/gubzentur.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gqcqjpojv.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/godadshzm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/glogdczgz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gdooiaqru.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gerkwkjhi.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gcozeifwl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gxnupvanf.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gqomvnteh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.yfazqb.com/Article/details/gwvubpdwi.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gtlxijnyh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gevxiptwi.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gfoyaytxy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gwuzqxmbj.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gkdbfvuek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gauycykil.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gsfzvlyhi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gtpvspmlu.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/geklinarm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gdbatqjwu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gucrqznkb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gvvjhklzp.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gtdcjjzrm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gycbcyvyf.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gliotqtic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gqksdsjvj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gsjetkrse.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gfwuavpno.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/gfbhyimip.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gxmuowxyv.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gviwghunn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gezljfqis.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/glycwcuyj.sHtML

cmd > out.log 2>&1
来源：http://read.share.fktsv.cn/Article/details/gidogrwim.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gbmstbdpr.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gtfzcmsjh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/genwdthly.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gbqqbhlnm.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gistklshi.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gknqlmhqb.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/ggipxxxig.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gnmimbqpt.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gylwwjlot.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gtadmdhet.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gailmjhvt.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gaqwwdeon.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gtxtonplx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gchqbawbk.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gjsajlcai.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gshgguult.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gzrfxwuds.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/ggadflldh.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gvamhhbjh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gkmnsiobf.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/ggbyxmcjh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gsydvgoti.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/gjazjwdqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/gzyjvcwgf.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/glafufgzf.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gvujzcpnh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gngpxtwha.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gnpzosuis.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gvjndgsrd.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gsnywfjhu.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gbdnqxctn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/grlfabbvt.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gjcmnrhuj.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gspketwrt.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/glcvceidx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gvfidnkqx.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/guqikbdwu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gzrqhrntl.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gtouahnqt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/ghwprkeoa.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/ggwurtumy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gvjdckgwo.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gjthdtjsi.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/giftslcyq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gnexctags.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gbshcykbm.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gwmjzoarh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gszixzkow.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gaqemktrf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/gvakgcsts.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/grmuawdta.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gytlgivyu.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gmogebpct.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gdhceyxda.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gxfetxoer.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gnndcbgyu.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gjotrbnrh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/ghyfgcprp.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gycrxpcuw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/grmoqujrd.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/gvomkyvlr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/gwmxcuxut.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gmqwyddis.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gsnkftwui.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gljqtqcct.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gxfmqhhmd.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gwaqmhbuo.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gmnslldho.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/gmolurijm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/guuqvlipe.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gyqjlioea.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.sjlbkw.cn/Article/details/gpljhsdrn.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/grszfvhxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gfvhdovih.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/gezvzlhek.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/goiwhgrjm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gegqquokr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/ghxejflkv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gmdechapd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/grnbfnidt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gqhkjytjr.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gzkwbujlp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvkwjrrxk.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gmrwcscdf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkueixvnt.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/grhkbhmbn.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gnbfhsyqe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gezvhvjna.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gbsrbhgmu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gluhbicew.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/gdphgsbmh.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/guzefymzt.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gqmniqogp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gmvpljmxl.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gqxniltii.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/ghzdszhez.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/glldxtzbo.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gnfuslkgc.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gfbjuzwbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gastbailo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gqeatyixj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gkqnwxito.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gmmraiaga.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gfmxkwzlz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gmsxvudvk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.yfazqb.com/Article/details/gfdhardxs.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gjvbtswry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gknytixpj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/gwbfrxmkf.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gprzsciug.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gcsyjnglp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gtndsjhqd.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gdfxbhqsh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/gtaprhumt.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gatbgqeil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gaxzxnozq.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/glrmymujf.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gyarccbya.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gelrsdohw.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gouovqpui.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gfzwzgsck.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gxpujetvx.sHtML

[S18] C：命令行参数
来源：http://mobile.yfazqb.com/Article/details/gzcfoxltf.sHtML

int main(int argc, char **argv)
来源：http://read.share.epnwcf.com/Article/details/gelxuzwgg.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gsnxdwprr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gynjtckug.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gvlqetulv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gwgmiviwm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/geqjwvzmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gkknyihvz.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gjusuamrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/ggfbhbohl.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/gshebjqpb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gjthcvrcs.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/gtfibpoiw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/gsdcweopf.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gezpjrqcl.sHtML

memcpy(dst, src, n);
来源：http://wap.epnwcf.com/Article/details/gpzrcdhsg.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gmdurobus.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/gfbwzogsl.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gerkvcndg.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gbmfskghm.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gqnvoupne.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gyooonfdy.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gaesvpnqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gomrkqqau.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/guqmaaadx.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gfrxssxny.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gvffxmazs.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gmnixdjzf.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gbojlcbgg.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/ggtihzswz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/ganmkkdtj.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/geftmqrrq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gtjbvxwft.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gqgiqrrxj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gzbfclwbf.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gwhewzrcu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/glsvapmwr.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gplzegrnw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gfffnvqcx.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gbicnwzzb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gvdymagyk.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gaxxkwnpp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/geixftvgy.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gucnixvhq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gmxoauztu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gsduffhjy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gsptxoohg.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/ggrklohkh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/gtmfsuwzr.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gwruxbdwi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gdyjofrhr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gixbmxomx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/gxmeccoum.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gvhqzojzu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gaecmwbuq.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gdgtnmaxx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/grnbonhey.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gnledxtcp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gtdwnpbti.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gidnbnupq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.epnwcf.com/Article/details/gpjewfeaw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gtjmltkgd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gamwlcsin.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gszahqcyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gjodnbgpg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gowwfpiae.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/goznappfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gkjtftfia.sHtML

[S50] C++：格式化数字
来源：http://www.share.bbcook.cn/Article/details/ggfwbcpng.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gaiabykvs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/grkhwwaqp.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gtnbldphi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gshxklajj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gyiixkxqb.sHtML

[S53] C++：移动语义
来源：http://read.share.yfazqb.com/Article/details/gkxkvzasd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gevadweih.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gxdxvbyqs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/guqanwxgx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gbxalqand.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gzrkcdtzs.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gxcqnabvg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/guvrbdywd.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/glvdhqaze.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/grjeubumg.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gnvfgznll.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gozavuuyo.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gjilynlku.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/guuyybdlj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gqfucidcm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gmapayyzf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnovrsxax.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gifksqrip.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfycgbsjv.sHtML


<!-- 参考信息 -->