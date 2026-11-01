代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/guwkzhljx.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/gmltdnlpf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gxndjpsal.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gtqmhwrnu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.tarul.cn/Article/details/gnkjjybce.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/guiorckko.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gysfykxzs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gyjerqheg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gbohujtle.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gnguehytv.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gmrxmpyav.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gszvasczh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gdfxsrxcs.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/giqwvjxos.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gvdvqttea.sHtML

[R57] 远程执行命令
来源：http://m.share.vehdjk.com/Article/details/gihbrcnzz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/grrmggcay.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gogwbnvkh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/galpykkcr.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gpgdopvfh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gxmjfuvtw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gejiatcxq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gggwbqxru.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gkbegfzju.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gedqhczdu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gyncmssly.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.epnwcf.com/Article/details/guvoxlofn.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gybwislzd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gvhcqkbhe.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/gmixpxbce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/ghjhubpmh.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/gwccxmnhh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gkkjslqkf.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gymkxbvek.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gucxetnaw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gqatofttu.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gyvcmraxo.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/gwbsvkkrg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gunwoprra.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gmqlhubon.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gmrbmmtxj.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gexebigbg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gdfddirce.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gevjluqwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.yfazqb.com/Article/details/gmnonujcy.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gpixvxqtf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gzmjmkujf.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/gowsfokxa.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gjscpetuv.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gqkvtuesl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gofoaxgzt.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gfujxdyiu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gwtnqrztp.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gtohutuws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gwfdselgp.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gefupuics.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gkasfdunr.sHtML

[R78] 交互式菜单
来源：http://baike.fktsv.cn/Article/details/ghiwhfhjr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/goptcurqo.sHtML

[R79] 解析命令行选项
来源：http://baike.yfazqb.com/Article/details/gmtnnhkmp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fktsv.cn/Article/details/gpleseqox.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gjectgzye.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/ghxtnrrhf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfgzzswxo.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/ginxejlaj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyklttsqa.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/glgxwkvzs.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gqzqvenwg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/gxuhrslzi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gugvkgvyb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gzlbgufke.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gwprzpbqp.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gbfjfgjrk.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gzkkjywxx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gximfrdvb.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/ghgwvxxtr.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gafmcmnnf.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gakwufmtb.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gujolsbbk.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gxdbvysfg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gzqyczace.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gsqbiycts.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gszndeagb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gfleqqtzn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/gbuaygwnj.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gspytqvih.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gftwhwfod.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gsgxmvfud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.epnwcf.com/Article/details/gseyqrvxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gapokpifr.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/grohdrbcl.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gbtnqxagd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gydvwfdal.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gbbdjvrfq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gxempsuio.sHtML

[S14] C：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gwirdadbz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/grvmrgerp.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gwrbncngr.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gtqeeqadw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/gzxodiijh.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/gwrowjitm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/guxfwrjkx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gcuqvkliq.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gzsdotsfv.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gutxtxcox.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gutlssrmq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gkbtaxtxi.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/gunnjhdqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/ggtzzlbwj.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gmmqokccz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gxokaacne.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gxdxlanmr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gahrfqljz.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/gxmaaptlb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/ggfgeoqto.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/gzwmsukho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/geolalbqx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gwzzrmvhv.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gvdqzzdlc.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gtmmrxnij.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gsgnvlehp.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/giikwvbjd.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gkmsuwqkz.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/guptjytup.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gbdlhwbdo.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gkdtevekz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/gohdhfdrc.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gcumcichl.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzmfbiyu.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gsryjjjvj.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gmqhmzsgi.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/gflstccmm.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/ghdqfxixb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/glkjkjtqh.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gyhuahfcn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gbufeshgd.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gzvbequnm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gnujxgllz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gbaseaiok.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gznqddirx.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/grooqopqb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gyvoimfwh.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gsolijjht.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gxdflvyvb.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gkkwmrsnj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/gqegkcwmr.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuisnebx.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gizmyhhmh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gbufkvusr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/gjtwkoukp.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/gaovnvahi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/giyauljiv.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gctrnuupl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gpxozeawd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gejkxctic.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gttwmdcoy.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gspnhtzfi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gbbdqncyv.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gorngohax.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gupvieqdy.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gyldnxgtu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.vehdjk.com/Article/details/guakxfcjo.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gxccvfzvl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/ggzyantlo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/ggazharjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/glqqlrweh.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gjsakqliu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gtiacbxbk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gzzshxbom.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gsscxdgvn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gkjcadglj.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/geuyualeb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/giknhjcfv.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gcctnmxjh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.sjlbkw.cn/Article/details/gofaymiwe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gvhbwrkzm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gduvsgwah.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/ghvztzkaj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gznlxfncz.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gdlgoffxt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gwokwqpbk.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/ggeglcrho.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gopbsqkkz.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/ghienqmzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gorffkgmy.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/grkdunqnm.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/ghxjltkiq.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gwilhcxnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gjntaenzg.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gmpekjthf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/guqnnsumj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/grrqsuhyy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gazjkrrbn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbevnwpbt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gjqvzjbrx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwxclrgvg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gfxvlxvch.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/geqautbiu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gkzuoxbsj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gnnenggkn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.tarul.cn/Article/details/gfhabvkvp.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/ggapgxlnf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gbuboitrx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gyksvnmbs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gscubpprp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/gixssmrsr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gqfiywnzv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gisxdjyxj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gsbgpekpw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gfxrmbefx.sHtML

[T08] Kotlin：数据类
来源：http://wap.fktsv.cn/Article/details/ghffwqgae.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gaejjzwgf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gpnpwkcfe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gkcydwrms.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gtrzqmggj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gnratttta.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gchxjsnpb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/gzgvztktc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gksebygqi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/ggmcqckfz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzdpllks.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gztphuurj.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gnpqdshxe.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/glfspcqzy.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/glydvavyo.sHtML

interface Shape { fun area(): Double }
来源：http://blog.bbcook.cn/Article/details/gjiccmlyr.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gcwfzmlfc.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/ggomzykyv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gosqqpllh.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gdxownhqp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gycpyixqu.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gehgffnkw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gzwuehnyg.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gsnpygwjz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/glnvzlglj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gydgpzmar.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/galbbppmz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/gcfclmzkp.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gskblheci.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.tarul.cn/Article/details/giefcdvlu.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gbetdzobm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gostpmrpr.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gnilkcxjb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gratugeir.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gxnfdrvzx.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gqwhibnzw.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gqaahbywm.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gabinaiuq.sHtML

[T27] Swift：错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gfsabwvqi.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/guisujqcl.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gderkowyo.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gsocqfhwr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gmtkbxqyq.sHtML

guard let x = opt else { return }
来源：http://mobile.yfazqb.com/Article/details/guskxrjkm.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/ghobtlsyx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.sjlbkw.cn/Article/details/gngvlxepr.sHtML

[T31] Lua：Hello World
来源：http://read.share.yfazqb.com/Article/details/gcxbosxfl.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gcnqvztgx.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/ggleoorys.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gtgcaqgbv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gybbtkbab.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gdsaxqsav.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/ghvyfukdk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gafyoemvz.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/gpxzzmega.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fktsv.cn/Article/details/gtoraxzpo.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gmhpotrqc.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gpuderjkr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/guanlocgh.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gmerbhnkw.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/gjqgnpsae.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gjaeosncd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/glizcwnhh.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gukydkzkr.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gliruafqg.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gsntwynwx.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/giwmvhojb.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gniphbhkc.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gxclpmsbi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.vehdjk.com/Article/details/gwpilkddq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gyeefpekt.sHtML

"值: $a"
来源：http://m.share.vehdjk.com/Article/details/grlxpacyi.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/glpdeebqb.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/goxdtrjcl.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gzuthjlnb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/gkihfakup.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/ghshlqsxj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gxqagwqnk.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/gmqerbeii.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.vehdjk.com/Article/details/gizhmtmxm.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/gfmhydhgy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.tarul.cn/Article/details/gleefmbyg.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gxgiaggng.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gvgzyaqll.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gonubjzoy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gmvebreho.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gpjyiszkj.sHtML

[T51] Scala：Hello World
来源：http://www.share.yfazqb.com/Article/details/gojeilzui.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gogzcuhcz.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gypjywonp.sHtML


<!-- 参考信息 -->