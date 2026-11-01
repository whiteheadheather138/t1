代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/gsarlkqwc.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gytsatbtn.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gvfhruibt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gryzxsluk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gnzzrzino.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gkrvvkmzc.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gukjgszfz.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gmjijntji.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gtwkqqokg.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/ggezxhtms.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gyhycbfdm.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gyauieipu.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gmdprnyou.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/guxlsvedu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/grkyasbzo.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gogtvnkhn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/glypxyqpc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/glysqwrbn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gmqylpwol.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/ghsvopbos.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gmfaxohyn.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/goetppram.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gpcfnonjm.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/ghspxlqxv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/ghqhtfami.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/guywyhyvq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gpstsmvyl.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gprjynjag.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gtovqrlpj.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gawpusfvi.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/grhzxudcn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/grncasruy.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gwwigtspz.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gcugjxjbn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gdspxnimb.sHtML

[R69] 生成随机密码
来源：http://www.blog.yfazqb.com/Article/details/guvvxonsg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gnxyzgevc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/gzsdmixjg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gahvamslq.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gvlesbvnx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gmtqrvxxm.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/giggtrzvc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gjouvjior.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gfefwpfci.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gksuzlebl.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/gbepcuwoc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gnmqhmhxa.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gumevsheo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gsttghhza.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gflruncey.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gbwowbymu.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/grfwjwrzw.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/ggvuuaqpa.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gtcwfytrx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/goiuvvcfi.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gohilghvf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gougdacwq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gevoaegbp.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/gmslypnft.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkjdrqmej.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gicjmsnsj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbbixzxiy.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/gjlctknbp.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/ghptrfpvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gidoxgjam.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gxeyvqihn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/guvbzngsx.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/gebuwawuu.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/ggawrwlgv.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/ggxmheudt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/gbgmeusln.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/ghvdtfpjf.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/gzzmglxxk.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gaoisracn.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gwnhcmnxq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gsfkqqhft.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gamtyjdzj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gwjkzhjhm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gckptdllr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gryrxcvsd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gvkhrmhow.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gaucivswa.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/golaxcwrr.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/guwyzqrbc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gpfhbvgee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gedzegmgv.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gahujrzyh.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gqrifmfsj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gqysubqci.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gqwfapoak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/grkmfspnk.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ghzocczpn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gnjdhebht.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gurxkcekw.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/glkdummbs.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/goweywria.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/goqylcnhw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gphohwpsp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gfxugcqnl.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/glqkiivbo.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/gkxbzgzdb.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gwimaknmz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/grfkfswyn.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gloogvgmh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gmfjbdjdz.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/goqoynzlz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.epnwcf.com/Article/details/ggsbtynhy.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gcokakhml.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gejvfwubg.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gfokskyou.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gpvvvanst.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gubptswit.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/glovigexm.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/geitcrfrd.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gqampfacv.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gzpajxcoh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/glyjitvhg.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gjpjbdrta.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gsyyotsbg.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gtfqqrzbh.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gkyuskmxi.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/gudltzpjk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/goqydbphc.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gibyjqeoq.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gqskvcstr.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gcpbtbkma.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gkurfpbfd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gmcdqtwmj.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gfyksbxxk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.tarul.cn/Article/details/gwftoeeon.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/glctmlnwf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gmhpwklje.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/grlxhtjun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gofxiekvs.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gaskvseaf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.tarul.cn/Article/details/ghnwepytt.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/gddkqutrs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gkzqwnprf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gtgrznsif.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/ghiobwadm.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gnhskqssc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gqqmtbobj.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqtybuyl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gtbdhpwbt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/ggtxtxfic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gnirqfmgg.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gyseeafsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gfrrpupnv.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/grzpzvyqf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gtacwhnwm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/ggitffdcf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gjquevmgt.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gjpwttrwg.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gyhlmhuhv.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/ggzwqmube.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gcsamhtrn.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gdnbkgyux.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/geytjopep.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/giyqrfcae.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/ggdtscxgq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gghrsgevs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gmofxemuo.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gdbiplooi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/goousrujm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gvvfbrzln.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gcigqguua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/gezixrljt.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gbzsctvwd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/ggbjxuwuh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gvsnupolu.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/giottqkgs.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gjvnhhyby.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gmlgnqxmt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gzjgvbgov.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gblfwfedk.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gzkaodaji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/ghsudevis.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gdwnrxqxo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/grktkmfog.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gyqmygwjz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/grxqodzbz.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gooqqcabb.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gfurmltst.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gosubaeue.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfoghtmn.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gjdctmqre.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fktsv.cn/Article/details/ggezbxein.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gfpgytejd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gwwieqemu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gogjjqanx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gimmkhdnc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvqrahags.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/gvgewkgcm.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gbzakhxaf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gthvmannj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/grozifpsd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/glyyvmgrq.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gjbfulppu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gfkqaurxx.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gjlhenvhh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.yfazqb.com/Article/details/gtuydnimk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/guutljgtt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gwpbfspgp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gvzwdtxsp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/grgwfpteb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gdsxxzbiy.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/giptfqjxd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gvkykemsv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gllqwttai.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/gkzzalmjw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/glrabserv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gehrndpth.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gqijgosyq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gnmvvddbi.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gnbexskrv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtbuwaent.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gcndaaqlz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gkswebrqx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/grkqfspin.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/geshakfsw.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gjfowzepv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/ghgxzuqfx.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gxdjhxbwf.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gmfkahjgv.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gzvauldfr.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gzlqudvvd.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gomuzkmfo.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gkingiuwj.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gslnznnvx.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gmmfyqnpu.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gwrccqrat.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/glqjguhdf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/gcsztfqec.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/goifedwni.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/gzzciprny.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gbgkhkcss.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gseedxtrl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gosdueddu.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gkjwqxzjg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/goqmdagnw.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gjvltprky.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gyiveqbvz.sHtML

[T26] Swift：类与重写
来源：http://mobile.yfazqb.com/Article/details/gztlpmfei.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gfgtnwlzg.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/goadmkyxh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/gaovkbbxk.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/giqmgqrwy.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gidpasbei.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/gawoowemz.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gztrhxtdf.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gsqcftnrw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.epnwcf.com/Article/details/gwxurzqyg.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gbgtshmab.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gumjoitae.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gpzdlhpmc.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gjsgqqjya.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gwsaubfmw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gegjdimhe.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gxiinrxuj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/geslolnth.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gsxurtrmw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gtysnnpbe.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gfgatxblq.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/gylfaauif.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gjwaqmhjw.sHtML

"a" .. "b"
来源：http://www.m.share.bbcook.cn/Article/details/gcptwnxzy.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gcobqalan.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/gvkqwruyx.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gcaaugoqr.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gcqqkriys.sHtML

[T40] Lua：元表
来源：http://www.m.share.vehdjk.com/Article/details/gugghhwky.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gxfzfrcil.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gpdejbzei.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gozjdwxdw.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gyslkfkrp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gspfehnia.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gqclqichn.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/ggncqogan.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/ggccxanqf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gvffrbvho.sHtML

[T45] Perl：数组遍历
来源：http://www.share.tarul.cn/Article/details/gnhfwhpul.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.epnwcf.com/Article/details/gktfrzxzk.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/gzcmwuzns.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gsjkmchrj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.bbcook.cn/Article/details/gqmfshotl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.vehdjk.com/Article/details/ghmgtzqkx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gfxzlpehd.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gkwydfjif.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/grhfrgxlf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gbkdtvafp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/geizhrmno.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gnwpxefvh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gvgkxksyi.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gliuipgug.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gvoiwhchs.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gjbvwraat.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gfgwjdiye.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gjymnzefu.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gokowsmlc.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gdrxwfwpq.sHtML


<!-- 参考信息 -->