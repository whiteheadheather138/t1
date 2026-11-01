代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gdggjfvso.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gzbkoiaxe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gjfkgpmfr.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gmpjtpwnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gceetajar.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gmlceziem.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/gyiucavbn.sHtML

[R11] case 多分支
来源：http://mobile.vehdjk.com/Article/details/gsljcdtdl.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/gflfwwiol.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gvtxsnaoi.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gtubdiice.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gmtysohdq.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/gyvcjiiwc.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gtxwzartr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gqzimmgpp.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gnojelnao.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/grbogfnzg.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gthxgcazo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gtnmhjuiy.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gqbzqnjgf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.tarul.cn/Article/details/gulqdozio.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gldcwueyy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gfsmvywvy.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/ggqiusnqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/gosdvebju.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gtorgglch.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gshjwvjkc.sHtML

[R19] 数组长度
来源：http://blog.vehdjk.com/Article/details/guccodsgb.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gznhkjjgo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gugexvqln.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/ghtgqvuak.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/geanvfzxc.sHtML

echo "${#s}"
来源：http://mobile.fktsv.cn/Article/details/gfiunkfyh.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gvfaoxctb.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gydgnpwps.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gjsghwxve.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gcopzwxeq.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gxoprviee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/ggwybxxjs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gvkbmkles.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gstiffolu.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gmsehheen.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gwcpbnuli.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gvaigmzzd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gugzahqwm.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gctqpvljg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/goxkjsavj.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gmytwstax.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gdlnppuel.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/ghebzzncz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gqkcmmgrg.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/geiyusclq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gvaplxwzg.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/gssfqnrkf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/grwugdkuv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gjtdvmofa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gnuhkyfyy.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gkirlxiai.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gitqdigkj.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gbtjbjiom.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gpsvrennk.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gwfzynkdy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/godcrfqkd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gssrdrmkb.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/ghmcmuesp.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gnkwzuplk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gjvedgbjo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gqedlbugp.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gtdtyajng.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gxizglvdw.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/glgzxpsge.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gcrcuztux.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gacbiihnd.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gsxtsmnnl.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/geapqwfgd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gexgbehcf.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gayskiqtr.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/grguxsfuk.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gbuahdage.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gryqaovzs.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/geqjdqdup.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gkcugyake.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gltdvqsip.sHtML

[R47] sed 单行替换
来源：http://m.share.yfazqb.com/Article/details/gxcsmulel.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gsvfgervx.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gvpvjcjju.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/gyslaayrn.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/ggalhvjzr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gnvnbkveo.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/glkumxgmm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gsmukswnw.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/ggybtixvb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gumpmggme.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/gnqwdoong.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/grjrkvizv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gblifvwge.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/gamvliqvw.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gpxlfbncp.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gttstvyzp.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gfubrgczy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gvsrzzrvt.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/ganavespe.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gwjpavurn.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gtymwrsrj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.tarul.cn/Article/details/geiutqwhm.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/glyuhpddv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gqcetiath.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gmsledgaq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gvdswbavz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gghmhrxua.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gzolotmvh.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/geirzecat.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gsxjhpptf.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/grxjccewg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/ggfztaxoj.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/grvjzjhvr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gihhwmpwg.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/ghutyhlkh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/goqjrkegy.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gpuljhhfi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gtgbiqnkv.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gejhrxfmu.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gapurtkdc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/gqtgmwnsh.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gdbnlqzww.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gtydkbctv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gpefynltx.sHtML

[R69] 生成随机密码
来源：http://www.share.sjlbkw.cn/Article/details/gvdzeetoc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gwcaheptt.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gdmmivllo.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gsihjssbk.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/ggagbpmwt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/guhqplcsf.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gonklrcuh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gwtfvzsqv.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/gpawtkqdb.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gwlyejnyt.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/grqdhtzdw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/geilaedqy.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/guhpficga.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gsbmdtlha.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gdptuxdig.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gogwbtlda.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gztmripxc.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gwstqjxlr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gqmwshcng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gmqgvogli.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gssedsyid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gthuoicrp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gjeatnomj.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gkxfaeklg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqgyljhbd.sHtML

S. C / C++ 专题
来源：http://baike.epnwcf.com/Article/details/gtluahojq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwggbkjzo.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gzusvrovj.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/ghmkrbbqr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/gzxxxcykw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/ggmnkbsys.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gshuejtkw.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gbouelfap.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gldrcuthk.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gqdbhfwba.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.tarul.cn/Article/details/gvjkfrgfj.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/guurvuccs.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/geaehvmos.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gwzaqctvi.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/guuwetdjz.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gvlsubtpy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/guhqqmamu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gaiizatno.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gefrhalud.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gfiqayesc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gfugutwyd.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/gvofpfyhu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/ggdalklev.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gygwxshga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gpfedpalu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/ghuzeynxt.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gdaoqffwi.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/ggzkjhncp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/giqzwdzsr.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/guwzjzgrd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gxncrugjl.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gzruqeinj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gctityzgs.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gykiyxiiy.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/gmxrqecsz.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/grujdyypp.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gdfhviafg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gptcoskan.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gxxqlmlid.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gubsplver.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gcuhfernz.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gqqtxlcyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gaxvevzmp.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gxjwdioyu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gudzhpojw.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/grjrnxqao.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/ghxllqdsa.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/glfxraeim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/ghxzfzqpb.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/grfxxyimw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gdtkynkxu.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gbnptoder.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/ghhwlfrbe.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/ggmctzmtj.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gwvbwjqvr.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gffcfxhne.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gjyvusixb.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gpqkydkfk.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gakbrbvau.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gqrcbjtdt.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gjgaehwpp.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gqldxtqvm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gjdozzsva.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gbnbxwkow.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gkqviaxkf.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gusnlejgp.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/gjelpixmh.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gylflujyw.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gxylckszd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gqwvaeyse.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gobrrjyai.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/guceqlxmu.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gdjvpkqba.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gjvidtrne.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gnlpjuucy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/giklfapko.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/ggpbflcen.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gipxfufqq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/gvjkkuwdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gchcjpoxk.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gdrparsuk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gbkgwxmnx.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gjmcvjamg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gpchhusqg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gynscazmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gpzzbfkft.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gruwzpawv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gkntpowfw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmfeqxjf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gghbpboth.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/gaizazycq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fktsv.cn/Article/details/gagoggygr.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gjxnfqfsz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gvpbsjlbq.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbwbknd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gegyczxsh.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/galwcwcvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/guxswzfdr.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gglwtrjjx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/grhvjtzxo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gusomdiwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/glyjuherd.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/guspnweno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gomhuoeaw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gnthqzxgn.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gpfuueadd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gwaxzkidf.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gdzftlnfi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gpmrfxnzu.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gredywdzh.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gpszmjjlw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gcajoqdlm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gebmnzouq.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/goodapleo.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gvnxcnnyq.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/grwzblgzf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gtofwardw.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gujfeyrou.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gvwrkpina.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gsrvhykrj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gwiuqwdbp.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/galgdeaef.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/girzloxlp.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/gwyopibtu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gvhitbkqj.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gtafbqelz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/genkoezmi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gglhnbkxl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gvgyljryi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsxthgwts.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gcwfpncvq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gomtuvfxx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/ggvohgvxu.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gfssokxjc.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gepwxpppp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gnwhdlurq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gvunrmrxa.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gxoywlhtg.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gczndteiv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gtnuonrse.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gnijfillf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gmqxfqbri.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gyqmdenyt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gudxxietn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gtfzlqjnb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.yfazqb.com/Article/details/gvjdqrmfc.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gybbupatk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gjxbnefbt.sHtML


<!-- 参考信息 -->