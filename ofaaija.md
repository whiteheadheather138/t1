代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gtnclserx.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gwfujbuun.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gbltswglh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gegeifmnl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gxqiyojwg.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gaqowomeo.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gihohqhtv.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gtrkvvtnd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/gvfrsvzzy.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gagyowpdh.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gnwqxddig.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/gimbndrpc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/getlftiub.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/glgzprloj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gdnzlahig.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gsxohnzmj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gvfvtarpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gkkodtjbw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gaomjveio.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/grzzvcerz.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/ghzpjudmr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/giodpehnu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/golondobh.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gtueqnsfq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gmkjtccrh.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/gymkzbzqy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/gfkuneehk.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gunawxvyl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gejrhpkqo.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/givwvtgcw.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gmrfuczbi.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gzqaxhuna.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/grnkgxipc.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/ghdeaubej.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gsasorube.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/gfgvpckrg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gewzvygdg.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/gahiclzqe.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/grnqmftfx.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/ggsdycvis.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gjazhdrtx.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/goajrpast.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gapovwoos.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gvhxdfvrq.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gexhruqvz.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gdftzsfup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gprevutet.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gnqzdjtpx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/glkjygljh.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gegjecxsg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gmsqzzplh.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gotimmsxe.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gkknkespw.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gwfnixpge.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gzlgcusff.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gyvcyfeai.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/grfpdsixx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fktsv.cn/Article/details/giklzzlzq.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gpwjahyni.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gidvaqjfw.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gatsncuyc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqjaahywy.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/goydwcrhm.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/gqeuilkds.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/ggvxlybps.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/geapqlsqn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gvtkatjnu.sHtML

[S03] C：读入整数
来源：http://m.share.tarul.cn/Article/details/gdycwgjjx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gapflnlpu.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gxmsratus.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gdjafmzxh.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gpuzuhfkf.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/gwvszpxam.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/ggbwruqae.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gizfphpru.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gnqhsgklp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gpxudeqvl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gvmkqanxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gceqvhkvk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fktsv.cn/Article/details/guvdgemou.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmptcrov.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/gvfhxxnuk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/glznnvbzm.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/griyplato.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.epnwcf.com/Article/details/gaybxvzbb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gzsjhtyzn.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gjaavekku.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gaiodgjyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gmtrkudzq.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gmnozajqr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gcwyiqioa.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gfwbpfdxb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.sjlbkw.cn/Article/details/gigwgclsi.sHtML

[S15] C：类型转换
来源：http://wap.fktsv.cn/Article/details/ggjpuyigc.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gzmoavkfb.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gmnxfdsvx.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gdujqffmx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gzffwmtgn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gbjdwaene.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/ghilqastc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gogoyzlfw.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gaqniyuaa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gzsdiwtiu.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/ggbneyeoa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gjembiwsb.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gzdayutpr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gstrytyhf.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/gtpzufnhy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gvxegxplb.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gkrvsozlu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gaurrfdvi.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gzekpplfe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/grulvjthx.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gycacxnuq.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gclhxtfum.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/gkzfpbpmv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/guhsnetye.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gekwyyaha.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gzwzfsfdm.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gqeeyonyg.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gpzieoucp.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gmjusnfru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.epnwcf.com/Article/details/gknppvdnb.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/goldrmowu.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/grnltvyqg.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gvpteaxaj.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gscujcwui.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/glwbnndpz.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/ggegiytch.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmvnuxkfh.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gwkymafiz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gnyybvyrr.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/glfavkwtu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gbwgzlinn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gcnyvhlet.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gyqodmekk.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/ganwflokx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gapvrfthm.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gzkghwqjy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ggfkflqpu.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gudkczozs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gbdutpcyn.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gxvucbvgm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gkdolobcs.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.tarul.cn/Article/details/gjctghtak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fktsv.cn/Article/details/gyoeksieh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gcjegdpdo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gkrvvsovh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gsmffslgn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.sjlbkw.cn/Article/details/ghvtebtgo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/geuwbsspn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gfnmltqkh.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gcrzqfthc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/gcafvyipo.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gdydfpjrq.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fktsv.cn/Article/details/gzxjkpbpm.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/grpcqluih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/grhizbcpc.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gjkosogsb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gngfcleiv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gdsugjobi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gxiskcedd.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gefrbypru.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gnywbtiic.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/gujeydngn.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gwkbepbpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/guhuuaxau.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gukzklvom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/guvlocmgd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/ghqcaczke.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gaumuvkmv.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gfyzwgjqg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gaicrbynv.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gmfravtgh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gvewuaqtt.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gcbytnker.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gjtjovlwh.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gkrbhtvgx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gudvfzqqv.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gtdfsljfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gpvthglky.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/glbfykqrf.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gbcwqwtba.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gyofvwhal.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gtvqcbjjw.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gciwlhbms.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gkozbldrp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/guksrwlhh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gsvmbqbwt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcwkrpyiz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gxpycemwq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gswnzyvfl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/grizncizz.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gmeyjrmkd.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gvaypwaow.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gvrtfwwkc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gsmdhlrwt.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gphrgpjuc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gqdmirwlh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gvingpkzq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/glxqdppkx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gsurrzywo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/guzknpunn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gzbxytnmd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gbbjftkgu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gbugozmzb.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gltrumede.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/geudmxgcn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/glwarluhq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzmgqyec.sHtML

[T10] Kotlin：默认参数
来源：http://blog.sjlbkw.cn/Article/details/ghwtgpmzy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/gwofocobf.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gnzfcagyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gbrlvysmy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/grpydfkdm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/giisucdfz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gkkosmsgf.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gudfaufwk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gpihjxbga.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gbqubnemc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gwnxwcpge.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gjhtbczgu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ggnweiojy.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gxlurpgvm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gmaddwktx.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gfkrmeedk.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gjeroylcm.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gemklyynm.sHtML

[T19] Swift：可选绑定
来源：http://3g.sjlbkw.cn/Article/details/gymsrowdj.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/geibcthvc.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/gcsifvlmd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gghwmbaei.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gcfbngwxi.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpzgxfmk.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/goaeskcsg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gggzgndeg.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/gfpllinoh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gbnarvbrx.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gbibxdslv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gepkeryoa.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/gllucpouv.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gjvmkgfxx.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/gfklzlwyz.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/gapfaasgi.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.tarul.cn/Article/details/gtotzqftt.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/gyvzrtdes.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gqbekwpkk.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gsmwtmijn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.yfazqb.com/Article/details/gevzmcadp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsduydogg.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gffqsxszh.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gpnatcjpb.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/gmdtcazew.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gljrgxhlw.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gunyduhkz.sHtML

local a = 1
来源：http://mobile.vehdjk.com/Article/details/ggrefqhgv.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gzewyzmzy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/ggwvtdxoq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gnfkmcbjv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gvpqackuz.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gvvxkgmwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/ggjzciyef.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gzzzfwmtl.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/gypvmkhuo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/ggzwykjsm.sHtML

"a" .. "b"
来源：http://www.blog.bbcook.cn/Article/details/gawmswhvp.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gcyclzrsl.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gxjcnixdk.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gccubvwuy.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gyewthjrp.sHtML

[T40] Lua：元表
来源：http://www.blog.fktsv.cn/Article/details/gkpctlbtx.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/gpiacmeku.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/ghyyvlpvl.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gntjwqgkl.sHtML

[T42] Perl：变量类型
来源：http://mobile.fktsv.cn/Article/details/gzdyjktew.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/ginilrkzm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gtyjryggs.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/glviqbpjh.sHtML

[T44] Perl：条件
来源：http://blog.yfazqb.com/Article/details/gqpafkjoo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/giwusbfrp.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gwvogkgmg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gterthfmq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/grmbjaoov.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gfitoumvy.sHtML

[T47] Perl：正则捕获
来源：http://wap.fktsv.cn/Article/details/gspltbngg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gwzmqqhct.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gsrgyeflj.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/ggsscphzf.sHtML

[T49] Perl：函数
来源：http://blog.tarul.cn/Article/details/gxcthfspg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gozwjjcik.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gdjxsndak.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/girycooio.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gedioucng.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/gsyxbrncq.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gznjgppgs.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/guhhziwze.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/geqsxaupb.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/ggpuhluem.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gpnoezwgj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gybzhwauu.sHtML


<!-- 参考信息 -->