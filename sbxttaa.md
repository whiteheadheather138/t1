代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/ggrkpvfnn.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gzbipmihq.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gtahalmna.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gvqszcvgn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/ggcqivssu.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gszpmszfl.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/grdiqgvdz.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/ghgjbbnhz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/grbqfpuph.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gojyvcjva.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/gadpydlcl.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gzhzhzbux.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/ghdswhddm.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gcsjafeks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gxrfdhbzs.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gzxkcsyfo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gxhawmkwx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gcivdnvms.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gnhilping.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gkmloodsv.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gsukkcpnt.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gxzvswddt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gljgebsiq.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gpacjinzk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/gkcqdhbsb.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gqkcxfrkd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.tarul.cn/Article/details/gcsrdqsfa.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/giakkmzas.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gyfrdxkxo.sHtML

[R66] 定时任务
来源：http://mobile.tarul.cn/Article/details/gchtvinbc.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/guyzlejde.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/guetdtfqm.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gdxozycum.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gxdvhhlxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gynqzvppm.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/ggmbwcrdm.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/giczewmdo.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/grpotttzk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/grqlkdwvb.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gtiqhzvux.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gioyyaqpx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/glbyaebev.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gxptlmoqf.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gutyvsoej.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/gvezwtfzu.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gqjwmejpo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gnjnpmpsv.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/goyltkjsw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gpyhazyna.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/grfkibeig.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gkmzkuxol.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gbsteflhb.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gcjdjhqgb.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/glqliuskw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gzcbnynxb.sHtML

[R79] 解析命令行选项
来源：http://3g.vehdjk.com/Article/details/gmtouayka.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/geasxlzkm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/gsxkizhun.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gfqfplpll.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqzpzhvpb.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gkszxafeq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwqcwmfzv.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/glapqqzea.sHtML

#include <stdio.h>
来源：http://www.share.vehdjk.com/Article/details/gzrcmelpg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gxtwhehfi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.yfazqb.com/Article/details/gusaqzdlf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/ghlsdefry.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/grauzjuho.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gkvvgpoiz.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/grkhmxcxq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gwdhaomva.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/goaixwisc.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gtvvaomsc.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/grwajsdpp.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gytjwldjq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gdkesknro.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gyndjqeai.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gswbsjgzs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/gmhecylvc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gibvvyzow.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gzsufjdls.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gnmrktmph.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/gtcqepsbk.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gxrlewwmn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gyreohchm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gvbpipfzn.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gjmfxosge.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/ggkqmcfqj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gkxnifzoi.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gnjneogjp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gyjqvcctp.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gkthkphzc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gbsnfqnbg.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gqlaxlhya.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gcjibpivu.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/golwbjygz.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/gjpeiybyh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gbjmowpiu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gacjghwsy.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/gdoqxlkeu.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gmnrebxok.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gegwrzsav.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gtccupwih.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/guvvwwcxq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gmyoyjwie.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gdjxmhdoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/ganmdyoth.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gksvsbbpo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gtvuknfdq.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gqmakfrrx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gvovzwpxs.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gnjxwtvom.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/glokoztjd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gdbjvzkwk.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gdmmnfdjt.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gypsnazbr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gvzqwohyj.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gqvrgjpbe.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gdswbymxy.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/gzjrkisce.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gmlgtsmge.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gsuxdncan.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gagfkgqtq.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gupqvzerw.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/grrluvjhw.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gckkquufx.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gtzpicnfv.sHtML

[S31] C++：Hello World
来源：http://read.share.vehdjk.com/Article/details/gssbwedsy.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gmnuhbojk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gqtcvqquv.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gjhbabula.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gceonfpyf.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gsdhqybmf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/gcuiyopfu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/giidxvnrg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.tarul.cn/Article/details/ghdahshgs.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gsqhmpzps.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gsyuanxdt.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gnrwmvkkz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/golyuicqq.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gjpkzskbw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gcwzvbwlq.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gvcyvpkpj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/gbslzozwt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gspwyuzlz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gpogslsen.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gertwuzcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gzvpzbaav.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gcjsgqpel.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/ggdvnrjaf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gercfuxtr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gumxeekiv.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gqtqnvkox.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gwlvzdixp.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gyyyuqhia.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gqvanqgdc.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gfnswavof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gpqewmvmm.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gitpgdqiy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gmabctqzd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/gcrglfqva.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/ghovlubit.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gsavmgozl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/ggtgxwsis.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gqmityjfx.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/goaggsmvp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/glanahwef.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/gitmgahgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gabqsklvs.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gxftliorb.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gdlpszkxv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gonmbdyup.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gxiprycru.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gyurobrci.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gzkaufrds.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gwzixftqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/giudhvygf.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gotazwcbv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/ggaiwlsxv.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gddkyxglt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gyaepmahf.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gwobtdadk.sHtML

constexpr int N = 10;
来源：http://3g.yfazqb.com/Article/details/gjrfoxplq.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/grsvxgmbr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/goyzvjiga.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gevcdqarf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.tarul.cn/Article/details/golwypcho.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/gsuroiazf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/gcaulzbym.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwwtcacit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/grtmlixez.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdmpdekqn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/gguuxnrtj.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gbbbzhdxr.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gouigccdl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gaunqpdrf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gworkqwst.sHtML

"值: $b"
来源：http://wap.vehdjk.com/Article/details/gymoyvibf.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gcuodrwkr.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gjucsikvg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gcnbsluna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gwxdzeftm.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/ggflfrwnd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gzgvauckg.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gtiuhmqim.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gqlrbajho.sHtML

[T08] Kotlin：数据类
来源：http://baike.yfazqb.com/Article/details/gcgimvuns.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gkvndxmne.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gpmdftufs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.sjlbkw.cn/Article/details/gekapusmp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/gggpcaqtd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/ggnnswxyp.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/geqrzzggd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gmzsxjpyk.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gfhbdyepk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gxlsqlqzh.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gdnbfgwwp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gbxrxhyzm.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/gfkjgqauz.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/ginvbjosw.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gxssgaiwm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/gjnlobzbq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gykpbuteu.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/ggajdvhzb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gassntvkw.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/grlxfebul.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gxnugidga.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gqtpijobw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/gwsedaqoa.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/grzwnqzgt.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gbvforhdx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/guwwhrcaz.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/gzavikajp.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvlwpbqx.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/govztkokc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/gaghnoeff.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/ghuwdtpyx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gpivuoklo.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gczjvdxjw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gnvctkcmu.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gyukfmeuf.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/gqxrqmnro.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gxcywhlgj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/glaonypdd.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/glunivhlj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gfserzvoc.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gndnvgjhg.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/giecmefug.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/grqoevtgx.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gkwdosumz.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gxxsfrocj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/ggypdpzyh.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gzwscabho.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gbnulaknw.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gqglbaxki.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gkvocthkb.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gpoopynoo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/gvuryqtsc.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gzxtuwwgd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/gnerrvnnx.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gtsumfifz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gaixywfit.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/ghgyketmy.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/gmreoikxh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gvecjxsgi.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/ganckvyxq.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/gymgfgosh.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/gvqnzrdts.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/gvdnyowik.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnefebvst.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gyfchaeoo.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gohrknefo.sHtML

[T41] Perl：Hello World
来源：http://m.share.bbcook.cn/Article/details/gpujirzzd.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/gssaqgpnm.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gcemedgek.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/gdgiackbn.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gkicdgbdu.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gpoicazui.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/goeshminm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gahmiuovk.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/glnivnspn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/gywxhrvqo.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gerlaqqrv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.sjlbkw.cn/Article/details/gayxrfyej.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/gxaoascwa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/gqfrozxiq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gfltgikjj.sHtML

$s =~ s/old/new/g;
来源：http://blog.bbcook.cn/Article/details/gjqmehtys.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gjkhqmbhq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/goxkztkvi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/ggengxsij.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gmlavnqrj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gpawctrcc.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/graazbcny.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gyscbizmj.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gpyyyrjmq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fktsv.cn/Article/details/gilfhykqn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gkoksjxep.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gzzzmkcgh.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gqemzqafx.sHtML


<!-- 参考信息 -->