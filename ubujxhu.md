代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gkdapeyzs.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gxlajyvro.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gbooqlyra.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/glrcndpna.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/gqbgcyrwv.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gkztctbsv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/ganhtcjua.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/giqqmoatr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/glzeylhjd.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gnuufwlmc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gmxulberh.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gwlqjyiuh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gsgnshbxb.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gdeykcqka.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gaacuptah.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gziglskqy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gfqlmjgjd.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gkshwnovs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gdxsjmtok.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.sjlbkw.cn/Article/details/gsenehsmc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gobqagedv.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gdehpgqnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/guprgbywj.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/geqmqgwmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gzbzcybhj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gsiaqwtvc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/gyayobqke.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gfzfvlyet.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gzgyovqxc.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gjtdlsqlw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gvjowyzvy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gjednmxnr.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gurvziwgv.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gpoqqxjuv.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gyzfkmkdk.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/grrkrujcp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gagqpgaem.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/ghoxecqpg.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gntmkghuj.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/goganexro.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/gibcctnrn.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/getsdzbyk.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/gupvyuxxm.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gptovgwec.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/giipvgahm.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gzqqruebu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gskavfxwh.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gzwkzolsu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gfqvinkhw.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gxljnuvtn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/goxbjjoee.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gapkxpxgc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/glrbxqcpm.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/gxyzoojxl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gyrfllrhx.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/gnbflvklz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gtgmcrgxk.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gyzzqdpps.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gnyyjirzj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.sjlbkw.cn/Article/details/gshjaavbo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/glvckknxs.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gsmausrec.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/groigyxgt.sHtML

[R55] 压缩与解压
来源：http://www.blog.bbcook.cn/Article/details/gwmeiqkrj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gowxrocjp.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gxotacugj.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/glqoxdyly.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/gcdtzecvf.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gtyceawnp.sHtML

[R58] 下载文件
来源：http://www.share.fktsv.cn/Article/details/gvibvnisb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/glurourrw.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/ggnczvhxs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gupjhqobb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gedufsktg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.tarul.cn/Article/details/gvyoyyrdm.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/gkmbryovf.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gcdsikvjv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/ghuglubtv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gsuslvmvz.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/guqhpvqgj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gdvvbbral.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gknaxijog.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/ggxaelepx.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/ghgwbfdpi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gqtgxwhne.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gzntkslmf.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gyhrgafyu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gbhrshnuc.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gxchnbtzn.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gynspgurs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/gcupychfa.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gsntxpxrx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gtruwmrsb.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/gvfuzflxg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gombjcreq.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gwwxekygv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gyfmarhpc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gnaoixgym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gcoqspupl.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gmvdendod.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gxikbobcr.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/guazwcxhd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gchjwxsdg.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gtdiqkpzs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gpljzjbaa.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/gywaqcvjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gylanqres.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/glzeynwro.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/glprlfqop.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gtigyglpi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gpjjglrln.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/gongcojnt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/getcsljrd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gkjmtbnbz.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gmakkhuub.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnwhfldce.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/goxnmsufs.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyppixqfh.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gmouwycks.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gigsddklc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gyrakvesl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gjtpzoiqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gpprxmzjz.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gjtrgsjlc.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/gdgjdvjqb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/gyrcobcfu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/ggfiyvhid.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gjqstiewm.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gmgdfamqk.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gcgqkvfnn.sHtML

strcmp(a, b) == 0
来源：http://m.share.tarul.cn/Article/details/gxcqcwgsy.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gvvtuuqaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gstkicihl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/gcilgfyzf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gbylrkxgt.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gtvnrlhbn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gucaxgwmv.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gskphhehl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/gxdfjjuky.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gpwhszdbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gofjqwcrr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/grtsqvmqv.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gpbwkxxah.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/gojpkqawg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gslnwaidf.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gqxrvuphl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gohvmghfv.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gpvwixrgg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gbycnhsrp.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gvnpnjncp.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/gmbbfjxxe.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gtfdffncq.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gimbpopyh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/ggrywxhyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gyzbdcotv.sHtML

[S18] C：命令行参数
来源：http://read.share.bbcook.cn/Article/details/giciaxaxx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gbnekvdjh.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gjwwqtash.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gbpcfekgr.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/ggbffowuh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/goocgcshz.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gobjkbhim.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/gkbzfnsdu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gmvtvgzzx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gazlgbtdw.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/geeaeozgf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gwpuwdliv.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gwsdarchk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gxnwvrusn.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gigjqiwrr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gkomwudoq.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gcfgwifhx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gdcwpbpeg.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gxjvihupg.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gbvrxhwpk.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/ggedocyhv.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gjyjxzlfm.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoeyjxqq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fktsv.cn/Article/details/gwbvzecnv.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gefpqgnge.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/ggnzdjnyz.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gmmotsspm.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gqpistywf.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/gnyjwxofc.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gkhxgeisp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gzhxyiwkc.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gortqocmh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gtwbppjlm.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/glcepalbq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/ggjqgjzwe.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gymkwdpxh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gllczwrnq.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/ggzyylpym.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gfpvkktea.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/grrtdqmio.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/giylcauix.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gctjbelqy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gxoifveqw.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gwkquskan.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gwaughxxf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/gpfkjwtfd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gfjthzkxo.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gcvkdbjrl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gfhrsqrhr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gznjngezw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gwxpgxznp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gwoeqrbbl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/glvdqqnqu.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gjvcyibvx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gslntxcer.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gqfjtlrcz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/ghrnizglt.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gzyrnqcnt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gabwcrrpi.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gxuisulvp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gorpnmryr.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gcpkwnbvf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gjetizbpz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gniozlarx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/giopyviur.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/glcmrxfzc.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gtvrlzatj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/gehtivnfn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gbobhvavg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.yfazqb.com/Article/details/gvrbxycka.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gyrccsxni.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gomuhhwbj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/ghzxqrjqn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/gigwbfkzn.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gkplyevmf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/ggcxyuaxu.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gjhodcgbi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gsshfqfkm.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gmjvbqkbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gvqqblkef.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/gnyqgmzkg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gbrbnfrdr.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/gkmrmfajz.sHtML

constexpr int N = 10;
来源：http://baike.sjlbkw.cn/Article/details/gzymkdpuw.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gjsolsvje.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gxcklaegl.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gpowlukcg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/gbqyoeodq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gpqxffbqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.tarul.cn/Article/details/gsrplokbi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzsxmkotl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/ghtibkoth.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfendzbsm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/goyxednrv.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gtqqbdsur.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gerukchmo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gdueqthji.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gvqaatpuz.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gtlyppwlh.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gsclvztui.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwgfivrh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gtulcvurg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gwnaldysr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gwdaeegdm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fktsv.cn/Article/details/guuskhqot.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gbrsmukdm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/glpqhqajw.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gjcdjnmtu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/glmrnpsvc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gqygwwdov.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gkouucovw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gmuxzqmqm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/gipwvnuat.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gcpnewess.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gkobgrdbo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/ghmhcyjzo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gppgydpoh.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.yfazqb.com/Article/details/gyzvdvnhg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gcbrsvogr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gyhhpxvti.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gacytaxdh.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gbodjjtjg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gzjjzlpsz.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/gnoumqejl.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gexftgctx.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/ghwkzlphs.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/glcyvmovw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gyffxekzm.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gblggnzsn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/ggdbpzgjr.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gbvmzoozq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gfxeuulne.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gkmnwpsis.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/ghllaydsa.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gmvxgtwtz.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gkhbcghpe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gltbunouo.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/ggoraklcs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gzyhlkutz.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gircgdbzk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gderffrvh.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/ghsabajar.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gcqxdapal.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gfjvxhvkq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/gnvdwzhji.sHtML


<!-- 参考信息 -->