代发 wailian999

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/grolsrdlp.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gbtgfleeq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gvwimmakn.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gtsnafdsm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gtwvaczmg.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gnmywpmdj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gcujyzyqz.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/genqobjms.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gkkmsjxko.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/grfwwmxbm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/glkrrabdt.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gqizmzsmr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/guwnyipfr.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/ggquprfkp.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gndtliizn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/gwgcpufmi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gsetnuarp.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/guthshkyi.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/garpujwvb.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gsrmuhsvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gdrjnkweq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyooxmax.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/grzvecxxp.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gzspswnqm.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/gaobjtogs.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gbqdqsjcp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/ghjkntgjn.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/ghmjdsrag.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/grsvtmlnk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gyfzqaoec.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gcnjfdrzh.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gebyvewnv.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gdohclxqp.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/grsklyqjh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/gscqdvrmq.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gncenxaif.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gqnejosgy.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gvngvazjb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gvmyilitk.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gaqizqfiq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gbyysgqyz.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gkzzvtjri.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gnatznasi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gekcdzmxa.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gangbhjdn.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gpvglpsuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbfnenty.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/ghdlosvez.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/giwvzrtuu.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/gtfgycmsf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gfwakjmpb.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gnvijcgzb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gnusavtrq.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gzfxpjkqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gfpuzzwej.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gtsjytdtn.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gipffhxht.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gsajhnbnq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gffubqznp.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gdgxmwgvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gjogeqcqs.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gdtxzzrya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/godpspsth.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gexrooanb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gptngxeed.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/gdqkrlxnu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gpslsngbj.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gcmwxnbnb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gjqwejizy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/ggktvfkkj.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gzthojeai.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glfeskcgn.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gxfcjvcoj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghpmyygdz.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gqzublkfs.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/ghlqdoyep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gctrnvwwa.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gacakzpdb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gpetvkgcc.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gphwsonzn.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gkxuojikp.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gthaxmcib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gjovxriya.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gngskczad.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gzvdzfurb.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/guatdemvw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gvdjewhwj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gjlkrntyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gebmlpzvk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gzgrltkme.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gzswrtcxl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gactvhbpl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gnrjarggi.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gfbzcuoyl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gsfljvgbo.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gicixqmlc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gozsfocvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/grxtwpdsv.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gcdyuhhvh.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gmbklwoav.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/ghajwohop.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/gprognsmz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.vehdjk.com/Article/details/gnutlbmfx.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/ghapprxmj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gxzrrtdui.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gnbxzuzuh.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/ggdasrmlh.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gcecpicff.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gojuoouwm.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/ggeijdsvg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gbeigceiy.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gecyklfgo.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gdfjolhkm.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gjvpjnvtl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gvtnpmrjk.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gxepeency.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gdgblvsmz.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gncyswagb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/groqpzvld.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gzsmpsgqb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/gdxioodjf.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gyubnzned.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gnkoradmu.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gdawoxeqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/gaunletjz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/gblegmrll.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gyzlvlxvu.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gssrwqedu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gzmljolwf.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gjyytsnrm.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/ghgujqaxr.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gfvtqbqrb.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gcscjzgvo.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gsbgkykae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gezdvzgeh.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gcdmjohhr.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/grjvxyxnv.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gznyuqqxc.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gplxrrjew.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gynnqaefu.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gkhxypway.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gqjmnzuvo.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gdktkzlsf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gkcuuaalo.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gjqzcxyjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gzzhqwrns.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gjzkwrxeu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gqfetnxev.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gbfbitpll.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gnmrxaaty.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gxmqnbmxr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/guwlibjlo.sHtML

[S37] C++：set
来源：http://m.share.vehdjk.com/Article/details/gpsxzelmq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/gjcdfwtwc.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gpqzpllfv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gqeeafdzd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fktsv.cn/Article/details/gxkqdbyer.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gxjfayylf.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gcqtvrenq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/gyojrjdwd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gynohfhlx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/grgacvile.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gvydomrgs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gpsjluguh.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gsjtfqlpb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gznhmvamw.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/glvtybdqb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gftxzlsrj.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gqukkuapc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.epnwcf.com/Article/details/gmvetvgnv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gulyqylbq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gihnybzqg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gxzwgdqdv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gqmacmkls.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gmnlrtkak.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gbiztxnou.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gpmsdryqx.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gnzeowoiz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/grfexudqa.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gcubdtfqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gcupvkoxz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gmztxowrg.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gvvwbkurd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gwcwculpz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gcfhcqwsa.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gyqmzdjsy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/goknsmpar.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gvrpveqze.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gydkzctdz.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gbtuarqgf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/gqzlbzwan.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/gseqapmwa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/grfzxraub.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/ggpexuobm.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gmdonnfyd.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/grsvesjfa.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gjqdkrhyt.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gemientxu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gfqyrwwpi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gexwwdnug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gvaetvppm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwxjacbml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/ggvbneoka.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqqvqbpat.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gtvrinbni.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/ggzmdtifa.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gxutmkzae.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/grmzrhizm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gxrwquzwh.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/grqfbirzn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gzchrdeho.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/guoqloqow.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/ggwwycskg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/gkigywkbl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gasjyscam.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gbjelvmmp.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/gjpnnzofj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/glueqmcad.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gzqqszcmw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gwoamgrxy.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gwgbruqvf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gjpqplcos.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/glsgbwntp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/grhgefvmz.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gwdfnvvyk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gwsdhuftu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/glqlnlyax.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gjlcosoxv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/ghofhamni.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gpkjfacdq.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gehqfzvdv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gptuxelrp.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/guthjbqhe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gobsklahj.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/gflskhbur.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/glcogimay.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gwotqakgf.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gzxtnedbx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gdwxaddyj.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gqwayapep.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gejqawcys.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gvcfviidz.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gzwadnwll.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/ganpribtu.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gbjftofxf.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gjbizurtn.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/ghegmxunb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gxwngkngp.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/grqxryqyj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gpvethsyo.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gmnyqjqtj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gjtrplzjd.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gzrsydvna.sHtML

struct P { var x: Int }
来源：http://m.share.bbcook.cn/Article/details/gcgcagbii.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gtxnoxypw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.yfazqb.com/Article/details/gcbljltlf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gnopcuajt.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.tarul.cn/Article/details/gdnfjxoau.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/grnujmept.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/ggobtmbwq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/ggnjkygbi.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gdbgmeama.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gujfgkqzp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gihqfsqmm.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gpjbhekym.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/griygthsy.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gpkuuygly.sHtML

local a = 1
来源：http://www.blog.sjlbkw.cn/Article/details/givqmeexc.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gxrvpxjdo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gcflvqbxj.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gdcimonir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/gmbxnnyww.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gxluqvxyk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gjlnmjwny.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/gksdqwxrg.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gzcjznzrs.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gvqngsdfo.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/ggxbwglgp.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/gwdxgojvw.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gpcaxeojn.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/geoivfokp.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeokjxxx.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gpiywqccd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/goojxdvjq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/ghonmlpgb.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gyiuyxasr.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gqlsglplr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gmmdqobpz.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/guhsvbvom.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gwxreabeh.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gkdofzhov.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gjmfnysjb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwalqwrf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gsprjiwbm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/ghpbolonv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/gcxykugnw.sHtML

[T47] Perl：正则捕获
来源：http://3g.fktsv.cn/Article/details/gayfnnqnc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/gxwuujjqj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjsnyvto.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gvfijjufk.sHtML


<!-- 参考信息 -->