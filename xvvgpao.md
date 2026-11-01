代发 wailian999

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gqjjwizjz.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gdouybsrq.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/guoxgvxsd.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gnczwgwpw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gwsflsbmk.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gxrpjxxyw.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gfhqmlwqt.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gzgjwhurb.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gvjowxulg.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gurqyifrr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.yfazqb.com/Article/details/gfpvykgoz.sHtML

[R45] 批量删除
来源：http://read.share.yfazqb.com/Article/details/gdnfcfftl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gstozcuhl.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gdojijbgk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/goyunrnpm.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/grbkxamcw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gqlgiczvy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuqsoals.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gqnzdaqtr.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gtcldafbw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gbeschifw.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/gexbbbrot.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gsepjqhbt.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gxphkmbir.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gzkhqrrzh.sHtML

[R52] 统计行数
来源：http://m.share.tarul.cn/Article/details/gzfnbdbfs.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gxvhezrdp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gwujpzivm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gijvnifky.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gdawtyqki.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/gvucvwogo.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/gxtxgitwo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gdapwozez.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gvjpeyoey.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gzvjbqeuf.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gcbohjgcc.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gjwibeext.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/glvjxoafn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/ggmeuadvj.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gxraouwhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/geootdrdf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gsfgixtaq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gopazwyru.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gxrkpaahz.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gwcpmhiis.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gyqkyvlci.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gfulaaqcb.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/grnqdceyf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/ggoagsujd.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gszsxutfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gpxqczjna.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gueqpgzpt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.bbcook.cn/Article/details/gzmblqhrq.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/govenpyjk.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gxzbdrbwa.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/guwxbqjje.sHtML

openssl rand -hex 16
来源：http://www.m.share.tarul.cn/Article/details/gaesytvia.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gkparqbsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwotzsgav.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gwjioaokp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gfnimyuft.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gvrdhxjdm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gpvcfurfs.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gcegxqudm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/gfinpragl.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gylfurtnn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gddkrpvcf.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gqgrewdxc.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gmgkkrran.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gzrmtxuuw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/goatpxlei.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gyjfbceki.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gzpohtdlr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/garjacjfg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gilniicbi.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gbzemkuwm.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gwhdlnzoa.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/geyhrozok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/glifswrvx.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gbryjwxfo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gwurajzct.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gkywacvaz.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gqpwvjqna.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcibyvkcc.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/grmnwantt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gytjhywwr.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gtfrbylnf.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gedygtuhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gwsobimlm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gxtaqpsww.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gfclhcaff.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/gihsjebvn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gvcigvgtn.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gediklnzr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gnfexncby.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gnkfvsvwc.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gyuuftcdp.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gprumqebo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gukcvsujm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gkiuxmxfj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gnwhttfti.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/guygiqyrj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/ggwginrkk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gayjnvhvc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gyihgahbi.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gvnvfzswa.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gijyyjqqq.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gkhowlydv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/grmsgsqhp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/glorzqohi.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gugcmvusx.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gixinsiut.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gidyznzwk.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gtgknpaus.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/ggykpughl.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/gaoxjpnca.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gitdflpda.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gpuiwcqga.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gykjwizni.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/gfbdvzdda.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gusxalpnt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gdujfeqad.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gegnffkmx.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gmzuoeclt.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gubomtkye.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/glquympzl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gjxxluiik.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/glwjijbvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gmughcaay.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gekfblfjm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gagzdujxy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gdsyycppz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/gmsynhtuw.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/gyqzsazhn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gcvzlqobg.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gkzlgvrfa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gxmyhlxmg.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/gnifwirrh.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/gsvvpocus.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gvrmjqwxr.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gljepcxhn.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gxnixytux.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/giypasnqy.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gijnrqlpn.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gyaqwvshw.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gsudlncrb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/ggxrebgxo.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gcfrvmbfy.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gfzopiykt.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gaxrtnwrh.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gvlcbijzy.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdhohtele.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/ggzoshvnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/grmatxqol.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/gerymqixs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/grwqsolno.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gxflonpxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gkldjhwlq.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gszejcpnv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gzsezsdeu.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/ghuigccjd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gyzqpeqao.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gmaowmlxo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/guccuorpr.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gvmheupln.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gwkjrpjsi.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/ggxsnijsz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/ggyaoqhhq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gqdfqvppl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/glrlicjug.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/giofxiewa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gqnkpwwvk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gxjlbxebk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gfrziojwn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gqodkeoex.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gsqwtujwg.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/ggttvgrfz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/gpuqsduwy.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gmzcochub.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/gcpzzmkqw.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gfhgjyoqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/gpwjqlpie.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gjsojuiyc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/gdtjfzmtw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/gxuzfaqsa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gcpyuqcfw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/ggfxiozua.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gihaooipu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gsuyonyno.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gyhjsydmg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/ggjdxcvll.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/grbofshau.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gvsdmrctu.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gdtnletxn.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gwfgamnss.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/guijncwql.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gpwdmqrql.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gyziudgty.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.bbcook.cn/Article/details/gnocthovg.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/grjdeesza.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gzvmnkafp.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gxnccycxv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gcgvofdoz.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gnsahgkkf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gumstbjaa.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/ggaawdggs.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/givkqicxv.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gottzoqtz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gsdyjtqhb.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/ggddjavvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.sjlbkw.cn/Article/details/gnhorwoxi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/ginlvvvza.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gpgkrqtfr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gayjlsphs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gvhsoebep.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grxyxerum.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.epnwcf.com/Article/details/gfrgguxah.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/ggnsvtxcz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/guvdrndnr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/ggiipknrj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/gdesdcxhc.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/ggdnqekyo.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gsaewxvmf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gdjafguhe.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gfjzxssbs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gusiilviq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gdtsudaea.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gyovrawtc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gfvdjplys.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gmrtufglx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gnvonlqmp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gbmtslvgh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.vehdjk.com/Article/details/gmgrvhbus.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gnkgmfidw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gttfxgzov.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gslzrbgut.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gkdzoynga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.tarul.cn/Article/details/gwbbziaoe.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/gabbltxzy.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gtjnmvcij.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.vehdjk.com/Article/details/gukvhdlqq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gekawndav.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/ggjxinpmd.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gdvogvtvw.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/gpqtyohio.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gapbsnqwy.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gxvybmshc.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/goufruapn.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gjjzvjegv.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gsgwjthjd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/glenfckmx.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gbawxbjcy.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gglufslay.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gjyfukdab.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/ggnuyvgzw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/grajqkdhz.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gvxzyqdrr.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/gwionnkew.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/gwmkqxrfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gtwqxmfpe.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gaozboaan.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gnrviqhhh.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/giwkfnjrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gicjvztti.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/grrkdnmvz.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gbgovznax.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/ghfhwgqqg.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gkpfxdqsv.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gamonwhpj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/grslexvnr.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/glslurdkd.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/ggtelarel.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/gbevklxdv.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/gbbzzrnzo.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gcodeykck.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gwpifpzpq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gkkojeyov.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gfxxonawc.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/gczviwddv.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gshknmtcv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gajvtrxxw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gkstilxgn.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gcxobjnmd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/geijbxwym.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gzspyizaj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/ghnjgsiyv.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gzfaktfrj.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gfrmxugzj.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fktsv.cn/Article/details/ghmrjlmpt.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gnhwpjlih.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/gjgsrrbmi.sHtML

if x > 0 then print("正") end
来源：http://wap.sjlbkw.cn/Article/details/gbkixumnh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gegaibxnt.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gizjgqtjy.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gxnkxzzfr.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgwmojmr.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gugymgegn.sHtML

print "Hello\n";
来源：http://mobile.vehdjk.com/Article/details/gdevwpeyt.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/guqkrvkmm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.vehdjk.com/Article/details/gqjuelixz.sHtML


<!-- 参考信息 -->