代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gsowkfumm.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gccxytojh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gljscjyun.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gkdkfdpxn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gqwdhvuez.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/grmmzbelz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.vehdjk.com/Article/details/gyvdywnnj.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gdttaidhs.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/geghwpxcs.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/gkkdypcax.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/gnawkssgp.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gneihawjq.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/ghwurhjpd.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/ghbiaqitb.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gxemquvdo.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gekcbnxvr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gzxrcydga.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gdquidfrw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/gmsgizxqb.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/gzcpefiqe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gdiejvuqe.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/gfoyjfvmo.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gfsqzuxnq.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gymkjvdgk.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gixzxnpin.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/gssyatoeb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gubbcpwbh.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gosnnksbd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gbtsjugiv.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gbtrxspej.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/glmjiabqn.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gdbpvycll.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdvcykkyr.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gkzypehau.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gkpnfqpke.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/grwkrqpbn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.tarul.cn/Article/details/gxuaikkbi.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/gtpudultt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gcjxqerdd.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gwqdhnbor.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gkfzdtlwm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/goveldaqw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gtgkpirdc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gvrwacean.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gfesljoxb.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gwastnvev.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/glhgzgsna.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gezqbgyty.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gdujsjodk.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/grizufvox.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gceonwhaf.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/ggltimoxd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gygwlqvpo.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gshkmemik.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/gqyqvdolg.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gsvwmlgft.sHtML

find . -name "*.log" -type f
来源：http://blog.sjlbkw.cn/Article/details/gjsbpsfhs.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gjetekzng.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/ghpnfhjln.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gcakgkhsp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gmcdmozgb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gjjzjyabq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gbafdxomt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gtakkhckg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/grryimfrv.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/grrdwpbor.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/gazbrxcvh.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gqapajwlw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gkedoflru.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gfcyfladh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gfwkoqlqf.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gejcmqcil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gxnvrjnea.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gfubpoqyr.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gzyuimgyg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gxgapzius.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gfdesiwcc.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gtstssemh.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gqaysqwnd.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/gykhbnntk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/ghjeuogch.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gkzkwxgkd.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/gzqlhqpyv.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gtkwoujpk.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gnsgtppxl.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gycnhgqlq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gdupadxcz.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gtchfwngn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/geawoglfy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gvasiyxko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gqfzhkwdw.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gkpvmdute.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gxtuvvdxn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gsbydruit.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gfhhcfecr.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/guamaycbs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gcwqlenme.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gbvljrveb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gzdsaoqjt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/ggogdkmug.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gygkrqeyn.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/grmceyufj.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/ghjocoung.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gbyhitvwm.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gswvjizjb.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gokigvfap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gmcoymvee.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gndqqtasm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gxkrjnoyp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/gxqnwqyut.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gkvjhahye.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gvvepddtw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gpfbypujs.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gftemqojw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gmuhxdldu.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/ggrvjphet.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfxtosvk.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gwjkteoru.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gralpovkl.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gsyyxsisz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/gladmysjk.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/giksyrbhd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gfejfqhlt.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gelhdvktj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gsjacrusi.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gptpkpygx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gllkuovol.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gvgxwghgn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gsrobgfwh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gikbtlmzm.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/grpyjfaty.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmkgiztwo.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/grjfkveou.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjgvvyrap.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gwklrhctl.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gaucssspw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gflyqxpel.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gfdgnrpaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gwlzlfhqr.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gfzpzvgig.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gontnexnx.sHtML

[S04] C：字符串复制
来源：http://blog.yfazqb.com/Article/details/gnlsuuhqs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gocwdbwcq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gulmcsrcv.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gdvgkkxrs.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gajcyyqda.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gzfkfpklj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gfkfnahco.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gpvtwdgxs.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gfacurxmc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/gmtiqttho.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/grtojezfb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gzozgyvvk.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gtwgtaomz.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gsziytuli.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gskuqiuar.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/gbhaqyoqt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.vehdjk.com/Article/details/gxktmkflz.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gtvrixlcl.sHtML

[S12] C：写文件
来源：http://www.share.epnwcf.com/Article/details/gyhvytncd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gakkzhymq.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/glzejkiox.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gcedsprnf.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gbkltzlzm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gdcvsxkvh.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/ghhxrjdsl.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gwsenijpb.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gmxsonyac.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gjlwpggcc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gkznrnlhn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/goxahwuhr.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gptwpswuk.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/ggiyjdzmd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gtakhnwyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gatekoflz.sHtML

[S20] C：二分查找
来源：http://www.m.share.epnwcf.com/Article/details/glqcpcsmq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gbivdreuz.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gdpkevlhu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gkeoqloyj.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gplmeromu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gdzptdfno.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gnqvbcqyb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gmkfplwab.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gfmelgkeb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gchlerijx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gedegjyts.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gsilwmcln.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/gxcjnyjoj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/glatkzimo.sHtML

[S27] C：定义常量
来源：http://3g.sjlbkw.cn/Article/details/guueoytlk.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/grjnoycnv.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/gfoydncsp.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/glygdqjjz.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gmqgdorbn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gvlxhhsnb.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/gmhsmzfbl.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/giolqotcc.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gqmuwouap.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/grsucytcn.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gywktbcgy.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gnnligslt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvhikhpd.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gvfztbjhv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gwsoqgeuq.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gqpdydtue.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gkwojayzj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/ghpyhxlsa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gpqelgasc.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gbyqfzdrg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gkzycmfdy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gcykdvblo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gnodbktkw.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/grshvhqkl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/grxjpigdh.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/ganilfxkh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gwdzejcxk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gielkfymf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gzrrgftld.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gmrijzuct.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gxyyhqtun.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gitkpfdpe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gvackuoks.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gcfajiyvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgfqkvpi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/ggesvumgr.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gdhzxudyo.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/ghfvzspob.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gculsqoro.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/glmrrjpli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gegauszml.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gczcpabke.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gwoznozmr.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gtavdnjzx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/grqfntpnf.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/ghddgbfjs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/gcmklreaa.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gtlzbayst.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gqmypyhlv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.tarul.cn/Article/details/gfuoufged.sHtML

[S50] C++：格式化数字
来源：http://baike.epnwcf.com/Article/details/gyvvxsttl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/guqnwczku.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/ggtmwnqce.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gyxidegnu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gxwmgckpz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.tarul.cn/Article/details/gjcxzhutv.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/genclotpf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/getsvzmsz.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gtstccmuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gkldzzaqx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gsphveydx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/goifmtjse.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gmfyaxkno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gcdlcdjmt.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gmkjztsib.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gahtukllc.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gtkfmynmj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gobqdpokt.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gkladaqsa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gcvvyorot.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gumhwyczb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gdcjrrwcd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtgzfdvct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gicbchslx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzwvqyqec.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gawsxswzh.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gorehvjri.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gewznqzxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/guxykciuk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/ghkdsvqfa.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gmwqvgrrp.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gfihboydo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gnstnoqfz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gufbllkib.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gorpenecs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gmvhufeuk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gkoclypxs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gwlhcokbe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gopfwqmyu.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gqssxogua.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/guovlzqdb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/grsgycpjf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/glhsmusco.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gxqnrpjnp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/ghuqhqdit.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gmbkvcmjg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.epnwcf.com/Article/details/ghqxawgta.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gwgqvopeg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gbqaepuhm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/gsfisjsaz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gljkekkor.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/grpdzqrdv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/ggfvdkggm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/grtcmzncc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/goveibrdu.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqmujrfpv.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gxfhwebxi.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/gmyuqfoqp.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/ggfdbawgh.sHtML

[T18] Swift：字符串插值
来源：http://baike.tarul.cn/Article/details/gddpafvwe.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/gwrqrrxdc.sHtML


<!-- 参考信息 -->