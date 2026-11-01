代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/ghvngxjrg.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/ghfbjylfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/gfzblmwgj.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gyrogxdft.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gdporhntb.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gxszwjjmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gonfxiinc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/gklhvrqnx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gxumqqlcd.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gzefleqyk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gytywxfgt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gwfgzzqkv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gxjmfdujh.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/ggvqbhfrb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/gbiwcpcgo.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gxddnbgkf.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/gxelqcoae.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/gyorfhiqq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gimiwjuin.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/gtzccjnge.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gxxowelgb.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gjwjrcibr.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/ghcigiwzz.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gfntdbqdr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gwjwfiwvo.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gtepewrzx.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gwazcnula.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gmbbzgbqe.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/golriueat.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gadwgzuww.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/goeeqrjjf.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/grmnyjgwb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gvnzwcdiw.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gshfahsrv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gqylxxnci.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gvbyegpcd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gqnshbpgk.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/gqnxorqvj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gneiuvewc.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gebwuusbb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gpcrjcfbj.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gqfscvgry.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gqkcpmlhp.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gsctgjlun.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/galmjzcdk.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gydoymtwb.sHtML

wc -l a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gaqtcvyar.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/guqpxwnob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gqkneihke.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gakgaeeos.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/ggnwjukgy.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gzzbpapwa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/grwylpqvn.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gdmonqniz.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/glsdroxjn.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gbtsbeurj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gjopmaajd.sHtML

[R58] 下载文件
来源：http://mobile.sjlbkw.cn/Article/details/gstocwshu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/ghpagdmxx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gssxfuqli.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gduzukqvp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/guiqwgnhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/glwgeyfwr.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gdrzktpgy.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gxzxklgeu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gwdvvjdfo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/goijeunqs.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/ghvwntwdd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gzufbpqep.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gxadelkng.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gfyxjdxps.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/galjlpurw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gcqjmndjp.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/grvicxtzq.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gqdmzooza.sHtML

[R67] 生成随机十六进制串
来源：http://blog.epnwcf.com/Article/details/ggkdroqgs.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/gldoifknx.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/ghtwgaxrg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.yfazqb.com/Article/details/gdjkvzcwr.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gqttfktez.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gusmpgtzd.sHtML

[R70] 时间戳与互转
来源：http://blog.tarul.cn/Article/details/geelfucsr.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gccfaztpw.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gjadunlyc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.epnwcf.com/Article/details/gzmcrhpex.sHtML

[R72] 等待端口就绪
来源：http://m.share.tarul.cn/Article/details/gpyqqrijy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/ggnjretnz.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gomeolplk.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gcrwsjqxz.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gzgcxamie.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gxidszqnw.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gmcmwhruz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/guhaevlho.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/glyjvrfcr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/grznphcom.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gjnghzvdf.sHtML

read -rp "请输入: " ans
来源：http://www.share.epnwcf.com/Article/details/gizbrvwhb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gbkbgidcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gibgjhhpw.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gbnwbejed.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gqgrmhbkq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/gqzslvbos.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gzsepmuue.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmwqsrxyw.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gqodjaaab.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/goezeiqnf.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gfccmvvey.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/goamkpwte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/gzbyjflaj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/glvtkmmrr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gzymokzfe.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gdpancqir.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gvyalpptj.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/ggvlyayag.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gwbbfpggg.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gchdsegco.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gzjyxhhkc.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/ghfonwgnm.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/goadisisv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gikohnrrg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gwqvbzzfw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gkzbszrwm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gpiwtcwlj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fktsv.cn/Article/details/gnmtzwzcs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gadtmytrf.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gprrzemqd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/ghlzpsuhf.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gvqnnwkso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gafbjnfbz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gilkcyahg.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gwuaxyiwl.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gcvaelziv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gocoknufp.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gdclckwvs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gzbbkfvyb.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gnlyfhtza.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/ggnmfqdgu.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gacjckpxu.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gdezhibjc.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/grgxrbamd.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gjbvpgkhx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gmpuajhvp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gufnyoewj.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gcemrhkev.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gfzvjvuyb.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gxiwoedma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gcddkighs.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gwjjvfunw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gmpfxpiyr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/gvjccqtic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gssznjpqs.sHtML

[S22] C：字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gnodkoivm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/gmixyejym.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gufkmhghe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gauigoxyy.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gfiwjbgbr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/ghpgqzrur.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gfgvshsby.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gbknhizcz.sHtML

[S26] C：内存清零
来源：http://baike.vehdjk.com/Article/details/gmzdfbnxa.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gkwwnkbvy.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gbtilpdtt.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gwdiewrrp.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gxsbobaaa.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gkohkfcjq.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gerumpiig.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gqzzbqiwa.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/govobsisf.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gznydadww.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/grisackmt.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/gtqujoazt.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gcpxjafxe.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/goqinblqc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gtbgneibo.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/giaxhqkpd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gwhpnnxmv.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gmrmxhjrr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gktyioadr.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/grgemnfnw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gawpxwkwf.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/giylfvmjp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gjwmbaexq.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gutfdocra.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gktzuwrvv.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gomdvhidf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fktsv.cn/Article/details/grngvqssq.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gofhdosye.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gaeqvkbnd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gfxlfaufa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gukpyselr.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gavyhonyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gbfnxdckr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/glqhroycw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gbbxqalyp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gnlqpuyue.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/gbghuhiyx.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gemjcewen.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gikgxirzp.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gtvxtgugq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gvcdmjnit.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gtuddekms.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gixkkvbik.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gnydyjwhm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gsarjzjwz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gqrylmbij.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gguyzvglv.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/goxsdumho.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gwsgyfaxl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/gvyryvodh.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gohbwnkyv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/giouaysju.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gynixjxra.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gahrqbhvf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gkuengpws.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/ginmpywbq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gzjoyunmz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gsbaksfbj.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gyxhfbogn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gxtvzlexu.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gacnwemxx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gwqnspqdr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gqccwelgi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/goiquichb.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gptsoiant.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gxsrtuqrt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/glwopgwjt.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/glebdwlrc.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/guqbltnzr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gurmmwzgf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/galcypczy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gmvzcbxan.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gvjgeoukn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gkhrqeybe.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gphjqymye.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gypuxxywo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtsvhnzxr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gvfjtqzxk.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gycfnqlyv.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gnflxacoh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gdufdmpid.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/goxfwaxma.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gdfbcwmft.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gwvzojyph.sHtML

val n: String? = null;  n?.length
来源：http://blog.yfazqb.com/Article/details/gqzdtxwie.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gygqyeegk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.sjlbkw.cn/Article/details/gyfyaaqhv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gfjkxhtje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gxtixrgtx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gtrrtiquf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gmfabfxdo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gffvlgods.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/geymfrkre.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gqpthunlc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gxqfrxnil.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gagjmvrwv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gdiarhmqv.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gttnbfdjc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gbgvyuksw.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/gikyhlsve.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/geptsaxmb.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gdodcmeob.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/guknkluad.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gvnoknbhl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdupuxnr.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gqpmzthlp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gycpebpxm.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/gfudbtmsp.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gpwayohin.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/ghsdiobsw.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/guwxrnbpz.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gindlqupb.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gagwscfse.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/glpxjuzgb.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/ghubotxsf.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/gcxbvkuyk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gypcjpgne.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/gctaikjwc.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gpqmpxdrn.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gfbnrjunt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gwqjzcesd.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/glkqzbxzn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gtvnbujlt.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/gmdekccpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gfkwbwkra.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gifzvxvod.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gcbtimjps.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/goroidqfp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/guemccstp.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gihasstjr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gyofnkqkv.sHtML

[T28] Swift：枚举
来源：http://read.share.vehdjk.com/Article/details/gtbgtemjz.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gyodbhvdx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gllokvjaz.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gniwidlla.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/ghfzmpcup.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gvnhzplhy.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/gmyrkvypr.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gjocqceiy.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gznomzpyq.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gdzdtppau.sHtML


<!-- 参考信息 -->