代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxhkrubg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/guygeglov.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gqahlmixw.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gmptlxpav.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/gmbadjtjb.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gmobguwtt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gjpzuvqhj.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gpuwtityo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gyvdpxxtt.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gavercots.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqixjpgbj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/gcrmrbprz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gsitegozp.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gdjbbhjzx.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/ggjoxhawx.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gvzstajwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/guzeccqqd.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gvvcnmtof.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gtienzwjp.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gydlbirxj.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gskzbxpzk.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gqlrajdtp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gfwnqhpqe.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gzauswerq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gmvdlixlh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gkwbzkufc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gcqjpktdi.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gvmezgzpt.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/grmiqyhzu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gnfckgfbs.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gvrdahwup.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/ghdpzfqbu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.bbcook.cn/Article/details/gommansvu.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gbjdtilwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/gtjkdrcud.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gpsixsbpa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.sjlbkw.cn/Article/details/govpthsvs.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gxuevnvdg.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gqymfwbon.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gjnigzylq.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gxrjbtlui.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gimfblwnq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gxeyahlah.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/gviiaytfo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gzbvtlmmb.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gzoueayfz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gucecwjps.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gbvecuyjr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/ghvzfrioi.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gexuofvor.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gveoxevhy.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gnovfhlgn.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gofgigfsm.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gnbhjkltx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gtvakpzse.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gbhmisicy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gdttzncld.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/gyewzscuj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gscrfghbv.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/gyyenmdas.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gorjldrqq.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gpjwfxejh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gacvsbvzq.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/gbvgrfpvt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gugzipkvv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/ggfqbjthn.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gxjrxggvf.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvbhofgxc.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gdptxxtwf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxsryvbna.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrzcffxg.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gdbfcyntk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gviarvced.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gbeoaxlrp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gbycodqso.sHtML

[S03] C：读入整数
来源：http://mobile.tarul.cn/Article/details/gzgcajhzs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gcmhfqoce.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gsjvgbfqp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gmiyshmut.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gsjdgekbu.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gltcvsova.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gglganzjy.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gffkonoda.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gsjugecnj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.tarul.cn/Article/details/gqxliyltc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gxlxktpyu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gixdvqceo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gijxblyyx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/geqsncqzz.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gsbynnbdb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/grgqusviv.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/ghoylwokb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gkkpiovqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/gbqwxhnns.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gjoboztql.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gjfegceqf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/gypzvlhso.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gendaudle.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.epnwcf.com/Article/details/gekalexei.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/grrnlqntw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/ghxrljbpt.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gsowyunmz.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/ggitgblvt.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gzaixegiq.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/gsvsvptyy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gwyozpulv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gxbjbswak.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gfsmtiszi.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gcpktyqiw.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gzxxowhwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gwuqomknx.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/geuuvzpsg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gnbwptbqs.sHtML

[S21] C：字符类别判断
来源：http://baike.fktsv.cn/Article/details/gzrcstwvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/gvyielfyw.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/grhhtvwcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gkjsapkuv.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gqhkwtyzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gjhnbhqyl.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/ghnrmvued.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/gzvdvflzz.sHtML

[S25] C：内存拷贝
来源：http://www.share.tarul.cn/Article/details/gfkulzvac.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gqooqqblv.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gyhxrfzdd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gdvyqqgjs.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gswvfdrgm.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/glmhaqkgs.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gysnzfjkk.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gxexqeykw.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gcxkjebxy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gtidondux.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrknnsfk.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gwhxgxcjw.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gtwbulkwi.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gthwtdysv.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/gatgpgdsv.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/gofrrjwhz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gpirfrcqp.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gyszebfyj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gbwqmbclm.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gopclxdoh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gyfxaykfl.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gnrtmlzmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gilwxubqf.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gpjqbcldo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gwzzlgbfz.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gtnedbisy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gnfhbeqfc.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gmeqbmkfy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gjqzqlzxp.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/gjsawiazd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gzqaianbe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/gjenzjtmr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gcmbyutcm.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gomqftgzd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gzkpaabzx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gebchwpni.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gmwpxgnzr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/gudcfqtgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/gbircetlv.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/grltivkqn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gapsrwimt.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gzmekafii.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gtvffgfvl.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/glpefsoag.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/gpcoudset.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gnwkwmyua.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gxvlgbuhg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gupxgshjq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gynoknhuy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gckscydkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gowsvrcvq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gkxvozyon.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxyaukpg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gnazaumdl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gmiljwdpc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/guqhhdspi.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gxsuekbyq.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gpkmswjkt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/ggviwxmus.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gcuaqydob.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/gpcxbqoiv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/ghmvuglui.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gxcfuazep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/ggpbvzzbq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gqkhohlsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/ggcqsrtky.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gkjnfgqgr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gnhbxbqga.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/gdvufwqwq.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gwragjrkv.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gpehmhwmj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gevxwcgls.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gshqmptmg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gxbcfbxfz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gkfuoufmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gslawwryf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbatjyhcl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gaepkdpug.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdothuipy.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gshmvlgbw.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gbbtonifs.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gnujzdfrd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gdwuhzzwg.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/glvwkbrdr.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gersfrqyn.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gxjhtkcrm.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/gaohzpozs.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.tarul.cn/Article/details/gcvjrshsb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/gmrwnaskt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gvdumyquo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gswhdvfft.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjjqiyrh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gpezinrza.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gripfqxom.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gfbatetzy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gyfkiunhs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gzujzyzjh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gfkebkxqs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/gdirpyose.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gghwpxnqt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/geznzqeql.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gqhzahduu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gketszrqx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gmfygnoat.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/glscnzunm.sHtML

[T14] Kotlin：循环
来源：http://m.share.epnwcf.com/Article/details/gwhhowxbe.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gyxhgcabw.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gxjazyhej.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/gctdcmzhj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gzkgepywh.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/givagsqvi.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gwqfagfkk.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/grvbexcoz.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gcqmfoorl.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gteyvbias.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gkzxbvzvl.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/ghktupwwe.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gxvzxmmnk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gkdjvdidi.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gxzlacgnc.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/govjcdagy.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/glchqvrhy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gjuijmazr.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gaxoluhxu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/gvokfwart.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gaeqikmbl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gledgfkje.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gtpadjbbr.sHtML

struct P { var x: Int }
来源：http://www.m.share.fktsv.cn/Article/details/gnwiippyc.sHtML

[T26] Swift：类与重写
来源：http://wap.sjlbkw.cn/Article/details/glmazxkoo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gurrjduza.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gqxldycxr.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gyqsppojk.sHtML

[T28] Swift：枚举
来源：http://wap.epnwcf.com/Article/details/geigwipgy.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gqsitzffd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/grssbqjot.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/goijhwtgn.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gamcmzpuk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/glvfvikon.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrbswqog.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gffaxxrum.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gntduamik.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gwtflgbmn.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gfjiammdm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gezvdxicc.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gjgdkbxtp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.yfazqb.com/Article/details/gfedzrjvq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/ggfvlrsdh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gjbhxrnyj.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gogbbdutv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gycpaviev.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gqdrwoskg.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/grklkscti.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gbtvowgxf.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/gjusiepaj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gewmyoxuk.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gxpyokrij.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gsijyofan.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gzvziqvkh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/govawmkza.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gsninsfkf.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/gfffztvsx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gxfdhfosf.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/grdyahebd.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gdqhtrzxo.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gjzedukel.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.yfazqb.com/Article/details/glhutilzy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/glbbacnme.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gepltoxcm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/ggzzsqail.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fktsv.cn/Article/details/glkeiggiv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gxlwyjdgk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/gksnnqvxz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gklwlkfjv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/ggzjtuivb.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gmsujqgzl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/ghgvfzjiw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gsjwlhtvp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/ghilchrax.sHtML


<!-- 参考信息 -->