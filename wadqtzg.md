代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gkvcpuoku.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gwzrilxfy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gjqdyqrpg.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gmwbgbept.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.bbcook.cn/Article/details/gfmtlkffz.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/golsomgbm.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gufdtbznq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/gguspkish.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gtdwtugtr.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gmypobsrj.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/georhnvwh.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gxekwhlvb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/gteicodej.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gsxxhjiyn.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gqxxrccfo.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gngyurley.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/goutehqpr.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gqfiyhbou.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gvtnifkec.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/givlxrikn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/gfebzriaf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gfmxymrrp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gbajxapff.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gtcemolfk.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/gdiezhogj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gvfwsalgo.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/gchnnhxgj.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gfasdnwje.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gccbscnqb.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gzfuoihwz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/getvldxou.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gmbiuwktr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/girtswcgy.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gyevtoeow.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gjyoniwaq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fktsv.cn/Article/details/guagexkzs.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/gfhpytxyz.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gsrmdzwwg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gqhzvzibl.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyzuvckb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gpkahldkx.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gmsoritrc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/ggddlfwzn.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gaulrplmx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.epnwcf.com/Article/details/gvkoklkbh.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/ggzyqrxef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/guccwdaeg.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gvrxfgxuf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/ghyqikfvc.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gtpvuzluj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gkbmhfcvv.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/grblukodc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gunjcsmux.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gztlfotwu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gnjjmlyox.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/ggxazxchy.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gwvphsooj.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/grtppmmhd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gvxbodlop.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gpplhflcz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gkwcyxovi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/goulyhlpa.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/gkvlsbhak.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdpyqqxze.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gpcxstxcr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzjybvltm.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/gmrfwxubw.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gmuwtfrco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gdeccymio.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/glkflsyya.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gggljurtc.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/ggkcppfxx.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/gukwmntja.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/guspvupar.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/goxhcjzbo.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gcbyrnbek.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gyrcfdsyr.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/glluafkmf.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gptxagudi.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gaaumzluk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/grexkyixx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gfjbhyrhv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gataiwbri.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gmwtupsgp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/glpbltmsz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gwaupilkz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gkjtvieno.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gjdspjqcy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gmyyqdihi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gindrmupk.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/gcxwschnu.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gvkqbihky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gmxzdtzcf.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gxpkfyjsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gejflfegh.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gwcqkojwo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gwlueupke.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gllenntue.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gzqswcbhz.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/glsithzab.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gddmffunz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gnujlhgue.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gqqhuitvb.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gezacdehd.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/ggjooepwd.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gyrfgonkl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gjpcsjqha.sHtML

[S20] C：二分查找
来源：http://blog.epnwcf.com/Article/details/gfkcrowoq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gljzmkixp.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gfmxkuzyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/gavfrunck.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gilncyezr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/gqqxupwgu.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gnbrrrkqo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gbqblwrrv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gljsrtryd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gnbdaeygr.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gtupjzmkh.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gkjvccelw.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gqlpndsft.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/ggcolonpp.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/ggsgwhlcy.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/ghhjadoqq.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gxjjdmkhl.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/ghcddjlhs.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gbbiqibfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gxrrdyofr.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gvbnlbkob.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gsjlunsaj.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gukgakxht.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gmltdsrdx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/grmmbcpbj.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gfqzeszkc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gymgwwdqe.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gaefoguyx.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gfkslwxac.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gfztxpnqn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gyaunmmgf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gyytzgsaa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gzpnizcaz.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gnnogtugv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/ggetpbgqx.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gzsjtqrfz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gpauavkjs.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gneljzwlv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gqnlslqjr.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gsoentxia.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gfzfopmmg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gkxfyswqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gxvqssfwf.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/greqkcdqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gbbuimeue.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gndszlrwn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/grimeavyt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gsyfvtvkk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gngaccxhi.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/godcmrgst.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gxisxrofy.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gjnoixqrd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gczttnbja.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gczkgyxur.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.tarul.cn/Article/details/gwnleombm.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gowdsmuqs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gshoxrmnk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gfqvmxdts.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.vehdjk.com/Article/details/gbagxjoak.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/ghneoslkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gdulyfbif.sHtML

while (std::getline(in, line)) { }
来源：http://baike.vehdjk.com/Article/details/ghbvwqjih.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gasvtstnu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gfpbahefs.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gqqvhmtaw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gihxjupdk.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gmyxtngee.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/gprmfkwjp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gmzarprqi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gdsukbjqc.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gzulqtyrr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/grxpehvqn.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/guxwwavfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gasufijrx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/guvxmjmwn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gmzeylrgy.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gtqejfifi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guecmjczy.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gwgvogqse.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gddmaycyo.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gcdntnvvd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gmuegqerh.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gmatnkwyv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/guomrwajs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gevlcvpxu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gmqkjyyds.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsftsrwnr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gsukvqsvl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcrxhihbz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gbhiogkqh.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/guyojspdt.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gzkgdyfjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/ggdwmmqej.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/gownxekms.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gqndgkihp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gkxmshorh.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gdqabhwgj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/geraqhyvs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gzyqgypxf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/ggjfceoqd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gmxkukuag.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gtjwpkrqx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.sjlbkw.cn/Article/details/gfqlbtlxp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/ghrtnmrkw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/glbikwfqb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gzlgktrah.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/glczaexqn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gzneatzzr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gvjzsqatv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/gpsasxwiw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gdgoqzfoy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gttbchzqq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/ggdgomyts.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.sjlbkw.cn/Article/details/geqiybzht.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/glsdpwvvr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gbrjebvvu.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gnbxqqtvr.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gesskauiv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/galenwilo.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gfarhliln.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gkkidklzk.sHtML

[T17] Swift：变量与常量
来源：http://3g.yfazqb.com/Article/details/gougwnjng.sHtML

var a = 1;  let b = 2
来源：http://www.share.epnwcf.com/Article/details/giqdcxoun.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/grrwyuqhe.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gdxgdfeny.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gerceqwec.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gongzvcfs.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gkkwufxqo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/goseaodjj.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gjdlrjxxo.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gfhszxzpv.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gfkkwdtyw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/grvrjthyz.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gbkpfrgzu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/goszbxbls.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gvnsbpnhk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gusqioyid.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gclvaxpdj.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gghdqbgra.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/galglbmwk.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/gxscgaszh.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/genjophzl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gnmeygoqj.sHtML

[T28] Swift：枚举
来源：http://blog.fktsv.cn/Article/details/guirutsze.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gndgkzxfo.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gjunhisfz.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/gfqyyrpzr.sHtML

[T30] Swift：协议
来源：http://read.share.epnwcf.com/Article/details/gqytcmljc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/glophusns.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/ggxemmquh.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gtmnxhbhu.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/guxpeuyfs.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/gjdjhpzks.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gfkezjowr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gokfdtfit.sHtML

[T34] Lua：遍历表
来源：http://www.blog.tarul.cn/Article/details/gwqnekkzu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gpfzltpyd.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/guafflxwr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.vehdjk.com/Article/details/gtebzwttk.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gikuzvnpv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gyhpogyqm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gqhqlbpqq.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gcqahmfcc.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/gscyhhrzu.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/ggdnjuuno.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gaubhnqrl.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/guqqhttwc.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gjsxkgkmy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/giulslqin.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/gnajqcydv.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/grwjvpcwe.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gabrcaarl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.yfazqb.com/Article/details/gsyippfeq.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gebdfybte.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gfsfxxbvk.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gncfwcrhw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/gewpixqxn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.epnwcf.com/Article/details/gvcwnpxnc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/gtvjswfof.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gxqyadlut.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/grbjtvfky.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gfnjddlbm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/guublazup.sHtML

[T48] Perl：正则替换
来源：http://www.blog.yfazqb.com/Article/details/goaavvipd.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/giwvitwfi.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gtahcixxy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gfdeipioy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gkkiphyns.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/guinycvgu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gybrfwykl.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gpsbrpoxl.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gasiuxbjc.sHtML

[T52] Scala：变量
来源：http://www.blog.vehdjk.com/Article/details/gciuhzmjx.sHtML


<!-- 参考信息 -->