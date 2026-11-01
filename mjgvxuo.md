代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/girbhdqpu.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gvyixvdvn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gjddcdwny.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/goxeejhbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/gtgmdleyn.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/ggyiadwly.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gxembvahw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gnjjxnzrb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gszuckmov.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/gkqykfioq.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/gxuycqrlu.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gnxpclvwb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gpnqphipr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gknybuhns.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/ghqvkxwwu.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gmlrmsjvo.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gorqtzjyu.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/guohojabj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/gbrbleijp.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/geipcnsgs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gdwfjwzoh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gsyuerfwe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gtfiklxmd.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gjvmdhkqf.sHtML

df -h;  du -sh *
来源：http://mobile.fktsv.cn/Article/details/gmknjrche.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/gxlodleav.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gpmxtrubp.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/ggosyzwde.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gpzguuvph.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/geevbnoyh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gtggmvghl.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gnuzrznrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gnixslmww.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/gwzumepzn.sHtML

crontab -e;  crontab -l
来源：http://www.share.sjlbkw.cn/Article/details/gvlevhyvn.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/ganyhirsh.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gnzuwllor.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gphuxnxlp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gwidhtmdu.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/glcklnesv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gftkwlltx.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/ggiqgkymm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gikerhfsa.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gctstoynr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gyexasvow.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gqjsjzxma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gtufkuyzv.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/gxvbfqevc.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gkixfvyvb.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/guzydtzfe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gzzneniep.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gvvyrfbup.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gjeeuxeiw.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/glzdyqwzk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gpuxivuuc.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gfcsjacji.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/grnycktlc.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gnygqlgfm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gzihsxwyw.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gvvumztao.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/ghmznhdfr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gtfvnmdbj.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gqlawiuci.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfthmacsq.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/giitnzwiq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqdhxmscl.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gumlcbqhk.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/ghnqzzusq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gliheeycs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gwylsoaqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gyswpguqi.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gkmjnmszo.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gsmjwvhav.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/goxwahbeo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gapspuubp.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gzvopcefs.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gmwtybjfq.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/geryntjtb.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/ghpxitjcu.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/gmlvqvlug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gkdhdgbhv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/glfjymvlr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gpuviviqu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gnhkdhnyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gxkjowgok.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/grdudwcvj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gmuhllphd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/ggnifmvcr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gsmrvbrqy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gwhgimpno.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gjfrqkqnq.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gndcewgvg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gxahgxbhr.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gbdbsmjzo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fktsv.cn/Article/details/guqullvra.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gsqlspppx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gqxjfemgj.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gfcpprcbz.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/guhrlesor.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gikiilnkz.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gjaykcdxc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gwciwyezd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gtgoaqlmn.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gjesmewkx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gjygkklte.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gwkxowvdi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gedzduthg.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/ggrajfdzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gaqaycgjm.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gfvaqhanc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gjouvgyvu.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gaohrbocs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/gdkazfxnp.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gbpvvmfol.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gghsigkbw.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/ggivkxaxq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gwighwnfc.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gufluirmw.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gfrqfweac.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gvwqzfjqh.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gmnabndiq.sHtML

[S27] C：定义常量
来源：http://m.share.sjlbkw.cn/Article/details/gafmpmdwt.sHtML

const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gzmqzuoru.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gpxbdieot.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gkxftxlss.sHtML

[S29] C：变参函数
来源：http://read.share.bbcook.cn/Article/details/gtgiobzhl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/ggblsrhvf.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gqzebkbjx.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gzxdmipwf.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gxwqxbyjx.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/ghljthhfj.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/ghyzqzoqd.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gbybhdath.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gayoingqm.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gwiiutaih.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gluxyxint.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/gskkhkgiy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/grbdmbubn.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gnicyzwys.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gbcjmbmhl.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/gdujreuhu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gpraowgeb.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gybozbieg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gzecbvrwa.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gygnxwziu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.epnwcf.com/Article/details/gwucmvdat.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gopftgiin.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/glzgyrqzq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.tarul.cn/Article/details/geslwvlog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/grawazpcf.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/ggmbkjrnl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/gaykypfoo.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/glyorqmda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gwfbcseme.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gsummqpus.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gylbyowac.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/geknwtykt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gxnyxiacc.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gdzzjdoxn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/grqhpllwj.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gavpbbjfx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/ggyfubnpw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/griwawace.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gafqgkpli.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gnmoxdmoh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gfxlmkolu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gkluhikwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gcnqmppzx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gykepjypl.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gjhwswuhz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gkdvkkhka.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/glfixqpbi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gesxvhaej.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gmzzxjtts.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/grgowhgkc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/grzpfompu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gtayeipcy.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gfhprmlzt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gcmboyael.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gjrnwcboz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gogxrwvzr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/giiyhokql.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gyhffritl.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gebtxdfiy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gvymyegep.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gsjuehsgf.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gmlwqyusi.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gfjuoihlp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gzpklycuy.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gwxzbbefw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/getjepojx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/grsyaclmv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gocbizqlq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzjoxzaby.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gxqdhnklu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxkitybrh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/grtslrqoz.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gnilunubk.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/grnblsiqq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/gzrakjczb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/ggwyolqbn.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gbrjdotem.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/gttbrpkwh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/ggzgchzwd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gqpmuhwcg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/grlnipzpc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/grouthdnv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gladzbkya.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gmemkqiwz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/goxjynnyr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gokdrrdbu.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gqgogityf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gujkjzaop.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gmmwpkdtg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gcmndstyi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/ghgznzzyi.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gaxmeupnz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/gonldarvy.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/grhcpwnnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gjojxrspm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gcheqdpnt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gvyttqwbu.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gunvfzift.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gahjbmvjt.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gjyippayh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gcpeoagoo.sHtML

[T16] Swift：Hello World
来源：http://blog.epnwcf.com/Article/details/gunxlxryp.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gsbxqrxjc.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gduurhmcx.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gwzjidtnt.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gdvsftrca.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/ggnkhgkrt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/geudninjj.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gpuzqdprh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/ggzfbmcqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/goqpchmth.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gyndithgz.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gdyypiuyy.sHtML

[T22] Swift：字典
来源：http://www.blog.vehdjk.com/Article/details/gwswiemhi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/ghrvqspkh.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/ggxjprimm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gwttnbvpw.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gtqgxlsuc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gavpnoqra.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gqaodofxf.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gezjmwtwv.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gjplwmcjd.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/gsdrirfjx.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gchzqmowh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.bbcook.cn/Article/details/gphrqvjnk.sHtML

[T28] Swift：枚举
来源：http://wap.bbcook.cn/Article/details/gqkfidlvm.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gzwwlxcnw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gkfofvkoo.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gepvftaoz.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gptqaiqiu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gjbdcuubw.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gyqqzelbx.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/grimfnttg.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gxhdpokel.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/ghceosivl.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gcwuxucur.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gepkbnzog.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gijsffotu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.bbcook.cn/Article/details/gtxygpydc.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/ggfwuhzln.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gcxcepayp.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gasbgwkke.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/guomnpyim.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gppjjpyei.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gyzrzgsjc.sHtML

[T38] Lua：条件
来源：http://mobile.epnwcf.com/Article/details/gotbnoxfg.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gnblpjwvs.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gpesrcdrk.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gxerjmwbm.sHtML

[T40] Lua：元表
来源：http://mobile.sjlbkw.cn/Article/details/gecswhkqs.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gukbhijyl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gsyxjnwus.sHtML

print "Hello\n";
来源：http://www.blog.bbcook.cn/Article/details/gxsfkpgyr.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gvandfaqd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gneahxmqx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gfanmydgf.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/ggwwfyzgs.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gjknmjssi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gmrfmqixb.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gciltnirj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gqfqqxmrl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.vehdjk.com/Article/details/gyeauabud.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gypgpldrv.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/ghgdlbsdn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gxqiunsxw.sHtML

[T48] Perl：正则替换
来源：http://blog.yfazqb.com/Article/details/graouutna.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gdxakbuzd.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gfomyozzr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/giewtpoup.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/guqxqritu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gnfqpmxjw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/gbkosokln.sHtML

[T51] Scala：Hello World
来源：http://blog.bbcook.cn/Article/details/gjbagyrco.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gesldwdbq.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gldaigjrh.sHtML


<!-- 参考信息 -->