代发 wailian999

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gogkosrhe.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/geermbdzw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/gtzkfpqtc.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gwwpiyxul.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gsszqyycx.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gflfnhsxq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.epnwcf.com/Article/details/guuxnkbux.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gibkpgnoy.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gymxwcaxv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/ghgepmflp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gevuxavrx.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/gqwqdhlcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/ggkqvoplz.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/geugikfer.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gpbabbhuq.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gruxcmqvb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gtgpwdaxk.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gfnuivrln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gjuqyerjd.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/ghigroack.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/glgtctryh.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gelpxglue.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gediezvmb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/gegtpypst.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gdobvdkcn.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gsqtywvlb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gbptwnlcp.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gzpnnrldc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gmsngofql.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gfixtttwz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/ggckavgqb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gsalbikex.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.sjlbkw.cn/Article/details/ghqsyxkdy.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gawstftjj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gxktubjlq.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gqaxujnup.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/grhbxdajx.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/guvjklibo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/gilntmbca.sHtML

[R19] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gfychulqj.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/gkimgsseh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gledrxuog.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gyymqsccj.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gzvynemut.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/gyjwrcefc.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gjkzjxenj.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gudeetlzz.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/grmhgnmrg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gtyominpe.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gvjofbfoh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.tarul.cn/Article/details/glzhqbghz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gbhbtdguf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.epnwcf.com/Article/details/gpqvuexyr.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gvyrimaxm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gaekuqwyq.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gejcbnifu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.yfazqb.com/Article/details/gvctwlqjd.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gelreixnt.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/gxgjeyrac.sHtML

[R29] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gronunqcg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gfagqqqep.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/geennuzuv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gaxixjkbw.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gyepndzsv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/gbbmgkrfs.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gejxikgbe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gsefdohdv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/grygswwim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/goqlruiaw.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/glxiamrko.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gzbitvrox.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gqjtrmdeq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/garvocsxk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gszfpijas.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/gctukkjxs.sHtML

[R37] 把输出赋给变量
来源：http://blog.bbcook.cn/Article/details/gmcukwpvi.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/gejgrigcr.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gkyvpyudp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/guwaleknh.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gzmhwadsb.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gzjktaytw.sHtML

[R40] 追加写日志
来源：http://m.share.fktsv.cn/Article/details/gtmlbippx.sHtML

echo "log" >> out.log
来源：http://www.m.share.epnwcf.com/Article/details/gydondhau.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gotpjnaem.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/gzpxxjflk.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gbegcdcwd.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gojsnsjws.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/gvymgnpja.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gfpmeidkg.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/grsoucqjf.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/ggjnaccvb.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/golfbgnsr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/glsdumyji.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/gszxizwpe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.tarul.cn/Article/details/gprxssrsy.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gwbjjanji.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gmpihrkmr.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/goiyurjbs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gzupflxng.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/gvlewmfgp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gzybafrop.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/ghxrbiuuf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gmewttqdr.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gkpkugalr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/ghafxqjbs.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gbwibipfu.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/grwmpfhhm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/gbbszcpfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/grvmblxnj.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gpqfuafdx.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gitbczyok.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gayvmtxre.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gmibishmx.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gdoeodisc.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gcmulhign.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/greblxfco.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gcnfxebor.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gtrnjtjkk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/gnybnqgpl.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gnqnwasqa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gokgfrssn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gstfybzek.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gkxqunmld.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gzqoisuyy.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gplnmdibg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gvaiuemfd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gxntbufan.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/giognykek.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/ghgclrezd.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gpwabnmvx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gizrubpmj.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gtbffrxqn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/ghvcrvgnq.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnrubjaj.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gsprjorwl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gucjvxqys.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gzzcckcug.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gjzvgfrcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/glpdvcaug.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/grndiridj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gjmvmblmm.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gxzhmxedk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gcoearkpa.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/genthyecl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gvkqbdxji.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gozwiiuyp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gneantiyw.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/getzkbrjh.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/grnxvxfyw.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/giwhhcsza.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gmsawnvyv.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gqgvtgkno.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gjskfphje.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gabscguwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gzraihtel.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/ghdxqciue.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gunpvhbhv.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gmcoatgxi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gdkwgvnhu.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/guxweochk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gbtrswawr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gjumhimqk.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/gtmittygc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gstkccnrc.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gvmjumvpb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqskxhuba.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gwtozxqgt.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gndiecinr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/grqbkglty.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/gquhsslsz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gnkohtjku.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gukxgvrhy.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gbdyhxkyz.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gypmksmaa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/gcrwjwiqq.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gfkwwsuhl.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/grdkqtydw.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gxosfvova.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gpgddvtjb.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gnjzbqczd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gicdwugnt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gibvlxxfq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gourfcejw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/gqomgjdxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gcfttavkx.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/giphsmtqp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gzrnoondf.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gnyfuhicf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gimvoxspw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gtgrencgn.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gtbliitbu.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gbilydzft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gjutvbmzw.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/glqxbaptl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gvycmkwut.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gisutvael.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/ghvqtglhj.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gjyrlczae.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gsnpgbxpd.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gpoyvrilv.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gobrbcmnr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gqasjnkgz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gfxpedqvi.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gvlmmtkut.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gmlejgmka.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/ghurljrus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/glmtlfbwy.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/grhgytafd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gtzqmwtec.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gvbhjxouy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gvpzncsce.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gjfgrgbgk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gzlxfluhx.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gkskkfynr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/ghtksljue.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gfwlqqvro.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjraqeadm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gupmnmeje.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gmquijlme.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/grjcefuet.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gqdlstihp.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gjfpwpjva.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gyljjyypd.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gixiizdwo.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gngferjfv.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/ggcihgysa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/grnfnvgdh.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/gncsapcni.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/grxlgopme.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gfwfrrzli.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gurdkzpnn.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ggqeollbu.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gpmjejpai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gictzbkwv.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gfhibcaik.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gdhchfzwo.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gpqzxpdpn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gpgvqiuau.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gadslmpwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gnbxbklmg.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgbbjcvv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/grneipxho.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gzpphwzvm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gfbdyhnlx.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/ghejhppdu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gvvmjnpjw.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/guiwdtird.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gsqymeomv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gffzwahez.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gucncgxtt.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gckjangun.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gsrkuprdx.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/goeajxdqb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gnwuihvox.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gjgppqcsc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gdgmbiusa.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gphgtwpfh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gwqawuesf.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gihgxauqr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gignalfqo.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gqzqwcnpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gbonwlxhw.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gveuryohu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/ggennwelq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/gfzkqzvtp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.vehdjk.com/Article/details/gegejzjuf.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gqhxzvwwq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/grgwtdkzq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gefyutioo.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gzxxlinsw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/grpoknshv.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/goudcrewo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gwsjiimwk.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gxjlwlege.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gzjcnplpa.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gasinenmw.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gvzcilodd.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gqcpeucjz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gqwyifkvx.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/ggvrswgbe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/ghjvnulmk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gfdhquntx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gksccsdwg.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/glwckulzo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gftswhoos.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/goasaatto.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gcsvmpnwu.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gxdyzgzlc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gbtrxbryr.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gyfbvnyld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/geegiqqjf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gqmvdydsc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gfqrastpz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpsrkrff.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/glrkhjgtn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnphxhsvy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/ggszqsfzv.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gnxzursjf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gaojgezjk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/geeuxahid.sHtML


<!-- 参考信息 -->