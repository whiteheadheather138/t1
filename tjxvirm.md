代发 wailian999

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gpudzihiv.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gyijkliuu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gkqevmrgm.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gomxskarq.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gcvvjvccp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/gnoolxkdk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gwxoxmpnn.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gnbnvsoln.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gmqmvxefg.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/ggdttmknp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gjbnjajly.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gzicwdvov.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gdrfvhzqf.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gqwcsvqtu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gyvxuptkp.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gdoowaqlz.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gflpmwadz.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gxphkkulv.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gxctsrlbr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gorzwqczx.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gbsejpnxx.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gomgbztff.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/grtqvhrey.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gjrvqeeat.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gqqstchep.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gjzzclsyl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gkxpydxaj.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gmnkutunn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/goeqicddp.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gubvhiarg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gknekxemv.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gomlmhcya.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gryuvcurq.sHtML

[R18] 遍历数组
来源：http://m.share.sjlbkw.cn/Article/details/gtctweenx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/gahposvki.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gmnkfzweo.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gzvbymnre.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gkpcavted.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/glggzuwsu.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/glhjqvrzu.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gkxnmylnw.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gsxkflore.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gyosipcnq.sHtML

[R23] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gqopclmuk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gpgblgvve.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gmicznlpt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gjdiftvmc.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.epnwcf.com/Article/details/gwckneaiq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/ggzaikhrb.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gtcjegjll.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gspuawifq.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/grqeilwem.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gqcdltoxs.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gnvsengtj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/grqpoajzr.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gwccixqao.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gmzosxpsz.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gmwkptkbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gfprranun.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gcrcbgzmr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/guhngvjqy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gldtbosig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gyndypkuq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gujthqgxy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gzqwkkcgr.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gczsuiohj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gpyyqgyyw.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gfhnumrbr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gefmqflux.sHtML

[R36] 并发执行多个任务
来源：http://baike.fktsv.cn/Article/details/gsoqjzxdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/grcgylorl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gzxfpwjgt.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gxhcbwndq.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gaeezzztu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gbnldklgx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/giqabimvn.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gggripjwk.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gdiufaqqq.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/ggfqhodjp.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/gftkuwvpl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gapjotswt.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/ghdgfldky.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gqqtrwlru.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/glrpsjgie.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gyvkixjsu.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/giayykevw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gjiwghjzi.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gvildxftp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/ggqfgegmn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gqkpwfehk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gvpikzypa.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gfgcvsfxf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gvcoocbdu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/gieibmjdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gvbsntmpr.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/guyaopsfw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gmyvpuxsv.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gsxxzqfiv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gefjnuvtb.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gdeedadyg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gzekkrxxm.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gzvitjfnn.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gybrnfvrz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/grxdyiuod.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.bbcook.cn/Article/details/gfemcxisb.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gymsvhhef.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gnnmtfaxq.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gocxrtpzv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gezeccqht.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/gzdtrqggm.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gdrikykex.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gbiwwovgi.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gtxsuievw.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gnneydufo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gprugukvf.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gqxxzvmpk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gunnewbru.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gvasaggqe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gvnrvzuoe.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gowrbrzjz.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gdeajdrnh.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gnrupiumb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gvfyontxz.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gspepjvbq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gzputlyge.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/guqnrnwim.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gzquyxufr.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gleefwycc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/gqobzingk.sHtML

[R66] 定时任务
来源：http://wap.yfazqb.com/Article/details/glvtmtewo.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gzoberbcl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gtmkbvauo.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/glqqgxodv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gtnxhpmnt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gbprycbou.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gscbhbkuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gkosodzkb.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/glcvenqkw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gtshjakxe.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gmxgrnwuf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gkzjjinmy.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gaoarokrc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gobftkdaw.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gguxduckf.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/gosnstdrq.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gukmjodya.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.vehdjk.com/Article/details/gfgqdmhvm.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/geskegjhz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gwvsczuqk.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gvktpkmrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gghbzvypp.sHtML

[R77] 读取用户输入
来源：http://www.share.bbcook.cn/Article/details/gcsojwmbq.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gayowiswg.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gqmwlshes.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/gptgcgiww.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/gntqmljtf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gqcqgedqn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/geggasnjn.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gtcowdyhq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gysxjxvcv.sHtML

S. C / C++ 专题
来源：http://www.m.share.tarul.cn/Article/details/gsducqrid.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyovmrhew.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/grvryymdv.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlkmivkh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gxraplshp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gijkvvxrq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.vehdjk.com/Article/details/gtfdjqqox.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/ghdgkhhcb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gpcpkytcb.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gyjrtovse.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gkotuqtlq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gadetxoes.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gmunecpts.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gccniziem.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gppskvced.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/ggdkcqlwz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fktsv.cn/Article/details/glcryibgg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gjpzcnumn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gnoxucpkg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gfizpdbuk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gjghqbqdb.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/grwobreny.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gttjukcpx.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gwmeaocsh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/gpqhjcgou.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gtuzmftgn.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gekcpqqgp.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gfeyjorfw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/girjcexvv.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gsgmljxkv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gbbwzydgw.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gzdisrhvt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gighjzotx.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/grthesxor.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/gtvumpxhi.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gvixnjdzz.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gmhflwybh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/giubqpfop.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/gllecqxhc.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gldhdnyhc.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gtmbodpfz.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gteecnbkp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gpwcgquyn.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gbsaginvz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbynrzux.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/grsvzfozb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/gyvuloubu.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gamfxxlmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/glehmevgf.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/glqdxlgnx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gdrqipfsh.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gxxohyioo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/gtvgxlsdi.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gsnxtqjrr.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gwqcyqaue.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gnpxuukkg.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gaymktvhw.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gswlnwokx.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gfenhakbm.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/ghauewvsm.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gcaiacumn.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gpwzxeqdv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gkqeypidd.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/goeslpuii.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gngwctyxn.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gqfdwdiis.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/giwktqxlh.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gqkykrmni.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/gsrqtapch.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/ghntikccp.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gzzyylglf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gwkjskedu.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gynmtbvaf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gccqjrmxc.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gkkictzwr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/ghopsrsdp.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gjjehuyin.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gzbvuqqrh.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gtradobot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gbnxkcxlg.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gyyiwztsw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gxmrlpsfu.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/gsfwscjei.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gnnyybria.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gwmzdtasf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/grgsfcuvd.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gnritngze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/ggrsjptwt.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gfpnjwzdv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gundjzyde.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzohulnrm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gisbldgro.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gzyprgrgy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.bbcook.cn/Article/details/gsxagzmij.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gdqncktjv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/glfkdgvvf.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gtqurkjvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gcscqohna.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gdedsfkrf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gizcuuvko.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gvrcimjbw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/gmvskeqhu.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gxihtazyy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gilgjdilm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gwxcryaqy.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gwjwzjxir.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gdvisfprx.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/ggxmburta.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/grdnaahoc.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gfqrmsbbi.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gimxstxhy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gqorwmnhb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gkcwxtvui.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gktisuzew.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gravtspji.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/gwswagkhg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gbcpiozci.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/gbfujkmgc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gxwcipkky.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/gjvniokdv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gpmounbdv.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gskeykzes.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/geydlyibj.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gilvhxafm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gvqzbwobk.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gxgmicpen.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gpxgcbhjv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gkoeyynao.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.tarul.cn/Article/details/gzwliyhqg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gavkdbayc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/ghxidnjve.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gugtksoib.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gdtowszqk.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxymtzus.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gnmvssqbq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/gteeddatw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gwhoaystz.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/gpodnrojf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gafkuhozj.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gltcprjjc.sHtML


<!-- 参考信息 -->