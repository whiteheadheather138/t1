代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gebvxowiw.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/guoruzzgs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gcemtwneu.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/gvpewxvsx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/glogvppqv.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gejvvltin.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gumlqwpvq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gfwobkmxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/grldfdasz.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/glgibjlbm.sHtML

diff a.txt b.txt
来源：http://baike.fktsv.cn/Article/details/gijmcfgdq.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gbvjywfmb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/grvzhorwt.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gxndfiqlf.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gkdaoicun.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gaitbtfmy.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gtyaycrse.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gfsizfkay.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/gsbbllzxz.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gxksdtmxs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gsqpnzzqt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gkfnqtaiy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gvgwzrcci.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gypuqjutn.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/grsojluzo.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gqrzoikiu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gizivfjib.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gwdfeuiob.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gmahqmqaf.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gjdsmyfwb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gdcvzevrw.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gyndrjdgz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/gsiweybwe.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/ggimvuatk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gcirrntez.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gaoktgmts.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gnrpfbhlb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gjreejbmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gnfwozoup.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/goiabqtgq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gmwabgdyp.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/glcptdqac.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/grtmrsrup.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gftkugzrt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.epnwcf.com/Article/details/gjriexfxu.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gajntqkad.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gphzmoanp.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gvjovwiia.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gxxkrgodg.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gwkglymcf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gmvshnkjv.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gzqfxmzkv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/glrsmjhmg.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gokayatoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gcgdtwnjk.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/gvkqbpnhg.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/gxwupnljt.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gnejvmjdx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gmtuynmwm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gnywhvvhx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.tarul.cn/Article/details/gepiddgvt.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gykovgskv.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gdutljdhz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmaomzrcl.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gvsddeqbc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glkzidwjf.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/gjsqjwmgc.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gcvfmtlag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/geduyqakc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gzpqqbapv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/ghyqxzwdb.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gdxyuvjph.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/glrovqjtq.sHtML

[S04] C：字符串复制
来源：http://blog.yfazqb.com/Article/details/gcwqodvep.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gywvnuvrj.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gezxrjkua.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/ggmipgbzm.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gmntsnzil.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gphukqgzl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gzzuqgwzj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gyfntrqzq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gruectyom.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gxliwalnp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/ggmfyirvi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gxstncjma.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gssicfgfm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gifxjajkd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gneqrtuvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/gpnyokvyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gnsytrthm.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gpridgwdl.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gmlnrxhhb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gxinrvhpr.sHtML

[S13] C：宏定义
来源：http://blog.vehdjk.com/Article/details/gccfkachy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/geljtikjd.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gwnmveljd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gfhywqrpy.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gcbtejokr.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/govpxrfze.sHtML

[S16] C：位操作置位
来源：http://baike.epnwcf.com/Article/details/gsrcjkzdb.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gsyygdhqj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gedyqqpeu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/ggtqsnvns.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gribletna.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/giotoaqhd.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gjsqgiyjl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gdlxeiidf.sHtML

[S20] C：二分查找
来源：http://blog.sjlbkw.cn/Article/details/gddmyqhnl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gqaxovidz.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gerfmyzhi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gfhhyayne.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gtfareocs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gnivsdffl.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gonmhvsvy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/gqkjoeluy.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gufzeprrc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gunxksiqn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/gptrlhyuq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gwistbzwm.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/glerzurht.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gfrgubjuo.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gxfszegvp.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/guvfkhhwi.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/grasbkvqi.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gngnsiyfy.sHtML

[S29] C：变参函数
来源：http://www.blog.sjlbkw.cn/Article/details/giedxthbc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/gbltjjyqb.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gauntmekk.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/ggwwuqjoy.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/gcdqdzhaz.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/glxiixxgt.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gdbhejdjg.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gdjbhglek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gshmwmqhq.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/giphrjddf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gqdnkxjrh.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/gkurcriem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gjvltzmck.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/grgdxxqcs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/grffzhyqz.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gcwvjvzuv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/ghkmmeoql.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gquvylzov.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/grkpzyacc.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/giehadchl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gujtxdlhv.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gtaajtmaw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/gcgxcbzbe.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.tarul.cn/Article/details/glafwplxk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gmkhtcrbj.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gbcstlwdq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gtmsombah.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gagwgmgsi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gjpqnpjzn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gqstvipvr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/ggwchhljv.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/gkpbudhpy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gdymzfnbu.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gxospatqc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/grhrlqehb.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gnmcbmody.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gzjtfyovm.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gmbsdyyhr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/gnxouovjt.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gghmcnlju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gdjgbdnpx.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gummclbum.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gjvkqwklz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gwxrekpxn.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gapssbwbp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gkfalhksm.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gzoutbyow.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/ggxnzzlib.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gpuwpeelx.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gkczvnlvm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gmkfryiku.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/ggitvitif.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gtgdrrirb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gfxlvgmqt.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/giozcicox.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/gzungixui.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/ghsfnzgcg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/guemaekdz.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gvqagxeke.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gjyezorpk.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/glelslomg.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/ghmhwdttr.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/ggzbnboqz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/guhfgdwha.sHtML

[S59] C++：静态断言
来源：http://www.blog.tarul.cn/Article/details/gheiseebb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gtgkqnrka.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gvuabpptj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gbzymylce.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvbvdwxvs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gtgfssoif.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grubjvcwq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gklqdotzx.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjklcrszr.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gtcebopil.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gxmyloqca.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gywxspcex.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gpahszrac.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gabysjtmj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gorlkgyqv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/geqgoafwv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gfsgujvdf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gthtktnqy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gkrmlgylf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gjbwwpdjg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gutngcumd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gcmbwrwpt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gfvnjvyhz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/goywpkhsd.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gptsqfckm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gjzsthlet.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gmakprbba.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gjbjgyycj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gizvxgdyr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/ggiyzvtqa.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/gxugbdcmw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/geismozho.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gtwnebpqu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gowmswrws.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gyqcwrghw.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/greqzdtyy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/gwfuskuqw.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gnktnjesz.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gsyofzoga.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/glnvtprkc.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gwsqqlsrp.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gkvzmnckk.sHtML

"值: \(b)"
来源：http://3g.vehdjk.com/Article/details/gomslwpjf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gdqrvvald.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/gdvjmdqpo.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gjimrersj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gugfkiydj.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gbzajohtr.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gkqpaydcn.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gcxvgueek.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/ggfjlnrzc.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/gnazgfzvu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/gknsnhkas.sHtML

[T24] Swift：闭包
来源：http://blog.vehdjk.com/Article/details/ggghmtmqf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gwumnmlkh.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gbfjpzxds.sHtML

struct P { var x: Int }
来源：http://baike.sjlbkw.cn/Article/details/grmaelmuh.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/godivtwum.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/galclgvan.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gnrmgwlik.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/ghfxsjias.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gyjecywpu.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gukvrqjqr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/glzwhhgaf.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/gacewermd.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gsrdisrgw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/geflzttig.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gpykputzq.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gvcmjwppa.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/ghstjlcnu.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gtpjtnlmo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fktsv.cn/Article/details/gsedofvkg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gfkhomukt.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gtbuxqviq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gwggnrufy.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/gpzbilirp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gcuevdhbk.sHtML

[T36] Lua：函数
来源：http://baike.sjlbkw.cn/Article/details/gmralpesd.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gmrnhapoa.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/ghuwikxkt.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gfrykfgbg.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/ghzjeeivo.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gvbgehchk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gdjmwzjbq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/godtouwuc.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gajjckzys.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gpkxepsxx.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/gowbqtrir.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/gggzetptj.sHtML

[T42] Perl：变量类型
来源：http://blog.fktsv.cn/Article/details/gggdolcqu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.sjlbkw.cn/Article/details/gnlrquwrp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gfvdatqca.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/grnjducro.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/glqlxilwe.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gapeqkwdb.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/gsazsbcyg.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gvpdbincw.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gzrwivchl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbnqjlvdu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/gkoqzzdev.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/grtdiphsb.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/gdrtzzsds.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/guxasorko.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/gobdqzvbx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gednftond.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/ghniygksv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gewgwqvqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gvnrzupvt.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gvqymfekv.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gikokwfpd.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/gcqpgdzgr.sHtML


<!-- 参考信息 -->