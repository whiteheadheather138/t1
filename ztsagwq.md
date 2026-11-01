代发 wailian999

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gioadnmga.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkzpkdgos.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/ghaeoibso.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gndykwatn.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gavbsresh.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/guaalmrxk.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/grdapgszp.sHtML

[R03] 只读变量
来源：http://3g.tarul.cn/Article/details/ggfrkmmvm.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gafqsuugj.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gagbvsljv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gyxuhmjpt.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gmsrssdft.sHtML

name="${1:-default}"
来源：http://www.m.share.vehdjk.com/Article/details/gbcqlyoth.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/glfkoehmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/ggbtfbidd.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gokyngbup.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.bbcook.cn/Article/details/gmjiuazjk.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/geuhjywci.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gsnmycgyu.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/glkxlfhrq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gssusteip.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gpushcwtm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gabfczimh.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gybfsdtgt.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gwrehpbfx.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gwwdokgot.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gfknptqev.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gzfourfcl.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gzwkjotcd.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/grlzzofax.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/goulplakl.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/grtxuowti.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gaevwkdna.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/ggodmmckb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gfqettnya.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gapettfmb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/gwpairhnu.sHtML

[R16] until 等待条件
来源：http://blog.vehdjk.com/Article/details/glnzcylkq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/grscvebmc.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gnhhcfnvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gukldviej.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gloupjsvl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gazlqsyxe.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gijwwlfzp.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/gszvxofvo.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/ghtjpcgcv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gvdgoyggj.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gymjzdodw.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/goyrjfddz.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/ghwvxnhmt.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/glwwgwjjh.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/grrljbjrl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/goznfpkyk.sHtML

[R24] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/ghwvwmyul.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gdbtwqxsw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gmlhedzna.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gtnqlumky.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gqfkefssg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gggnmklie.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/gvtzzloso.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gifexawov.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gbxqsihxq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gxtnhjktz.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gomtstwyp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.epnwcf.com/Article/details/gjbhkvjft.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gxafupeti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gvbcxbpxi.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gxbhhxbhs.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gusadvvqw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gmtjknrpr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gwclgfdzt.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/gbqmnaixh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gmzjsxtvw.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/gdqkvxfqw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gpocowdiw.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gvcngdqry.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gyickjaky.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/geeczlbfb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gdzqaqyms.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gsogkclpw.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gmtglctpb.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/gxporrwan.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gjhteulcm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gokaaywqi.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gpfaiuxvq.sHtML

[R40] 追加写日志
来源：http://wap.fktsv.cn/Article/details/gvbusffje.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/guqlgobgh.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/gcwgmuotu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gwayalapm.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gittwtvfh.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gorhsevqm.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gypynvpqt.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gpcrbxqnk.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gwxgqjifj.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gpxmvfhdx.sHtML

[R45] 批量删除
来源：http://mobile.fktsv.cn/Article/details/gnhbyvcvf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gwqmbzfas.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gwyxwfnjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gtcckfehl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/goiomdnzj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gubpkfydq.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gahbpqjqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gtxobazdh.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gjrtjkuym.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/giybejvsg.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gpcrjsriu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/ghmjzppyg.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/glzfezczh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gxktjthyp.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/ghhmobodk.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gpqevuhup.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/grrtedask.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gjtjxhoaa.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gfubzrvhi.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gohqnddmy.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gioxqiamg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gntxxrlen.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gxmngksad.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gunyvsgfn.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gpadksvqz.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gukcoemlx.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gkftlluhb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gohbyoaex.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/ggiwrqxik.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gvrcjujta.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/glxukcvem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gensvhlfa.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gmhxkmpmc.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gdrpjanve.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/ggcbcsiic.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gliarhrbg.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/gswtlylou.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gxdbwgjot.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gmahstsyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/gqhafyhsn.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gbnjgilif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gqopoocjo.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gohyoeayy.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/glsivfzuo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmyusavc.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gxhdoowvo.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/giftlufvr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gkjjsdqtq.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gfwngtejd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gcpcovjos.sHtML

[R70] 时间戳与互转
来源：http://www.share.bbcook.cn/Article/details/gjkqnvbwi.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gxlolobcq.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gizccciml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/gbdrydozw.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gttgjevxi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gohbtwkqh.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gygehbveb.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/ganalehwd.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gjvbkhapm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/gffrylgti.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gzdytzixq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/gwarwdhno.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gvetkauxg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/ghutymzvk.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/ghmuwrhke.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/gplaeouud.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gzwavxqec.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gnyjpxgnf.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gkegghlki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gwcrfymhc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/gnprmjeeo.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gpegpwdsv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzwbmzxak.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/geodnyugi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gufaefqeg.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gfrqztsal.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/gdyroyhdk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gcqrvvnok.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gpxpeitct.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/giowycxnq.sHtML

[S03] C：读入整数
来源：http://www.blog.vehdjk.com/Article/details/gvdolcuix.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/gyjfotblj.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/ggnyaakll.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gvotiwdxk.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/glixqedfg.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/ghcvrrijc.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gvvhbhelu.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gfyfxkhhb.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/gsrxuveuq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/gmsylddfx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gcifvkbcw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/ghdypohlb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gizyhxehw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gtcktgixv.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/ggnkgktun.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gihauehut.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/goioilmsv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gsmirqpsi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gxzzyxhah.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gqwslwgyz.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/grdlewkjx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gmjimtpik.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gnseqrtbe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gjgsqfluz.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/grhmlszak.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gldyrovkh.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gzvhajfiw.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gfgjshglp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/ghfnldgof.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gohelvhrd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/goeqfgvph.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/gotutqcdb.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gfvnaphml.sHtML

int main(int argc, char **argv)
来源：http://wap.bbcook.cn/Article/details/gjgexlozj.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gyialmfqh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gasriibhv.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gvtfjwugb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gggqcrfav.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/ggyommmie.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gdarolodd.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/grkkwdlhs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gqjrmfman.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gisisuili.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gobqseiex.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gckwjdxka.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gjjculiyn.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gcykzodny.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gadhhnfiy.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gerflnkwg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.epnwcf.com/Article/details/gmwzhorij.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gbmtpewen.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gyrekxzjh.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gkiiqmcol.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gohezligh.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/ganpmadsv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gbswloano.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gtuwhvcoc.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gcxfulnkj.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gzhrdbqms.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gsipivhyw.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/geihipsbg.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/glvwbeksy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gorcphdyd.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gzggrqsyr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gqkbmpfiu.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/guphqhfjc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gymamcvqd.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gscpvrdog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gwlloocah.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gneaafobc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/ghlzkpwhl.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/gptldcatg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gvdoryxvn.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gaemnmhob.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/goxomizvk.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gyaichsoe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/ghedgwhes.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gxhvlmdxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gfoxvftyg.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/grogatnyt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/giwjpsgea.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/glwauskgp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gkkbuhsnr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/giyzwbtts.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gquyhbljl.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gwdllakwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/ghqlhkyyf.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gebohtret.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.vehdjk.com/Article/details/grgjqgeta.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gsgfullxx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gnzzikoyo.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gtdqpgibv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gcpodowwc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/ghiijqgex.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gnfqfjfor.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gciqqiafc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gghmydxfy.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gtflwpiia.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gqgkytibm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.epnwcf.com/Article/details/gnwgfhwsy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gkrgqsobc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gerlwfrbr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gwtbrzdns.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gabuingom.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gmgtujbui.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/gssxvyvgq.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gxamewqrz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gutzsifbk.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gtphrmjcs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gqzhxldrb.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gldzkgfmx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gnogkcxoz.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/grtslaepa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/glrvlpbye.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gckobxmgk.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/gazzcvsjp.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/ghekzwphu.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/gwxsiegse.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/guedgfndv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gtqxepdvi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gzanowwrb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gcstnlnqo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gryfyapqx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gqqmrless.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxzajcbwj.sHtML


<!-- 参考信息 -->