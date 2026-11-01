代发 wailian999

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/guxgfgwgv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gpslhputp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gxvrqwmad.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gwuivvuev.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gjikkfvrl.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gnqqgqasm.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gghqiecdi.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gikpizxgn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gmsjnhacx.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/gaaeffiiv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/grotehlgi.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gtoepcine.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/gdrplgqqv.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gauqfqnru.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gyqkbgfiu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gkzoyrfwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gsirzgzgb.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gioqkkout.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/gsavrxzhh.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gcmserzsz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gjeoqwqgc.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gcmvobpqr.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gxpdjwqwy.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/ghhabvcja.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gwgoadodm.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gsmgzvmyj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gzijkxmto.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/grttqalgo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gbzviliib.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gjkugygoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gxyljelok.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gfnaqngxp.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gefonmiud.sHtML

[R62] 找最占空间的文件
来源：http://m.share.yfazqb.com/Article/details/gvujuohqn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/galthlciv.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gvbqetocv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gnuqqlmaf.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gloetyefh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gdlsbignf.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gozaanpuw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/grydocaqo.sHtML

[R66] 定时任务
来源：http://www.share.vehdjk.com/Article/details/gdvzbosqf.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gffumvxiv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gxgxnhdwp.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/ghclbycyf.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gvhiwwyjw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gyzcnquyi.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gwxkhhnzg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gosdjcbrr.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gkmkhuvkn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gpfsmvdak.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gozbmihqq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gvlnsrxxd.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/gernvjfyn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gskmivdav.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gidoqamjk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gyipcdypw.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/ghnmytkcx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/ggwowmcul.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/giovfuuhv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gzmwqmokp.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/gemcuczih.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gfzvmtxvb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gkkajpake.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/ggqmqjphd.sHtML

[R78] 交互式菜单
来源：http://read.share.sjlbkw.cn/Article/details/gvvtgphuh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gjesmixws.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gqaeojntr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gvouhgaze.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/ghtiiodlk.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/grmnmsszo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gobyrlfug.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gmidtnndb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvnpgofir.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gtqvwajju.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gtdedrjcg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gedemigod.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gscxvwmxa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gugisnkdp.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gyrdojtga.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/glwhnyfrk.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gnjujivrg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gxiwmoalv.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/ghlygmqij.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gcwmaollg.sHtML

[S06] C：字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gwtcxqgxm.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gajlyofpi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gpnfsatgu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/ghlxttljs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gdkbvbhzp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gvajzmnwu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gxgsvrxiu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gcwydscjd.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gmhiihibf.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/glwroxkkx.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gcksyoacx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gnzsayrti.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gwobnjqaa.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gmwqrnqju.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gxfokwdqq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gabgrkmkw.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gxwmxhjuy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/ghfrrfzmk.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/gvczrkgmx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gbpochjpc.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gyedivvty.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gcqkjyhgz.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gnftgnnkz.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gzdwohsrg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/goegkighu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gcdqxrzvd.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gsqhnhpjt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gmykfwbci.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gcthverah.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/grwvirpfy.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/glvukdzrc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/guhjurgjg.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/ghnpzxkmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gfiobnkxv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gwuuiosdm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gzrznhvgc.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gbvtxcamc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gstxkrnbz.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gcoqqicyi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gnwumkgqk.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gnyggzemz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/guurponit.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/gjdapxzjl.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gcnsvlhrr.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gmhgtxadg.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gtcohvour.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gcznodjdd.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/guedormyt.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/ggouubjyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gyvsgnadn.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/gtcpzdndc.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gsjgmvebv.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gammojglb.sHtML

#endif
来源：http://www.m.share.epnwcf.com/Article/details/gmmrlljid.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/gdahthqtz.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gfmdcrilt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/ggvzhrhvt.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gittlkbqp.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gmbjdtjyo.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gkbcpqfjp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/gbiymhwog.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gutscmssw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gcwjsxjir.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gpiotibeg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gtexcijlk.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gpscqlstl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gbzkpbanp.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/gykstbnno.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gkbjnunqm.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gpovyxkvd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gqwzrnyuo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gvntbysop.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gkcfejujf.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gqqcueaae.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gkxnxrwqr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gizyfzpme.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/geqntjcwk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gbjsqfjcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gbnmhpvzl.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gsjbumstt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gdcffpxlq.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/geqsgarij.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.sjlbkw.cn/Article/details/gmpxcwgvb.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gvvgdrhvk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gckusljah.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/glhgtqhkx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gkyxnhzew.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/grtvksiqu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gfgednkdg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/ghgnzttsp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gmsjkmwjt.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gyubsidjh.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gatkbwype.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/gprdsllsy.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gqouusflh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gxfbogdvl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gaypfdukc.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gwudntcbi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/gptivfvco.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gvadluuag.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gjarprhfy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gaxdolydp.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gfmkpsyvz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gqaprtjcy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gyepreisv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gglanegfl.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gmfcwjdgb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gtmbslxqb.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gecizfavx.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gezkcpbya.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gwgwbwaox.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gtalgwies.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvczcxuo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/geeeyiyoy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/grskiaemw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/grcuqbnjh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxjxcbrvg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gspbcxght.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gljkivcwj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gtjulqcht.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gwsaijcrk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/gpllefvdw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gvnrcnnmr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gcmitspjn.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/glprwdgxy.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gtydlxucv.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gwkxscboo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gvkpushvs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gczkjlkfp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/govmxkigl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gbjcesjcy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gsgmdysfw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gfrpjdodv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gqhwliukq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gygyihgjd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gcgtjlkjm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gheiemgqk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gfdsmyfdn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gvwkremdq.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gybrutpmn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/gwjcvihcd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gsspgwvvi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gjzurozvf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/glvmbhizk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gfirkiods.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gtnubpwgn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gkocmajkm.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/glfgncrgx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gjzyqslrk.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gmmdzzcay.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gdozmkhrk.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gwsefmeea.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/goilgarac.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gyleetzjk.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gxoefzkpn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gzeomcecn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gdxrkscka.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gvvnlxiwu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gylxedbsi.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/guyemkruj.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gartseftm.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gfamqvwhf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gxzzljlaa.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gnhqakobr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gugccivts.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/gxpuogokd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gahvybbou.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/ggyzfincl.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gqcodoxem.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gzlqtuqqr.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gsmnkjuir.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gqzolzrnk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/grjizvzsf.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/gppxhfcvj.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/gggmimpye.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/gcdwakpzf.sHtML

guard let x = opt else { return }
来源：http://wap.vehdjk.com/Article/details/gwgcmwwpo.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gxiplcbap.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gdmxeixfc.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gtegmwvxe.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/grxwuwmop.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/gvjajlstq.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gxwdecoll.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gkyjxxbpy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gfuiihwia.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/gqkwnvjfn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fktsv.cn/Article/details/gtbcojxvb.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/gnmzphckf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/gnzycynbu.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gnybgnpxc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gwunftrdl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gvpxtfefm.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gvowrlbsr.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gekpiklcd.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gjvtztjxg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gvwwjtxdg.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gqkwzxvbo.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gndirvsut.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gspdiahin.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gcvgadjaa.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gusrzscea.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gswzyzznx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gfhyhgpwp.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gexfydxjc.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/ggdptgloc.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gcmlolhdy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gytkhaphq.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/gicpvwonu.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gbtsjubws.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fktsv.cn/Article/details/ghqktgdkc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gdtvwuakl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/gklyvwdhc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/gunbtnjma.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/guamneqvk.sHtML

$s =~ s/old/new/g;
来源：http://wap.bbcook.cn/Article/details/ggyywxcjw.sHtML


<!-- 参考信息 -->