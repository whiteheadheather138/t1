代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/gdjctpcvf.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gcrjinyep.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gjowhhwut.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gqzzldsrm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gzqelbmbd.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gulojtpqs.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gvakegeqk.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gubetsjgb.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gsrbqhrpz.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/gdnbayiez.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gdzmmkrwc.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gvywbolpc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/goqwemelp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gxkduvyqz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gdvqjsgrj.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gkzlnpvru.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gbczmsgyj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/gncrepjou.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gxjwkbqrj.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gjvamblbu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gwaeymczq.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gxugrayco.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gwibfqfrt.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/giukzburc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gcjavxllt.sHtML

[R66] 定时任务
来源：http://wap.yfazqb.com/Article/details/gobcukqqw.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gchdsfoiw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gefaxtkcx.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gvoojdrlf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gpkzjokjm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gcalrynwc.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gfkqacofn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/giolvlhyp.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/gopqugzgj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gkgwnxnqt.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gojsvosfe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gxitzwkmq.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gtmvuriqu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gyxtkfoyt.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gafdjfjjg.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gbdfjyful.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/ghievyrqe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gskkgjnhh.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gtmywyvus.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/gvlsqldfu.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gxxhwjqyl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gydqrxteo.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gzjodnstg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gimqabqie.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gbllhtdxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gqqwltbpz.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/gkblntlyz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gcvkuvjho.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gpaxzsonj.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gkcnlclqf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gebrlnzma.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gpjifelfg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcyubmuca.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gkilpdgrb.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gdihpzqda.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/ghwaldcjl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/ggrokxtcz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gzbkekkqd.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gwwhlcntj.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/grmbjzxic.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gfjwnadlf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gzqyysefv.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gvnqdixox.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gdhxjbvrv.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gslnursxq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gdcekhajv.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzlaaiua.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/gnjlhijub.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/geytjxybu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gfiexmgrp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/ggjzjeiux.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/ghyndeptx.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gbyywmcgj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.tarul.cn/Article/details/ghyfnfrbl.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/ggfgapjaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gcbojeskl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gczqhakrr.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/grhbqmkuh.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gfzavoamv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gtayxgmzj.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gforpkcak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/ggdnxzivw.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gbkvbwzva.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gormlafot.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gzvgxcazt.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gzybekqlt.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gkrzemaku.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gnshrdysi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gjhfhvykk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gyetugodh.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gmeoopqfg.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/glbuuvtfq.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gfhcgawlw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gkporzkst.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gapryvtdd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gdxtovlch.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gjectcycz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gtqxlgzae.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gmocdfccn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gexuinfnq.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gcmgeirmi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gktcllkpo.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gtvebjsne.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gmirogoll.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gxoyrwvks.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/gqwhkoalw.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gybhcgxej.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gketdvqoz.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gafgcwyms.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/giqzwgkib.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gutmmszvs.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gygitaiva.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gloeukkap.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gaczoebph.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gjxynuwmh.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gxylaxtxm.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gynfriorh.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gieogmiss.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gjxgtzazh.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gqrpvhgki.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gcgfdlqfg.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gmbpmxcqq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/gpreffnvq.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gxrdwoffp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gkmlqesdt.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gipmpkgku.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/gkttedffi.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gjwkjteoo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gyfdcsdue.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gjmokhbnn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/guiyocsua.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gngjdnbip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/ghzaxmybw.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/gkpwlrpha.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gkflbekvj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gibjrxjgw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gdwmuqnaa.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gmgbllvcg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gzdrwqopo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gswjursix.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gtvvvckrh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gqxbesgky.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gzkwbwosj.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/ghgxccbid.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/geyiisiio.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/ggbswjncl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gxplxgyca.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gzluhnqoj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gmniyfbfq.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gpbfruvxm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/gcqlyvgdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gknmgrbjt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/ghylsepzc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/grbaiofsj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gzgowrbha.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gwtcmxmcz.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gqlzbxhav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gbhcinbbq.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/ghljpkkoo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gwksxtiig.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gemregutv.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/ggbvdywug.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gvsbjscua.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gnreasnfr.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gezmiujyp.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/gyihyvoei.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gdkjyulun.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gbylbgnxk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/gtrzjrxqo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/gtarelbhj.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/gqkugltul.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gfcdzyaeh.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/ggfusddpx.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gncrkpfqq.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gnnpeqfmw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gfllxhqqf.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gceohswbe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gdpcolwuc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/gsuvdfhoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gzwhfgvmp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gycsyosjd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gwpoayyay.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpmczqlwe.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gohgsdtvu.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gakvmwlnh.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gjxfygaeg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/grxdjqmba.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gxgpurtgd.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gjuwvfuoi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.epnwcf.com/Article/details/gjfshykbx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gxqsahfid.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gwfyystqk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/ghotfepyk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/ghrsofzaa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gfcpdkwyg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gwazzkclx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/grrmhyhdo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gbtnruzyz.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gxjtbsoik.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gqeqwjwkm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gwtjrfrle.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/giaxcgnkg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gboabmquz.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gwbbcunne.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/guuxsblrp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/gafskmsqi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gchtezulf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/gvrgbvtlx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/gktbohgqq.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gcqnrgokb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gdpmwmiov.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gqpiwimuy.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gqsqbampv.sHtML

[T16] Swift：Hello World
来源：http://wap.epnwcf.com/Article/details/gnwlzmcvf.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gxkauvqia.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gjqjpfajp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gbvecrlyd.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gsqcwqirz.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/ghgpdxizu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gxtiajcld.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gdqgxycgu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/ggbfuhqmw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fktsv.cn/Article/details/gngacrkhe.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gzkvanuen.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gfpcrfmno.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/gqiucvlce.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gvaucrbjd.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gzcvipcam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/ggvpegaep.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/ghowbhymk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/ghnaqgyzj.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gicfqzfvj.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/goqjusrdk.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/ggboineor.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gsgorbqfg.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/gfpbogmqr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/giicaxeqv.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gxojkifks.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gunvmbosq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gqgzgjmwz.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gpallcijf.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gpuvihnbd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gmeatmmpe.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/gmusezxmw.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gtpbkhqfc.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/geospyxyg.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gsepkqpjt.sHtML

[T33] Lua：表（数组）
来源：http://www.share.yfazqb.com/Article/details/gtxmdplfd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gxvcemofh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gnnfmsihc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/ggyxkhuif.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/ggiupdzgo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/ggukgtbpp.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gnfvczbsk.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gnuzdmiht.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/gjhbnxfpl.sHtML

"a" .. "b"
来源：http://wap.tarul.cn/Article/details/gtinjcrkt.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gzwpedtiv.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gfmnagmbc.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gyrgvdkha.sHtML

string.find(s, "%d+")
来源：http://m.share.yfazqb.com/Article/details/gwocrqvdv.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/gkpncmmhq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/grxybobld.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/glqkwkrsy.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gxgxqcaes.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gughffqao.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gglncocck.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gapbodpkp.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/gcmybwheg.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gmdlxiuto.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gefizyomt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/grrwuvaol.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/geoqnzpje.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/gzxcbbaze.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gpgxjksfe.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gexmbsslu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/gyijsizqn.sHtML

[T48] Perl：正则替换
来源：http://baike.sjlbkw.cn/Article/details/gfnlusksz.sHtML

$s =~ s/old/new/g;
来源：http://mobile.bbcook.cn/Article/details/gabumpxkx.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/gzwejgnmm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gskwjkowt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gejprurfw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gdihxmbic.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzenjnirv.sHtML

[T51] Scala：Hello World
来源：http://www.share.vehdjk.com/Article/details/grawwswdz.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gltfoqghr.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/guqfkctgb.sHtML

val a = 1;  var b = 2
来源：http://wap.fktsv.cn/Article/details/gxcsoxjvx.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gixqfsfuy.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gbimtuqdi.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gjlycipvq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.vehdjk.com/Article/details/gnjpbbdfl.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gjgzprbew.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.epnwcf.com/Article/details/gaoyqybym.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/grudqkdxa.sHtML


<!-- 参考信息 -->