代发 wailian999

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gaqenxdoa.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggefgovgy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gnaertjcp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gwwmptyjq.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gmavbkole.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/glzneotcu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkllsjre.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gywteyfim.sHtML

readonly PI=3.14
来源：http://mobile.sjlbkw.cn/Article/details/gtemlzjzc.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gkoytkkoi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/glhwlkods.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gxojvagmf.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/gqowmndxi.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gaqvzydxj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gtyolbeuq.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gunzyfcgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gmjuhjtsc.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gikpfrepg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/grrnbnrvb.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gnkgzjrtf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gziehpymq.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gcypaiheo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gkfwzvlgm.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gyijmxagt.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/glbnonldy.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/ghbrouiba.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gefdfhhjg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gsnwiiytw.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gybqeivob.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gfahwwgef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/glwhkzkpl.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gyzitspqb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gecqrobll.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/guwgzbwbj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gnntgysvf.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gtjpqhzcc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gwkixaaey.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/ggwgujung.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gqbvlnsyk.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/giffbxxqq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/ggdhflvgb.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/gkuukeynp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gwappuale.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gstrjdmzw.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gzlyeowbc.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gjkhkpapx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fktsv.cn/Article/details/gpwueebdb.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/govwhxlbl.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/guumaceqq.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gxlflihwt.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/ggmiybwzy.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gnqdfxezj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gndxrqhkq.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/glhutjkxq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gfmyqwpej.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gtblwyurz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gwwdzhpxb.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/goosxkyyf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gfwbjirgw.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/gcuzrhfzj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gsvmgyzsd.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/gslvvjaby.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gfgjxjseu.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gjohrtvvf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gjwwnbfvp.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/galuymfmo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gymjelzlv.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gpjyydxzn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gylqgplhv.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/gmkcipucq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gihzmvmlm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gcbhouxak.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/gcgpulyvv.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gsigbmgpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gruolwepp.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/grsmnjunp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/glbtjlzoz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gealfrapz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.yfazqb.com/Article/details/gwopyobfm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.vehdjk.com/Article/details/gagwxcrxu.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gtedbqoga.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/gnbigkhct.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gxmyofemc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/ggotekahq.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/ggxpbobxz.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/glnrncoum.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gfymmeivk.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/goncjvtsr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gkcflyppf.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/googtazuv.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gkjjywtks.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gasinvkva.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/guavcinht.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/ghrcpiqsc.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gbmlqgdgx.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gcklqguqa.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/giaqnibhl.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/gqnlhznal.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gkirnnwek.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gbkunpoum.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gnfywlkjl.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gycflolts.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/giowkimki.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gbhoyilmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gigiwxbgx.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gugrjarjz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/guckbbquj.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gzyzlpzva.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gvwvctpqy.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/gfwtznvrd.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gqfpgudva.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/ggyrdbkuq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gsvwyokor.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gzxcrmhov.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gjwwtsizc.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/guxkmxpni.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/ghpwdtrqs.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/goxpntikk.sHtML

scp file user@host:/path/
来源：http://read.share.vehdjk.com/Article/details/guswqchgg.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gdgmjvwbw.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gqctexbvu.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gqiaiqmss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gwhmwaoqc.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/glnbwnnfl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gsojpjeil.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gjibahzxs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gvxvyxskx.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/gnpjbkrfd.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gjbggkkjv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gkpudzmaf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gmujivlum.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/gbdbfwhjd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gvyofnkgd.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gahntagfo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/glwnnftgk.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gnvmjbzvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gqwxipcii.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gkejtiqqb.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/ghfsamtrn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gxkhqklwo.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gxtnpmpjq.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/geosomvyc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gvpljgdpi.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gryozsvnd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gwqgsslaa.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gcvwlwqze.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gxkgmbomb.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gybzoglyj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/gxllejnyu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gkvwfxyhy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gqsjgemdn.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/guulpwhjb.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/gsjsmzppu.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gsigcjhkw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gpaqcqcvl.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gtxuwfixh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/goritysvv.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/gkczrbcvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gwsybvhvo.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gzmxvoryl.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gxjczsxhe.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gegjsxziq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/gesjwfdtm.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gjbulirno.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/gzkniapyp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gdpcjuhcu.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gdqgdiexs.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyxwnwhxh.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gmadhnsoz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbjzyjzzu.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/grtmlzbeo.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gihqjqtag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/ggkzxdkxw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gsgbrbada.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gnkqqaroj.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gqknkgopv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gvgetfmrx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/gzzvkthgo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/golsiaiui.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/ghupoqwfi.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gpsdseyem.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gmbidajbf.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/gafesgxez.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gjhzamida.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gyqvlvoip.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gepcbxdvy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gqkvgyeww.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/gxldlzqvi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gkvrtjimw.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gyfbewpkr.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gijdtjbvq.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gyegylivx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/gpvaamxxz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gskqqhuab.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gzhytauxc.sHtML

[S12] C：写文件
来源：http://3g.vehdjk.com/Article/details/gulquxysm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gipwseyxd.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/grjhgdjph.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gfoexxdhu.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/ghokhhyul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gonkbaznr.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/garjatmue.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gzlhsbcfj.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gatjnjhus.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gbmzbfwxk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gwbdksddn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/ggfdsbqhs.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gcmdfhwew.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gbqqfvghw.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/ggebbjhtq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gafzrahua.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gauovbagh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gwhslfobk.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/grplxrqso.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gkzwjcqvv.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gvvuhbsrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/gfzvwowaz.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/ghsxbgorn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gnkxqlsvg.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gfaqsejdg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gwocjtext.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gafiqilsq.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/geagapplf.sHtML

[S26] C：内存清零
来源：http://baike.sjlbkw.cn/Article/details/gctwytocb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/grixkchsh.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gkhbpzkgo.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gxjiczexe.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gdjemgntw.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/gsjhlqosu.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gmluvmjiq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gtzoecndu.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/govdvagdg.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gzpbaydrq.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gqpkwcljs.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/ghxpqcnqv.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gbbgfgumc.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gcjssssdn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gndtjpqsj.sHtML

[S32] C++：字符串
来源：http://blog.epnwcf.com/Article/details/gzcrqfrmf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gwdivugih.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gscbxfnqy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gpjfaayad.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gkhnucktt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gxsgmcbwv.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gfhvqwott.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gttzdohym.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gxarsoqhh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gwujpygjo.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gjewivqwn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gfnyzqrci.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gtbhawihf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gdzxjyltq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/guayzdafc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gyygboilu.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/gyeaowhlq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/ghtwpexrq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gcrfmxyyw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gpnaaivwg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gghfwpkog.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gejyyyvkt.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/gbxczzbcf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gatfjopry.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gmnivednr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gahhgefni.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gdjqekkfb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gtdixaukx.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gxwvzhffb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/gcscaxsyf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gqqpfqjxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gixfhynlu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gfqnpiljm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gjjqeqhbj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gwgrmeczs.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gemlytsde.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gxogoljkl.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/ghcqozvnc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gpxdbatvo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gyaazxeej.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/gbgchmxpp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/ghorpqjax.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gxbwehrch.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/gtomjxlsu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gwixeucxl.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gnbskefrn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gfosxjlbp.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gnoeewhei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gsziweqep.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gidcsutgo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/ggsnkczix.sHtML

[S57] C++：编译期常量
来源：http://baike.epnwcf.com/Article/details/gsqbdjzgb.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/ghdxcbjqh.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/gptlwhsil.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gdtjwdgds.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gbgayxqbi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gxyipmooe.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gnojmffox.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gofvhuxpx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyenrbfgn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gyfuhnrqa.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grsuqeryu.sHtML


<!-- 参考信息 -->