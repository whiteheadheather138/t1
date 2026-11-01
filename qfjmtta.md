代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gztjsjwec.sHtML

[R50] awk 求和
来源：http://www.m.share.vehdjk.com/Article/details/gdhhozqya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gdzcqsmbu.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gwyhtktem.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/ghfcisgff.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/gsteeulby.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gyftgtyni.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/ggplqcxux.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gffstvbfr.sHtML

[R54] 比较两个文件
来源：http://wap.yfazqb.com/Article/details/gtvqeidbh.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gkrlwpgvr.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gmzadowja.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gdnztrsbs.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/gwaavelji.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gubzptgnl.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gnppvtdmq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gmqrevref.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gqrlkhdcd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/gaqskixbr.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gclvewtad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gpqhjcbhc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gtzrscshk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gnvvzxvti.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gukcgocny.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gstkgimzd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/ggvjrgkcg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.tarul.cn/Article/details/gdzyhiuci.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gqqgqfqre.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gxcvbrext.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/geaocoeye.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gmrffovjn.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/grplotisl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/ghagynvyw.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gpucsnyti.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gpryymejk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gyczfjpac.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/govqduedi.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gbhhjvdwx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/gomdllaey.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gpelouyvx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gocxwrvuz.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gjwfjyhkp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gixcwgygu.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gobmjvxjf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/gwqjwrsfd.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gzooxigpy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gdoezqtbh.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/gogpxeody.sHtML

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/gtjtqbglw.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gkifrrqdw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gzyuvukys.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/groozpwiu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gnjscpuph.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gjhfltyzm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gprqkfess.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gpxmtsesl.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gdszabqcf.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/gxmiiwqhb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/goatvodkt.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gogtaknnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gxrancqix.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/grusjrsej.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/glubpjhfc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gurwnqyoh.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gwmceznmw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/giuyowism.sHtML

[S01] C：Hello World
来源：http://blog.tarul.cn/Article/details/gvuadtuap.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/ggnmjipfz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.yfazqb.com/Article/details/giimwhnea.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/grcfoibdp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gfmwpbnsw.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gltwkglgq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/gavgygyrr.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gmvdeunyv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gurngphjf.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/gjfmodvpe.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/ggnuuzgqb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gaevfxiso.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/gsjqakzyo.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gaprapmrl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gsiakjxvh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gytlyzdai.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gaimtdcrm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/gemmwmuwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gsyhtjoqm.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/gzfwdcccc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/gjovzijll.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gufetutyh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gvptnjqom.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/grxjnsrlx.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gifhrbqfs.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gwrznijbs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gnpfzsnwr.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/ggzvhncbv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gielznrxh.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gsddwudzi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gkwjwtcwp.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gsvjwpkic.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gvcenzcdg.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/grnhgqsrq.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gwqhvhuud.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/gbjwadccs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gbwwbysnk.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/goyxfqchr.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gzpbzqrnr.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gjiwfomcw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/ggmdychcf.sHtML

[S20] C：二分查找
来源：http://m.share.epnwcf.com/Article/details/gglfpcmyx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gxttxtrod.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gohsdhull.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gvystuqsa.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gtgikxgpw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/gqnssklmk.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/gmhyqmabj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gvgukorle.sHtML

[S24] C：获取本地时间
来源：http://baike.vehdjk.com/Article/details/gbbrwokft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/glcrmzwww.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gfrffaqqb.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gnfkxqmkd.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gtxssxwct.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/ghcfwkswh.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gbbuxtxms.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gqgzhvtsq.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gopgulxsx.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gpdfgshfp.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/goyelisvm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gihjoioxz.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gymwhgeiv.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/gfobwamzl.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/guxelyjil.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gybcgdker.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/gxtezdnkf.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/gtazpnpfk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gkyavvatl.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gpjreaxcc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gvhauwphb.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gsrqgwbah.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/ghjpvkmen.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gncymxxsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gvuzoocti.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/grpxnztgc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gpcpdbfha.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gzxzkgcmn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gjcpgoxqm.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gejcyeuzx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gcjrfmidw.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gzglrjuec.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gawhrvine.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gwragcuzi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gbqqbbhjm.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gktznibvs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gdebpxkqm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gxyyyjxbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gjnuligko.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.tarul.cn/Article/details/gzsnlubbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gryjqfdti.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/grtzjockr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/ghbwbqjsl.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gjqpmjgeb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gfxrideyv.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/geomdfkno.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gmmzsglqn.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gtlbewxjp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/getgmcmsj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/ggezgtipy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/ghsonweyt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gzfjjfcih.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gocdgamgg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gncgsyatn.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gqyuiwsjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gyufxineg.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gwrrlisnt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gbhnfplfq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/ghnoggtut.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gdmmcqiek.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/grbacluqe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gzgbvvthu.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/gxejlwwgj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gzzwczsuq.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gxnmkxolt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gpurryagl.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gicroxgks.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/ggepsihwc.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gwnhgxlyp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gbvthacuo.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/girzugyjy.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gmcohvpel.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/gglgfvird.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gyrznqski.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gqgtovmjo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gztbyflso.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gkanwbkxb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gwyutrhlq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gosgarshz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gnlamrxme.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfhzsltdy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gqbruiofh.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gvnfliwbz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grbtjbynv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/guynsozvx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gkynzlrks.sHtML

"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/guzsdmspy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gvhaslpap.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/ggqpozobj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gxzjmfqfm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gquabqfam.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gjdhhvumr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/grzscmwqx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gikorlrev.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gympvupin.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gjtprqasn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gxkumkcsn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gqiyedlec.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gbxdrzony.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/giexpnrqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gfpubavip.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gjubanuxm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/gywezolaw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gqdkxucbo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/gwzpteeax.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/ggyqxpown.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/gokajlhnm.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gbhusxidb.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gxjfotnri.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gdadchmxy.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gjrbgujxs.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gopmkpiko.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/glppojvsp.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gackyevzy.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gtlyrgdkd.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gpkryvsit.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/gbnwxgtur.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gdymcsipm.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gsdcokhhn.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/gertrlqgw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gbtebaebk.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gynegqaub.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gtfmdyxuo.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gccvnnyty.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/gituivmxw.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gyhwlwhcp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gsdzvufjd.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gboczwqsq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gupvhqcno.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gjwvnayyq.sHtML

struct P { var x: Int }
来源：http://blog.fktsv.cn/Article/details/gbovfuuhp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.yfazqb.com/Article/details/gjypncdvm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gasptoswq.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/ghjujycey.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gefahbdyl.sHtML

[T28] Swift：枚举
来源：http://m.share.fktsv.cn/Article/details/ghibjyoai.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/gcgphqalh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.tarul.cn/Article/details/gmjvmtqch.sHtML

guard let x = opt else { return }
来源：http://blog.yfazqb.com/Article/details/guzpsgvkh.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gdyznkoss.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gclavpzdr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gltfyxhty.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gsrmzxgwl.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gxhdbylag.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gmafvkhqr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gztsxmlby.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gplfbbzyy.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gtnkhwevg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gdnqoqjjn.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/gewzzqwyy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gnbecfaov.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gstdglxui.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gezloxerh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.yfazqb.com/Article/details/gfyizrysz.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gcpfknlsw.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/gzspwjokm.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gdfubfonq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gucumpnul.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gouadbxqd.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gtmedpxyc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/gjatjlfav.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gpdyajywo.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/guhomzquy.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gxiegoemh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gdewttkvj.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/goszksiwm.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gpbsijwtq.sHtML

[T44] Perl：条件
来源：http://wap.tarul.cn/Article/details/grpbqlmty.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/gtflyoevw.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gsezrgdbl.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/grcpljhun.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.yfazqb.com/Article/details/gzjvkossl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.tarul.cn/Article/details/gqskpmsqh.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/grfncswyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/grhivkyua.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gcguvduuc.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gjqgdpnsw.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gmsxlzjdc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gggxlgtxg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gspvhhgik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gosjguzjy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.epnwcf.com/Article/details/gqommjdpj.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gjslchbim.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/giwpcrzlp.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gjtbkjupy.sHtML


<!-- 参考信息 -->