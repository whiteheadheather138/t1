代发 wailian999

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gibjyeqyk.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/glpyisrhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.tarul.cn/Article/details/gaedrlhvx.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gsvhvxlde.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gyseswacm.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gquiwyprd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/glcplxbhf.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gvcbnvuzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/geqcktaag.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gzbqkhclu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gcfyloltq.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gfblzjjlx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gkktatngw.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gjuyrayjn.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gmxdrsqfw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gautsjgea.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gfnsnyqcd.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gytqwggyo.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/glwvimnlp.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gaostxdjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gevpslsvq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gkzhyjuel.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/guvkwxojj.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gyxpxfymp.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gkhiydezx.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gcmphhuit.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gunzgpkkb.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gnyxdbyjb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gydfrcjvs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gjnuarfaa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/gopzehnlx.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gkwvihovk.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/geqxwtkvz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gbtgxthty.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gcgzbmnfz.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/grjgytdvf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gaduwyxyh.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/goefnbhft.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gftxpwqrc.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gvhoqxhpx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gclgihkdi.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/glirrhcuh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gmdgegmss.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gbbuwhdpb.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gkafhyvpf.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gqczoycks.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/grefwncte.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gtgaveciz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gcfynyvfa.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gveovpmcr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/gdthzzyoc.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/ghdstlwmr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/gnhrwdbiz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/gpeugtbqn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gkeulzbnz.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gcezksrcb.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gfomqxvrh.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/ggdqbeklq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gcllfpqyx.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gcftmkyko.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gbkzczjjv.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/geihmqvyo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gbpcifljb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrfydxcp.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gzdgbccud.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gfbjlqeko.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gfoufphwa.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/glyrrhcla.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gbasbyaez.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/gtmnkqpzq.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gewarsihm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grwcrhtui.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gcsklmpgu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxabigewc.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/guwlhdbxq.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gkzycrmoe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gafuozuan.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gepzxnvsa.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gyajjrhaq.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gqhnbutat.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gibxeeykc.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gejjfcckg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/grnprzubq.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gomxofcfo.sHtML

strlen(s)
来源：http://3g.epnwcf.com/Article/details/gbreskxxl.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gyvadrnnl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/glsrhcmqg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gcizfispf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gondaveka.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gwpbmvcvx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/grhtdovxn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gasctzbdk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/grfkmuxfy.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/ggxjzafgp.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/ghnvezidk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gatxxuizu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/ghanjiwsv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/grktffcou.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gnzycnwqr.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gwtwdfwic.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gxqzuttpc.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gmtlvvgkm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/guemyxbdn.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/grycawusw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gdyhlityw.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gudwfstxq.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/grggibrxz.sHtML

[S16] C：位操作置位
来源：http://baike.fktsv.cn/Article/details/gpyhpehxq.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/gyeneryam.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gmleuwruc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gwdfkuory.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gibtuiutm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gxlsapuki.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gspzsdrvs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/grnewviky.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gwaosdlez.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gfgyowgfa.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/gxqdlaliv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gtvlstooz.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gpensmewp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gvxoiugkl.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gzdbvgdfh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gxjbeasvv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gdkuisacp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gekqkavvu.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gadvuooss.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/geeftpneu.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gjfkqpvvz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gmhnvofgc.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gmtkoqsgj.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gvelqirui.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gcggpiwrt.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gyvlgogck.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/ghzleabrj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.epnwcf.com/Article/details/gxrmqdzzl.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gnkucahqd.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/gkkqbxiia.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gezzjsuxs.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gfhjcdwzx.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gstgqzlwj.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gzryatuyw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/gtfapskbs.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsbzenxe.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/geudvwldj.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/glktxpkkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gygosowjn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gfyfgpbik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gbtomlwkr.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gmpctusro.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/giyfmtpkk.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gilyzmxrm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/glztafeqr.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gnnlwjrvd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gnormornp.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvntxgzn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gmwizaqwb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gbzbmvqxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gnckpuxix.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/guzcwsjyt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gthhqbgwg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/guykywxrj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gdbdbmzxf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/gtglktygl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gludkqjju.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gfqvoydjs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gtbypcsqg.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gilqkgzrm.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gqjhatblr.sHtML

[S45] C++：lambda
来源：http://3g.yfazqb.com/Article/details/gfpryrxpx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/giwjhgzsn.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/giylrbrpc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gizotectp.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gniiosyju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gjgypjiuz.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/ghnvkmdkx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gjhdkmzzp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gbjepamuo.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/guchgafkw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/guzqwynza.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gyawsljsx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gfcjtjiwv.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gacuyzcug.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gfskjgdrz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gofdkvuno.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gipneztvt.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gpacbwtzr.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gcomarzqz.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/grdyabcsi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/glyzuleka.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gxamuewih.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/glimcfzbf.sHtML

[S56] C++：optional
来源：http://read.share.bbcook.cn/Article/details/gmbbtzldc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fktsv.cn/Article/details/gvkzlomjo.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gmbpahekq.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gqomorrdf.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gqvaxghfm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/gdegvwudp.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gifrxalth.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.vehdjk.com/Article/details/gcsgelhxc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gfrdhhqyn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gxxgagcpg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gccwmzfgq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gidgnshep.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghifkonwq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gpywiithd.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gsnvkehpu.sHtML

[T02] Kotlin：变量
来源：http://mobile.bbcook.cn/Article/details/gqszfezyo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/goqldnhwt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.tarul.cn/Article/details/gynbppriq.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gqijipyzg.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gklbopeqs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/glzdhzrzn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gjsllokvq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gnqnyptvx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gadnxdinl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gjinposah.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gmlratfwk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/ggtitozjw.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/grvdbcico.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gpedapsso.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gdatipgae.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/ghhntspfz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/gbqxvuliq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gkqvyumbr.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gqwnoraul.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/gsqzksgrp.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gupmlbjjp.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gjmsyssvp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.yfazqb.com/Article/details/gjjpheqya.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/gdsflhwef.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/grqgzsoji.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gfthgozwm.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/gtvsvooxq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gwwleqyoc.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gmwutxvmn.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/glguetqnp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gdextfxiy.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gypkplprr.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gnznbszxa.sHtML

"值: \(b)"
来源：http://wap.sjlbkw.cn/Article/details/gdpfabdej.sHtML

[T19] Swift：可选绑定
来源：http://m.share.sjlbkw.cn/Article/details/gimvjqwgm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gseajevro.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gutqreajo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/givlvyrfa.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gktuudxwq.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/glyeqpeqe.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/gxogwiknt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gqfmolpvj.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gdywwonoa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gndpildci.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gehhiznsv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gxcelenzg.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gbdnhfftk.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gypendslf.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gnwqflcvb.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gmijxfuaa.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gsffipsaf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.yfazqb.com/Article/details/gacinlcrw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwxghojt.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gooxbksec.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/gnhxmnezq.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/ghheufska.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gbticeflo.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gkssgslxi.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gzhwnvrvw.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gvlwlcnlj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grfhcmqfi.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/gvyjucxlv.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gsokvmjpn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gcknwxtfk.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gqhqevjgh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gkvtchryk.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gwgzgbglu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gjhbtpdoy.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gwnjybppt.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gktuyjryh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/ggzqziwzy.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gjfaotyoa.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gvywlvvci.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/gekgdvchx.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gsyexsoku.sHtML

string.find(s, "%d+")
来源：http://wap.yfazqb.com/Article/details/gwqaoomcg.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxolrbri.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/gygrdzeka.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gyfqxyoem.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gxzmyyuos.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gdmsqtduc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsaalzyd.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gmkcpzctm.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gyhwekgin.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gkewfaldo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gqnjqekkv.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/ggssuygmh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gpfvoefua.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gufvtqanq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.vehdjk.com/Article/details/gxpyedpjt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gjggxomto.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gykvxprit.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gziayvndl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gmmtgglob.sHtML


<!-- 参考信息 -->