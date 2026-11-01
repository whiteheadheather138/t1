代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gsqtubwor.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gbsmipzsi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gfepgxkmb.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gsazsnbwa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gsdynmsyl.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gyrnqcikm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gxecjdpqj.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/ghncdwgdn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gfwwxuowc.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gnaxnqlfa.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/geyjnbrmr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gbbjkftjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gclebhqmu.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gctsrmvwq.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/glsushfgr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdpmfcyi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gvwygslhg.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/grzlspllp.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gcyoznjzf.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/grfjdmldm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/geufjdmrf.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gczeycsip.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gkkjsqpnt.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/ghbedxtbx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gjublnkee.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gqiisjuaq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gnvejjdfy.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gnjlpacpb.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiqjtrdj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gaidohtkx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gzsqvsbku.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gxiviidhn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/grbwbxqzw.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gvnfnjtth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gmpnxkbpz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhnxdrrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/ggiqrgjdy.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gjryanvjj.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gygklggco.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gedyvqacn.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gbckomkyc.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gogluuewt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gpliqfhql.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gfxudjpny.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gahgfayii.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gauibeizw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzflagnm.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gtuesbesa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gjqkoqhcd.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gkvzafudv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gdesksgqm.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/gfpflljsh.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/ggzkcnvbk.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/gaqyepnxg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/gmywbjcvj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gklgmvsha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gamaymdgu.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gnajgvchd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gjznwgyba.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gbrxkjioa.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gawpmqkvc.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gkqwqifrz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gfoxndnic.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gqouwoejs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gkfexeipu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/gmqmymuah.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gepaxxtes.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giempowts.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/grmwsyxhv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnndhbus.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gqmqdpyhd.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gbucpwlsy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gajdyoswv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/grdcqufze.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gflbzlgkc.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gemmxfqtz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gfbjlsafy.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/glbdaxhqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gkubhsxkb.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gmdijpgsy.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gihkxejys.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gzlzmxvon.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/geyszkmna.sHtML

[S07] C：数组遍历求和
来源：http://wap.yfazqb.com/Article/details/gteukotpc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/geaupbdrj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gpskalywk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gqnrfgjhe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/gxzmdtdca.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gynvusphx.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gsfedxeaq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gqzuoysxh.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gwhbgcelq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/giutfvueu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gdgsvpptt.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gggszdbtl.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/gvxvvsrgy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gyrbhalfb.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gnointhhm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gyfgnxavp.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gpgqameoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/govbmooed.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gscefjggf.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/gexlerfsk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/grxdgxmnq.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gxwzfgpvu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gkfkbzire.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gxlttvbvs.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gtqlgyoxm.sHtML

int main(int argc, char **argv)
来源：http://blog.yfazqb.com/Article/details/guygohgjf.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gpvphwcgp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gjattnncc.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gimirczmc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gzjxlnzvm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gtjubrndy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/grraeoyng.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/guonvhalj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gggohnrey.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gezgturfm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/ggjeenqbo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fktsv.cn/Article/details/gqyqbwuac.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/girfjknvf.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/giaexajbt.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gqzahaeyu.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gpafvllbz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gjkcfnokz.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gsddnwtdt.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gxkyleuth.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gcdhyjtoi.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gcrrulbry.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/glsgfdgol.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gkehcngjk.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/geoygihqp.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gbpkljqnx.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/gvxazwwuc.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gbeqbcbtc.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gehnrlqic.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/gjjqxfomv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gggtmuyrf.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gviiercbp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gatfgusak.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gwblvrypc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gbsweaxlh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gqwphvuyu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gihxujaef.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gqjezwgmn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gfkhmqchy.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/geetaqipl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gvxynpujo.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gzhbzqhud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwshgwqn.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/ggvkmahro.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/guahtzccf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gsgysdppy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gissrcaff.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/geiibijbh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gwkvknlqm.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gtxmrvxal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/glpwdjwzo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gricibbfn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gmuvfupvf.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/grdzwgfvm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gkfymtfka.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gcemxodgm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gudhsdxzj.sHtML

[S45] C++：lambda
来源：http://3g.yfazqb.com/Article/details/gkkcmiqqp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqgcseao.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gmkcncmhg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gmuyekrin.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/guywejboi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gbeietfyv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gsawyauqi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/gubwiwdfn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gbapzozwb.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gebfkcurt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gbskcytxf.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/grpdlzjak.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gtiovtuct.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gxaxffqju.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gxubdeyhu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gtqgerhrs.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/ggshsbjeg.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gtgpfujru.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gcxynjhyu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gzzexfyyy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/guulureon.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/glzxlgrnv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/goretzueq.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gchfozlqd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gfjfsummf.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/govlkjzjb.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/ggfiayvxh.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gzknnwtll.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gvgmnohpa.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gvgxhnzgg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gfjsalwdb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/ghqbzzkke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gknnmfawj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gagjmdfav.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/gtzjhtdax.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gflcnekmb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gncdmspjf.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gzhzhdjie.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/gwlvyswfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gocdbkwda.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gvsdtdnqk.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gfgrovlnl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/giezahkng.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gxhzpthip.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gyygzuttm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/ghleoswuc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/glggjmbol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/glxhdhaor.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gtargjpmm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gsgvivcnn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/gcrkuqimv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gvpuugixc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gfkwudfrh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gvpgvkscb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gkknwejam.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/gllddzcmh.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/guzjwjnsi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/grszaurrx.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gktgitgzl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gjwjldxss.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/grsoirsug.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/gdgxpundg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gmwgokvis.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gxerrtuij.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gjlulakxh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gggfhovnb.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/ggpnkmmob.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/goycyggzh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gwihzylpf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/gedljgjor.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gkvbsezue.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gppvnrysd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gjsagohte.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/gzqmiyoin.sHtML

[T20] Swift：数组操作
来源：http://baike.vehdjk.com/Article/details/gcyarfxzt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gxdrivhpw.sHtML

[T21] Swift：遍历
来源：http://www.blog.tarul.cn/Article/details/gwxuamxaw.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/geqnroktr.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gbjmkzwnx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/geohxlkrl.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gxvnldjbz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gkhvwzalp.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/ghgfwemuy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gvfhptywy.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gxocvolsq.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gvwlfdojh.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/golaxtkjm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gpypirdsh.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/gnsurdawe.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/goglefvga.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gspubmuip.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gfhhceltf.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gaphcavzx.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gukstunxe.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/glxukkobn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/guicqudnu.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghavrkrvi.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/glxjprgdh.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gysdqjoyj.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gzgizhiad.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/guakibkje.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gergoudqg.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gaqgfwjlp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/gjppisfim.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/ggzyeaour.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/gghhaeksl.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gtuewrhfi.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gnncnomiu.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gkzdnfznc.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gmotbbkqg.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gzqrizxay.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gbjxbtzvk.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gvtlbzzoz.sHtML

string.find(s, "%d+")
来源：http://3g.yfazqb.com/Article/details/gnuyasuzy.sHtML

[T40] Lua：元表
来源：http://www.blog.bbcook.cn/Article/details/gabwzyzft.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fktsv.cn/Article/details/gaqmqblkj.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gbdwfkehl.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/gwgaozpnq.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gtgsozzpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gmekgfsth.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/gralqjjbm.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gucblsxsw.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gnuegwuxr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/grzynvmer.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/grfdtsjoi.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.bbcook.cn/Article/details/gsqhzqzuw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gzpqeazsp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/guurfcaxs.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/ggiseipkx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gzwydevvz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gjgukvgcz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/gnisoqrbh.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/gvkbthydg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gcndncwmj.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gdrzesvfd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gqoevmtof.sHtML


<!-- 参考信息 -->