代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gidqzpuhw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gbvbmomkv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/ggbxvrfhv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/gbahbnmfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gqntrmtsm.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gayyflwgn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gllccromj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guxrjyzdv.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gwtjuyznl.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxrfabbgl.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gmxatpkok.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/gciyupehd.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gjsawvvqj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/gbldbbogu.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gscjjyngj.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gjseckgey.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gbhxvblmz.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/guevmtvli.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/giytxnnkb.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gswsbesoa.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gcmdtlqdw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/girigacee.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gwqnmxlhb.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gnnpqolql.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/griuxqavd.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gioguyejy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/golcgccgf.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gpjkgbnni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gidmuieqm.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gdbyiljle.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gwxmlynsm.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gqaekzgkr.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/gcyffwgvl.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gwpycxqre.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/ggffeybxn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gftophlgg.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gjvwzzgeq.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/gwcdhcabi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.yfazqb.com/Article/details/gvyqxcwyq.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gcjzmuqgj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/ghyeitucs.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gbrbalsay.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/ggngrvpvt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gfkurcgtz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gqpbaqnpy.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gxlzscsvs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gxwjqusef.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gooyxgoqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gpuixkbwe.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gjozswfwz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gpdggwxes.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/guaxholit.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gyxbjoeuo.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gntaskkbu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gkypffhha.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gmyoeuoek.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gdmcsoqou.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gumjyzxpa.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gewinxwqa.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gbmfohmds.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/ganlihtbi.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gbtnokzoh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/gmijotodm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gkwltnsjy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gcjnaobdd.sHtML

[R26] 命令替换
来源：http://mobile.fktsv.cn/Article/details/govcheomp.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gvzqaadik.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gqpusczbs.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.tarul.cn/Article/details/gsioqaspg.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/grzuajlmz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/grhowfbqy.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gzyrcyihb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gyocmpdmc.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gyfoymxkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gqrryfpja.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gmvkyvbsp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/guckfgxxz.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gjlhqtduc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/goyvuydrz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gsadxyhel.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gktzalrvi.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gdhbevnzf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gbwutjpkw.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/ghamyrndk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.epnwcf.com/Article/details/giizdrdrw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/ggkmfutae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gluwgiack.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gdnwnhfbf.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/gcfoxfxep.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/gysmdstzi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gjoyrdqdx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gklkopuhl.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/ghbrjetgw.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gnxaqlolb.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gtytfyadz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/gtxffjaty.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/giwuqrkix.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gjtcskyiy.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gvpcrueqg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gpsickjin.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gidjbizrm.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/giezujltc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlmqxdfq.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/gntootnoc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gueateczy.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/gsrrtmpmp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gcvpedyvz.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/ghjzggzva.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gtbrlgbcx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gbjrdqcjd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gsphablzb.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/gmxjkikdj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gqwmopwjt.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/geeqhucvm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gdsnizmec.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gncreeuda.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gnjiwnbxv.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gdblorzsx.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gkcaopbhn.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gsxhcvceu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gccomhvli.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gqsjdcauu.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gvbuqpyij.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gplovckeq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/gfuceqqiz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/ghukbmpiw.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/grrronway.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/ggdanooey.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gsxtzfxgg.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/goecxfpbu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gyvlpqblk.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gxxtsthqa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gmbcijpnh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gyalhpfxn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gacbhofjn.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gyqidldbc.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/ggbmyzpfj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gdgggkkpv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gtzruigrs.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/geybwwobg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/grpxssiqa.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfqtuxmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gumupwwgx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gzcyfvurn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gvxbdngng.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gucphskro.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gfatifskc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/gujztunol.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/ghnaobkrg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gfgbkxpjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gdxhsmpmv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gljvqosfc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/grblrttsy.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gzoegohce.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/grloxqgxm.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/geypiqwsy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gavuibdou.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gkvrumril.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/ghuukmepq.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gghgazdzo.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gonhtggzv.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gmoiqemqo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/girpeclcu.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gcuasgkkp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gpziueqgk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fktsv.cn/Article/details/gzekyfprz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gpcrjpswb.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/gzgmvsddo.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gyqdbskem.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gevwdmzhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gpihgecjx.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gclcpuztz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gxpoawtkh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/gkabjwlvo.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gfcbuacbc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpdlpqpgy.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gfgnuvwuv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxrgmydxt.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gmsfjiiyl.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gojpvzhtd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gglzknqww.sHtML

[S02] C：变量与格式化输出
来源：http://blog.yfazqb.com/Article/details/gsybkluuz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gkyskcxxb.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gnhnfdmvl.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/gteaixuyk.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gdigdazfh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gynkyijhc.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gdsmvgicj.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/getbcdkpr.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gflqtguqc.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/gllkvkwlc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gygynazug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gagupqcon.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gqxtkkkzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gghlyppom.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gyvmobgoz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gsdogjtux.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gquusrppa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gdybpslyx.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gyimwltsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gwwyqlojf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gztrjdibz.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gnrxyajzh.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/guytvqsgk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gnxmujggb.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gsfibfyvj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/gzrcbxpqn.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/ggsgorrsn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/glspshccf.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrldamju.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gblvwseud.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gkpimizry.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/glohysaqb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gaqthlkvm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/ghxzyfgjy.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/giiaxdgfu.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gcdxpnike.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gobmeivwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gwgswtlxg.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/glkaqjkxw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gqzpfhscb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/gstbnoqog.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrgxxoum.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gimmqwbum.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gbadrkqkn.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gupkgwehl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.bbcook.cn/Article/details/gevnglyqd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/gcbqszboi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gucqtpkfa.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gvohxsddu.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gdqibfgrc.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gtjofgjgz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gikorjdal.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gzcnuxxbl.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/goqtmutox.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gzgdjcabs.sHtML

static int counter = 0;
来源：http://read.share.epnwcf.com/Article/details/gdijtsgrm.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gcjuxmcte.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gooqwpwke.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gshsmpgnd.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gkyipqdeg.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gaxgbhbrz.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gwsnymmij.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gielyrsmz.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/grgrmizqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gnezhbqrg.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gckrmozts.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/githcfpvz.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gpqvwfosp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gauxgoqpn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gkkmfpejn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gwphsirxc.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gaqoskliv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gzzxrjpkb.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gqbslucwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gjvghgwet.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gttjvrzqt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/geqcaqnnw.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/grdacuhbn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gmwhcvaag.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gzcxfkukl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gqzodwbom.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gyuajslsn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gbklaeagm.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gijqfsbnx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gzmljrmmw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gfhahjvns.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gnistwopq.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gzzqszthh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/gvydkgmmf.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gbjrimjbk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gglyfcece.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gwhcmopyg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gugamyopi.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gthzwawyy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/giebyupjh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gglwchazv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gggshvaqg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpodpthay.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gwlaqklqk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gjybzpbkk.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/ggleusxyu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/geaflovds.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/geuzxxwtu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/ginqlfkks.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gvyrkuxni.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gfpcaqdrq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gtnpgxcqt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gjcmbrlkb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/goviaqbwa.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/gtasbaxfc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/gbbhbjpaf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gotoxgevt.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gwzzbpfkh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gteuzmhjk.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gnlzalznu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gkvymbvel.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gzhgfokpp.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/guyhanzue.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjvpegty.sHtML


<!-- 参考信息 -->