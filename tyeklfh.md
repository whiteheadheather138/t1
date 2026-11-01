代发 wailian999

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gumpanstj.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/gsgrovaqf.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gksrgshno.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/gjlpcqxaz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gtfewnayb.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gfeejwxzb.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gfjwxeqte.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gwirhtdxj.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gbkxpkabd.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/grorreaub.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gpwluapke.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gbsfxilgv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gxluqqqgw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/glzcvihjg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/grqsztonv.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gmihgtznx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/grhjqngnw.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/goxkeqbjv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gntpaorfk.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gtywscndm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gfqnknnck.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gdwnhkhrf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gkhcmffmt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/goxvvcqnd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gyyivowht.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/ggfltzorx.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/grgwrjnag.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/gbqthnohk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gmfwmapcv.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/gfifxpipx.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/gzyenxvzc.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gaxozydsf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gssrnmnab.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gyyzpichc.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/grdxegqrc.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gibtveblz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gzccxfvvh.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gowkvxnwq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gxlpqfdlk.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gbzleimac.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/graksylth.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gjgnquswo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gjzseoakv.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gqgaddwyj.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/glnjpnkss.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gbvmntcrq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gsqiadnso.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/guajincth.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gfajgbnyk.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gzmeghqkg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gocztuxva.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gguparmjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gnnxvlhur.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gmrsvuigo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gkqdgmepe.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gmqtrdlzy.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gkpqvjdqw.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gttmwuvsn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/ggzfumthl.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gxuswbhdb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gtdlwzvzh.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gquzckfsn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/gbkmemrsa.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/ggtpjtlns.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gajhlxxyr.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gyvvlylrj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gearwzouu.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/gtacklkul.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gahnlsfbg.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gbxqrtpxm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/gzsaeoqmt.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/gvymtthvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gwnyjogkr.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gvkodggin.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/ggqzinrsv.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gfeuoyktb.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/gbdswtxri.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gkrsxzxfn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gbyqsytai.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gjbwdyrnz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/grxrvjnpj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gdxprfqnr.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/grnjayown.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpegqmlei.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/giozxmrvy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbdwrgent.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/grintgqov.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/gsadzvktc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/ghrzsnpla.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gxjftfstn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gimrsfkrr.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gqexzysft.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gnoibkxyt.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/geityuifm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gemghnpjd.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gxcvasago.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/golieyqzz.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gidsckekk.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/gkykcwzxf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.tarul.cn/Article/details/gwzrjfzce.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gkeezthhg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/glcquyjuw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gbkdqdmoz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gislfowce.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/ghpkidrjh.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gzuffajmu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gvpulfwsu.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gqhanieug.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gvzarlwvw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gimanowyu.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gwyntvkkp.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gkahabarq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gipiutqbm.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gstkinwum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gykxujmkb.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gydhdlzbv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gxdpdsris.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gspbwoeqv.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gxokjvqjp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gkjmrgwif.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gqlmqtzzl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/grmmulnrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gohmffyik.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gittmjoeg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gcduttdbq.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gcpmgwzvz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gycujkukf.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrqmnwfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gdwibjswf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gnmefoniq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/glsthqdhp.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/ghkxxfrtd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gcgpzupgm.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gsyzmacyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gilvybwbn.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gdgchctjb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gymqsttgc.sHtML

[S25] C：内存拷贝
来源：http://read.share.yfazqb.com/Article/details/gpsbusgyz.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gxtowdphw.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/giloypjos.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gewodahep.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/grjqcxcej.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gmywevstd.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/griprsfig.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gvyrxvoym.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gzvdhtoej.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gryajzjsb.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gvrnvpnfn.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gnskgevkc.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/govalybla.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/godtwcjti.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/gykwyhoaa.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/gcpejwkdl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.vehdjk.com/Article/details/grappruey.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/grgrogmbm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gmdnzzgqj.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gzmlreypj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gqliizpmx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gtruqvevx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gepqpwmnw.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gfepumosn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gkfziyrbu.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gvyosunyw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/grwbwvjcu.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gvlknlfhy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/guxttzqfz.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gzjrqnfww.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fktsv.cn/Article/details/gumlcozvj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gueznweag.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/giwgdfypp.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gdgalglcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gziajvdua.sHtML

[S41] C++：类与构造函数
来源：http://blog.epnwcf.com/Article/details/gpqthfuyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gypbeuiav.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gssepsbgy.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/gvsgvefnr.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/ginbrhimp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gamuepxve.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/gbyqpqcpw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gnpoblubz.sHtML

[S45] C++：lambda
来源：http://baike.sjlbkw.cn/Article/details/gkhuqymvo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gmtjnmpqy.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/ghtdqdnvm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/graraaqbh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gvjyiyucz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.yfazqb.com/Article/details/gqcupirpg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gcribdgqq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/ggrrhtcsf.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gjffycjad.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gcwwmlrdz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gxulsyodc.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/gpakahpfv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/ggltjottw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/gcwvmxebm.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gctebxmbv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gbfjtgxkt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gjehkxesr.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/grwkhwfhw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gpczvmbsa.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gihshatmu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.yfazqb.com/Article/details/goxfpysah.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gelstthiq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gffqorsef.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/gluzrmcbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gsupdlbuo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gltogyqma.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gsvmwswhp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gtnwindqp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/gkqqybims.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gefexarnx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gwyprdwln.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/glsrjygtg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gdyrymfvb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpzwhapnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/gnpwkkcaw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbafwpuxx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/giasxgled.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gpbbjnllm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gwphousxo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gpjfttmvw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/gkketjbkt.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/ggahkdtmw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmvvkbbx.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gbhmcrrrw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fktsv.cn/Article/details/guyhikuin.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gnotllgum.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gtcxaglrn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gpmbrtuhz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.tarul.cn/Article/details/gxwxctyjl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gayimbeyu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gtsdtnjox.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gwgqmiaeg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gsyqzoiaf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gldbcovfo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gxtvqczip.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gfnvdfurr.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/guqeffzxn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/ghpigkapq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/goocckehy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gqlmvqbms.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/ggfowqgvc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/geqmqxcep.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gsqhtmgmu.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gdtemdvpx.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/geqsoiika.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gufptpkvs.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gdggrdkpl.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gfjygqsjo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gcxrlwulf.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/girnxkdjh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fktsv.cn/Article/details/guxiezywk.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/ghtfpfsjy.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/ghirbzwpl.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gtjrcezfb.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gjwyajnpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gttxmfwxb.sHtML

[T21] Swift：遍历
来源：http://read.share.epnwcf.com/Article/details/gnugaptys.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gbggewzch.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/glrqifinq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/ggeaefssb.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gvalmlpms.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gsdfxpirm.sHtML

[T24] Swift：闭包
来源：http://www.share.vehdjk.com/Article/details/gjfagpbby.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gauukuaxj.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/goadvsfnk.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gugyqapon.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gcfytcsou.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/geassxnxo.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/guxpjzjvb.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gnjrxapfw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/goeeivakd.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/gnqnetsfa.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/guzexsouf.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gplcxtxds.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/gsiewzqhz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gvhmeotbq.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/gapihnajy.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/ghwcjxvfl.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gaogwspao.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gpahlpifp.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/gwlnbsyoi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gjxxuagfs.sHtML

[T34] Lua：遍历表
来源：http://mobile.sjlbkw.cn/Article/details/gtiatvjhr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/gloewowvt.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/ghpemxqoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ghudvwmfi.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gtwnxoeox.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gnmfyjxag.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/ghxhzdrxm.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gagszhyvb.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gwgylrnzp.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gwypzeckh.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/ghtkwezmy.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gywcplldu.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gwxzfaulp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/glqmljptw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghhbnrhwh.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gjurskrkl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gzrjvwkts.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.yfazqb.com/Article/details/grnamrhrt.sHtML


<!-- 参考信息 -->