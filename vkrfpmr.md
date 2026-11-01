代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gabftofrj.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gtzzgxjrt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gkkfsbimd.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/guhgdfzru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/gkqseusmr.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gygfzbbuz.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gvdskkpnx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcougume.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gzepudqcz.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/gijfqjhwu.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gxkmzdpkz.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/gxdkkwyeh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/glptlzmig.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gekhagwkq.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/grsgpmurm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gpukfppif.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/ghjiblvjj.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gpychlpgk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gkovhyudv.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gqmdpbgea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gslqaykgk.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gzcibbgiy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gssolvtha.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gsuazhzvz.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gvspgdztv.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/ggajoxcai.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/gfsrmprgh.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gnwmokihu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/ggcdrpnlr.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gawjzfiip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gtzutddmn.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gxxzlhwez.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/gswmjxdut.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gkypnzfex.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gpfqlypxs.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gpffdnbjj.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/giszhdmpa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/goyqmbbmk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gtaruhxzi.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/ghaufbaoq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gwmmomdmj.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/gdcpiotjq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gvuurfnaq.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gkhwuxcrc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/ggvvwqkyx.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gxicfoonp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gaqlkhftu.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gvplvkdac.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gczfpjcjg.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gxkljcmxf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/glnusedwl.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwotqxaw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gbmdavkva.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gzdzchhna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gmvgtuwyz.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/ggxmsfddt.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gzsgiytxb.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gqulccrni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gqxtrbkmm.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/globriaoj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gkibogihm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gyftqbixn.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gworjifwf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqmtsncwm.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gtwyhrklf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggnrvkufn.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gxfwxwnyw.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/glitmehxu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/glblnwoxm.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzcggdnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.vehdjk.com/Article/details/gqstmbplv.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gmrjtgxku.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/ggpvzzbwb.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gjtxdxjyz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gnipfhiqc.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/ghvzzukhr.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gcwnxuscc.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gxxpswrin.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gcejspfbi.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gyewnfbcl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/glsbxgnim.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gmqfokieu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/ghnjgkxdy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gxclidkla.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gnfjeonlp.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/gueqasjsp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/giwejdjpm.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gqbravhfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gtxafvace.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gesemjrcf.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gsstjgcbt.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gipqeplim.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gtbszjoot.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/guvajdxpa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/ghweifvvs.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gknnygrwj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gnbcmshwk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/geckbulna.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gafszmauh.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gknnefaxh.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gomqiztgb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/guaayfbeb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/gnsmiewah.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gwsdgcqft.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gjqwjeqzw.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gfpmkeowh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gmghvcqrm.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gmerwfrri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gulyiwmne.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/grcgziwvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/grkbeewit.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gnviicdnu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gxpblyavx.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gdtrrlemw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gdtrwghel.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gmpaqazhk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.tarul.cn/Article/details/gllnmmmmj.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gyiscnmqt.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gnnjstyto.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gfzxpshgs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.epnwcf.com/Article/details/gggpzhehf.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gotkidpmf.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/guapmfncf.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gqaiyarzs.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gcznpktvm.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/ghwjnnuin.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gtbehxzjx.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gtlvyrtzw.sHtML

#ifndef X_H
来源：http://wap.bbcook.cn/Article/details/gccupgazq.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gogegusha.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/ginfheylx.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/ghedvdudj.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gbfivxqqq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gmktdeibz.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gwlqwffcm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gobfutpzg.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gxmkkrlsz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gdyposmzs.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gkibhsvqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gxajdzzkg.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gxunrqaub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gdfsktpmx.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/gxzbunoeu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gnemzirmj.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gpbikmzhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gnvbsakct.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gffuqqomp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gfutfuvvj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/ggnvauiyk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gzpsxspmb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gevopdwci.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gofonqqdz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gusqrrxlw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gmntubexn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/gsmfugmgc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gssaqlktj.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gqjfxxrbr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gqqknptuz.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/ghybhwpjl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gzuucxfje.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gikrkrmfj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gltioxuph.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gsqzsmfuk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/gwfvmydzb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gofdnquhh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gisnmfonm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gmjkymtxv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gcxpugvog.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gapijfqnm.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gytfrkbij.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gafofkktm.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/glksilwxh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/ghldhzxyh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gwwvyeomb.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gpctsyasn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/gexabcgze.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gplqyeqga.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gpoxmmnwb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gquqkbpjl.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/giogiirmh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gfmhbfofp.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/gzmhzkrim.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gzetewpcc.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gyqxtusch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gitednevy.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/ghbesfiih.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/gmicdgrpw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gpfgrteid.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/ghgaljdnk.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gxoxdkoqv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gjgdlckig.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fktsv.cn/Article/details/gnajbtjeo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/goukvebsf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaxvzbcky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gzuxfhagp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghjhzepxm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/gxvnbbrzc.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gvfpsuwic.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gjjrfvxqh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gtmlorsoi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/ghouablsm.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/grmmbrasc.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gzivmheys.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gtvvdpzgr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gibccrnsa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gfketwivh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/ggizklbuu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gtsnvkeyg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/gkpziolxa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gsrhvfmoa.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gkbcmzxot.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gngghvxof.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gxlkrpbak.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.tarul.cn/Article/details/gjpbolwul.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/gyskinder.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gdamgopmj.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gofhecubi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gyttiapec.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gcikyuqmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gefolhvwd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/giotudjic.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gnwmggwow.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/ggxjgdfvx.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gbbudokgb.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gnumodffr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/gcwnbppob.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/grwssowjj.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gazplbvig.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/gmnsflbkp.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/ghqjeazfm.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gqidovzlb.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gzrnnfnfn.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/gysvterlm.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gbxmtsvqi.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gnwtzoarm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.tarul.cn/Article/details/ggsbrymiq.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gkhnbhbmf.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/goxvzkxff.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gcbgrvgiu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/gmqrbkozo.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gpepcrdby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gwbqjorzd.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gponeaoxx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gqipjtkpn.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/glxbxabxq.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gkxdhtmwi.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/ghwhpnvsh.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gyryqdkjl.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/ghlspezne.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gpogwuwzu.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gbhclrser.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gclravjvu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gjiudvypy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fktsv.cn/Article/details/gjyecvdvt.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/ggdlbezbt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/ghrnsrqyu.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gjwpnzsac.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gpxtblamg.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/grtyhbafa.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gbifranwh.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/gqdaosdpp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gxewdakrn.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.vehdjk.com/Article/details/gzhtxctnd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/gxipyuhhy.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/gdntngsna.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gtyklovkf.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gobkydnrm.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gvpolnnbo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gxwbbphgw.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gpgbbdtlb.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gcnnwhgfa.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gmwlxpetu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gkrfuqvst.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gshvtrcxj.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gkbkjkqdj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gnmuygjqs.sHtML

[T41] Perl：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gdjaynazg.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gwxefrnco.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gsgunkqmd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gratxwxtl.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gigqpjkzw.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gzehekwyl.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gfuezuruo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/goxpgjvfs.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gyomuuehb.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/gvwegaepx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/gctvifiom.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/gfbquupdz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/gobjrtycv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gacddmmyr.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gxlodnoia.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gbycmspvx.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gbusocjjd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/guepkhohy.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gfvvpmtif.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gvuihjdng.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/gdpxrlyym.sHtML

[T51] Scala：Hello World
来源：http://blog.epnwcf.com/Article/details/gphnazdcq.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gtkkazjlr.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gdayrrdil.sHtML


<!-- 参考信息 -->