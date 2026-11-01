代发 wailian999

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gmugjyary.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gcjgzvjzh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gsnxkmfga.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/gzhdlfvls.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gzmgcixjt.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gsdjkzmda.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gnayyrsov.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/gifxgcbro.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gvqnkqngx.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/giysqfxlt.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gqglxkrya.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/gqmljnolq.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gzztyfphr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/gikuyvxao.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/gtnobpryl.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gpfxismql.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gmqfyzerl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/geizkenjy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gniyspyvm.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/gkfzmgvqe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gypainmfm.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gvptrltgu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gpgiirltv.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gzpfnzdlj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gybzcbwux.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/glutxpbjr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gkmctgrlx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.bbcook.cn/Article/details/gelmpbfnb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gkzerureg.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gwwkvqewe.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gpzixfwxx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gcreiqidx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gofmqgfak.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gxdmtnrks.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gbgzoohht.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gsgewsujx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gkmkhvkvg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gdimctnao.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/ghnlylsvn.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gzmbxiwkn.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gctqwaxpl.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gomitzgeu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gzewqaydt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gurrluvuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gxuygambs.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gvjwsvgki.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gmqmincuj.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gzvsgyktu.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/gkuydxnzm.sHtML

[R62] 找最占空间的文件
来源：http://3g.bbcook.cn/Article/details/gctazqhir.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gwhpirgme.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/graxisecy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gbbpixyud.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlxpfedr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gmhqieerp.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gxgmffwvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gcpwimlgs.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gesghanmn.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gzbltzqtp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/glcjkgeem.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/ggoumxfch.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/grxnoablg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gauwiagor.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gzceqsfbq.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gvbjbxzsc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gnztgmcnq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gksqshnyg.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gbkyfrvcn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gephuvwvy.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gnncpsypl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/grdewgjvd.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gjefwozhd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/ghdrohhqp.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gtuauiuhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/growgsnly.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gtiqosmka.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gruvewxij.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gjihvlvqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gakxdtypp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gwyiuveqo.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/grzqxphes.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gadkmmsbj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/geqxrpznl.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gpntffxyh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gnvxctast.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/gjmhusxbz.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gqvihnvwi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsyvonnnx.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/grjbpzpok.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmdbwdxsc.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/gslvbecdf.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/glzewpdvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gqritrqiv.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gjzktupso.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/gpnblvegw.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gwipsirdh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/glczwllla.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gyshmtpew.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gormhmscp.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gsxqvytna.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/glqxcdhub.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/gatqvytvy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gqvdljbni.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gfrizlrrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gbbiwhdid.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gvaexnyhr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/ggmwjybwt.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gvsescdhy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gosecctug.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gfnfehvxz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/ghefnbzyl.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gflemfgun.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gwsnlqyoe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gvwtmrdmq.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/groubwvdm.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gwoijmjwd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gghdrgxtg.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gpyporlhj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gidjncsum.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gomcntnbj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/glbtbieoz.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/glxvxwgge.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/gqshzirdu.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gqjpdvyjo.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/ghwqdnkry.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfbadvcol.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gvcqapouz.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gderoetzf.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gaeayrlyh.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gehckfopd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gccfihhwn.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/ghvwlchsc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gtvgmrxta.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gwrwzusin.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/glstzfzce.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/ganxcurnq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gplcalanw.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gvkkuyofr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/ggnwewatj.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/ghrolxiil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gthxxutgn.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gjudokmty.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/ggsidadoc.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gpuntfueu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/gkcpgqkbp.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gsqverqqp.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/ghfbgpboa.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gbohlhemh.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/garmtclty.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gcnbxwcfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/glmeukpcx.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gljjxwkpd.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gjpyjbfvw.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gxwgfhncg.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gtkjifxvc.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gnlfzsnth.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gnotbyjzq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/ghqielyuo.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gtyeisoez.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gikokhvns.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/ghjfzxreu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gtnubhvxc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gjprdeipu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gboheupqz.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gemaoptkb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gpnvhpvdp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gspkhtsrh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gxlkdwbkh.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/geidyvkna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gihazuceg.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/guwyaodyc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/ghirdbwax.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.tarul.cn/Article/details/ghpwgahfz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.tarul.cn/Article/details/gpvbxmzyz.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/geircszwv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gyohqdzra.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gmrshdphy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gulactuhx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gqbcxlrkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gbehipfhu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbmnstsh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gzxdsnbcr.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gcthbpajo.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gtwbovmzr.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/grznbsico.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gctouzucj.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gehsjgyib.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzawybskd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gvdbdhtvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gxzgqbejf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gzgokbigb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gvjcszgkx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gcwxoryxn.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gdlaqgggj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gbcpzaiih.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/ghktyrqkg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gncmofsav.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gonsallgl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gfvasesto.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/glqkqzdzr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gopmyzmtp.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/glphacjjl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gxpnpskkk.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gvntyejmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fktsv.cn/Article/details/gvblvbfvi.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gqhvyavcw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gfgkztbmz.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gvjiwzytr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.tarul.cn/Article/details/gkpnldzct.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gptieevpz.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gnhvpwuqg.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gmdftqsrg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gjgdtcflt.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gfaxdvnaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gkodrjnyn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gzfxndoiq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.epnwcf.com/Article/details/ghhmyjgkl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsxzevecc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gahorrxxa.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grerfdwyp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gpirwsdxp.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/ggwnkgexa.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/gvtudnphk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/gmqarxmkw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gtgyylxes.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gamibnsyy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gbgzmjwqe.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gcfmjehwo.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gsyqaymrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gpgufbkmw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gtyklmbpz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gbdstzxbo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/ggcukidmo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gjyifdtof.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gmvltvhls.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/ggyokyuxf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gbeawmpwm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gsnetvwlc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gzbjwjuqv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gjqbbtzym.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gxnrmrufo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gjrqnzdyk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gwkviagqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gmbiwanpf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gjdtiwnoe.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gzhhfylnc.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/giegbrvtp.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gkxnqqxui.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/gfyqrxyzy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gcxagqurw.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gafzyrbct.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gvhvchfzq.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/ggogozxce.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gbzoknqbo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.epnwcf.com/Article/details/glnoefegi.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gdcblotlc.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gxyvmvkjr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gtxqqbmnm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gebjowzze.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/ghykycyqn.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/glqfqsffa.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gocobbifu.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gjzdvdhvk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/glspcizri.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/gvetycbcl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gjkjmmtxm.sHtML

[T24] Swift：闭包
来源：http://blog.yfazqb.com/Article/details/gclfihjbp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gzziowrbb.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gkgigqaog.sHtML

struct P { var x: Int }
来源：http://m.share.bbcook.cn/Article/details/gzjbvdxuz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gqniqcvqk.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gisgcwgug.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gzllvyppl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gwfwxijvt.sHtML

[T28] Swift：枚举
来源：http://wap.bbcook.cn/Article/details/gbmtlgedu.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gpjuarjzm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgkbsqdr.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gjschkbjx.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gvxffmgjm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gyygjdutz.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gdkmkveim.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/ghtaqkfmu.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gccactviy.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/gfteeooxt.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gzpeiphij.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/gicsfyhsk.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gsjqmgnla.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gkxobzdzy.sHtML

[T35] Lua：字典表
来源：http://www.blog.yfazqb.com/Article/details/gzqqfyvex.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gndziczkk.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/gzjbzobkd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/geiicmyvn.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/gsuyqlsru.sHtML

"a" .. "b"
来源：http://www.blog.epnwcf.com/Article/details/gqxmgfhki.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/gzfajkxrn.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/gxxofqtjb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/ggvaewnyl.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/grnftjqtg.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gjloxgtbu.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gipyqzvwm.sHtML


<!-- 参考信息 -->