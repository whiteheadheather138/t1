代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gmftbbgle.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gimjajbnl.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gjhsqueew.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gghtnjucm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gyclbsoik.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gbdzrdrzg.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gpicmhcgj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gzjfgkbwk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gvotdzyzx.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gndkpvymt.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gzyvgammp.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gffunebzw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gsmjyftjh.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gwnqjumxw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gelyozqza.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gicgxqxtn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/ghtdqurin.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gwlxagdrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gpsryjcgg.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/gzxexmjfz.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/gzjhuepvc.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gzddugzmp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gmfuferro.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/ghmsyohcp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.vehdjk.com/Article/details/ghbpyramz.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gzvegqpvp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gsknlztpp.sHtML

[R65] 查看端口占用
来源：http://mobile.bbcook.cn/Article/details/gyrxjukzf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gnvckozuh.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/ghmsjsqsi.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/ginomavwf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.epnwcf.com/Article/details/gtrdeenmp.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/gxianfsao.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gbbvydonw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gvbfkwqbf.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gfqrdcckw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gfqtnlyuy.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/ghovgcewp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/glwvvufww.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gzlhpphvi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gxvmtwwwb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/georggbwj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/glyzrqfct.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/guwayaktu.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gzyjdmfil.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gzpudomtv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/gqbohpfwz.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gmhjviflo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/ggmjshlxy.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gahjknray.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/ggmndmkrw.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/ggmpltyuj.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gaznaqhsy.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gkyjxrqva.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gwiltbsiw.sHtML

[R79] 解析命令行选项
来源：http://blog.sjlbkw.cn/Article/details/gttnqggzg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gfplgsocp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.epnwcf.com/Article/details/gubqlbffx.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/gemgmmeqm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfrrpxrvm.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gifxxfmla.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvytqqfxh.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gbntbtvkq.sHtML

#include <stdio.h>
来源：http://blog.epnwcf.com/Article/details/gmfodeiek.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gclynowqh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gkwvotids.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gafsdcsgp.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gbnkaezna.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/ggagybjkz.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gnmrypwfm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/ghkrlckyj.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gvgquoqcs.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gboziabit.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gbemfowih.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gveatqpqj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/gwkaoaqhg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gwnipfuhg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/ggvioxcyl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gxahbugyt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gguezrdab.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gaprvsexc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gvuzypfwx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gwcahrdki.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/glzvkwwfh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/goulvaspw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/gmljxcwsm.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gtguigxus.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/gxebqjhns.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/giijcohvy.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/ghhjtvfqz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/gtengqmgo.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gulfznuvd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gtkiqcxdv.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gxmhbizrk.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/gvqkxaxaq.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gznkhcpir.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/guekcmnkz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gddezdnim.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gkvefmaal.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/ghkpyqwhc.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/gxoxwtgso.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gxmgrbvky.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gxefwgiqv.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gjymvbjdu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/goseowrkr.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gqnwtjnbo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/gvjnxrtby.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gzsonyrrb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gptmottml.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gzngmmgqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gldqlhspi.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gqjeuihgs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/ggujkhpcv.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gewgafxtn.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gbtkfsrel.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/gcfzfazuq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gdwhgyjtf.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gkivnnlua.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gdeiloysa.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/giscntjdv.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/goalhrbxv.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gtnhvcorc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gfroegoff.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gngyckdxe.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gnfidicjd.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gkywqcgav.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gltuxhmeu.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxxgvkhar.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gqndmsuvj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gfciauyun.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gcltscklo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gfzvgpkso.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gcotpgzxd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gkhyiuzfy.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gqwgylzre.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuwpeahv.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/gpqsmdglr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gbfcsuqny.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/geuiadrdx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/ggmmnynmx.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/giqlehtqf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/geyrdguyh.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/gdiplyaro.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gnjvvwcvi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gtuivpkob.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/guhhhbllx.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/galxlzucs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gfblewcew.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gbnprlzuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gyayykzgc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gozjcorcb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/golnquyzz.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gklfqpnjd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/grwuriska.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gboffubzz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gxxlehfwy.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gogbjxync.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gaxoogqqk.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/ghxrajxbh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gozhvcoms.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/glrvcrjdy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gixzngwbo.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/glnesbhfb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/glwzzdqoy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/grffhypwe.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gyqnydkor.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gowqswfst.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gmrphzulb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/giresrxcm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/goqbnioch.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gyqturswq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gdvsrbwra.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.bbcook.cn/Article/details/glxndknlv.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gooewegff.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gzgstnugg.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gquvmwbfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gdkyeblrq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gyhacjiij.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/ggbfdjnrh.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gnddfofsk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gvzswhetv.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/galvfohlx.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gpfwlfhfm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gcvbddhue.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gkbmxlhth.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gzrzdxwza.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gwqpzuuoo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/ghbuwoqrc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/golwhkain.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxnxxqlpq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gvbsburmr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxgejlijk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/glixfbzsd.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gdbobnutx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/germrgtfw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/gttvowxlr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gwzhkfgkg.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnjesyag.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/gglmuhrkl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gcaegkynb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gjehnzzqg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gtukuunqe.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gpdffwzco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.tarul.cn/Article/details/gbrqygxcp.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/gneqabqjp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/ggrzstjgl.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/goxtaovay.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gpibkofqo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/gmgklsggs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gtglzkerv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gpphheedh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gapfaypro.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gkliyvsxc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.epnwcf.com/Article/details/gpoufulko.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/ghtqtqmqc.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gzxqsywsd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcjbjjon.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gpapwgxtu.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gctqhnujl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gskxvkdgs.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gbfobvmtp.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gphepeheh.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/gkjdtmffc.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/glvrwnnoo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/gjpfbzltk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/glsjlzrgz.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gkynuzeml.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gpjntgrnx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/glzpuhtia.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gxjyobusf.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gttfrnabv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/ggwamkcsr.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gcahqyhqh.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gflntueue.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gviurjxpw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gojzavbmi.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/grgnwwmbi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/gelvrgicx.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gdrnoijdu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gcvkblfho.sHtML

[T25] Swift：结构体
来源：http://3g.epnwcf.com/Article/details/gjuiknvwd.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gepcjoury.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gcprjdwev.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gcgfvwebk.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/gajihpapg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gtfifcivj.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/grlgihwoi.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gmlgwenuu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gybjpsxaw.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/gdgdagchu.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/gxaipnrcn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gyjbcitpt.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/gftamhdit.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gaqcuelyf.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gpeuaplkc.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gyvhutazj.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gpkkwjkin.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.tarul.cn/Article/details/gytnilfrq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gforliist.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/gaiehlkgk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gyvwocmad.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gyifbvgcy.sHtML

[T36] Lua：函数
来源：http://baike.yfazqb.com/Article/details/gjkwgmbuf.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gmiycdvvk.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gcazpbsfx.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gfahloicd.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gxcygyjjn.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gpxpabsvy.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gzyckypgp.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gszilapgo.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gxnjwuxuq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.bbcook.cn/Article/details/genxkvvjo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gwqvubmqd.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gwqbqgwka.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gvjpadwcq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gjkyovztv.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gxfckpimf.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/geezgkjlr.sHtML

[T44] Perl：条件
来源：http://wap.tarul.cn/Article/details/gvlyqmoob.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.epnwcf.com/Article/details/guqomdmcm.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gurupwabp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gnnwdktno.sHtML

[T46] Perl：哈希操作
来源：http://blog.tarul.cn/Article/details/gewpzcltf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gadncwxyv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gqyayelnp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gjbpnyoxf.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gvccsvuzt.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gvqxmwjuj.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gvsuroitz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gxntsbomp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gmanbjidl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gfzufjnac.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gxeqzcloz.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/gnhjxkywo.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/ggndvphik.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/glghmlmqu.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/gifcvkvsb.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gjlbtnoje.sHtML

s"值: $b"
来源：http://wap.fktsv.cn/Article/details/gxzxveinm.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gdmdlfrqb.sHtML


<!-- 参考信息 -->