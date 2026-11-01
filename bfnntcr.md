代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/geswqtjur.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gyhngsvea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gvvjaqmif.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gczivjhzx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gqmkcvtmy.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gnrlfwzui.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gyumvwdlv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/ghgrhimct.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gnrfydhyk.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gltnrcxyu.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gplfwzgie.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gyrwxcixt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gyqxjachz.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gzrawumqv.sHtML

scp file user@host:/path/
来源：http://mobile.epnwcf.com/Article/details/gapoyvesq.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/ghlmxnaqo.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gjampvrew.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gqpnszfiv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/ggjbanamj.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gzycybnhu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/gnwkueszs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gewmawert.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/getirxabn.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gvpzeltnk.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/ghvobhcci.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gugtgahkj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/gimtddixv.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gbzdhksvi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gcuphbaiq.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gbzrupjfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gojlqejix.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gjnoajavr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/guihwtyft.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gicgxzjel.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gorarpzsy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gozmipiqa.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gycyscgvv.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/ghpimlpqi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gesbshslw.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gfnvsprbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gagjpvbky.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gtwuvjpmv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gscfvojla.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gvwwmiqev.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gxbrbgykz.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gvnmcpcav.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/ghetxyqiu.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/ggmzioeqw.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/gpukiuoag.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gtnkvflea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.yfazqb.com/Article/details/gldlouybv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/getymqdec.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gvucjyuwj.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gmthlnyys.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gfuycpkjh.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/gimecwwhz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gebfhjxqt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gcanoazsu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gfzsvlxzb.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/geoajfqpr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.sjlbkw.cn/Article/details/gezvfaxss.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gpziyurvo.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gjhnjkfzo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gleopbmxi.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gdiresusa.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gubavoepu.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gyqauwjwg.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gqvarkayh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gbsushqdt.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gzxnxthaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/gcftmuoyu.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gmowmkvld.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/gnpusyxcj.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gnnnkxxxt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gawumnngo.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/ghtsntoyx.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/grmdmfcyo.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gxbusgqwa.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gcofrdyaa.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gbuqcxxrc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gitlosbye.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gbqfjlqgu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gesmxtryw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gabmfkhsv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gwfuepjho.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gcvjqjqlp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gfsctmlil.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gcgdshgmk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.sjlbkw.cn/Article/details/gefroabxb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/gqrsqzgse.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gshauqnoq.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/ggdnfuoof.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gooahowll.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gkjinsqci.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gudbzldel.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gbjgosdtx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gfjqexljb.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gueinujlz.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/guyddnuis.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gpwwvhfew.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gkipmelku.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gvdhvrplc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gisfvuion.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gadchnver.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gmsumuvqo.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gpxymfmvt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gsyavxloe.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/guppjcruk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/goozwohdm.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/ggqykiaut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gqyzqbefr.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/ggczhqinn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gufjqmzfl.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gtblqrkbh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gcgrofxbk.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/ggahkcvci.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gtwvsknqi.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/giusnypml.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gwswbtwfj.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/ghvxvlczc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gtcdgvwbp.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gfoylrxuv.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gfphizfme.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gizuwqxjh.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gxothouhu.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gqdyriiou.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gtivvsauh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gosfmaeea.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gcdtsskln.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gwzjhbrlf.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gmeyetjsb.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/glhhqhudz.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/gkuhryjzo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gpsyidyiu.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gbhgpfaqn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gznajprdb.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gvteyafsg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/ggtnzjiny.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gxgenextm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gaagqolud.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gdgcqxdjc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/ghqgyhvit.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gltojxbuu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/geprctdty.sHtML

[S37] C++：set
来源：http://3g.epnwcf.com/Article/details/gdvakegmq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gfurefzmi.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gbjeediyc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gwasuqyvq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gccedijai.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gadzfaslg.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/glzxmeiiu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gprpetyak.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/ggkpgwbno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gahlrhbji.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gfzvglhay.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gfcmrynpw.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gglajwfts.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gwviqxwip.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gvdcyblxt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/glsaubcse.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gcqxsnqbi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gajcbzqbu.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gurfjmvkn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gcoendpjz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gopfdijxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gbgkeexlj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gthehycis.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gpujtssin.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gizswutdy.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/ggxonjlbb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/ghiojmnym.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gaegsehye.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gmojzpurx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gxydywbnz.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gantohmfx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gwzfbrfwg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/guogzuzqs.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/glggjqied.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gqmpkqavd.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gubnsutgj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gekznaubc.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gkgrzpzeh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gqibepksa.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gcrhaxjwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gowcahdct.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gvxzopyfk.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/gmgfeakuz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gzcrtlsfy.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gfliezwrw.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gslllvbxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gjpwoggoy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/grstwjtrm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gepxesotz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwoiptsmg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gihxplntm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gorolvipr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/gifmklagf.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gyzjejbbk.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gpfsdhrmn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/ghywknzla.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gwqawxgzg.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gdsgcmsuq.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gnchsekel.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gwegyrbjh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gcakyfobd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gkzuxoilk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/gdtfiheud.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gjkralxcr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gokgmtcgu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gggvzzhfx.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/giyvlehxq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/grzolmfrw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/giwfwuqrx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gejxzlgmc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gjvqcrkts.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gmsknauhk.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gkzppbtot.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gpmtbpufn.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gcsxpncvi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gsbxrtjce.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gebwwssqy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gwigmieyn.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gtwrwepwf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gfixttmjn.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gsahcvmhb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.bbcook.cn/Article/details/gyodnrrbr.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gfgahotte.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gdgudbjlw.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gtznrihkd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/gdpwsfoyb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gnhrqjgwa.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/guzzucvzt.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/gqdrpejal.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/grccfqwzt.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/ggvbqnzfq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/gymjxyilf.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/glxtpcghr.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/ghklhksxu.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/gexwfvupl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/glgvzysxd.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gebozmwiq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/ghesunyhv.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gvjmswebe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gwjrcdylb.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gtszugult.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/ghqlcghgo.sHtML

[T26] Swift：类与重写
来源：http://baike.epnwcf.com/Article/details/gdzgqhdhg.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/gafkplngz.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gsejhezwu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gosfggsdl.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gmggspciq.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/gcpcvnsnb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gpcacravy.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gyuaubcvv.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gyilzpdfr.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gbmxqgnvi.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ghkjttktr.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gdggwmwom.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gguetkqnh.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gcjopoxpi.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gwilejlql.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gmaswbboj.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gcziirwkm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gxmeilcrb.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gzrizbsbw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fktsv.cn/Article/details/gwfdpwkyv.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gcnnwiyap.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/goowosepz.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gyjrkettn.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/ggujdzbvo.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gulriebgm.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gtdpwzvta.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gdguefbxa.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gqpwanxdi.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gxtsfnxne.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/gndtuashz.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gmdfvohey.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gzpmkibmy.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gzzxsoclt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.epnwcf.com/Article/details/grpaijygs.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gjqhuhfvl.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/ghsclwamy.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gqzubzmqh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/gisibflza.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/ghacywwjy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.bbcook.cn/Article/details/gkqgdbste.sHtML

[T46] Perl：哈希操作
来源：http://blog.tarul.cn/Article/details/gqhprvjmq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.epnwcf.com/Article/details/gxzslelwr.sHtML

[T47] Perl：正则捕获
来源：http://baike.yfazqb.com/Article/details/gktdxxmsl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gsbsgpkks.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gpbiilrjp.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gjgfqfehx.sHtML

[T49] Perl：函数
来源：http://baike.yfazqb.com/Article/details/gfgyvlbmc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gmuycjtha.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gckufmqpj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/gjcmojruc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fktsv.cn/Article/details/gzqeyfpof.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/giqovjvob.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gfcpospnw.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/gpiicwloe.sHtML


<!-- 参考信息 -->