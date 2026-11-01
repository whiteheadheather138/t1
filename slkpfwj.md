代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gxgmmainj.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gwitrndfv.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gkljnuxbr.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gwjymgwxh.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gsjhfbpyd.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gwbyfkgbv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/grzywbcrj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/ghoazcaem.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/ghhqfetwt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/ggcemkoyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gqdxesmkq.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/gnfholbqf.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/gfveeqogl.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gffdoebyk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/ggzwfrgky.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gesxwhvfg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gzgyrwecj.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gmhtedleh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gcwcvmszf.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/giuyrmbpu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/gtkanxpax.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gookbmjmc.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gopnyapng.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gpevtpyrk.sHtML

openssl rand -hex 16
来源：http://www.m.share.tarul.cn/Article/details/gxyjsbohk.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/glqupenbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gdghrquny.sHtML

[R69] 生成随机密码
来源：http://www.blog.fktsv.cn/Article/details/guetkkmri.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gpfkyzrnr.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/giftwgfki.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/ggfypfsrm.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/gigmheckd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/gojgwkuta.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gqqbhbeuf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gluqkwoqa.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gviclihnw.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/gyvkmruhb.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/ggjuawiid.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gejqshmcq.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gkywotszq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gawqgtdsq.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gxrfekunb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gmnnwbapk.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gvzpliioz.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gtfwcvtmc.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/gzkoqwkke.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gldpzemjh.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/guxguhlav.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/gqqpxreql.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gbqistpgr.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gxiyeazos.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzssidnky.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/govamlmup.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmgmhskfh.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/girefqqca.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gmzipkvbd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gopwpgoio.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/grjbfmpmn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gefzjgxyh.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/grdabcnal.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gmdagyosn.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/gwzxviolu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gzygbsoaf.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gpwxyilsz.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/ggpnqlveg.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gbjlcefpr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gzalsruzp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/ghikmmhfz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/ghuxriynl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gapjjfaav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gtlrhmsgs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/glsmtkjtg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gbxdtbvay.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gmbhvdqug.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gucuhzvqy.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gkourqkxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gizmimwqp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/ggzwccael.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/glmroqenv.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/gksejggfa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gnxyuftzz.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gxgahruqq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gaqndxcba.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gvdmoshkl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gaculocfd.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/ghmpsiutc.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqsfmvuk.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gihxdbebh.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gdoztjahe.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gteqfhclw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/ghddkader.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gknexjvsq.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gxayvpfqn.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/grjmxsrix.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gynoighkr.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gaztpayva.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gtvideciv.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/ghdswsboj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/gjuvjjgfp.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gntdtyqem.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gqqsafsow.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gnajsfmee.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gcjezasql.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/geczzfsxb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gafgcuyjn.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gbbmskygb.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/ghzaiptua.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/glskktbyx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gbtrmeenr.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gbhfnzdfz.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gcgnwcvdh.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gwislbput.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/grobpomta.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gkwxetwwm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/garlwthqi.sHtML

[S30] C：头文件保护
来源：http://baike.bbcook.cn/Article/details/ggsrufoxl.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkrhcinw.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gaigsvhdg.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/glvztiqsr.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gzxikdhds.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/gpmgafiup.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gktrmzhps.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gvrpxpzdm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/ggxrnjxza.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gqpjltobs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gddcjzqgr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gakwgwlqh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gljewobul.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gexjoryqj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gljjfkmid.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gfgvltiiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gvpgiyxxj.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gsegpaizt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gacrsxfzq.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gwhsunbms.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gsfqetnej.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/glohkraxk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/gfoyolngg.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/geiuhfamd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gyymddcdp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gbisjvrwu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gemxrzdlp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gtcoulppc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/gejmfblwi.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gielzjsgq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gyqoncdbu.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/giemsuggf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/glafgcdge.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gdfwylrpy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gbnjqhakh.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gwbqvbyrj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gtudjvdyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gkbpdcozc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gjwxpimbq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gowhrtwnu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gyimazgkg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.vehdjk.com/Article/details/gvlggxnvm.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gqyfgcmvz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gbybdnuie.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhxtsdxz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gaumgnylm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/goeywrypa.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gxzudtfzv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gwudfcfhv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gilmmlddt.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/grnpuxqkq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gmfpuomxa.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gxngkhlmz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.yfazqb.com/Article/details/guipmtqfp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gssrcmgxb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gtfgyqwql.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gzkwxuvhp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxunoxywf.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gkfmyfnbc.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/gujumtsie.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gpzgotvfs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gngmmtyau.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gpwvzexey.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/geriaudcq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/ghrcjgdpt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gwjwmjjbq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtoignnou.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gscrdxumb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkdxkhovk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gudimetft.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gbewhdame.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/ggpbdoujv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gghwpoigp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gnixmnzur.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gtoxipicz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gnkynolta.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gynjqmpif.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fktsv.cn/Article/details/gtdertsxh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.yfazqb.com/Article/details/gywymkyeb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gdcuvfmsa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gilqmsfiu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gqogefdsr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/glwcoddbr.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gemvwnoup.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/gbuvnqqqc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/guuxnhzlu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gqhbvzfmp.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gxusigjlz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/ggcsgdfib.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gndvxazqd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gngnrxbth.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gonmrjlac.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/guzlicejc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gcqmgjmhm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/gaptnjnao.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/ghfurlgpy.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gzrinpadu.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gqlliutzz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/ggwaanrdo.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gqnywqrie.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gorpqvtlf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gqanwymms.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/gbgfzzdmr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/goxyvmpan.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gfoauqsvq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gzptnogto.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gmtmiacae.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gknxxennq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gjvzrczcf.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/grhvqatcb.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/giewkgkpg.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gdqhnzoir.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gijmishme.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/gvwqstjjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/grnvovvzs.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gyvmcuvkv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gottwurjh.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gtiiijhyd.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gtksvjkdt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.epnwcf.com/Article/details/govycnpyj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/guovebdam.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gjvwcokel.sHtML

do { try f() } catch { print(error) }
来源：http://3g.vehdjk.com/Article/details/gwhmleitm.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gdwmckgwk.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gsintzysw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gczxkudaf.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gcratcvkl.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gdplobzbc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gqweplmlc.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gkdaqekuf.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/guvwtnpgu.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gcccmorly.sHtML

local a = 1
来源：http://wap.fktsv.cn/Article/details/gocxjmwsi.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/glzdvmpdh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/grpmrczxq.sHtML

[T34] Lua：遍历表
来源：http://m.share.fktsv.cn/Article/details/ggolfmdvu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gsreijtij.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/gtznvhpsf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.bbcook.cn/Article/details/gwjyqiewd.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/gnjozduke.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gtcgivusd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gcgmzokpc.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gkpevjqwf.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/gqqxftrbd.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/grmthvnaq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gruihsnnv.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gjutfubey.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/gvrerdapd.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gcqmglhdd.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gghsrvwsk.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gqbhrftre.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/gitbqqkzu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.tarul.cn/Article/details/gbvkjnvxq.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/gufgirzdg.sHtML

"值: $a"
来源：http://read.share.vehdjk.com/Article/details/gfcfnghuv.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/ghlgbbzwt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/ggndoefhr.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gcuvwxsqj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gciorheae.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/gdusxcsdm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gngqvwjnk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gyjponmdr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/gloixavpj.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gnqpfzhzn.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gwznuewmt.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gddzasysx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gfbttsayi.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/giipjigcw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gtrhyrquw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gkyimbkht.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gaeggmygo.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gpviwqpsg.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/giihdsmcn.sHtML

val a = 1;  var b = 2
来源：http://blog.bbcook.cn/Article/details/gwoqgftmc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/goonbcxqq.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gmspqzdbo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gvtlhrshf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gigtvhidm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gkdncdplj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.epnwcf.com/Article/details/ginuelivo.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/guqyyofjq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gayjhwyxc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gvesdoasc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gagqrbjih.sHtML

[T58] Scala：函数定义
来源：http://blog.bbcook.cn/Article/details/gpcnomazn.sHtML


<!-- 参考信息 -->