代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gxltjheut.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gpivantpl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/ggrqxqfwb.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gnmpdgcff.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/gwfedyrgc.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gsnpmfkks.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gknrhfrul.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/ggrlmkfkj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gmehotgjk.sHtML

[R54] 比较两个文件
来源：http://wap.bbcook.cn/Article/details/gaoweqnqv.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/giwalsvyv.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gvsgqysei.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gdgbzgwbk.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gyyeiadtf.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gbnjaxzsi.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gtmtfqsxw.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gqwdrlitc.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gayoszedf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/geypmvzxv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gvfsagxex.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gbjunatas.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gskzyzxer.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gjktgvzjz.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/glnrezzgg.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gfamhizxw.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gomjkhrum.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/ghmethnhb.sHtML

[R63] 内存与进程
来源：http://www.m.share.vehdjk.com/Article/details/gpfrjtxae.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/gdubsdrrs.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gusmqzmmq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gjhgsnceu.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gnxsihbli.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/ghxdrtgqb.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/grfhiwleb.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/glwzyhwce.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gdzrrkdrh.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gjnvoloxi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/gfddsfnbm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gnithdqsq.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/godawucwx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/glwfioniu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/gnvezsdrw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gcxaynule.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gmebeeqys.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/gtqesndbd.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gszdbmrho.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gweuhnjan.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gwlhpudpw.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gabmvnjvw.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gpdcshktk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gidhzstxy.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/ggljfecys.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxjzyaul.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/gjinthchn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/glzgspuuk.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gvtzkxaoy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gvbmnrlnw.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gajaeynyl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gyssceutf.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gjniznnvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gwsdxtxlq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/ggnnwihvz.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gylttoccd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzzmqxaib.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gbibpdsyk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpsrjjhvc.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gegusmshs.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/ggvprudcu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gsxktkvtm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/geffngmey.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gmjtfzfcv.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/gukhjmsbf.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/gvwnxfvvl.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gesdauziy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/goxzfhyax.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gtpgsrdfa.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gorgdqjbl.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gyvsfclwt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gquykobpu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gxnfalfon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gehjkcnww.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.epnwcf.com/Article/details/gzvnvsbzn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gkralttxb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gaoipuldp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gepjisovj.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gblbptfxt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/giadodzub.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gdraovaxz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gfltncvvx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gnaljnjzq.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gbluriuor.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gvrgnljyr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gaeiwivkn.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gmuxrjhkb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gypbqnsda.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gnunescis.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gkgshnnio.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gyzmitaby.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/gmlhadwqt.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gulropxab.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gxwzrzlkj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gvjpdhhgv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gxlcrdegb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gzcvstnmk.sHtML

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/gogkqqpgo.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/gzzgdaknx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/ggoxqhyly.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gvalselfc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/grnihpgma.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gtaopgdic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.bbcook.cn/Article/details/gybuwakmp.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gyxestyom.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.vehdjk.com/Article/details/gcbrycrux.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gxsxnueyv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gveeqlgyd.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/gwcvidphr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gwhomxyre.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gglbforfe.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gtquztyoh.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gysrshqgr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gtxhtvcuq.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gpupndfyo.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gtlklyppp.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/ghcripuff.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/glysudfhm.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/grukvyzjp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/ggojpqpzu.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gmbpdwipr.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gdthwvxdv.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/grpnbrzwk.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gyuwhgylc.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gavrboxos.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/gccwndysn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gqpxfqkbf.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gxahzguwc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/geuqqgfwq.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gfyqcdevq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/gopcxjvmb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gurjcxmsp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gcsfbfrir.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/gvizbbgpk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gozdchlzj.sHtML

[S36] C++：unordered_map
来源：http://mobile.tarul.cn/Article/details/girjxnjdk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/geeyetgmt.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gsnhmikhz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gqwnzjfsd.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gnsqzhpfu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/gvqpqrrhd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gidzoulfm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gyhxnyxmg.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gczhfhbgb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gcdalxnex.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gdpkrsigk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.vehdjk.com/Article/details/ghyhqyfok.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gwcvttnyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gwlpyrpye.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gojoifhec.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gsixoulkv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gspkpdxsx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gmsgykpwx.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gnlcuqndq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gwwemvbxu.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gncrjvvxk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gofdimnkk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gsnrmunys.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gquazbsjz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gsihjhvvu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gifdnkzjw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gupagydum.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gvafaiiqg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gvkzcasds.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gtkqtfixv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gnkiicvlc.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gkytvnflb.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gixvpoxvk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/ghwrpmrip.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gcnzmswkx.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gtqilafiu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/grmadftqw.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gsajcdbiv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gckbouwec.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/grlafnisq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gxtzpqjqk.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gyuusonhd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gutgvnwnw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gkzxjbrix.sHtML

constexpr int N = 10;
来源：http://mobile.bbcook.cn/Article/details/gkaghssnv.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gypvmthyh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/geudihtwj.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gwkwdoccx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/goysgtftk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gyzfdkzpc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/grcrlcbnk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsykgobbz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gdfoavfya.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grhhoujml.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gjblrnuhl.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gchzqvevo.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gimpjyqfp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gruvwswcx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gnjykjnpr.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gkpqjmcbs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fktsv.cn/Article/details/gmqctkqwk.sHtML

val n: String? = null;  n?.length
来源：http://3g.yfazqb.com/Article/details/guxphslky.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/geyhnzbka.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gjojbdjtu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gntcnamwg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/gfumkqzhf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gmhulvtic.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gdbvjxhnc.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gxvtnmgwp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/gfkuikuty.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gffehsscf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/ghfnandct.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gzkrytzbd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gmbhervhg.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gohtbkbmq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gxnvqwfdl.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gqklwnfdx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gaufkbcyd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gepujdxes.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/gvgibqxph.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gfveandzj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gwguiqlym.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/gaxrbarts.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gcicqbjwl.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gptcwzcpj.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/grixlqygi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/glebqtitw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/gpbkxffdj.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gojmtxkek.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/glwykksdu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gunwsiqsy.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gbvhmpvbo.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gaxotkmbn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gertgtrzt.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gboyxkeie.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gusqbnpla.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gqmpmlrlq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/giihrhuby.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/gjduuzgmo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/grnvaofbv.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/gtxbtfkwj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gjegmicyj.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gcyuqxvsp.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/gjdvlperr.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gcwzsatau.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/gpwqtmcva.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gejrjkzyt.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gqtnycafr.sHtML

[T28] Swift：枚举
来源：http://www.blog.bbcook.cn/Article/details/gzropxekx.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/gbzwltlvr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/grrgrxgao.sHtML

guard let x = opt else { return }
来源：http://m.share.vehdjk.com/Article/details/gqamqlftg.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/goekalbsk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gjrdrrdzr.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gvtaqtvaz.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gvufsedqm.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/gcaajscuc.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gfmybmorw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.sjlbkw.cn/Article/details/gcaqeykld.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/gbcszxgin.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gejzhrxil.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/gsfdupbcf.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/ggozybykt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gpgymgpft.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gmarfsjkk.sHtML

function add(a, b) return a + b end
来源：http://3g.epnwcf.com/Article/details/gpinkrjpe.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gvsuplvty.sHtML

"a" .. "b"
来源：http://baike.sjlbkw.cn/Article/details/guvlgjxes.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gkhaddmbv.sHtML

if x > 0 then print("正") end
来源：http://wap.sjlbkw.cn/Article/details/gsngdzrww.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gpbputiuj.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/gwhuyyobl.sHtML

[T40] Lua：元表
来源：http://3g.epnwcf.com/Article/details/gwlsmxsra.sHtML

setmetatable({}, { __index = base })
来源：http://blog.bbcook.cn/Article/details/gpfekfedt.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gzfqfzqpy.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gerbfnsdm.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/gwcvefufi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/glmzksepy.sHtML

[T43] Perl：字符串插值
来源：http://baike.vehdjk.com/Article/details/gougjfaer.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gimyjcjcj.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/glltkaevd.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fktsv.cn/Article/details/gmaponkkn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/gkntkozyf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fktsv.cn/Article/details/gabkvqiru.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gkaoahkbe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gicnmpymp.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gaqlfzour.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/gffopxydn.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gdikdtjmx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gyjxqeeoi.sHtML

[T49] Perl：函数
来源：http://baike.fktsv.cn/Article/details/gpdeogwmu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/giczvgjyq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gvptrrkco.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.epnwcf.com/Article/details/gemavmzob.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gtfpfygug.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gnuyzsian.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gczsmzuvs.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/ggdrsnhcg.sHtML


<!-- 参考信息 -->