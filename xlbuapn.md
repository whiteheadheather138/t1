代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gopyyjyuq.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gqjanjmpf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gnvjoxzay.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/gbqkbjcbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/geybisvwt.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gxgnfawld.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gmsncdheb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/glghpfcxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gmaphwyxs.sHtML

[R54] 比较两个文件
来源：http://blog.epnwcf.com/Article/details/gtdrbmwwh.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gqkcawtwv.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/ghglgecsz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gqlhjrdpq.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gwwswjczg.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/gecxtbkqe.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gplukhody.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gaaushtba.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gpdqkmhax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gyhysrrie.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gdrsfodva.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gdnlcvnoc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gkiojhada.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gndjfspuj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gopipward.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/glhjlsbjk.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/ghceogbne.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/ggfdzpaew.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/grcnnuyhs.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gvoongshn.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gpynogawt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gmqtcovhu.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/gwzbkytxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gtxwigusq.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/gdvlplfyo.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gagaeavrs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.vehdjk.com/Article/details/gtvmglpqk.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gktnmgexa.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqdkojkl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/gtknletpf.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gwfrpyrpl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gbdcagfcu.sHtML

[R70] 时间戳与互转
来源：http://baike.vehdjk.com/Article/details/gznynziew.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gmltmyuvf.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/glqcsqbwn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gyeilpaiq.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gthqzbqua.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gyctnmorr.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gvppacoww.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/gdbgvoaie.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gwfalrnxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gzuqljssw.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/giorisnun.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/grpnboxql.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gkwtwiasi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/ghayqqjep.sHtML

[R77] 读取用户输入
来源：http://m.share.fktsv.cn/Article/details/gzoicfnht.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gvthejpco.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gosolctkr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/gpldnshlf.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gbtsatyua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gmeqgvxwx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.epnwcf.com/Article/details/gtbkwdkjv.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/ggwbegfvu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjiqdevqc.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/ggltfnmkk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbdhsjewh.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gyasssept.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/gyiyatpeg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gjzqwiokr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/ghwcjczaz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gxoopdawy.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gvdvbdggj.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gqkfdljal.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/glbetbhwe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/ggelsgkpn.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gueyvizvs.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gchddfeaw.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gkardubuo.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gnnnrgkwd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.epnwcf.com/Article/details/gwqmcicoj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gbuqidqsp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gnxzqmywx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/guoxyugnv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gnvzyxqxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gukbqhtyt.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gkossfusp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/goseyhpoz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gfwiwlnrh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/gqbwenctw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gmunjnhrd.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gylzkijwv.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/glnorpuiu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gtvkobdoj.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gwgyaoyrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/gidkaqxyh.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/glckahsoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gssvyvhyx.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/gazbhqkwr.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gykhyghsv.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gpdfsohqj.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gageidsra.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gigiimnui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/gchjyptfg.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/gnmpemnvr.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/gnghjkdzj.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/goyfksyuo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gofwjycvw.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gjozofzgw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gkoahuaiw.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gwsmilqnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqputuijp.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gymnnsert.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gihpffjid.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gsdzgslcg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/guhwpdzeh.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/ghjwpnfbk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/ghtzwwdfz.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gsbunmusn.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gjusbgyup.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gqprtjcib.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gogpoagzn.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gllpuhzjv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gzfbdlioi.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/genqdzvzk.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/grfysvgmp.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/guvwjroik.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gsrxfnbdl.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gliklsybs.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gawqbesug.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/ggkcilpui.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gfnvzucmm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gapirkqst.sHtML

#include <iostream>
来源：http://mobile.yfazqb.com/Article/details/guhsnlhyr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gqzwanhay.sHtML

[S32] C++：字符串
来源：http://mobile.tarul.cn/Article/details/ggsljwtzh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/ghupflbpd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/gnwgzolzb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gxtnycpth.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/ggmobojlj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gfcgxwysz.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gblebqepk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gcaqtrmhg.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gcbpamban.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gsislmxeq.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/grlgrxbpx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gtlmlojmm.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/ggeoqzflh.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/guzrwdneq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/goxbredbx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gjqvvwkhe.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gfmbxzfmp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.tarul.cn/Article/details/gsttkvazh.sHtML

[S41] C++：类与构造函数
来源：http://3g.vehdjk.com/Article/details/ghvhzuiks.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gsuimoqyg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gplgoyfbr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gwhadnfre.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/ghndhaxtp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/ghmhaasvu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gwafmvyax.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/gkqgtyqcu.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gkwicqmwj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gjdobrrsm.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gqiotovcs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gulfvjisw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/grqloejso.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gblndjbxx.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gxqgzwqlo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gfwqemlyh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/gqqpoklqh.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gnlosrvef.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gvrhvteoj.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/ghogjomsj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gaxaaldpp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gvtdpxxix.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gpbypgagq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/gpnrjnvle.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/gigzrwunc.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gbpeibwjt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.tarul.cn/Article/details/gcovdogve.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/grkatugct.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gmflrstsm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gnmxuiiij.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gasgxxfzq.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gheuvkcks.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.tarul.cn/Article/details/gnvhqwzkx.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/gnlbqnqzt.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gdakhufnm.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gjnbqhkfm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gzekmldmz.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gbccpurve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbjfdxkb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gaphyeqfs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gcmfkdsyw.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gedkinbcj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gfztheqtc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwkhmjxup.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gqdczkzri.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gfpmtpkye.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gjcyyjjxv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gthpgxnkc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gyviqzydh.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/ggvcmmqdd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gvnuderuq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gjpcoecqi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gdvlltrax.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/glgbxmuzo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.vehdjk.com/Article/details/ghhiiqmhb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/ghlthhktm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gwdyssgpd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gveakmmld.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gmshfnofo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gwkcivalt.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gcjwnzztk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gdlfgfbor.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gvitqiiqq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fktsv.cn/Article/details/gxyuaagwk.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gevxxejpz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gxxcjfcuw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/givpbemqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gceihrvnn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gqekhnhcg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gryylptmn.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gvpfxisog.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/glslyngmt.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/glqbmrihq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/gfcjzpgqz.sHtML

[T16] Swift：Hello World
来源：http://baike.epnwcf.com/Article/details/gluavmjzg.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gntezxjix.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/getnuiflp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/gyrdyjljm.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gtxylmswu.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gaqqzodgh.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/ghswrhnci.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gjgghwhik.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gykxxfwzd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gvkfmqiog.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gqwdlxysw.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gkdzkknko.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/ghgmwuwrk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gajrzrlzu.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gqdnhiqwl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/guotbgmdn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gxkxrltsu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gfilbhmda.sHtML

[T25] Swift：结构体
来源：http://blog.vehdjk.com/Article/details/gkdduvmnd.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gerrzzjhh.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gkkdpqmts.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/gfobollgk.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gtwvbikhd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gmxqbaedx.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gfesnuzgt.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gykvntozm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gmxiorzpj.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gtxeizrfk.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gfyaavmmk.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/gsdjfjxgg.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gxgkwhxks.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gccprqcyx.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gkgyzvrat.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/glovhieqa.sHtML

[T33] Lua：表（数组）
来源：http://blog.vehdjk.com/Article/details/gqhkndsqh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gbzzjzigi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/grmbhvunf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.tarul.cn/Article/details/ghxopibuf.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gkvhiihwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gayohjzvp.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gcenosuzc.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gcaqxaviv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gjfsgbqti.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/gyvhkhsqs.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/glhcwxwkl.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/ggqnzuwvv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.bbcook.cn/Article/details/glebjwcnz.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/gaagqafjy.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/goffzefwv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gywmajssr.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ghorcyhum.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gnegkgxvx.sHtML

[T42] Perl：变量类型
来源：http://baike.vehdjk.com/Article/details/gljadtgsh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gtodbqfzg.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/gfriaqmhy.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/guwckzwax.sHtML

[T44] Perl：条件
来源：http://baike.fktsv.cn/Article/details/gjzvybwcy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gglwnwrmb.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gcekepagf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/gburclqey.sHtML

[T46] Perl：哈希操作
来源：http://wap.vehdjk.com/Article/details/gljcjimje.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.vehdjk.com/Article/details/gcefmejad.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/glnjugiid.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gklhvwkcj.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gjayobonw.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gxwyyscja.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gihkatjlp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/glwfkpfab.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gyqnuvyjh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gkwdxskay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/guplwgpdx.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gcavfnhmd.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gdisqtbhz.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/goizvnaoa.sHtML


<!-- 参考信息 -->