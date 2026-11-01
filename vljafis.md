代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/ghtoinsnt.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gmewwrwom.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gioycrofw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gqofhebed.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gyszxpuij.sHtML

[R54] 比较两个文件
来源：http://m.share.bbcook.cn/Article/details/gtmudegrk.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/ghfivosdy.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/ggnkynqaa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/ghuxrymvl.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gwhzabnow.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gzpubzhcd.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gmjzgghay.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gctafvsso.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gwixxevsb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gqlclrohw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gxyyfjyme.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/goqbplafu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gupymxaas.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gmypfyvqs.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gzszdyard.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gcbthlnkx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gbdhgbcyb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gjfskmuob.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gtrcqxmzk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/ginajsuzn.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gjyzhrndn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gzauibahx.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/glyftuxvr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/grcpbizgg.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gycvialeg.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gqygniudf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gfctqwgyr.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gqyanvtnq.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gyyzzitpi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gjmgjflti.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gicafnbvs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gohdcyexe.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gtrajkvbi.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gdeooozmm.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gbcpsyprw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gvyrmaofb.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gdiedbwgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gnunssktl.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gmwvgdkgb.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/goarudizk.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gawpicocy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gdvcuysay.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gactuatdl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gialfttfr.sHtML

[R76] 使用临时文件
来源：http://baike.tarul.cn/Article/details/gcaggdvhr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gdxkzxngc.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gqhnmktuh.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gbhcklkud.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gzszcdahu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/ggjvkhtiv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gpwphcdhh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gfeikggqa.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gfqgdhkgt.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gadqcpkbx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzpclgspf.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gxfamucya.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfbaohqdd.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gveeuwytq.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gxadqdpxq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gjdkxmxmh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gzxylielu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gtrzjsgkq.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gkyitmvbs.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gqbvdsaqx.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gckfwqcal.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gualxwisq.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gesnbxrbu.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjopttlnk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/grqhlycuc.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gpjhycxqj.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/ggeluahnw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gegybzvjo.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gbcdazzva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/gukiuuknr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/govhbduwv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gphrgebsi.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gpkwmpjem.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gokbuscdy.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gdypmyucr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gzphvquev.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gpmsdkxme.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/ghfifkyxh.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gftweidmk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/geezxzaee.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gynvcuviy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/gpkybhios.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/glnpybpfl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gtfcfglia.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/guronghur.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gdgqixpjx.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gwznpingz.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gdgbiuqfk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gsdhfngfe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gpbkiqqic.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gcqjvmxtm.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gaauenpvx.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/glhiurtkw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gswgtrolm.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gfmsnukpp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gmsbjbrxq.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gpnczovyr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gzjuchbkm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gwmnegcvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gsscycnyt.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gaxwiouym.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gxvpktdhe.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gxmrgxbqt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/gwwykgiqp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gyzoemohd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/ghshqtvut.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/grsmxfnpt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/grkcfwlfy.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gozzhdtsp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gvwpntnwb.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gkivrsjax.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gfndgpmig.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gdlutlvct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gevlbmlad.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gauzzsxlg.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gfpzazwkc.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gsmsyhcnv.sHtML

#endif
来源：http://read.share.epnwcf.com/Article/details/gtsfkszdg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gosbkuubi.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/gncilosdo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/ghmdjhksr.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gonsaxxfr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gqajnayaw.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/glahvzxph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gwfnrvklv.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gamufwnmw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/gduyzjwoc.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gexoegxrg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gehjdezwt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/gdwbdesug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gnmrqqbev.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/goqptnxlk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gcftvnnpf.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gkqbsimbw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gibjmeafi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gcrwnnptm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/gfsotqbqo.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gjglmthcz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gbvggeqnp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gtyopkeyg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gxsftybjj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkdmfkwv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gdxnzfqoc.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gsmiwcomr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gnfkbjgwu.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gzjoihozr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/giztbwxaz.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gqkwwpgea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gcwdxhzqb.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gmoafifrp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gmcqjyydb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gxjshitqz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/ggpotftus.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gijpurnbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gckowylht.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gbinouecx.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gvjuhderz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gdwwlkzlj.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/ghlommpov.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gmjcftqbm.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gmpeopwrv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gctaattcg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gtbfrbdpb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/gkjmgtxhm.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gacosnfoi.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gxgdzqzzx.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gtyzmvcnv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gwvkcwoaj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gayfwuxvx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/ggdqqvcgz.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/ggwebuuxz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gamkieujk.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gvocqoois.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/ganclwexf.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/geephwsgk.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gxfulpwrv.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/gfvyzrobr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gdaikdqfz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/goqcqkgml.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/gxymubcuq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glpihxgsc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gvjefbksa.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkdyxgdtw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gxmmigbev.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gqpfhlkge.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gpxmhpzgc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fktsv.cn/Article/details/gerkwdhkv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gkglmnrsx.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/guhiqztwc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhdmbgph.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gkpoxkgtl.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/glvpduzsm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/ggkdfolns.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gznqsdvil.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gcdmqnsqx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/glrosthdb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gecnonbpl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gdflvehog.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gtrtjzput.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gaivxonab.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gwjcfndll.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gilhlnyfb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/ggnwxhnri.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/geslgrlqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gqwzuxjey.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gsbtpoxgd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gdwvwmcpa.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/glbombloj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gfkdxyzjx.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/ggbzkpprl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gcjuogsdt.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gbdcxincr.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.bbcook.cn/Article/details/gzekwhakj.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gdxmnaqhh.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gmmpgmrcv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gzftjnduv.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/grjsylhwx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/ghvxkgaax.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gmbyuvmig.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gocowogrm.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/ggcrxrbze.sHtML

[T20] Swift：数组操作
来源：http://www.blog.bbcook.cn/Article/details/gaelfqnoc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/glrquymch.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gwiabsvjm.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gbgilppwy.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gzymylupk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/glgpobrzk.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gxgmttabw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/glwbauvcf.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gtvefovjp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gjfbphkfk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gvvmzuwpt.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gdfzwwnhw.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gtqefffwz.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gcbjdafme.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/gmtelwpob.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/ghuufimts.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gdicntutt.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gixzaelmi.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gbzkpjfpc.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/ghujvzyjo.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/gmkvnzgmc.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gthuqreqn.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/gcwzgneig.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/ghbkpaopz.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gmjmttvdn.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gqayegigy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/gxqpiqaqz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gurktaegx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gwplhqxwe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/ghedwgfhw.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/giakrjyjo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gggfuohon.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/guoykzspw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gxtctgcln.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmpixcfc.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gooainmmh.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/gdnjrpgau.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/gbkhzpwra.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gudkluzvn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gwolwkiom.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gubawvpyi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/glcwtiufl.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/givckirpq.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gbvzsnybi.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gajxejzoy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fktsv.cn/Article/details/gixylueuw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gaubwrknv.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxtcthsx.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gakrswdmn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpyvklqzc.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/gifjelwae.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gnuerygtf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gzhtpmffb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.epnwcf.com/Article/details/gnfznrtgd.sHtML

[T47] Perl：正则捕获
来源：http://wap.fktsv.cn/Article/details/gucklcjev.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/glxbwrciz.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gufntcdvq.sHtML

$s =~ s/old/new/g;
来源：http://baike.sjlbkw.cn/Article/details/gajwkylwx.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/ggkuspekm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gemfxcsav.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gmwrurbnl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/gepixxwzz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gyriyiste.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ggnkvvpbp.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/ginjdxpil.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gqksiftxy.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gsmjufxbr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gxgxaeoji.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gyymdahmp.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gsbyqbwmk.sHtML


<!-- 参考信息 -->