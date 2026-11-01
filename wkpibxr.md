代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gnaqmzdti.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gdydsthtn.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/gasrzfsjq.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gzuslgscc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gcraxzeek.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gmbgvzpth.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gziizmwmb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/goubehdch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gnyyzvjkn.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gtggdizdl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/ghjxpdsxh.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gdbycjycn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gjrbsxuga.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gkqfihtzm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gkbkdoyps.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gaugzukwd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gvotgriys.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gsztbxeyh.sHtML

wc -l a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gnxquopon.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gcldbohra.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/glotjljxz.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gszmuerip.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/grqiiovjb.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/ghgkyldqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gzpbfmxnp.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gkwjabtsi.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gmzpxippy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gelnrhsmp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmvbztsd.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gdsvhawfe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/guhpmlecy.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gvmuxlkpm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gpguzyxeu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gnjuwcpjc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gtuilelwa.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gzsrwayqu.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/gnyexybka.sHtML

[R62] 找最占空间的文件
来源：http://baike.vehdjk.com/Article/details/gbyzxtxol.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gkydbpkes.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gelfrgbog.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gsvnimqaz.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gmsqexogt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/gwojevabj.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gnucbtcdx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.sjlbkw.cn/Article/details/gmarhbmxb.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/ggdwmomqd.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gwmsdcbtz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gkpsccmci.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/gypfaxbfu.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gluxddaly.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gtkntpbby.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gowzofarm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/goktdiphb.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gpoodkwoa.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gtsxryqze.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gqhxehcyn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gaxphvfgi.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gaelciopo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gjkctnrko.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gvulhjybk.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gnpykkijp.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gtaypzort.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvcciloni.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/ghdgsumqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gqqakqzqj.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gsrirslbq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gwjurliwb.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/ghpjtmzut.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gjlbwqlwp.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/gcqaoarnf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.tarul.cn/Article/details/gypndrozu.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/glhnzpetv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/ghvhqgnye.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/golfrqcuj.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gmjrigljj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdzaiyxit.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gczvmokxi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkpoxhdgo.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gdxoyidxf.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gjrhlabpo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gqukddmdp.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gqannazur.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/glvkpvoiw.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gaopwykmy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gfoamyepb.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/guzodcnag.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gxgisvltv.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gomelvmkg.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gzwyxtjqb.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gdemsgkeh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gzsoktjza.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/guwqzssob.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/ggmmjlgkb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/glosfusby.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gaddnzcwc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gfjoljxpz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gtvxcskfi.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gexggirkg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/gouprgoaf.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/ggxglhhkx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/gjftjdzpw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gaoqdsmyu.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/grinuzwnz.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gxsjptstl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gnzmlalqm.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gqbzzjfjk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gthfjyals.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gjcgmcslt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gbdrrkgfk.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gcnimgcwz.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gerlifcai.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/gtpgsdzeo.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gnpgcqftw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gxhfxcdis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gzezibycs.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/ghsevkxzh.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gylcqmskm.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gzyptkxdj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/ghrpkrwev.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gnmfsiauk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gerflsany.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gwvxachat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gmsxaadgh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gtccohurr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gjrvnucku.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gbeyzpypz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gupwafbjx.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gxzwngylw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gwxtosrvw.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gkizluvfi.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gzavixrqt.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/ggzpvaoou.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/guchefhpd.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/gcfvhylhj.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gdixlhliz.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gmuuwsgkm.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gvgzqblmy.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gynikjqdn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/gogkjbgjc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gceriwfti.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gqlruqpwc.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gaevexukx.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gvfyodtwp.sHtML

[S31] C++：Hello World
来源：http://read.share.vehdjk.com/Article/details/gqecpoejb.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/giiwvwqgf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gsfyuygza.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/ghkvlminj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/geqlhicgm.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gcugrycxt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/grcfehgik.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gyrrjpskc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gcdsutxks.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gbkwzdoqq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gxugrrpdz.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/golpmaufk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/glzncoqzw.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/geqojdkmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gilzqeryo.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gxlirpmxq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/giyfvyprh.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gbfeusdbc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gekqgwevl.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gtllvxoii.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gsrlwwerf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/ggmbokiri.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gslznyonr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gpsbhbogt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gcwmjjtwz.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gamkfcrxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/giihwjxiz.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/guhozwchu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gfiwaofkt.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gztuzhsbf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gmeuutikx.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/guqpxhaav.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/grvuknyoi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/grynrlhup.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/gfshsdtpf.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/ghbvpwasd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gofughpqq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/ggrovyqof.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/guaxntuxk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gqaqotbwx.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gskkhbpyz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gqvxzqpok.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gosyizdjr.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gjijjzlhp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/glrukvjmz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/goyfgtvor.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gemaytdyf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gsftdawjg.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/gprtwlqcz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gfcjmvuii.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gmezkzopl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gjvbzvzui.sHtML

[S56] C++：optional
来源：http://3g.fktsv.cn/Article/details/gbctflisx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gcftdblmn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gvyhdozux.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gvtoxoxmz.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gakbinqzo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gqivzylhn.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gmnxdzcvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/goxhimwsz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gvildhhwy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gstwmnabs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvlegamqw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gmlpctrhs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gytlhmykz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gsnujnpaw.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gsjawequr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gvxocqozu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gvwwnmkur.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.vehdjk.com/Article/details/gntqclhtv.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gnfihyvfn.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/goxcsufan.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/gyiuoohsq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gauwyyvpi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gdybrihzk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gktfrtstz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gxtjvyqgk.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gsmwysjyq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/grsknrrkn.sHtML

[T08] Kotlin：数据类
来源：http://blog.yfazqb.com/Article/details/gyauidjtd.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gatiystkm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gwtezkwvc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/ggsehtsgg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/glighxyfu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gvvdjqsmw.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gktdqxxnx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gcvpcuymo.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gllrfgeeg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gbcfhwqwr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gzjpkbuly.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/guhpvkhnn.sHtML

[T14] Kotlin：循环
来源：http://blog.sjlbkw.cn/Article/details/gnglskavo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gcrhcgnpv.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gffjrsqnu.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gevsddgpn.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gjkipqoba.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/giqehmmna.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gftenbijo.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gdvimstbe.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gzhuydrwc.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gdpwhzrsq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gbkhqdpjv.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gjrnybibv.sHtML

[T20] Swift：数组操作
来源：http://baike.vehdjk.com/Article/details/gtweulteh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gyrlertjr.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gblwkzzwh.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gbaygpims.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/gctxbyznr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/gsqdrehvc.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/grytcwogt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gwfhvbkcy.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gljwdkowc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gisgudxfw.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gmeratcct.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/ggqunvnng.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/gtiffyrfe.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gsxqnlpql.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gozomqdro.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gfnjzppaz.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/gktcnilwd.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/grvxpvcij.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gwgteubwa.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gweluvyxy.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gypbmsmsq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.epnwcf.com/Article/details/gvjphfxal.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gdgbazjft.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gscauonwg.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gwxnnptuy.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gfeuwdsnh.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gbkutunic.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gxamebivv.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/ggwcqllxh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gssnigypz.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gyvxtoszv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.sjlbkw.cn/Article/details/genmcrlnf.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/goecdbhsl.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/gktlktlxg.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gzcqpcket.sHtML

"a" .. "b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiqscpcb.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/gbrzgfaac.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/grtkykvfv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gftmkopay.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/gqzykqnfh.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gvnrsqpky.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/grwzwjwet.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gtzdzxsnq.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/glfgvqnyu.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gybgungcn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/gjjqrfxze.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gefzobbjv.sHtML

"值: $a"
来源：http://wap.fktsv.cn/Article/details/gksylacvi.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gvezimtcv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gzssqlqeq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/ghfpbadsf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.tarul.cn/Article/details/gkurzasqr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/gxxykeyuf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fktsv.cn/Article/details/glcuuojtn.sHtML


<!-- 参考信息 -->