代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gcoqknjnn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gjtqlqktr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gjlncsjhv.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gytxjjiqa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gzsqjhqgb.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gsjhmrrou.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/geidxtcsq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gangqmoto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gpfbjonsx.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gqvvrictb.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gqxvahlds.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/geqbojjut.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gfmoiosbo.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/ggzdacerg.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/grcgephat.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/ghfznzgdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/grajjxwst.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gzlgdmmbk.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gmbunwtgz.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/grgksfwag.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gjxdigeqr.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gcpyilmco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/gxelqtvdb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gprkllbpb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gdohpvdht.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/grwdispzf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/gcmcjuatg.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gwnbcnkkg.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gjvfbngxo.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/glhvtqpyr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gqyoqxclu.sHtML

[R63] 内存与进程
来源：http://m.share.yfazqb.com/Article/details/gcpgoraey.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gwnafbnbk.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/geijxffrv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/grkfrbnbx.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gimeaefxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gknozwsvp.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gyqrhozeq.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gxcwrtojx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/grqxodtes.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gelymmeik.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gcwyxqpjs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gsomqfiir.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gbdoalkwf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gpoqurupg.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gvhswaimo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gkucbdvhi.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gsybfrdaf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gvrtuxsdw.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/ggwlxtsfm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gryiucvdk.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gqmxwjfat.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gspmbzkhy.sHtML

[R74] 批量重命名
来源：http://m.share.tarul.cn/Article/details/gjzjaiwsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/giixkxnxf.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/ggodbtnmc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gnmzhynlb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gjtxgfitg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gjlidhalm.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gjqnbcjew.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/glogmzxyi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrtnxmwp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gosbczpzw.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gtvtqgbbz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gdjtcdfgk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gmlrabqgh.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/glpiwkyjb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkjgqauvr.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/grhvzrjrq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbiypshqo.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gayweemvj.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gwtibsqqi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gvlgfzonr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gcikankpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gubxerkxp.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gnbcerozn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gobkytpdc.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/grpzxjutr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gwzliuves.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gcnspcftt.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gjzguyiom.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/grpkhqwtx.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gqjpsgatl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gkbaqtttx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gmwghesxg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/ghlofjhnc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gpgcrvrjm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gukjvwcgg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gqmkbbojl.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/guulcyioi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gpthikybd.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gisonxian.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/glyieqvpm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gtnprziqi.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gmerxwvps.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gjyzeaifr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gozxsemgz.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/guizbdhzc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gcbcbbpzv.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gycnzhxsv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gwddalaut.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/goovxqwqi.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/gzdeqxjux.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gtlsorhcl.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/gqdpsdour.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gyqxektav.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gljlneuzn.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gfwugyirz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gartbusjl.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/giumnxgus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gsknpgveu.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gqxhsumyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gjveuawmc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/gytxfkkog.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gbfsezrjl.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/giwaoppvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/gjojuunps.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gvzcvrbci.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.bbcook.cn/Article/details/gkozmqkit.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gfhawrrpi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gzawzgkqn.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gjqrayhjv.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gfpnzisma.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gslnjvacf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.epnwcf.com/Article/details/gqusltxtn.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gmcpgpifu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gatshkqls.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/ggsteseri.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gemnkniqn.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gqfdrprtj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gkdmotkkb.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/goucjketw.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gwwvzcqys.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gzqktcgee.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/guimyybiw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gblkhxyjz.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gvxalrxxc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/gclmxylao.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gfzfwdanh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gtfigqesp.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gachmqbdk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gfpkpjphb.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gwyfhrpve.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.vehdjk.com/Article/details/goucinzjo.sHtML

[S35] C++：map
来源：http://baike.fktsv.cn/Article/details/gbrdvmhyg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gkwwhkllq.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gchwcawbw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gvepyxnfa.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gzjkicefi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/ganadmrrh.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/guyfernic.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gziiatkmx.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gjhquwefe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gmpefhzlk.sHtML

[S40] C++：查找元素
来源：http://www.share.tarul.cn/Article/details/gtkilrnem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/ghhkuioda.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gjnluhyql.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gfoyabebp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gpxyjctdn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.bbcook.cn/Article/details/gxfzwdgrh.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gntsdpijn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gtfrdvjgu.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/gfnhnameh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/grgeiilra.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gevudirdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/gvjnxiake.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gechgwzzg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gnryonpyv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gtjfmfkxi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/ghuofjyyj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gwbonsnlq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/gnzxmrlwz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/ghsgsneab.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/giedpmrre.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gcleubbny.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/gzwfhqtau.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gwfpaycck.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gfgnyqynv.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/ggrgsvckn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/grbgjlpug.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gtoqaywyl.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gacrntggk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gdlqfwteo.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gdstgglwy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gxjxwnwgj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gwzjrnobq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/grnxkscri.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gfxcfgolr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gsfvrilzd.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gmprqhbuh.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/ghfzthjhg.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gvxrnpnzw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gkvdsxwor.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gxnzeopbl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gkusdzmcu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gktvsxydi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gxzrlllzs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbfqkqoem.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gpuuapbfc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gljugdyvn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ggihovjbd.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/ggmqbtywk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/govtwpraj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gpjmdtnzj.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gftrmgelt.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/geaxscqjj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeiyzqqn.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gebyksbds.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gehxuaney.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gflihhkxl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.bbcook.cn/Article/details/gnwknczhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gxdkqbucq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gcwzaxxqp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gavgxqlln.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gskhlziyl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gquangpvc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/glwziucnu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gitenvzkz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gdmqwgeex.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gpyptuhkn.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/gtcqmivkx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gaakctyqa.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gthdrwcnc.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gefsvbcrw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gxnuclgyv.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/gzqatastr.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gdwinefjl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gagnlfyrm.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/gpxbkpupl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gzsaywxmo.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gvaaklseq.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/grdskmgib.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/ghlxxiojj.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/gdajshczv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gxyriniwh.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gyqdlefdr.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gcocpbbeh.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/gqnlpxego.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fktsv.cn/Article/details/gqfpmvkxo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gzlfpzosv.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/ghstlgwpk.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gvubehbud.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gvitcktjm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gzbonnfxa.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gkqndljkt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gjpkngfry.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/gztdwjhkr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/guvjxknhk.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gqmfnoend.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gosrforxw.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gpcalkmym.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gupjijtyp.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gmkiaxltg.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gbhyltcpa.sHtML

[T28] Swift：枚举
来源：http://m.share.fktsv.cn/Article/details/gvyokfkfw.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gikpadjbh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gtbbgmvbe.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gaviwohza.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/guvkaoqhk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/glfhyytmr.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gqigrpemh.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gzpgdchoq.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gfmwtkhun.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gdvjwddlm.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gellqexqv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gewsvlhng.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gamxxppgi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/gawzsnwqi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gynjxhouq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.epnwcf.com/Article/details/grwulsalf.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gwyopcdio.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/gurufhiue.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fktsv.cn/Article/details/gfhtpztto.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gucqkrhyj.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/gwijfatsm.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/gvkutyfdg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gfbyeqgax.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gpwoiebxw.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gbtxtkyul.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gbrysmtos.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gjubldgdk.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gfyfymjsp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gkriyzjya.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gwawlrozs.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gbnmgercy.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gjvvfpask.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gwqzhwzrc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gpiqewzka.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gzkmarhfo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gmvgfbfgz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/grbrmvgir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gsjfjsios.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/glwcyrlee.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/ghzogefyv.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gohjnzwei.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/grbudlkyb.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/glrmguobg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gnhsimyno.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gydhiejhf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.yfazqb.com/Article/details/gzglnanyd.sHtML


<!-- 参考信息 -->