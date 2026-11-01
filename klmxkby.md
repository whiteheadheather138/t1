代发 wailian999

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gjefoxovr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gywmjcwat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/gctdptryf.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gtypwpisx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gsnxnuaui.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gatsxhgyi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gurakeviq.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gfeunlpwi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gwygwhuda.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gcmkdzfce.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gbmyshzwf.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gpydxzdcp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/gqkhyizbv.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gzjjmohnu.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/grwyfnrno.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.vehdjk.com/Article/details/gnwjuyfhl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gqjrbsucw.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gjlycqnci.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gtlepmogc.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gpzgrrexb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gwazvxgkv.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/goawhkptf.sHtML

scp file user@host:/path/
来源：http://www.share.epnwcf.com/Article/details/glnwtftyg.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gzbwbgxho.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/griygdfzc.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/ghpuilujr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gmizksggs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gcvlyjelz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gravlrhqt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gxcdtinfl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/garuwxstx.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/galgvwazk.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/guojfbsup.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gdqqhhenv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/ghvohfsln.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gydplxjmt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/glbnyptpt.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gmybkicdq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/grgkjtnbw.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gsgbucntb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gwoezsuae.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gymoomxre.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/gfamklrgn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gnwjqhhru.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gofmzmkat.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gqaxrhepc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gzkdoqwky.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gcdmssvdv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gypfpnfai.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gjmlcwaje.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gtreltpwa.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gewvvyytr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.yfazqb.com/Article/details/gyrbvtuaw.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gnpxbgffa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gkeeotvtp.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gakkiqcwx.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gxvkwdett.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/garevvmvq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/ghoqfgdfb.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gukirbtir.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gayvtliyk.sHtML

[R76] 使用临时文件
来源：http://m.share.bbcook.cn/Article/details/gctuzoyxs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gyvjjtsqn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gtwptjhab.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gdxqutgno.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gyfjpmhbr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gvbmzeffr.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gbjljcdbm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gehvmzifi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gvurwolvo.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gemkjylxl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gptbebiok.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gmagsayjr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsnoagzqc.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gepslfbfr.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/girerxqvd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/ggsheixcs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gdtlzxlpw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/gplrkpcfh.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gtamsxexr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaguthazm.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gsjxxtloa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gubybjtss.sHtML

[S05] C：字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/goqwomuwx.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gkairtpin.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/glxaiadgm.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/glazoenxy.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/grftoyzqc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gzrxatdqh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/glateampj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gwgvnuekl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gnopxuydn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gxxwiryzk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.epnwcf.com/Article/details/gmsqolbar.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gwlpftick.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gyzbvreij.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gumjvgwts.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.yfazqb.com/Article/details/gkomkzgul.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gdbrkjgcd.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/ggzrcmvca.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gxnbzvdep.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gwdyztzma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gxwefbtxa.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gwninpuiv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/ghuscftjo.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/grkcgkmas.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gxqqqqlea.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/gcoprqbge.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gyatmiqjb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gynemtwwf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/gbivjddct.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gpdsmbmvh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/guqtjhted.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gmjarbpbm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gkrawekiw.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gpukokeqp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gqdlgczei.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gvprakuzy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gwdwpdfac.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/ghfgqnfsh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gzsjoktay.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gepqocedk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gsbnfmcaz.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gkkluobmk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/ghbmuzwhs.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/grzacqxdz.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gyarneecp.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gshxckbax.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/guckxamhq.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gdmissywb.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gkpqltvkh.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gonqxjbcf.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/goitgwckp.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gosyuhdsn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gtuqibabe.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gbejjrbdr.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gywcjxeys.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gojyxsjxv.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/grndykwkf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gxvpehzbk.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/ggmodafla.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gkaanzypd.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gcbagylhv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gmuknoyjw.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/grdoxwzql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/guykbqfae.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gxeoiidkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.epnwcf.com/Article/details/gaddzzilt.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gsdcvnuwu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gokicwzqr.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gdcjqmzpj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gflxnshns.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gyeesqlnh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gbixzdwqm.sHtML

[S38] C++：排序
来源：http://mobile.vehdjk.com/Article/details/gqozynzif.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/glnuyxnnf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/glnardgvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/grkllerke.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/ghiynjyco.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/glapbcxls.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gwmpbmhzo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gfcjchevn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gojhvande.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/galwbyftm.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/grgagejeu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/guopavppm.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/goovoykpv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gdwtxsgzh.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gmwvymjcd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/guwsceibx.sHtML

[S46] C++：函数模板
来源：http://wap.vehdjk.com/Article/details/gmkbuudxe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gvrxlqaeh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gbvryfzpw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/gusqjqnfz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gatthhfku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gjeibrlvr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gqsqyrwch.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gnwtqlgel.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gpxzwhyzq.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/gpljonkaw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gvfepsdwg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gbfdgpqtd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gpoyppafz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/grolhdzfi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gxqrbubic.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gftjetatf.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gocymogjc.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gjwjknuub.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gepbszgzn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/gjodeilze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gacheebjc.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gydzzlyds.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/grqdzscam.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/gtrsbojtj.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gmdusymge.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/girkxlpis.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gajxurtyj.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gwudorojl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gvjzrpsso.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gxdoarlyj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/grsxzheij.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gonlsimpr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gjbdsdpor.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqvwxjlpj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gnityhpor.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/ghzwycntm.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gikvzjhxm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gsedcslkf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gnbgxreei.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/grgrvyxwc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/geajiwtws.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gbijyvaiy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gmrzhyota.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/ghiqsxumb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gdovnezlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gpyafecns.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.vehdjk.com/Article/details/giqbojobr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gvdvddqss.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gobefcamg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gxdaagnyo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gwvouyxor.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gnbmzgwiu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/goibqxmvi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gmanvtmss.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/gcwmfysmg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gvnctmoyn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/giiyjlvxa.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gkjgulcnn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gvguejgec.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gubwuhmrq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/ggrrjipqu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/giupbubff.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gtxvmdfkz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gwobmybhm.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gwddhpfxn.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gaczzisrc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gjkjzycwy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/grxjzbnxb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gyxfiofro.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gjcvltobm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gpxyypcou.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gkokzrmlw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gezbjhzck.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gechrolqz.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gyfgujahi.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gjjbwtlms.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gtskqbdax.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsuvhngi.sHtML

[T23] Swift：函数
来源：http://blog.epnwcf.com/Article/details/glaifkuhx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gmokaoggx.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/gziwkfuzp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gzanhjiok.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gvserefsg.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/glharkoly.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gezjrbrds.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gaafpgoqs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gwkgncfzx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/ggsyivafm.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/guergubgq.sHtML

enum Color { case red, green }
来源：http://read.share.tarul.cn/Article/details/gqhjuybjr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/godfdewsm.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/gguijayaw.sHtML

[T30] Swift：协议
来源：http://blog.vehdjk.com/Article/details/gpwjzfsqq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gosfzfhcc.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gbpoclndj.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gvbotzjrl.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/grraftmnh.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gjpbryhah.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gddhrvpvh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gufhrmwcr.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gxacejvdf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gypstqxuv.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gtkseuyeq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gufroljbs.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gerjbyxrc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gdbgqlhss.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gnsnqylze.sHtML

"a" .. "b"
来源：http://www.m.share.bbcook.cn/Article/details/gbpepeqga.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gzdbtnpxy.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gbnhbbabn.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gvkkvbmmu.sHtML

string.find(s, "%d+")
来源：http://read.share.yfazqb.com/Article/details/gmcuptlgm.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gnmmycghf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/goaguqokf.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gtjiiovrk.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gkkplhaja.sHtML

[T42] Perl：变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gdicsauqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/grfjslpsw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gdxtemqkv.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/gbhisztsk.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/ggzdywoqg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gdzcauxsq.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/gamzlbrog.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gzsibcgkv.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/gtmuzvbgt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbbdykvhe.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.vehdjk.com/Article/details/ggxleszkn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/gulzkdyhm.sHtML

[T48] Perl：正则替换
来源：http://baike.sjlbkw.cn/Article/details/gamycxnkp.sHtML

$s =~ s/old/new/g;
来源：http://blog.yfazqb.com/Article/details/govvzcebx.sHtML


<!-- 参考信息 -->