代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gjlckmsrj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gfztpxcjv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/ggfnrcbtw.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/grsgrwqrz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gfeoepbij.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/grtnypfvw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gglgtucfc.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gsnqpnfaa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/gisjkdice.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gmvznzkwl.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwjuolxki.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gyptigmga.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gcuwhjhmo.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gnucrwjqh.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gphslpjvb.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gqrdmlfjt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.yfazqb.com/Article/details/gwnayvcth.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/garnnzdyc.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gvfsnrtbq.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/geapbhqwi.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/givouegqc.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/gqcapphen.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gkbjzlpzi.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/glucaspgt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gejvizgoy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/genjkdrff.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gsxmnujsq.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gtaoauzvt.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/ggxvlhtfr.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gugdcoumk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gesvipbed.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gjxccmrdp.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/gfxsekcaq.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/gsjgqmgkh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gwmipwswf.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gtxznxamq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gersazydl.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gkxtkgfsa.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gnzqwkula.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gxhfidkmq.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/gtzxcpqqg.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gomtmllxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gdbsuclwf.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gffytqnxc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gasqfrzva.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gklqmdgxs.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/geuhflohy.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/grdtdcyqa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/guajxetaw.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gdyhahfri.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/ggcylyfbe.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gpwtfptla.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gcivlrneq.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gumskqwdf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gyipkphah.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/geowzqgts.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gymvrfaaw.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gdulenujy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gsmptinqf.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/griwodcgi.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gagwkcqym.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gngqvxwlo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/grgadzcjo.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gotlgdvmc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvyhwvlcq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gkofoccle.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gpqefgpse.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyjhnqkqt.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/griqslchq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghtyguchc.sHtML

[S01] C：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gxqjcwzin.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gzrjndyrv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/ggwafjegq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gqckqxpae.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gjdnpzugj.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gprlwohoq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gddchjziy.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gmrnfvxkp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gragyzesz.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gpbbzwmlm.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gcbrlboji.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/grfsongov.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gspvxvhtm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gepockicb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/glqdgytjc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gurlijcbu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.bbcook.cn/Article/details/gmnsfdbxr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gfwtfesmf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/gqntqcoht.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/grwpowyve.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gwmpzhvik.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gqocgpchb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/galgkxxhv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gceqgdqom.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gexeemsaq.sHtML

[S12] C：写文件
来源：http://www.blog.vehdjk.com/Article/details/gdqcxgjpf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gpmqlbyay.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gurtqklnn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gyitgbqxu.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gddbseulg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/gswcoxutp.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gnjbbjmgw.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gijzuwree.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gwogsrmnf.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/galkebrmc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gtnwfpifr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gkzvissui.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/gxsyveuce.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gwfahyoqp.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/ggxtpynuk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gusnfhjne.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gqgmrpwds.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gkxhlphxi.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/guunziqzl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gmjiiqabl.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gpnlsfacf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gvygzfjzv.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gtfomlkrl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gcvhqaenn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gcnaihhww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gdxckymlu.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gvywobliq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/gytuelpgp.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gmrfrqcso.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/grwtmqqnr.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gflxgpvtq.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gnexyqkhs.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gtpayruug.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gyjdncmqy.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gmdvzjbzf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/giusgtmrw.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/glbrggkie.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gsswtvbir.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gfxxdafoo.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gqvuxvzxf.sHtML

[S31] C++：Hello World
来源：http://mobile.yfazqb.com/Article/details/gravipmhg.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gxedjxlkg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/grjmlzbbq.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gboxykqtw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gilaoeryi.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gxvyryoep.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/ggheykrdg.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/geiknmcri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/gvffhfldz.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gghfwquqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gfaiinedr.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/ghztbymvy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gtcxkhoxe.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gjufrmjgj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gcphppaer.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gkbqqylas.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gdmaknwql.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/ghmnwcqiq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gtctngqao.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gxkoiymce.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gqhqpdfqe.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/glqmenpow.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/geunbfgbg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gysvijcta.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gkwebhevh.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/gcgwwzaeo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gpdicqahj.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gsmghverg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/grptyuazg.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gykwayytp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gkomodcgf.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gjqqfatmc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gbwogkarb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/ghvfupput.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gyuyqfvhf.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gshltcbwb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gpueszkzv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gcdnxidlh.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gbpxaxnrk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/ghrciqjiw.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gujnqxoee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gbaqfofvh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gikckosua.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/guocvtytv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gdpjtiqjr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gvngafrgg.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/ghoakneuf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.bbcook.cn/Article/details/gsxjtsjnv.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gnfvbhdum.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gutwxhypn.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/gqcgyjbsi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gwjkozccn.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gvdzwrtvp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/gruutgbod.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/gljbjdtfi.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gmoycoqai.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/ggyvmwtqr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gmwtoxsbs.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/guuytjwwd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gkoqxfypb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.tarul.cn/Article/details/gvfuzphoq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gwaabqljo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gudoleeit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gaasdcvyb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gldpjnugh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gmwajxsyr.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gwgqdjvxa.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gpuloounx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gltxfswsh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gcqbtdjxf.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/ghwrsgqic.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gcrfuzonj.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/grkbckqsf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/gdqyarcyh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gujlilsrp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/gvmqwfjiu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/grfffyqwt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/geqhdftfo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gmklfnjuh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/grzbxidgx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/ggxnntdcu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gowdblqtm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gzhcikrbp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gzhkzczux.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gxlawzzbd.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/ganoyhcjx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gvmsuzjvp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gmesnaqre.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/grthafwgt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gvbljqbmo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gwjwyzane.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gbfoswoka.sHtML

for (i in 1..10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gtnkxfadk.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gfsjzgyeq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gfypptbsv.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gfkqprfek.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gmxronrho.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gchzbvpbg.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gopzlpjbv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gtbuplyik.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gdrdnuefn.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/galszkdxe.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gkyoqyeby.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gzctdxwxl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdipadvu.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gjjgyaozs.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/ggomqngpl.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gmgkqcljf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gufrkstac.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gdzrjfmvo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gmwgprgfm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gomgqsfer.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gyobuewll.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gtasdlzph.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gznempkki.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gjlzufkgx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/ghpntwavx.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gzozjtovc.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/glyhajgwv.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gldksofvx.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/ghswkyqik.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gdtnuwbct.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/gefgryudi.sHtML

[T30] Swift：协议
来源：http://www.share.sjlbkw.cn/Article/details/gpjapxjxu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.yfazqb.com/Article/details/gpjhkpxnq.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gbwmwuyst.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/ggoovapoc.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gawfuxvxh.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gebuqlohr.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gzpdwmnee.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gccoieyuz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/guavuooug.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/gmvjggoah.sHtML

[T35] Lua：字典表
来源：http://blog.yfazqb.com/Article/details/gxuhilcqe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gnlodjnxb.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gadpqftru.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gwpbcqizm.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gvnehfwag.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/ghfnicbis.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/gjcrhdgbc.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/giandyxro.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/ghrbkgavx.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gzdvtlyrk.sHtML

[T40] Lua：元表
来源：http://www.share.bbcook.cn/Article/details/gywzeoskx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gkwsuvwpo.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gwwmcwbof.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/gmdzszwrc.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gvfjgnqeq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/ggiiqklgz.sHtML

[T43] Perl：字符串插值
来源：http://blog.bbcook.cn/Article/details/gkfnasugl.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/gtngcvvax.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrpjkdux.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gozpxjxqh.sHtML

[T45] Perl：数组遍历
来源：http://blog.yfazqb.com/Article/details/gzpjnyhwc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gxvamtkil.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.bbcook.cn/Article/details/gjsayiecl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gwndoldln.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gjambjkre.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/gzmltppuz.sHtML

[T48] Perl：正则替换
来源：http://3g.bbcook.cn/Article/details/gxzvllnqc.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gkgpxsdso.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/gsqxypoip.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gcjvvywxy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gmzcqqebh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/gecklhjna.sHtML


<!-- 参考信息 -->