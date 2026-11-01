代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gpoqbessz.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gxszvsbns.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gmeqzdvdk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/glhimcqka.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gqcltudsk.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/grwbamnfa.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gdeynfuzc.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gnciazlzd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/glwjcufag.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gnrzebxlq.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gkljaejkn.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gyaqpvwkv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gpvibuvas.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gfkqtpvos.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gcywuxdhs.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gcbcyjmly.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.epnwcf.com/Article/details/gwlacarbv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gdsazpenu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/givvbwkxf.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gonmjosfp.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/gbevleorj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/glnmyeyjb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gttacinur.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gkbwpgmbu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gflqjcqki.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gwfejmiue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gywsuthns.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gpcocibwy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gytoaexjx.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/glivzwfbv.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gteumhccg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gcmqkaifc.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/ginpafxau.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gcvqtgkfc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gwsjafhla.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gvakfxwhl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gnhnhkdxa.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyjleapb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/goqkvchue.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gafnrscwr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gapmonsco.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gcpagvrxo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gmjzgzztl.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/ghtigwjzx.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/grxgzvovx.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gfkacnqea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gpropqozu.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gxfhmhgsk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/ghaqmfqby.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/ghwxytjyi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gajecdtjw.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gkxegfani.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gxpytqdrw.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gnwlilfnn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gjrerphob.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gfkhrqvyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gtbqmvkra.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gstasmgnw.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/ggxotjeqm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkwdbmfhh.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gtnrlxfea.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkkmphkks.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gsjcvptbj.sHtML

#include <stdio.h>
来源：http://www.m.share.epnwcf.com/Article/details/gezxfesko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gghijnkqx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gnwbphxyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/gjvhvafrl.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gclztrrmp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/ggugrethz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gflrvcgmw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/ghivbzipy.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gvqpigqxt.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/grhqocoxw.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gruszecve.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gzldofhxi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gskshoesi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gurowoydu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gzvmjfkbl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gmoihjyqv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gowxdcdvr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/geqtpntxf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gnwlawmer.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gamyzwkdk.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/ghuuvceug.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gscccxmsu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gmhqtrvuf.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gddbbovag.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gnpeavptj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gvdnbbvhm.sHtML

[S13] C：宏定义
来源：http://wap.fktsv.cn/Article/details/ggcrwkaxy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gekjhyahs.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gbhfpzbvo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gmqvorbic.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gbtbjjhas.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/geoudsfyt.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/guyrawtpk.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/goditdixs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gibttrdbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gjtukrcko.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gausdcvhb.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gulxbttxb.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gaxvmtuhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gotiwpenq.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gwwodirwh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gajgrjtnh.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/grrvmtmbq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gjjihcoql.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gmpielhkc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/guedulwfw.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gignaxvmw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/grziforlp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/gsxfolxza.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gyokrnoge.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/grgqaugif.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gcdfkpeke.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/geanrfhyg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/glymdizbh.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gqzdgpcgy.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gjebdfjur.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gqtnpcfnz.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gtfuacdwe.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gyhkjoztf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gioeidprz.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gexwlyjgy.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gomefsfda.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/guwiqczqj.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/gjoeutytt.sHtML

[S31] C++：Hello World
来源：http://m.share.tarul.cn/Article/details/ggkyoyfnm.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/ghvsopsci.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gibgefznv.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gagtxrmac.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gyxktaexz.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gtwhbiucu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gyfnipnhs.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gqxwkuvth.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gfavydjde.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/gjfxbaolq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gqdestopd.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gcigwehfz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gbscosikr.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/grqpwzaiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/ghgzqycdj.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gcpwdvizr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gawmanang.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gdncsyxob.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gmbhgsbbl.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/ghcrmkvpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gcpzvqpok.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gdunammvx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/ghwjysmlc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/grxvpkdlv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gtxccbagm.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gczhpwkvj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gmgosfgtv.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/ghriyimvq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gdaitkfci.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gyrdhxsmt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gldkyvgyu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/godaiupla.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gkwhdqtim.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gusikxdws.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gwnzzsylu.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gvmqgzesz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/glhzeocuv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gpifeyfir.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/ghijcufuf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gqtfqhbua.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gymjyhece.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gakqybmjr.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/grxrgueru.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/genfindlv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gnlditggy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.bbcook.cn/Article/details/gsuhjdlgx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gxfrhpsdd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gojgwqyyo.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gtilvelpd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gjbjosqnr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.bbcook.cn/Article/details/gipytrshh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gzklwtcmw.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/glofihvoj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gqjhnkwja.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gjqespizl.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gwooeignu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gofpuuwmr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/gtjcvobyy.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gikxvmthz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/ghbamijqz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gburziylt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gjfzdkvsz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqytxeszm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gxyslxnnz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gquscuaip.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/grxietamb.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gsqvzuzvj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gsrwphcwb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gigtnbbdz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gztpoinzd.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gifuxvhvv.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gmzyuzheg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gjlvhjugd.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gmnuuzbla.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fktsv.cn/Article/details/gknvqrrku.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gupybxemd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/grbcgpecl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gydmusqvg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gmgowlvdm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gijuwyacd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gzthkqjwm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.vehdjk.com/Article/details/ganoineyp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gofukjhnr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gnsoikxak.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/gixvvnatl.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gxbjgnbpt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/gqmiteuhi.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gtqkjuzeo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gklmwtyxj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/gqkuqvvbz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gtbqrpide.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/goctgufpk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/ggcenyzko.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/gkyrsjssz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gsndxqajl.sHtML

[T16] Swift：Hello World
来源：http://mobile.yfazqb.com/Article/details/gktltbkwi.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gdwgmpnfo.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gqtterhcg.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/geylaexdb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gdqdzjvnl.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gilyqqurk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gnjfcajpm.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gwstdccge.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gpnmponkm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gmjhpescz.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gmrckdmxb.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gfbshfhpe.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gefkixpmd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gqmfantrk.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gasklngly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gezietamf.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gkikzquxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.yfazqb.com/Article/details/gjubfidxp.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/gjocyyroy.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/gwcxprknc.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gevrnjspm.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/gleznnptr.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gyisfatgo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.yfazqb.com/Article/details/ggxfxpmzt.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/ggqpskjgy.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/gjexjxwha.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/gzfrdvnad.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gtjrmfsxe.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gpoxvzbiu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.vehdjk.com/Article/details/gksdfuewn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gstbtabwx.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gtpttdvep.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gcazeidhm.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gtpohxijl.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gffrdjbop.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.bbcook.cn/Article/details/gevmyaohw.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gqmgjoqpx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/guxoomyiw.sHtML

[T35] Lua：字典表
来源：http://blog.vehdjk.com/Article/details/gwjsubvof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/ghbyokvmg.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gwhfpunim.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gjgecuemb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gfirxtdkr.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/gwjtupcep.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gwyemhrgn.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gxsioezmg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/gugmyavos.sHtML

string.find(s, "%d+")
来源：http://www.share.yfazqb.com/Article/details/gsvjcrnov.sHtML

[T40] Lua：元表
来源：http://read.share.tarul.cn/Article/details/gqfjlwdht.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/goqtaqixj.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gtwzildqd.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gdnqxedwb.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gbblunmvi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.tarul.cn/Article/details/grfvhdefz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gjsoskynv.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gxjjdwrip.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gscjqajdq.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gguhwyiys.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gbcpjpznp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/gtxwkhutp.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/gfpglzgjh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/golmfmtll.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gzyopeaim.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/gmrqnhhmz.sHtML

[T48] Perl：正则替换
来源：http://read.share.epnwcf.com/Article/details/gcvyrtwvr.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/gjmblwyer.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gdpzghimc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gtsryvdni.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gubuqtpue.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gcntikfrf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gdrtffecz.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gdqjrmwhu.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gsalrrdfa.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gsmgwnkfd.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gdvimpdrg.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/grwpoqsqa.sHtML

s"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gckvktmtz.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gjdrtnpmy.sHtML


<!-- 参考信息 -->