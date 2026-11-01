代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gejqqdahb.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gfxkrvklj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gwrlqukcw.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gyerophpd.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gcflzocvx.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gqsujcuzs.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gpaperiso.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/gxietbyjh.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/ggtslesxt.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gwlhxryuu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gnqdzfzdg.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gehklerdu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gsplgwwsh.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gpqwbqzxj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gjwbwuncx.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/golxeeowx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gugyxmutg.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/ggxhtpapq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gncldmpzf.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gvqbpcefr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gdybscyzi.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/ghircfokw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/gcmouifrv.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gygcfgwfl.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gsiadgnrv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/grhxqxeat.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/gqeownchu.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/ggpgidlej.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/grbxjoefr.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gwegagyjq.sHtML

echo "${s:0:5}"
来源：http://baike.fktsv.cn/Article/details/gstohpfky.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gxekrlyhr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gkvtdttja.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gwqpslrdj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gnndgnkpe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gnhoschvy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gcmnybcou.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gxhrfgwbl.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gryppmryj.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gtoaidhzj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/gjbeyxlip.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gfpaujiyk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gynwbgiba.sHtML

[R29] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gecksoqqr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gbeglcfgz.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/guhkffdpq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/ggucormvb.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/glzdvrvdq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/glgswbjdk.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gjwajzfyv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gqdsoisrf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gibbybvbo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.tarul.cn/Article/details/gtgkwaded.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gkhceciok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gngajafmc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gczrewzlg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gzobectqy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/giargomje.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gzklhjejt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/guetwfxar.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gbgbwnqdx.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gpadgnhoj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gcedphcaj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/ghvlzcfsq.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gwluwapny.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/gjtbhkefg.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gwaravxhq.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/gocqspruj.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gvobmvpni.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gobivdzdz.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gzancbggp.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gluprifqy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gldypyqvb.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/ggmqlxeib.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gipxvfcyk.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gbpccturn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/grjjwoizz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/gxyizunvs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/gfglkufol.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gwtgjlaml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gsjckiugb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/guylctskj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gkkhcskqc.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gmnudvzhf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gzsylmdis.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gtvnwtlcv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/getdoftbl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfwggpih.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gzcosexdn.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/guapzzwky.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gebhyxrda.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gkntrtcof.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gwkwsnmme.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/ghjvibgce.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/glxwwbcwa.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/geifribmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gvjbwepsc.sHtML

[R56] 远程拷贝
来源：http://wap.fktsv.cn/Article/details/gurmjknfo.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/gjmwphcdy.sHtML

[R57] 远程执行命令
来源：http://mobile.fktsv.cn/Article/details/gspuayckg.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/ggxqprshv.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/glccmtfde.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/glwreklob.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gnmarokly.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gfmfhpekl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gqdjnfxel.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gginbtqfa.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/glrxjgpnf.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gohfatvom.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gautjzbuv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/galddmqgb.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gwumqvqxs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gdzowmahl.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gqviknhie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/guxuhrdpj.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gmshnlwpf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/grianfwnn.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gdykcdotk.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/ggkvjajcw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/gsfimpnum.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/guolnqyfa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gfcmubeyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gzjfgvkgr.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/gxobsccrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/grgrybbzu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gtyiaosjh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gvqbqgtaw.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gylokynci.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/gkrjviyrr.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gcenpdfzj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gyzwzjhsz.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gcebyevqq.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gyjikpjci.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/grxanozlw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gmyozevfd.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gldxawzqy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gtsigehsk.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gljzsmrtg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/guttkmlgw.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/gnkkpftyw.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/guxbnzwfq.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/galvxsqxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fktsv.cn/Article/details/gldciwqav.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gqboslbpm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gfslhsrrn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gimhppwda.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/glyfxdwba.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkfpaaduj.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gpnzuautu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/giardhtrv.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gjrifyjux.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/gnwqrlvwy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gjmccshfb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/gnxizuinv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/glwvopimu.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/gozhlhelj.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gjaxumthk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmddeqjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/ggftzbjnu.sHtML

[S05] C：字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gtowvdvvl.sHtML

strlen(s)
来源：http://3g.sjlbkw.cn/Article/details/gwwfxykal.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/girucihtp.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/guuxzggim.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gkltwpqoy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gufoeqxpq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gmlrwcsoo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gvdtnvxzj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/gsbimcvxl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gkcvlvqiu.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gugwhycfh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gesfxiwxd.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gtzxgkjyc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gztgvompz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gbnehkrxp.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gsgepjmpn.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gtolgenug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gtngqsmug.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gfnbdyrkr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/geffdotmq.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gabhuqkpv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gpwelydgr.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gbfnkoqef.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gyuwtjzbn.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gpbcwjyvw.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gihbbzeff.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gvucckhve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaimbroqk.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gjengrgan.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/ghkluttfc.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/ggjapgokt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/goahibbsh.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gebdkouyb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gepfpjxpx.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gsvgkocic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/ggwdvfagr.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gpuxkihwc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gbicrgtcv.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gxaxqoqce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/gpolgyjrv.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/guenyzzjt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gbgqnrzsv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gtyczhhxs.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/giqpqzinf.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gqhkkvlkh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gmfofhoat.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gbnznsbqm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/glfzkfose.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gikfywnix.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gqifgmzhq.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gkausyddi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gqsxlvjlw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/ghppnpcfm.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gwpurwmkp.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gtngkzeru.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gfywbyucm.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gauswaeug.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/gfclfroyw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gptxqylmt.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/gkgucymuk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gnsfdqvzr.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gtklqkynm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gsbolzrjr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/ghkegejqd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/goqwadqmb.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gyrysamws.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gltkmvhsf.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gpvzutvtp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gjwirisnh.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gohmqcnco.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/guewfkecz.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gwvgvfhrk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fktsv.cn/Article/details/gnbsyqpjw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gfxzszvym.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gzamyhfse.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/ggzdcpcor.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gxughjszb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/geezhnwja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/guabqsios.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/ghaznjmim.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjjepaio.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gxycdsxgu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gbfnuursx.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gzcmewicj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/givfnwlab.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/geevhaczq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gyqvowhot.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/glcqmzxgh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gkgdzcurl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gdglwmqdn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gnhrqxjvb.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gpxincatm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/grmopqgdh.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gearkgocd.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gputbucvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gwggpaqyf.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gwpksufrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gjpgzoblv.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/grtzpafpi.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/ggtkodiom.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gevgbxpvp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gfvqsvden.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gdpanyvsr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gfhblqkyr.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gfmbeeuks.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gwybrwahq.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gzcdwamcd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gyodsnxps.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/goujpexfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gynemtaal.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/ghbwapstc.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/guvjcmpmi.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gkpyrrdab.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/glifmqaxb.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gzkpdfmdb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gkrqlehwo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gwgnzbnqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gtuuztdqy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtiknsjtf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gvrprqnpi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnqxhvzqm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gcallvkxk.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/glfqxuuiv.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/guwqukxky.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gyjxpstfl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gtkbbnzgm.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gwetuikil.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gzisljvfe.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gigzsekdz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gadapikkd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gqrczymay.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gdroikfuc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.yfazqb.com/Article/details/gnqgeywon.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gfzovvowf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gzxlvnwdx.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/guxzlthho.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/grresrdgh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gujztwdgp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gfzueviwq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gyjhahsfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gxqxpalzu.sHtML


<!-- 参考信息 -->