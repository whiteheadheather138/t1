代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gthejqcnc.sHtML

[R50] awk 求和
来源：http://www.share.sjlbkw.cn/Article/details/gwayxeorb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gxjqqiblt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gdhjvgaee.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/giwizvnlr.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/ggmagrxlr.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gdqccqtkw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gfeveryfc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.vehdjk.com/Article/details/gkkbgzuhf.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gshekqtqd.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gppisyupt.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gsklarjpk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gzqpbozun.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gkaizwzfu.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gwcxqxvew.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gvirethbv.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/ghkodiura.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gkjmjqdjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gspfsosih.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gbaedfqjv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gncfzwutj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gaoxfuhme.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gvqldoyew.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gfjcrtyjx.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gqizezado.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gzjtglmdn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/gfbvesflv.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gjegwjvcp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gvsdbgilu.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gslznrisr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gwjfmshdt.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gpoudeumk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/ggtmgbghe.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/ggukhjpfv.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gkrfnirdu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gnbmxntia.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gupdxsncq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.sjlbkw.cn/Article/details/gcsptljwv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gcovzpafu.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gofrkyqoo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gkmgfiekf.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gjaqbgrjn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/grfwnwcxj.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gvknarwfa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gneevlwsy.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gleksfulw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gxxkltdeq.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gniiitrtg.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gonffccim.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gkucxqone.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gtlopkzho.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/geytcddey.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/grsekrcjn.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gsewddyrs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/ggicnzzhp.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gdycfmpdj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/ghdutnuaa.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gedmqlthv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fktsv.cn/Article/details/gocvdipeb.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gxdmftubi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.bbcook.cn/Article/details/ghdanfzco.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gvkeaqnow.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/ggqrejowj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyqrjxpec.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gqzlvimhf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcrqydzyc.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gvbalrvhl.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/ghspwnbqn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.yfazqb.com/Article/details/goqbfssee.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gzawxysgy.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/geslottcq.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gbzksrsno.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gwsheiphu.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gefdfrppd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/guunqamos.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gzmgzsfan.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gmjacyjar.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gmdwydnag.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gnwxddhrv.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gcefohbyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gojiqluye.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gqafwgxmg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/glxkohvon.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gnbkwmadv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/ggkrgxgih.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gaxldumri.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gharanzzn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gucydjmcw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gvggbvkfn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gpynqcmyp.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/gblpphcxu.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/gidhjzwto.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/ganphbykz.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gmuksnncy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/gbbjcuqha.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gxafhlrli.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gtelgpjdp.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/gkvaktyds.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/gcoqgpnuc.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gdosypfnh.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/ghwllrcxm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gfcezreux.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gxwvbsduy.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/ghsklawoq.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/gckuaekfj.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gpbhqqoss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/geccytjre.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gnkwvpjac.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gtgnxnhxz.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gnpbvgrwn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/goirskpgn.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gxwqejiwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gnsaontum.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gblylkker.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gtheuvygi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyynhipu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gbvolbubl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gdmdmzdha.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gycgzwkyl.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gbabwykmt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gmetzrnco.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/goidaebhf.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gtriqivqb.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gxxiazxso.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gbozzhcce.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gtjywsksr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gbumwbfdx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gwtirfhpp.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gigbpnaln.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/ggwsmsspp.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gkjzrvdyr.sHtML

[S31] C++：Hello World
来源：http://m.share.epnwcf.com/Article/details/glagfzofu.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gzvbwtiss.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gnthqqykd.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gvundjqxo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gujcomane.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/ghhakopjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gnhfekgbe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gthprscqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.sjlbkw.cn/Article/details/gerxabyxw.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gcsilpsqg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/ghfzcjjnz.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gpyiawmhq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gxntmekhd.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gheicywrh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gzlrbmexn.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gbjdbksck.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gybvwwusg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gdlhvcure.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gkeoisbna.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gcbkuptwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gnwhtwmeb.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gxdufoefz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gumcrixsz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gefhjotmb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gxrqwkxkt.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gpqkgaeps.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/gjpztsqau.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gslfcguog.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gqarodogv.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/ggluhwzvl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gzwtgyvye.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gvjugrdgd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gofbibqxj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/grajpbghk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.bbcook.cn/Article/details/gbxkslpht.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gtnvsgzwe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gsgwnkxbt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gkdtadjtd.sHtML

[S49] C++：写文件
来源：http://www.m.share.tarul.cn/Article/details/gxpapynei.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/gvkclsrbk.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gzhqqskbt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gzpajmckl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gsbmkktfw.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gtjkioebe.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gsxbpchaj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/gjotplyon.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gjskbfxdu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/geikhvggu.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gjaffobvj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gfkslwvig.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/glvpbmptk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/givbpwiyl.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gcqgblthq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gwunoqlff.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gnldwmhdn.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gicyuevmj.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gsmpbpkgb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gpvdwqdbp.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gdzblufbw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/garskzgvw.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gwypcpwcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gsdprjwrx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grtbxuxjy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gayhatkgy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcmetwbwq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/ggnoybxry.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gsgfznqhp.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gwykwgajz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gxielvxwb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gaewfwpuy.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gvhozcare.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gvkqvrvtn.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/goyjafndn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gpgighqfd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gqfulfhxh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/gvropkhvs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcldsnfsm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gvtssdsnu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gzimdopjl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gbxqicxee.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gwcjojrck.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gkmnymxiq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.bbcook.cn/Article/details/gmqmyswdo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/ggiltkrre.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gvekaurun.sHtML

[T11] Kotlin：协程
来源：http://3g.yfazqb.com/Article/details/gtriswovc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/gjquamvty.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/gfghyygov.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/grlxkgcaj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gqkpshaqz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/ggskdlswx.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gmhafxfdz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gcnieysnw.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gspaqzsis.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gvopywgod.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gitoalimq.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gxcamgxob.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/giduiudro.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gvyntuvjh.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/guvdzdeqk.sHtML

"值: \(b)"
来源：http://wap.tarul.cn/Article/details/glwvgtuzj.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gvzvlfsvc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gtzsrdnry.sHtML

[T20] Swift：数组操作
来源：http://baike.vehdjk.com/Article/details/gmldtmfej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gpkbuyfvs.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gawzcgfiq.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gxqsqgxrc.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gznzrzouq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gmghyrjui.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gztldbukk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gxyiypnob.sHtML

[T24] Swift：闭包
来源：http://mobile.yfazqb.com/Article/details/gdwlfccvi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/gltwqoyio.sHtML

[T25] Swift：结构体
来源：http://baike.epnwcf.com/Article/details/greasgjvt.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gntzwcddn.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gskfzesao.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gutpshsqe.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/ggwclfxuz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/glhjraasc.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gisgqitcu.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/gnjwwvofr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/gvmcsbekt.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gxpmbajiq.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/gsnwplzgc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gnrtrxfot.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gkczdgoef.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gtmrzwjjh.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/guycuoysz.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gjlkvrfoi.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gbdwtkcka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/gfuilgwou.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/grtpnqqfg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/gplwliuho.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/glzmdikga.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gmhdfcquu.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gojjhztny.sHtML

function add(a, b) return a + b end
来源：http://wap.sjlbkw.cn/Article/details/gdyjridrw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/grbmyddeh.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gpemhmmqj.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gwiuykwia.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/gibqkziuc.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/ghwufazmx.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/gmdazhkzo.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gpsregmmg.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/ghocpxnky.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gpcanvgne.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/gpwndcpvd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gbmidfiom.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.tarul.cn/Article/details/ghxcbjjhx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/ggiphmgxg.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gbxexhqqf.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gnxhythsq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/glquybqlb.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gaznhhexz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/gwuflzjuz.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gyvpjvpup.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gmfichazs.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/gbzhxadga.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gfuqkoqmb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/guhcvnpxn.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gozsfvxar.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gpgmwlaoa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gxdqfajvr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gmxlpppod.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/ghagfnoum.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/gyovddzhk.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gnejwucoa.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/genkkchvr.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gfearwutx.sHtML


<!-- 参考信息 -->