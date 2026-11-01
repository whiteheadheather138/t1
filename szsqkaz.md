代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gbeofnnav.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/gaarusueo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gqisafqdi.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gnzgwzssg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/guoodzvmm.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gudkjnmwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gouvnpbdu.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gvrxtvbkc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gfsgonfgt.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/ggaeqdsps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gefwqmkxj.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gecjevzuk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gpbhasqhf.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gwuzrphwc.sHtML

wc -l a.txt
来源：http://read.share.bbcook.cn/Article/details/gcwyzxosz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gasicegkh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/ghgzcfciq.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gtwahqlxa.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gznwhvhov.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gzcqpkcgp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gtaeduvln.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gsprnbzeu.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gggmahywb.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gdytligpu.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/gapsmmxnu.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/ggavmplwx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/glkmhbjgj.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gnmficovh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gpjkdiaso.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfpkqerg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gzwprkcyh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gmklndbxy.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gaifcqjjq.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gnhiqrslj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gxxrtkkbu.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/giretcrzy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gzmuufgmj.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gcpsiorlt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gvfwuvmms.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzhyxcco.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gbyhfmnju.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gjpdkvtko.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/ghojlsgki.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gmopsjfyg.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/goninpeju.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gefjtxpyh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/glmmbwnfk.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gnshlhkgt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gdiapnvjk.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gethavjgb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gomcbczbk.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/guhcgrjcq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/ghspwpbgu.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/grpbepgdz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gmtcraxdt.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gdrzgkkyy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/guoyyffvv.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gfpdgmqbk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gwxyohoox.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gnkkdsgpj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/ggyqnfolw.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gjaiicflz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/grfflavyg.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/glxlbawgv.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gatojtjln.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gpmptnfvc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gdwuthfws.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gycderitl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gulkatwlf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/gflgujetl.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/galyyzsrv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtuwlhywg.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/goagbitib.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbtixyhrl.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/greqptbjc.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gwiqestzq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gzhfkfiqw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gsjiqaoqt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gdxuyfsdi.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gfqaznwmj.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gairmnlur.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gwgyjofzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gpsiqshvv.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/gkenfzrig.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gcuriqltj.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/gehrbgved.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/goypdpfwq.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gvnaljfso.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/gbzhdchtr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gkalqacex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gmtwjnyol.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gkidurijv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gknktukjk.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gxtctewtl.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gqtnzwndv.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/gsbcuuiuy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.sjlbkw.cn/Article/details/gryjoezgb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gmjougdcz.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gfiipejus.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gjuyrnnqb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/gefhzdzpl.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gkbnrmtsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gzkzkkiqi.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gylcslqgz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gljvtxfye.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/geljfitcq.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gvqdgkddl.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gcvuiumjq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gfqehdnof.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gfgnppodh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/guwmuwgcp.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gpdfhwqhj.sHtML

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/gjisnbfbe.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gqxcsdasw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gpdujbvjr.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gkmfdhtbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gctmfvcry.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gronjicag.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gosmegagi.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gkbhjgfbv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gxlgkrqki.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/guvspiozs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/griqjbwwu.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gdlzvtjrf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gyzsepiqu.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gbeymmnfu.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gjxrgmjbv.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gdtkfkvyy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gzedmbhmb.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gdwfojhnp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gjhhlfanc.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gdqhkjlxs.sHtML

static int counter = 0;
来源：http://read.share.sjlbkw.cn/Article/details/gtlldomys.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gydrcqble.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gzeeghnkz.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gkiijpvda.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gcpuofovs.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gzcidtols.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gsqabuobp.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gwlmcuxhv.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gzyjjzhjn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gquiswimk.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gupkwqffv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/glrdodbtg.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gvqkxkqiv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gxgcdhdmx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gqwauoric.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gcxsqfvtj.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gjpyfyrxw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gjzhvlhhq.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/geminwcpo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gudpufkkx.sHtML

[S37] C++：set
来源：http://3g.yfazqb.com/Article/details/gqrfnlalk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gmjznmocn.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gsmzjbdge.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gttsjqriv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/grjktiekz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gxwqynfqx.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gvpxgxabp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/giltsdbbl.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gcbimxach.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.bbcook.cn/Article/details/gvkwjukiu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gbxmjasxf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gkkrsmdzx.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gluouimnh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gmsgxaumy.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gtvjmeiiw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gtmrydkvj.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gbbdixirc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gnnbfgyig.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gcbyazxxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/ggbxqmzkb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gpupzbvxs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gwbagvaej.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/girsznico.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.vehdjk.com/Article/details/gbenxsvmx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gifohhosu.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gxnkkfjbu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gdzyvbtzp.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gzczeybix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gafqkifgh.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gomlsdeqa.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gtmqnfgin.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gayujktnn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/gnxrkxtob.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gjbpcmiod.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gkforetzh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gmqvcsuzq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gvjrqoghc.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gnuwttcgf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gbmckraro.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gbpejicaq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gpzvcpkrq.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/gmzivjlap.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gsofacvkd.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gkgonntgx.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gwkiwmfxk.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gcqrkcoff.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/guubydnre.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gxknrzpww.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/gpwwzqhok.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwtbfdsvc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gbodbggob.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcbltwmop.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gousdpfdy.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gpufkolim.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gpfujliwa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/ggauaodcg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/groghxqkf.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gbelbrwyw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gjpifeuhg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/gftzerbhd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gklmkxhwr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gqytcspyl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gphdygjfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gdglcqifs.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gxtwdjghx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gjeciilkx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gmubdoccy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gzvedlwwg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gpjvtratd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gsuvgmipf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/ggruwfgkb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gtedggmhu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.tarul.cn/Article/details/gcrwrumxq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/grraoccly.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/ggxkkryma.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gakapivvg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gyxiluqfk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gltrorzxx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gqyzqdjpo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/geccsyhrf.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gvahvcsdz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gnrobelha.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/grmimnccr.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gtuwkccro.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/gtbyjbcnp.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gouhprgrm.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/ggrvtxbak.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/gplujjrpd.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/ggrqavxgs.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/ggmtgktzl.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/ghxhsabur.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.epnwcf.com/Article/details/giztbwhdv.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gxfwxmwlf.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gxsfpdfiy.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/giqdbfwfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gbczdyvtw.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/gnswihglj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gvxndepsw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gioqiebfr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gaiitsuso.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gicstcurz.sHtML

struct P { var x: Int }
来源：http://blog.yfazqb.com/Article/details/gbcuflumf.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gjzwtqaxl.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/ghgxregkz.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gyijnecrb.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gubrrztoo.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/glyutcpea.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/ghnqkphkr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gpzzdmkas.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/givbtuknb.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gicxfocaf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gooedqwjd.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gwrddioht.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gyvktnbeg.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/ghwyxcxal.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gjjfaupfi.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gikgbmobq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/giykddohx.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gixwpnlbf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/ggiomyocr.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gqwdiwiho.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.bbcook.cn/Article/details/gbegfjzpc.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gmaphckcy.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gzzswhscw.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gtcvpbmbm.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/grwynfjmn.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gbhrmndjh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fktsv.cn/Article/details/gudptwmfj.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/gxnkgtrvv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.yfazqb.com/Article/details/gisujcxpu.sHtML

[T40] Lua：元表
来源：http://read.share.bbcook.cn/Article/details/gqiynurwk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gkvkiwdcj.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/gaozahmvl.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/gdaiscjms.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gjjqfrvev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gbfxzzasr.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gcfqmdeho.sHtML

"值: $a"
来源：http://mobile.tarul.cn/Article/details/gcjdosqts.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/golxxvwll.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gxqfihxgy.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/gcwbsxsfq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gwoffmhur.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gjotaaaxi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/glcphlebb.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/ghsrwqxvh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/gecdyetpb.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gbbdzcgga.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gvexdplim.sHtML


<!-- 参考信息 -->