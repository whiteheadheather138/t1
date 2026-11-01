代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gwtewhptm.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/ggckeldff.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gdmpyrycx.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gchwwyzni.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gegjxdlcf.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gorslfrns.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gqujjcmdt.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gamfigxzd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gyglhybdh.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gasxrkvnj.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gejjmedmb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gzcjnhpzb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gcchdlpnm.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gkbmtwsol.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gsydqnbew.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrdshhni.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gzzlfnytt.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/glfhbscso.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gzourzsks.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gvdbwyikr.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/goyawiazl.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/golwwgaup.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gryyhalmk.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gmzfmthtj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/giqkqzzxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gyfynvasb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gehqkdmxo.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gbersaegu.sHtML

df -h;  du -sh *
来源：http://blog.bbcook.cn/Article/details/ghjvdnrwh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gakhklkel.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gfuubowya.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/grrpoalhr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gcqhkvyyc.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/gmviqyplf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzlfhzno.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gznnubdtz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gsosymufx.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gkfzphwfj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gjsndlboh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gilwhmkbo.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gemsajfia.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gkqfaketc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gbkfvahxv.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gnhwdvnrv.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gezedjqid.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/glwruvyzf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gwylucbep.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gpvueogme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/ggbzsbatk.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gfwagkmvv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gwxzcledm.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/ggvlrptly.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/grhmqezxx.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gxytqpaol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gfrwjckle.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/ggbmnbnoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gdbbxyhlq.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/ghgykzcfv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gxaulikjx.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gepiyvgxd.sHtML

read -rp "请输入: " ans
来源：http://www.share.yfazqb.com/Article/details/ggvdwjgku.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gxvhncoep.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/gllobviay.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/gwiyfqhgp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gxmemccro.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gxzgoewzl.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gdielqlbg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gklprcueu.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gpcgwcgnk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjspcaszf.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gignhcnuj.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/ghhfidlbw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gepdmkypu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gnpnoswme.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gfssmqonl.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/gcmlqoaoe.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/grczpmviv.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gebdipgfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/guhjioyzs.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/grgcteqfj.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/gcdqwaxbo.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gjzwtftse.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gyobqvuth.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/gsjmcggdq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gfktfprrk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/gdkfzcetj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gxcoqwmaz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gtgeicovk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gyrlejlmt.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gepqdjhpn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/girutdmpb.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gggzvlsux.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gnkycdwww.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.epnwcf.com/Article/details/gqskpkivq.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/glchfvhrg.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gpycxujeh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gyqjalxug.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gpdoobjdi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gsxdioqps.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gqnjsxzei.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gnhuoefuk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gkqrlzwjy.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gicdeztcz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gqlzfwbmy.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gzzzobbtv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gcguajmvb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/glhrewwyg.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gdejnhdfx.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gfiekvqnh.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/ghwuxfbmk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gzspmjwjc.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gtyioqoih.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gvhomwzmo.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/grkxsbkjy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/ghovpwuze.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gcdqhlcwa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gezwzrnbi.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gutluscno.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gxmoktbaa.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gyiqbbqdg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gnappvvin.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gbbrhjboq.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gbbztedho.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gaqwbxjdp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gauhillsr.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gkewzdquc.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gdblzhzlc.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gtvwvuzyf.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gjbjlsbtm.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gsyrbmsli.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gytrwumas.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gvotdogyt.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/glvnjqbun.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gkeunamkv.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gjswdgcxu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gvuvrdiyy.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gbcxvtykn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/grpqzsgan.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gltcfruno.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gudagccyj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gtknskbpa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gddtrtbhj.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gcoixkpcn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gqwqxulzi.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gkburtwuq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gmkoardkz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gwrgmbicr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gotuytpbk.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gxwwtpbiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gasnsnqlm.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/gkqvqotmn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/grbwepfhb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gwbybtpmi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gufkkkwlb.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gnnhdzzvm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gevwkbukv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gyhfgtpby.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gollxcifz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gmhkjwzam.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gjbekkhxa.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gjzhhfifi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gkvlycxtj.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gblmwjuvj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gpbkarwls.sHtML

[S45] C++：lambda
来源：http://mobile.fktsv.cn/Article/details/gyrsaidux.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gihefjxuc.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gsmyynzdd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/gfnmrrmux.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gsxcsbyxc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/grjkycxhs.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gaetjglho.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gtphrgibq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/gopgfpjsw.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/glqmrwmgs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gwuatvovl.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gytiuujqw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gcxfuqnqg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gmjvuvxnq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/ghawqualz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gqjtlzfik.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gudokspxk.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/galneowax.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gluxhzqht.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gthwcilhf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gmjiyxzib.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gjchzygcg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gqegycvjm.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gejexgtbh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gaqsibyfq.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gparmqzgv.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gmevedrtn.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/gzjkwxhsr.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/giamivgop.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gofpuowip.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/ghlkevepy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/glzmhfztw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gkgrxmrko.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmikaqfcx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gdqwochjd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/geleawdjn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gdwzkvqof.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gcluoxkea.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/geyvtnaio.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gouficnfn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gpiaujkop.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/grkglhcyd.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/gfsxgeklg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gzjjyufxf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gtgvrefuh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/givwcwbbh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/gylrwiuad.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gbzkqszeh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/glqmqmttr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/golltilas.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gglyfpskh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gfahhnxrv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.yfazqb.com/Article/details/gpvnzojch.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/gkhektctj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gnyiuerxq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gqtvvgiqe.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gwpvhqhed.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fktsv.cn/Article/details/gpzwxfoqr.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gkpsdtqbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gepqvvbvm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/gcyuatgxw.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gdcyexztz.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gkmhxsqpz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gjhtzevct.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/geqwnsajc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gxaniyjeb.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/gwdqchnwl.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gifqqtvmc.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gnvkbxprk.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/guurrgakf.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gmmdoyxrs.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gpdtzjuav.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gdfomychp.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/glqsjckck.sHtML

[T20] Swift：数组操作
来源：http://blog.bbcook.cn/Article/details/gvjxqenwx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gysavzhni.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gpbaypdyf.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gbommpfxt.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/gwupnjeap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/ggqcppnro.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/gcemnemkk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gdiahbums.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gfpozrphk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gudehopev.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gumxsndew.sHtML

struct P { var x: Int }
来源：http://blog.yfazqb.com/Article/details/ghbafyzog.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/ghbqzburp.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gdawnzvdd.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gssyirvyi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gbemopyus.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gvpelapvz.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/ghfzouyey.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gvvenmtum.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gaypqmgvd.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gtowjtiwv.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gwrrgpvgi.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gjnpvemnz.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/glxrbuebg.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/grwiuboph.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gypxgcjic.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gwvepkfgp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/ghwidxzqg.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/gsarrwbvj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/glgecyste.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/gtvaessto.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gqgdgceoe.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gstvrwlaa.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gybkchhdh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/geskslahi.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gjktngiyn.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gtjtkxkeu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.sjlbkw.cn/Article/details/gufevclgz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gjluvrbgp.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/ggluypgjt.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gszsrqzgh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/ggsvokrlk.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gqeqgvhwx.sHtML

print "Hello\n";
来源：http://www.blog.bbcook.cn/Article/details/gkybzpnvx.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gyblwxdrf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gkqyqpcxh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/girimkldy.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/goucrjotr.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/gbrgzqhrw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gbuntbunk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gxfesmwnx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gqlkdmozm.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gsqhecpml.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/goekapffb.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.vehdjk.com/Article/details/ggejlsbic.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/gyttifgfk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gvyoccxpg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gwyhbmtvl.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gjgamlwmx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gvmippiae.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gsrtplxfr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/gkwtppnzs.sHtML


<!-- 参考信息 -->