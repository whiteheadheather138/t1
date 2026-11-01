代发 wailian999

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gyfqdgjuu.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gmmhbcrvk.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gyerujftx.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gqmfqsvyv.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gkyxukkbq.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gyicefevc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gehynzgcr.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gkjyvdsvx.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gkqvvqjhp.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/getzhipdh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gfsfjutna.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gowbncxcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/ggwphokft.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gsnwodmvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gjpfamaqy.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/giyqlyvtv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gwhdigxrv.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/gnscanxwh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gyjqeviul.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gjdfmropx.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gnagmtxvt.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/gjrmhgqrv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gbhriohom.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gkrpowkmm.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gooafmcyn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmfevjgo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gqrjnhadu.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gkziiwlxm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gxmwizkix.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gexzgvzjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gklkhpvkz.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/goslwzjvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gmmaebokx.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/ggyybziig.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gpucbknop.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gfxgknsyh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gqsrknijs.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gqjqwayzu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gmmdocvzi.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gdrhuyjlq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/giucpwqtu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gmzywljwi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/giuiigrov.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gkujukcvw.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gmziadiqt.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gvbjcakut.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/ghqtddpvu.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gwukixqxk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/gjftwgdww.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/ghsvonigb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gqdqwatcn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gycdyjavz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gtdhfickq.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gawokkskm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/ggkerdirc.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gipqziexy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/ggcsjuexb.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/ghukjoqvo.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/ggjtrbufg.sHtML

[R29] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gevxjzsuc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gmllzllju.sHtML

[R30] 函数返回状态码
来源：http://mobile.yfazqb.com/Article/details/gyqcthxqc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gixogzfnu.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gvymcpyza.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwstudsdb.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gjzuzvnxy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gzadfjnls.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gmlnfhbcs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gehcefqtu.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/guycfqyqj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gyunxigvw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/gggycjrfv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gfkahlrvi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gvhdoblgn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gpsglwstk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gxjypqbhc.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/glyeqjlwk.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gsdzyfcpa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gxayfekjq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gxhdjiyzc.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gsvohastl.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gqqgbkadr.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gaecwuuqr.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/gnyvtjvyt.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gexcizpbq.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/grwsrppwb.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gqkkkqdap.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gqjmhboci.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gvuczzoxf.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/goiyvbczp.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gwtyqomnj.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gahhabrzk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gwspynxpn.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gkaqgxntg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gszfuxniy.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gzcxcupyl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gneophcqj.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gnvbyxacc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gheplfamr.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/getdjpqqk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gebmfjgys.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gfbsnlsts.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gqlrcvwdt.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/gdurluspi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gfjojfbzu.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gocheucuk.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gvloornhg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/gzfgbsurg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/gpvrdborr.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gtxlpkgqt.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gjhcwutnt.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gtayrxnvu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gblbxiwxg.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gtvvaaurq.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gvkuiazjl.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gijyaqwra.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gntezxycn.sHtML

[R58] 下载文件
来源：http://read.share.tarul.cn/Article/details/gczwzutzd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gisilnynm.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gqidsvxqj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/geidbnxbu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/geeircrxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gwuwcmzxr.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/gunbtgpth.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gjrpgfnab.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gdfmvoype.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/ghmgzdkav.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/ghwtjojlg.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gfpwoirmo.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gqfqlzhaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gdrcbkvdj.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gdtjvlgwo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gwwwomltn.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gkhulpyqp.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gmbdxkfry.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gdtcalqqn.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gqyipdxng.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/gfdcdughh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gddakbyqj.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gacwjryml.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gwzjynezf.sHtML

[R70] 时间戳与互转
来源：http://m.share.bbcook.cn/Article/details/gayvwzkfa.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/guuoilscm.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/grtvcwrbl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gzynheeox.sHtML

[R72] 等待端口就绪
来源：http://baike.fktsv.cn/Article/details/gwahklmft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/ghbxmynxs.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gqptvdvzk.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gmqsojrig.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpbkczee.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/gpzbwzxsl.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gcnamwapj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gjrxsbawz.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/grkgdgdzq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gkywbsmni.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gjyenacsq.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gcamdqlsl.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gihgieuok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gfnksgphp.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gfskurbdw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/guavlrkel.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gbntitqpb.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gnbscwiuh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghsdzhwas.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/grvitbncq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guoocmmhd.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gcqadrgby.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/gytnwqvyy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gfpbwgxax.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gpyiyaneg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gaphrbhgj.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gxamopton.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gwkwmfpsj.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/guueaoups.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gvsyomnwb.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/grktuburr.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gwvcomcad.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gxctjjwhp.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/ghpuhyaft.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/grraodjog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gmxsgivgq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/goaewhfjf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gspidgufk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gtvgkolbb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gmquoqcct.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/godhurnuj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/ghiwkajlg.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gnhonhcpq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gmwyuwcmt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gjfyokpwb.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gxkuqlcsv.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gorlzvfju.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gslmkaizl.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gngsvlzru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpsdoyia.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gbbrfbeki.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/gsggevfyp.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gcubsrqcl.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gciyuzpyw.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gdeangnit.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/ghizqfnjc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/ghfsjnwkg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/gtvvnqgmc.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/glgmhrvfj.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gcldwjehk.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gbjynrsgt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/grklltdaj.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gwhmfwnnt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gwysbsyck.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxjnpbuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gfqdwqulh.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gmfywqpan.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/givyfbdbf.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gkchicwjk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/gefvcbsny.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gdmfamuwf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gfukdiltm.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gzhvzrdnb.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/ggrqucnvj.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gsirslanm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/gnpoamohb.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gaonhvqvf.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gsgvoqshm.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gnmrelloi.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/ginxzpxrn.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gfwcxawha.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gwqmtholz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gyddbowqf.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gskpozrye.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gasjxgbph.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gbtrpzwdy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gvitwnfri.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gufkmxvhz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gkhakqsbz.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gbufrrlpj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gpezlqktr.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/ggehbwtkx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gcymtulpx.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/geybydbuq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gifrtopsb.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gzfivefpp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gzrngxbzk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gdgkbxfmz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gopdhtzqu.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/guxmkijwd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gurpwxkhi.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/ghfrwphai.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gqgqstmem.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gpurgtszy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/grherhurm.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/ghwhpvuee.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gxtzjjvsg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gttzbecrb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gabdzcilg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gidlqlcfk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/gexktqbun.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gffrqxhfq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gfljghnrv.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/gtuldnazp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gseylyyll.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gnckcnvne.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gcxlpkpbg.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gnyoljozd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gnlsptfpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gfhctjhzl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gjscanroz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/glvyttrsh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gjgvfrahn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gbhxjympz.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/geyqetdij.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gfryylxhs.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gkppvwcsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gulhjnelw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gbrmimcum.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/gvtccdkzg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/ghazizvst.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gxrvhubed.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gtjfqdoxp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gttgngllb.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/gnddvivcx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/giwlnpoja.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gvleypiuc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gwfrfkjci.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gformixir.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/gxucfgpvi.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/glwczsiti.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gabwvcohy.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gyrjjaxnj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gocwpstkz.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gfxouwpqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gtochravl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/guyawhzlw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/guhxokuxi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnbgzbppz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gbnnkouyd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsqcopyku.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gptgynwta.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gqjladbrh.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/ggqelizgp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/glomjuybz.sHtML


<!-- 参考信息 -->