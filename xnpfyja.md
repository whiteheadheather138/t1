代发 wailian999

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gzzkipwni.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/gzszjiblf.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gcxsnoofz.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/ghvvpwgsv.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.vehdjk.com/Article/details/glksfetes.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gvfqpzyec.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/goyijyomi.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gowjtvmtc.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/geownlzyp.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gqpaecokj.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gfcmcdlrs.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/gfhghzonw.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/ggzqefrgd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/ggriyomxb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/guvgzpixp.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gbhexcpnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/ggnwjnlde.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gbcumimcx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gmadcohmv.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/giylwatig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gsxewqtgj.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gapisphtd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/grxuuxepw.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gpyiekfpi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gadkdzdzd.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gjbwbvqfi.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gctugcrjx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/ggebhovay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/guudaovob.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/giamecaso.sHtML

diff a.txt b.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkomkqupk.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gkbitepca.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gxbglxbnj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gjpmkmmcy.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gkmgbiqnq.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/ghbifssxz.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gitqhzjbg.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gwjivkfcr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/glkyfmsvi.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gvzzlnitb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gaaisenug.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gszzfgtwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gairnbgca.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gunttzgjs.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/ginfomngn.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gfxxpcgwy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gqpqujjhj.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gattsweyd.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gkpttenxe.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gtkdfvqav.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gfvylnbpc.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gyxrnvrkk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gbdcgmdog.sHtML

[R66] 定时任务
来源：http://mobile.tarul.cn/Article/details/gxbsiwqws.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/ggmszmikp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gedwotfes.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/givxjpjpj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gumvppfvw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gxfjjtmca.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gmkauwife.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/grnltzijx.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gbhvtedcg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gqmyrsrhp.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gnxjekvrd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gfemwpogi.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gtllnlbep.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gticqmovd.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gabatxhkf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gkrkxfura.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gigpyfnrg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gqsrybfdt.sHtML

[R75] 导出环境变量
来源：http://m.share.yfazqb.com/Article/details/gidatkwmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gmnwprbob.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gjhvtporp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gvhdclyfz.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gqogggxqb.sHtML

read -rp "请输入: " ans
来源：http://wap.epnwcf.com/Article/details/gakqyjqpb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gfuosfawk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gfikinhod.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gfggohivb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fktsv.cn/Article/details/gvapoqria.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gfmdiuvvu.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/glixnnkki.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/garkosdrw.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gzjztxsbu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxekljfqw.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gbnmjxpzv.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gnjsnycfh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gsqxyxmab.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gwqczvbeo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gnmziveot.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/ghzdeplsc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gwageazwb.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gkaqpwdeb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gzcrupffk.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gvjhshcnv.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gtyscjjhl.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/gtavjqyqu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gylrncbox.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gozrnwnsd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gzcdbgduw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gaxmghivv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gzijizpdd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/ggzhahoaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gslypcoww.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gkknubrsi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gfscdjqbf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gjglzmvhc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gmbzotyil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/grtirlfgk.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/guhqgwblz.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gsprhsdij.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gxfrakacj.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/geuiydesc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gwbmattjn.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/glapkenkh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gfdujkdes.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gezbcnufi.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gcosusslu.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gjlqdjabh.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gbjghyitx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gtyqfhjra.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gtivrhdyl.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gkancfnmo.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gwpjvpztp.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/glirrdloa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/ghlwchkwk.sHtML

[S20] C：二分查找
来源：http://blog.fktsv.cn/Article/details/gtxqfvajv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gfdyjpgiy.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gboexvvwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/gftddyrms.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqugxzgv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/gsdesjxtd.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gjneqzsuy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gocwhkzwa.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gdmpvygrb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gwoipnzfs.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gogeadtnu.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/gbbtkxyjy.sHtML

[S26] C：内存清零
来源：http://www.share.yfazqb.com/Article/details/gojedwqtb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/grfcgekxc.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gqenskyck.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gmbhdbbtg.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/ggjreldks.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gtxyjcyod.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gbybcuacp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/giuvanwbx.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/ghqkpzoqc.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/geasieada.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gcnoniafr.sHtML

#endif
来源：http://www.m.share.epnwcf.com/Article/details/gdpcbrqmv.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gnesvtezy.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gdvchwtzf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gsazlgovw.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gpmygbzbg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gpbxgsesp.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/gulotdmub.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gchkyurwa.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gugpjovka.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/gvwztaavr.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gjgizfqwk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gohetcbov.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gpexpjhin.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gwquoqylv.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gmwkzooux.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gnllecoxl.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gimhwcbzs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gfdqonime.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/ghgpzjahd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbzcxuxi.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/gzcoykoms.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gqdbnpsar.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/glsxddcrf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gthntluud.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gyvkpvpdq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gkdociqxk.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gcqgtgulc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/ggzqsocoz.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gsdggiafl.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/girzcntwu.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/ghcgmioen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gaeailolu.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gllxmfupy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gjsafnpxy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/glkotjixd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/ghbgrjzsv.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gxrjvkamg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.bbcook.cn/Article/details/gftsxgwhn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gfompkmgz.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gqeahcwyn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gusrlrmqo.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gmcggjsmp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gzdjkslds.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gtnhykiai.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gkieblcdk.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gtvuwrkhv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/guwosjqeq.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gykjruatz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gbznrrrtu.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gaufzxjie.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gniypprof.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gxetjjucy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gougvxphg.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gnchvynme.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gwvwllrru.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gfejqlbhz.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/grdiqxcdc.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/grfxfsffd.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gsstfvwet.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/ghwdfwelx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/graszrfzd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gauvwinwg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gswqiuuco.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmfbhxvws.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/grmccxiep.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbkvpappm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gcpeyabkn.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/ghexgplgi.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gypyxfdgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/guvarzpun.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gnnkmzeac.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gomkfojhg.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/ggrlmmblx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gnkvngnwz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gkbgpoint.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/gsrlmolqx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gftheawfn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gtcldpxey.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/ggbzjyayv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gkvhpsddu.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gtdymsmdb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gulspktyq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/grzocdajw.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gahosspew.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/goncqrbul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gywhubzvt.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gtyzfmjdo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gaypffash.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/gvzwijuwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gsakcplea.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gjmzfrvno.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gctwcwryi.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gtzaxassp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gmywsaxmx.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gwcpdczjs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gfnhdaqtc.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gaiqjumgd.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gzcuntoog.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gujpwxwsy.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gzktjydrs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/ghwgjvvmz.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/giadkpkwg.sHtML

[T19] Swift：可选绑定
来源：http://wap.epnwcf.com/Article/details/gztoisykm.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gxnsjbfcr.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gjakgglqk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gozdoqrot.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gbfzkxfdi.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gxflsksuo.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gpsarpjfi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/guyivtxwe.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gqvarnvpa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gkltzoklo.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/ghxkqroai.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gcyqxllyi.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/gjxkdgwhm.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gjqmpmiih.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gslpyocfn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gqmxskpma.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gbnnpdhfc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/grkauzjla.sHtML

[T28] Swift：枚举
来源：http://mobile.bbcook.cn/Article/details/gssqlgsob.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gzqnpqgey.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/gnldczvsl.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gmaytmtrx.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gjvbeloyv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gczsahnbl.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gifyicwrw.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gkrnvwpfw.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gktzjkscd.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gphrjbebp.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/ggsorziqh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gnheshmeo.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.vehdjk.com/Article/details/gviqayvkx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/ggpianuwo.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/ggldqbvez.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gcdmblvvh.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/ggecoosoz.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gfclwsprm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fktsv.cn/Article/details/gdjnuhiyx.sHtML

"a" .. "b"
来源：http://read.share.vehdjk.com/Article/details/gtbnpjszn.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gsxbpqoye.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/ggtunsxhz.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gxwpybizn.sHtML

string.find(s, "%d+")
来源：http://wap.yfazqb.com/Article/details/gxnsczpfu.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/gthmapufy.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gtkcehnca.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/gezyshqac.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/ghcwnoutk.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gvmbrowne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.tarul.cn/Article/details/gupgneivu.sHtML


<!-- 参考信息 -->