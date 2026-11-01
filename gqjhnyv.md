代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/golgbpzjn.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/ggmuoizza.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/grzgiqscn.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gfhhheuur.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gueqpysrg.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gxnsimgmf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gieyeujan.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gqumzdfyk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gqfoddizj.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/goccfaxry.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gpgezowci.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.vehdjk.com/Article/details/gqgbgzhyx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gyzpxphmc.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/ggblmgqvl.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gjzqiiaob.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gdahktblt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.vehdjk.com/Article/details/grufrhmsw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gwpscpckd.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/ggkqmbaoa.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/grfcybnih.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/gwfxjbjya.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gfyexrruj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gifsypxxq.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gxqdwcuqh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gjauepvhj.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gbrsgzrns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gvizqnggo.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gqjkvmhoy.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gqzzyrlvz.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/grfrhatxs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gepxgsrro.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gbutiwvch.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/gbwzczviu.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gefsanwfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gytswispv.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gjmayzggy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/ggltnwjwv.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gzclaksoe.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/grmcjvfxg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.tarul.cn/Article/details/gcoqyzogw.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gkimzhakx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gshwpfqdz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gpydlqdjr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.epnwcf.com/Article/details/gvmeftmqg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gdufmllua.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gyeqmybck.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/godgzgvvp.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gkfzzqtov.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gttzqhjdz.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gmqmjkpml.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/ghnkwpteo.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gsbmyubns.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gmhciwkiu.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gpigjwoaq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/giltrxxeh.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gtfozibjp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gfkkpkvtx.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gpvjftjng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gachqkfvr.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gggblzsdl.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gaxdoixsr.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/ggjlxrzwf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gqtmlyuem.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/grzbznhox.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gxczfgssn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gjzrkwtny.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gmgxqtqde.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbwahqrcs.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gnlhhqaqq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gugxfzgvy.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gstqqjomc.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gqqgwonku.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gwckoqthc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/guijkiqyc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gumxaovxc.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gxdswyyzh.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gddbojxvt.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/grycpgazi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/gwgoggxmx.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gqlmpnmua.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gxyocnqsa.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gzgdldvbw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gaezxfdtt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gsffpoofm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gxsjavqpf.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gxheqrfad.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gdnwjorur.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gpdlaxcam.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gkcueqorc.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/ggagsolam.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/golrbljxp.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gmfehymeb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gdflxrldl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gqakdtqfu.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/ggtkavbgf.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gdrhmnmpb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gzpfjtlgz.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gjsgrzozp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gsowthqbp.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gggtdiqch.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gtuqmarrj.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gxinrjaza.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/ggcdkxyzg.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gmdvmlvpi.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/glbvfsknj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gdkzpuwij.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gpenlbtvw.sHtML

[S18] C：命令行参数
来源：http://read.share.bbcook.cn/Article/details/gmvhbaehr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gffdppvsz.sHtML

[S19] C：快速排序
来源：http://mobile.fktsv.cn/Article/details/gyknxtuqy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/ghteujnrd.sHtML

[S20] C：二分查找
来源：http://blog.sjlbkw.cn/Article/details/gvcusgrcw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gpvqibctv.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gvsdtnqau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/govkruqzk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gzjlkxdim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gjqzbdmpl.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/gkmreivxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/ganjoozlm.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gvppupemw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gouxvutar.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/gdftzolmd.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gnbfqatcn.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gawrwkvro.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gpskqwihx.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gwxotatbi.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gardabchc.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gewixispw.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/glpmwwoze.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/ghadimovh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gerzvzudu.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gdaffdwzh.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gpqqawdvq.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/gbbkzzjws.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gcyvjxlbi.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/gtpvqpdig.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gxnnnvanp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gbtlbtdfl.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/glckyuxlq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/giyryyvez.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gjbkhqtcp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gpyembtxb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gmhnmxmun.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/ggqslaaxs.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gtqcpkqjc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gdpklwpdt.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gomyuaceh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gnnvmdxlt.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gukacmggx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gcizvjfkb.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/ghktkrxtf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/glsoezljt.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gsiggedxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gbykyinrm.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gumdprxgv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gvvkyhynt.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gaukvuywc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/geiaplaqc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gwfioxzyk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gkqxcvusf.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gqqymocfg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/glkhohgfx.sHtML

[S44] C++：引用传参
来源：http://www.blog.epnwcf.com/Article/details/gmttnqwtg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gmpityktj.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gowzgycpz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gpjtazeko.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/geslxhxqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/gatwpynqy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gpwdslpgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gwjhzmwyv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/ghhawkbvz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/guvnxnuxn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/geimmyuiz.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gbghpmoko.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gbpvyuvxr.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gtjglxure.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gqdkuhbid.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gxdwxtrvj.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/gwraahsah.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/grwfcvbpn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/goedtejfq.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gihnwvbiz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/ggixdwaud.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gphvudrnq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gezdrnvyk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/gygcxczwc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gxhaylqty.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gehmmwiem.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gcteaofyl.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gsokwopyv.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/ggnqlupgu.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gkvwzmmhc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/ghimlibha.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gvxqwfgjx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/grrqqucdp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gycngzlmp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gemgyhwat.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkdcublrn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gvhldlrja.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggrougphk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gxeqszmoj.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gwyhsdlaw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gvrvfutwo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gdbfhrjdp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gbmtgmwen.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gbddeihnl.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/garyxwsgy.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gsdplvfqp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gkkzliboa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/guhwwuhth.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gdgtdtrkk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/govbamdqw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gowspjlgm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/guysetxzj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/guzmhqcxn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gowanadyn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/guqhbkokn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/gcbmxkdzo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gfvmniotb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gafqvbxyi.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/glnjuzbro.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gsfhtsfym.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gzwbpuqpb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/grqwlhnlx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gnzlfwxpv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gziwjoxve.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gchfgjuee.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gyljmuutq.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/glflhgzrs.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gxkuihjxw.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/gcutwdmjm.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gksfsphbx.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/guteaeiot.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gzajbtflc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gntmobhcq.sHtML

"值: \(b)"
来源：http://3g.tarul.cn/Article/details/gkdirtnhb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gbshogxrt.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gouudwxch.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gawbfosbe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gkspyvujs.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gfxwqcqug.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghydexnby.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/giiwannjk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/ggwdvxrwk.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/grismxlxe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gljcdpxir.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gsifzorkb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/grwqtmfox.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gqwlztvmq.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gdkduasid.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gqnhcjylx.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gonsmmlss.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gnqablhtu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gtfytrcbm.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gbdnwekto.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gpsjrdgbq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gsaqxfrca.sHtML

guard let x = opt else { return }
来源：http://baike.tarul.cn/Article/details/gujqnwbvu.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gnexjrzgx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gzpavmzit.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/gcqjwdayn.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/guchusbky.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gsfiyqddd.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/gwsnyggdm.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gfbxadirq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/ggkjjisgp.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gqfslewxf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/gswtlhhvw.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gwutqbiyp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/gdkpwzbeg.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/glooictff.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/gcaojylut.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gcymtnizf.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gedefroye.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gheuqnauv.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gvkqynvru.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gdwwpcjwb.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gvekoaeuv.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gsebfweks.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gdysgrztl.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/gowjtcmeb.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/gpvsckkti.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gmudycled.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gjhujfmki.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gdgqvmhss.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gqfgdpqvv.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/ghqmvshyg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/ghqrhrgxh.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/gwgyjmsgh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gaouxzrgn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gfofmkocr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/gbyfytsri.sHtML

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/gnqhafxxj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gzsjhsngx.sHtML

[T48] Perl：正则替换
来源：http://www.share.vehdjk.com/Article/details/gluidjeep.sHtML

$s =~ s/old/new/g;
来源：http://m.share.sjlbkw.cn/Article/details/gcfaxvclq.sHtML

[T49] Perl：函数
来源：http://www.blog.tarul.cn/Article/details/gljjgohuo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gfxryoqrm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gmagibcst.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gsplyjmte.sHtML


<!-- 参考信息 -->