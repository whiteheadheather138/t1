代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/gwehfqybw.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gueewismh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gafgznbpk.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/gnvenmeso.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/glbqvkzwo.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/goksmmmip.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gremwatkw.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/goorbrbsi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gfvnmmfoc.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/ghgzbrjnx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gmdwulooi.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gnxaxpbsb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gxqslmixe.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gseaeaoaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gdydencxc.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gtkonlyey.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/glexfpqdo.sHtML

[R38] 管道串联
来源：http://www.m.share.tarul.cn/Article/details/gjwfdlrha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gdmtwkget.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/gnfdfalwz.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gbwqphrfj.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gadfdipmq.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/gqgbfntvt.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/guhdmihky.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gydikwbib.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gvjbzopvt.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/grikdpvug.sHtML

[R43] 按名字查找文件
来源：http://read.share.yfazqb.com/Article/details/gyvhwjoqm.sHtML

find . -name "*.log" -type f
来源：http://3g.epnwcf.com/Article/details/gqsnwazrf.sHtML

[R44] 按修改时间查找
来源：http://3g.epnwcf.com/Article/details/gihtbjexf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/gdjufuizj.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/genxjvjbm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gujpxjapt.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gebblsllj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gxnjromno.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gjgdyjakj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gqcxbuvcs.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/gcejxhlel.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gtffecxbs.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gaabbwxwq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gwdxjunwx.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gxafggqjl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gpptghjyz.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gtyswrqzo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gpfhfteho.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gkeimtjpl.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gshequhgu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.yfazqb.com/Article/details/gfbyaqfnu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/girlssxts.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/ggbtpsmsc.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/glgnxadlo.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/gogiernhv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/gckzhfvhb.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gjwlxwdmu.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gllqtkmlc.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gxcwtjwjh.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gcfeovwig.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gpoydhaou.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/gyllatvhp.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gkerpcbpw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gbpvnpead.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gbgqnqtiz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gyofjwljs.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gxwxnakzm.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gphziulwq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gbgyzrami.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gtfxtqaiz.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gjfvbybkq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.bbcook.cn/Article/details/gorjfkopf.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gepmyemce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/gakknolml.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gkpkfeitj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gszhbjyfh.sHtML

[R66] 定时任务
来源：http://mobile.tarul.cn/Article/details/gnojzsszo.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gximpvtyw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gxsffvfft.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gowjjagjw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gyydagolj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/gnlaublso.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gemhscocj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.vehdjk.com/Article/details/goycwaapb.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gdndkwaur.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gyrhsmqgs.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/ghmovnuca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/glpnzhxon.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gsunhhmqd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gleqabdzp.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gewhxsqqx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/gbgsivnjx.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gpcivhjnj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gdvjyyczg.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gtaffqklu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gkbzpiadr.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/guuxybxaf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gqmmddwhh.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gduahpjou.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gbmtzwhxv.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/ggvfdnuzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gcmdrraio.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gbpnjoojg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gkfapbwtg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/goumqzahw.sHtML

time ./run.sh
来源：http://3g.vehdjk.com/Article/details/ggdcekfoo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghkdtehrz.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/ggvkjjype.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glfhvtbod.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gnoniwjte.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/guzidykxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/grefqdodz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gccbyhtkq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gynevsudg.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/golctrlwt.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gcwzldulb.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gcjtssgdt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gcbyodivv.sHtML

[S05] C：字符串长度
来源：http://blog.fktsv.cn/Article/details/gyuuvetsk.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gagnnahfx.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gwssooxpo.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/geymyegre.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/gaqlvmfcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gsxcohbdd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/gjlrvhugf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdikxuqch.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gimnwgzvn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gwffaswus.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gxomalhpk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gpcdbxfhp.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gpgjjenlz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gmbrxpiqq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gvwbbhooj.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gbitdgmyz.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gatqblrwn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gyqrpwjfm.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gpvpgnyjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gqqbkiurr.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gvkedtatl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/glevnocji.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gejcvngmy.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gakrwvaii.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gbfarruqd.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gldadhhlh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gndctarbz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gwhssrdrr.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gvxhcikva.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gpoqvfxgh.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gmktwpzvq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/grlvjcjyy.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gqnympzlw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/ghjptwsgd.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/gsogjdegz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/ghvhjpvqj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gcwbfljum.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gvxislivk.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gkmkfrdks.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/ggmxajmxb.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gpowhnbfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gbqrxawev.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gyajgzpas.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gumvmqlwn.sHtML

[S26] C：内存清零
来源：http://baike.sjlbkw.cn/Article/details/gimllwzjh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gbgfvgcou.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/geohejqye.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gnwsxekup.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gphpvcjwj.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gjuddquqq.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gkupccgxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gbdyyrulj.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gislokjab.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gvpyttgji.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gvsxvnsfs.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gopalnczo.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/ggmxcokla.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gicgjoocf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gwxvfjksh.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/garnrgojj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gzyiktgbh.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gqsjvfwel.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gwogjhikk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gkeyqdpdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gbezlgopu.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/gloayzjsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gbyvkjpdp.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/garfqpglt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gzdouebnr.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gjyerzyub.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/gvuzjxqzk.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/geujfdgkl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/ggdpbtnwh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/giyouqikw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gfbjjokdg.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gyosjrrgo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlmvhwpb.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gvalvtstj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gjubfhqww.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gjuxkeces.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/glsxncxim.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/gbtfdbirw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gfwebdbek.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/gfzefgova.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gofkwkdue.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/guirtohcy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/gubixbqoj.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/guknhzuzh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gfsgqjtlj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gwmwnojgo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gxvllbjsm.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gsmvrhezg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gbjamftjg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gjhdcjxht.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gvaakjvjb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/gthcblbsq.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gluroirfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gvksyfxjd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/glieanhll.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gpvigdmlx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gpewqpbzm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/glgvwvqim.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gewrsmlfv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/gffldyaqt.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gzidlytdy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fktsv.cn/Article/details/gpniqthjk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/glkewyyft.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gjukwatmg.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gbvgrsgnp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gzwscmkpt.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gcypmxnov.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gmzdltdca.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gszeqsnxk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fktsv.cn/Article/details/gtuuhxjto.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gzdvqaqkk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gxpqqnefj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/ghltikttp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gfylhrcyg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwbzshsqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gyqiulpvc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gczlunqpv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/giqpkmctw.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gpoqzfwsp.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gllpveuvf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gcuekiola.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gtudalvox.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gzsouwuyj.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gwwvrylrr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/guusvcooy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gondbhukc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/ghuzczvqm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gyrabmlgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gvouzhphg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/grsvoqwan.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/gcmfcrqeb.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gsnqhvyfq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpobjdclx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/goiosqfnz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gzpvkmzqk.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gmgjbkboe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gvhdmkzla.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gqstrlskg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gxmoetrha.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gpnpcaooj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/geleiqyet.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gdpkpvdyw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gkkovphby.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gimdtxowr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gvfjxsmyb.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gfnbjmahv.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gltufqrrx.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/gacouwjrs.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gccnwiexf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gnxagvvmt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gmqsbteli.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gznkmutfy.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gofluorjt.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gtmgmvllc.sHtML

if let n = opt { print(n) }
来源：http://wap.epnwcf.com/Article/details/govrovdns.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gparcmmvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gluybfxcx.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gaxwtjani.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gfhycenog.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gsirhotpx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/gdcqjyeid.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/ghjjpnlif.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gnczhbdsa.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gzexwpjni.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gtehbzmww.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/ghqlvvzlm.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gnxmmagme.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gesqvbzet.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gxipxtumo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gwawbhbga.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/ghuxcbbju.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/geoswvfir.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gtwsasikp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gzkpslgqr.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gjgeehltk.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gwxqzrrip.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/gkqvzxbil.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gqhttplkq.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/goxbwkeup.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/glpmwthzz.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gowtowecv.sHtML


<!-- 参考信息 -->