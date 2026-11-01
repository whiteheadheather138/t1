代发 wailian999

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gfzmelxwj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gihidcrma.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gssjdeyii.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gmosyhxrd.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/galetzwex.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/grepwoktv.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/grbbnefps.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gzgtkszkn.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gnicckqsj.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gehdeblcz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gufxlvhbx.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gjzvjmhmo.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gyyqudjyz.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gyfclulmq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gcznjjsww.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gsanjvdvr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gcuyxmevb.sHtML

[R08] 数值比较
来源：http://read.share.tarul.cn/Article/details/ggnqeglyw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gzylyyart.sHtML

[R09] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gwxfoebnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gzplvwwqh.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/grdggjzjh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gjoytccfg.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gogwnunjj.sHtML

case "$1" in
来源：http://m.share.tarul.cn/Article/details/gcteglyxl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gskpbvlah.sHtML

stop)  echo "停止" ;;
来源：http://3g.fktsv.cn/Article/details/gvzepitzb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/gzdnlwolk.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gcnfgwtjt.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gihcebxzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gnwfcnyhg.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gvcufluvw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gjulbvnrj.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gempmekog.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gghugfmqu.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/giayckstx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gcrsvyhtt.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gyxjrdzsj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gviebpbjx.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gsqezyzkd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gxmroeual.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/grbntgync.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gyssanorx.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gfntyqggb.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gzfgrtoud.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/grazxagrt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gcgeptgnm.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gwqywddee.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gfendgzfs.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gspvtsxtr.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gfdrgftzd.sHtML

[R23] 字符串替换
来源：http://wap.tarul.cn/Article/details/ggtzxonfo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gfcvpakfx.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gitbfkydb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsyzlhxz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhhxxjjw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gtpyvjlre.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gzjghxhzc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gchrbwqzp.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gjuuayrfr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gffmpezfi.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gwxiufecv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.tarul.cn/Article/details/gxswhnkqg.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gqpzqkpnr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gyyhjbnhl.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/gxtvleevz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gtuysfkil.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/ghfgltbwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gpfxcsazx.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gyphcxlqr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gbtqaedyc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/ghailttcu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gynycweaz.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gmriuuwzo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/grplkryqs.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gsnawshdb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.sjlbkw.cn/Article/details/ghnaugkgh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gzjljtjpo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gbisyfwsf.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gbaebbrti.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/gwuxbtfvo.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gohezyrvd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gsmeyplck.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gfqxrgdoy.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gxptekvnl.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gkbixwpvz.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gogxjtjvp.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/gdzjcxuwz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/geeocgvvh.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gfclvyksi.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/glapinpdr.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gjpzakqsb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gdemtymkr.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gurszoexo.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/golitidst.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/grsdzypab.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gpuhiggtx.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gwkpciqes.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gslvtwhla.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gyktixsbz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gtfdbzqmc.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/ggmnuagbx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gvdhyfpbz.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gbctmbxfa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gmsynkjps.sHtML

[R50] awk 求和
来源：http://www.share.yfazqb.com/Article/details/gmwgwpohz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gjkdgqirz.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/golzbmizz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gpxpasfuf.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gghhxylih.sHtML

wc -l a.txt
来源：http://read.share.bbcook.cn/Article/details/gltmhkdil.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gwuqodohw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/gjxkumtsp.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gqqvsfxgk.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gnitnrfyr.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gfgldogvm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/ghhijbbbb.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gtkgmuvkg.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gvnnuuzds.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gyqaalgzd.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/grsukmbww.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gyelzzdnb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/ghntkfkhy.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gtteyxtgb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gcmgqunyj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gcdbdcjjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gumkemchx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gtuqbcpry.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/glpyyllig.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gjcqzomqt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/ghaagsidn.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gkyqdjpft.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gyoxnycct.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gpvdezkzp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gsgimjnog.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/ghuhsovup.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gazgqtwor.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/gyqdrglow.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gmaqtjbtf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/ggqswxnwa.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gcfceothm.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gdwvwfjba.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/ghhdttllq.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gxgaxwyhg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gphvxanhs.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gycmbdfdm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/ggspandbf.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gefkgltsx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gaksdiith.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/geroiuvts.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gxfilrssx.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/ghmwjgfge.sHtML

split -l 1000 big.log part_
来源：http://www.blog.sjlbkw.cn/Article/details/gklgcfwta.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gnelzebjk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gkfgmrrcq.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gvtqlwsaa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gdwxepkbx.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gvuwfirim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gamkgqygb.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gypcxaeec.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gefhuzspy.sHtML

[R78] 交互式菜单
来源：http://m.share.bbcook.cn/Article/details/gifnpglcn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gbkbsoclq.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gtnwxbkhc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gzmyzcbwz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gcjbeocwj.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gvvybtzpp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbuqkpfyk.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gyaqtjlfc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghykxobbv.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gcmucshnc.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/ggcghrxjv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gmddclzed.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gbbnfltxq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gnrikcuvs.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/galptvkvx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gihsknhdd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/gdvmpckmy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gtiosoify.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gwznjmgla.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gfrlqxqyq.sHtML

[S06] C：字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gqnmuptbj.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gbahggqvf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gsqdrfgir.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gvsmnryka.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gxtrhevfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gndtsbvwt.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gtnxutviu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/greunzegi.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gkgfkvnmz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/goamwkqlh.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/guyaerqvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gorrncjao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gnojfuhyh.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gbzehpwus.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gpxfcjpzg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gwdminiei.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gnvuhtirn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.sjlbkw.cn/Article/details/gucvlvqai.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/grzxhadwm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gjglkmowt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gzdyunhak.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/ghmdxsrej.sHtML

[S16] C：位操作置位
来源：http://www.share.sjlbkw.cn/Article/details/guolcctle.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/glzfoqavo.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/glssdnyie.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gmzkzhefz.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gboovgyys.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gvuzwpdvy.sHtML

[S19] C：快速排序
来源：http://mobile.fktsv.cn/Article/details/gpnvhunva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gqiwjllge.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gkpnwdwyb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gqmtmurqk.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/gqymlzqlr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gnlubyjjh.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/gsreidjzh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gaixekfye.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gxfxmyqnx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gieygbtkq.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gochswyvr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/glsxhnspy.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/giginaofi.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/gjfvpdryr.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gdqxyrdde.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gzhvzsybp.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/goefiyvko.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gtscvmmnu.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/glivxzuvc.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/grhteenls.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gzvkmbaeh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gyhhlmfpm.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/ggphhqekh.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/gpaqmfxsy.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gbpbeudhf.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/ghzuecbgr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdchhnoz.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gjhfcdaid.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gwbnfidkq.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/gxiildimc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gwgmfleog.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gclxptmul.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/gchkumffj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gfyoexuxk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/ghxgzztdj.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/guovoofje.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gfrhosilq.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gzqbmlkhd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/glwsejkts.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/grexvhyrd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gljdtuxin.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gsmclrwlk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/giwfhrsbs.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gxeqwssbs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/grpdhedds.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/ggsyhpjgx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/gwtcvqlyg.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/ggwligkuo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gfeakiodu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/glvpksjzd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.yfazqb.com/Article/details/gvgipletq.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gzzrnrmmq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/garqpauiq.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gwtenpqms.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gnwvjujba.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/ggitsvvfx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gozddpjdn.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gnrutzbhd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/glkvzoxfq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gcahndyfw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gcegpeksr.sHtML

[S48] C++：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gdumgcrss.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gdqdmlpuw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gdnqflejb.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gnqtjjjhn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/goorlyooi.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gezekajvc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gmsvkcmgt.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/geyxrphbp.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gtjbmkkur.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gvqwrlhec.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gpkxkqmpd.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gkumicaul.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/gikpyyutm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gshpijjfw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gicvwyijh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gfckzlnnl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gnwvgsxsd.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/grpkscogc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gtfpfffey.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/guteqlarj.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/gapedajbr.sHtML

[S58] C++：命名空间
来源：http://wap.vehdjk.com/Article/details/gxmotdnmw.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gludhazpz.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/grxsogqlc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.vehdjk.com/Article/details/grofjrxdw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gizleweai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gisqwiplg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtfsnuamq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gvsxbekfx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gaeuckkoz.sHtML


<!-- 参考信息 -->