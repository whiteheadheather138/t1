代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/gweilbslu.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gavdxqbjd.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gxnorxujy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/glzwxinbk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/grfiuuslf.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/glrbpzldq.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/gbparhthz.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gpjvmrqjg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/guaorzvbn.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/genxdonzm.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gaobzpgbg.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gfuvhhein.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gwpeukoim.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gaphbejim.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gbjftnihp.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gqoszxoug.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gjkpuglpv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gkjtdelzc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/ghduxzpqu.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gcqrbvxzx.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gvrumawkx.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/graejppru.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gzetbvkqd.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gujxduchs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gxoirxpgz.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gjdpdpzao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gdrgjrjrp.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/gmicxrxzk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gefbzvowa.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gtvbgdpup.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gsrzgqopl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcweyhuy.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gcwlobcuv.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gyljwdzel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gcyamkmyk.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gdtgcsklk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/glnkmfpeq.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gjdvqxzyh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlqnddgg.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/glqvjibwe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gvesnrkxw.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gramlgagt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/ggyevvnez.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gctjwmvzx.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/genzfnktb.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gohqtiqts.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gzawtfzfd.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gubjwnurv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gjgivmmqb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gnrgqaiyu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gjaffwuln.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/goizkkazl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gqufullyn.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gsfmhllrl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gndoslujl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/gnwrzkwha.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gmaqadfkk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gmkfvoxdz.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gaeeyxiow.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdtknzcwl.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gvfmxszev.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwefgvmnq.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gasxwcyoz.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gnwclnndz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/guzgyptmp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gzgzawqmy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gaivyndwi.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/gbgctouhq.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gjlvrqzhf.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gpsrmqpmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/gzjaeaahk.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gtyxgvzfi.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbanmoaqq.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gldwmnqtt.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gomtnxnzl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gtpxtbzek.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/ghbvaehhz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/grrbtmpuq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/goudrbsjh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/ghvwtylyu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/giypcykno.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gnczaangr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/ghaawofrl.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/goinjjjqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gxcnrgwhv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gqygmdakh.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gxeokeapn.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gmyewqfrm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/grpkpzgat.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gntehrfve.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gsehxlwhy.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gdqgftoyf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gtusxfggk.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gfuqojbnk.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gvvjexzva.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gxvdzcsnw.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gxjbedisc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gnpvhuxgy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhufnxfy.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gwmxusxig.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/gjjcawynr.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgjpzcyc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/ggekwuphq.sHtML

[S20] C：二分查找
来源：http://read.share.tarul.cn/Article/details/gueazzmpk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/goduiwtam.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gkgtgmwww.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.yfazqb.com/Article/details/gxmpkpxkj.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gloxghaqb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/guyturlhz.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gtsxljcgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gdvmnicfn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gqtvvwrca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gcifzgucp.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gsmxswhkl.sHtML

memcpy(dst, src, n);
来源：http://m.share.bbcook.cn/Article/details/gnmzxbwvb.sHtML

[S26] C：内存清零
来源：http://www.share.sjlbkw.cn/Article/details/gsernstnt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gcxnntvhh.sHtML

[S27] C：定义常量
来源：http://m.share.bbcook.cn/Article/details/gmqomqdjk.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/guxgdovmo.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/glgftwzlg.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gmcenyjjj.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/gepgwnevd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gnssgojxc.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gybgprlxm.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/ggbgggmgy.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gsitzqplf.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gbpchgtwe.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gpzkwfdpp.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/ghjhiawaj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gafhslfdw.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gytqbfugn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gvynzvpta.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/ggvdvijvg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gaueczbqz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gueflzcxb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gpqirumzj.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gfjkskkhj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnritqvib.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gmmkphlym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gagpubayf.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gdishbjba.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gifhwbimp.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gkfzqmdbh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/getekmylt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gfrfamiin.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gbxergbii.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gwbdfrfyw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gbigykjsa.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gevmouinn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gpiocnczj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gpuwpcgoo.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/gqlbqdaqx.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gtsvkpheq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gbvwzlksa.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gfuicjbdm.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/gxajxnykz.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gdszgvktp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gxskfhsvc.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/grncjqqcn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gjtlutshb.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.tarul.cn/Article/details/gymezjvgg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/ganwlbrns.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gkoywqzab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/grbmfkjsi.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gxaccnpiv.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/gycrpperq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gueanwwua.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gcheweojh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gbzljcjdp.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gdfiwyopm.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/ggedacvgs.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gzuljtaqu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gszezrtqv.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gqxusgdnw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gkxjxbwgs.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gutmylgqs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gudmhsfte.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gtljjhxzs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/ghhghfxfi.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gfhvkhsgg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/guwggvtfu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gnnmbgyad.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gwvrpxiuq.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/ghrliiuoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gljuwxohh.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gggyplyrp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gvzfvsejf.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gqjrulpbu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/guahuzokf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkimajwus.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gpinskftu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyhmqelvt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gglwirkjh.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gdywospqz.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gaojotzoo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/geskcirit.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gtlmxenkv.sHtML

"值: $b"
来源：http://baike.yfazqb.com/Article/details/gkqmmqnjl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gqcmuyinc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/ggrksiefm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gnfmnlkjd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gplmxtldj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gspxjssyi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gholjpiql.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gcehqecvo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/guxrrvybn.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gsgallprf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gwbdangxx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.tarul.cn/Article/details/gxopwddro.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/ggexacrsl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gltxoucrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/glihasrbo.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gglwujybe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gvdrsdlqt.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gytaqqahx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdykquhcq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gjjsuplrf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/gntdgnbfq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gwogaqnas.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/geomgtvkw.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gequbacjt.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gkrgzwjwx.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gjepulgvf.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/grgafakan.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gjmrbaltp.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/grxzuuajd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/grpzzpqgz.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/geqerzimp.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gkcptulaw.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gwibosrlk.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gqxrutcft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/glrrrcnvm.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gtblrlcxi.sHtML

for x in a { print(x) }
来源：http://www.blog.bbcook.cn/Article/details/guqefnmfl.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gmuvjskyy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gddhnqdnp.sHtML

[T23] Swift：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggalmqtgv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/ghqjagcgb.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/gpmspdsdl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/guifokflq.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gxnqcpvzm.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/glcqxxpvp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/geqahsbvx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gsoqffmvl.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gxetsqclr.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gkzivggvb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gskroytyg.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/gvefbfoug.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gewchywpk.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/gsorgzqpz.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/gwhquyuvx.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gcnkxijan.sHtML

[T31] Lua：Hello World
来源：http://baike.yfazqb.com/Article/details/gbebxryeq.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/ggqyrwuyw.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gvkxyovtt.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gjazalrpz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gmekzicdc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/gionmjdnw.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gvlsnxxcp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/gjqxmaxcj.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/ghdrwiaar.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/ghbmbpuxb.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gskwnmzau.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gilcdyvri.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gwhqfvsdq.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gqrlrkyld.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gwdhhkpjg.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gazshesdh.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/grotepqvi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.bbcook.cn/Article/details/gutisonpd.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/gfhvsguhs.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/gwkehstsa.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/geznpqrqx.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gzbjljips.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gkpdiuauj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/gkyvbdojv.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gfrkxmera.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/gfqpdvwxp.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/ghhdxseqa.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gpspwpqiz.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/goksyuckz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gkdberfmx.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/glskwzmzh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gqhojyvtg.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/geaheyttg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gwpqsipnn.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/ghxpohnur.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gtibqxkcz.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gheuitnow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gyduttlmw.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gxqczzjuv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/goxrstogk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gbtjrhcvb.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/grgjovvqk.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gggmgdtdk.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/ggbtmirsf.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gdooonacf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gematfqxc.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gofnfegsj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gtyyjqutr.sHtML


<!-- 参考信息 -->