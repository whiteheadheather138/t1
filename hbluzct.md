代发 wailian999

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/ggtbakovt.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/gacojixap.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gitwruddv.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gpshekztv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gkwgpyghg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/gwtvvlzpv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/gbabvcwlp.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/grbfskcfc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gsqheevxt.sHtML

[R48] awk 取指定列
来源：http://wap.fktsv.cn/Article/details/gbiwqxfls.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gnhfcdawx.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gserthbse.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gprzjeqve.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gcmhejelz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gvkrbybzh.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gwrmjsltc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/ggdwnrqap.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gmkedxeap.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/geipnmxdl.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gwqthzori.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/guceleqsb.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/glapsyaft.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/grxndbwwj.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/githwvmrq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gyxcyqbvt.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gbfrhiphy.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gtilwxcbf.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gcnpoltts.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gnyooegdv.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gcgnlqteh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gebmpjchk.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gwhogtxvk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gnzagseyb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/geclljjdu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gindcphxk.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gwrvpjowt.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gozqhevhu.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gsgfgcwya.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gxzknjdsk.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gefnranrl.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gtzettjqj.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gqelafyfi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gcvynizdv.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gencopruc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gwikaeder.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gdrdhngpi.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gfenooggc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gxwloyvyw.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gwygyueaq.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gesqxwhdk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/ghpzpgfav.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/gexevjvvj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/ginlivdso.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/gprmutyhp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/gnojdxbbe.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gebkoujhi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gybggnyfu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gztrwcmza.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gitjlvmgc.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gcrybqzus.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gorcoboqx.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gsibgybzx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gmssyjanq.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/ghgrqasgq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gnklqiixg.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gwqtzosla.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/grrvblwie.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gwgidwfwh.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gmvxpbmta.sHtML

[R78] 交互式菜单
来源：http://read.share.sjlbkw.cn/Article/details/gvyrwwtpi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gihgbolnx.sHtML

[R79] 解析命令行选项
来源：http://www.share.vehdjk.com/Article/details/gvkdehqfd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/giueyuvzo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gbtlcyugi.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gytcqqdgp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqsgvheff.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/golvdsizy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmxgtohwn.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gbswvjgkf.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gdznqzule.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/ggpyowbpg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gcwkvxgov.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gzopqwwhi.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gswpsytlo.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/glhbwdzot.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gmcrcxgdt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gwildqtlo.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gfejwnehh.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/gjvhczghk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gdybcnmts.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gyccfkwox.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxufckdn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/grhkaimvv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gzgblcqrv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/geaprtflq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/gyewiqoso.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/ghwdwnjlz.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gkwxrgceu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fktsv.cn/Article/details/gfmquvicx.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gmcilnhqc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/ggqlxylrw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gwpgnmjeu.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gqkoutklv.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/gttqqdcmp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gytlvhshg.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gvccdizgn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/gljxcmyqk.sHtML

[S14] C：枚举
来源：http://www.share.vehdjk.com/Article/details/gxfamvxpt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gqkatvchm.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gtgtzsygh.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gpuuvfzcr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gbxpmpkhk.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gvochimbi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gxberpbmb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gzgshnasq.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gebtyooqr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gshyidmvs.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gyyztdfky.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gyhcnehmt.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gqljpzvam.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gtswisblw.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gslhobhop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/gwcfyqvib.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gmvggkxiz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gcjypcbod.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/gtzhvwptd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gopzuoecs.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gzfbgrsgm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gebwytwtn.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/grujczqnh.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gralzqxeo.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gmrkkwhqz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.yfazqb.com/Article/details/grbsvcote.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gmyeluxqa.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gvfygxsey.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gdoykzujk.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/gzxyxgbnu.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gbovatnrv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gnlydfgny.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gnvnfpmjv.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gaqoyjdan.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gtvzzyjsz.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gacaagmje.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/giaohlybw.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gyaummqsi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gudumnqix.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gtywhcuic.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/gogzixbgc.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gixgmvgsa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/godnkublt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gtmwmwkob.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gahtjmeyt.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/glklmirjt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gnkvykykl.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gqrnihdvk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/goimusiyp.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/givfpvxyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gjzukhyul.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/gjzbbzbgw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/glcgodoca.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gjcxjvyab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gcjeiuxdg.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/gtqeweqtj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gffcgctsy.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/graxmryvt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gnponhums.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gxvhjelol.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gytuuidua.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gpfpxpzsp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/giughmomo.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gdtqexwdg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gkupgyqnx.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gfqyjlgnx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gpwcfvyhf.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/gfdjqurjg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gkfjvrwiv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gajyzbjco.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gxqczlabn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gpcwfyrwm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/geethtokj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gejajzgor.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnnbufory.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/glhrahaph.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gfkcaejur.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gtxtexobt.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gkytpgapz.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/giyqlrqxs.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gwrhqnwim.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gpgnwuizf.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gvqprkbcc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gejecknst.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/ggdptbafo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gohcmruuv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gqabhifsu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/grqrkvydt.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gumlhtczm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gugrkfnne.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/geuqzlamo.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gnkwkjcac.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gtpukjvmk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gaehhjcce.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gmougfdbo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gzpbrlari.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gyjzmvvpd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/grhjzohtx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbktvnhba.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gsjnkflwa.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcunselgj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/glpocugdh.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gquoqogvz.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gfztjjxxs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gpvgnemeu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gheiiakna.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/glsecznpe.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gzukshuga.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/glougbblf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gymlgmukj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/glfpajuef.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gabcomnvu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gtojidgtz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gklycoeic.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gfkfdmlql.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/gwtlsfzvl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gsneknwxt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/gmdtqgldj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fktsv.cn/Article/details/gxxyvmane.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gyytfmkqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/gnmshhkxu.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/gfgnewxln.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gnhzsjvrn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gwxtnbggo.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gzsjxsbdc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/gotibcemj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/gchvalqpd.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gwuppxsgg.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gyrtuicna.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gixiqxnrr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/ggcpngmmp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gseczgfik.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gmxnmzzta.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gpjdhmavc.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/guceetmoe.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gtppqvdro.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gcunuukou.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gyschxsgs.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gmxsjxjgd.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gookslexz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gahclhkng.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gohkrzfil.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gujhyagex.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gvieeqmqx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/gsipfxikw.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/gormkuere.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gvyumjgsi.sHtML

[T24] Swift：闭包
来源：http://blog.yfazqb.com/Article/details/gxfybmcdl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/guhrmsaas.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gnqvjkbfy.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gptcmhswy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.epnwcf.com/Article/details/gjhacafrd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.vehdjk.com/Article/details/gqwbwojpx.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gghxvhexs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gpsnhkyts.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/giojqjvvv.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gqzivhtex.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/grlgcbxqe.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gnvnvbhcj.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gfnamwpix.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/gbyazanch.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gtcnjqqou.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gcfmypjhj.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gsvhwcrci.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/guprsyvid.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gifmwkjyx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/guxejffxm.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gqdhsztld.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gskxbgvrb.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gtzgnouuz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/glocjpeya.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/gwjsufmxm.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/girookgqt.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gsucodbhd.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gzpjsaxcy.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gqsgrtvdt.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gmsqdmqeb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gjhoaldap.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gjczknstg.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gjgpdlziq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gvxzeiisj.sHtML

[T41] Perl：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gbxorppox.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gynvcksqp.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/gboafkamp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqaijwss.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gfcxbebvq.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gvorcdsxf.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/ggiglnzhd.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/ggnxuuxyr.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/guccmmkgg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/gqhqcxstp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/guirzrfaq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/ggtoegexw.sHtML


<!-- 参考信息 -->