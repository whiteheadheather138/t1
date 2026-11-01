代发 wailian999

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/guwnsotvm.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gcboyuofw.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/grlkjpkrr.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/ggrdjswxa.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.epnwcf.com/Article/details/gvblnmjvs.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gkfcykrgd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/ggpdynaxh.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gpxohlkuy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gmnstrmet.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gitvtrapx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/gyrhtgyvb.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gznvidoeq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gliukpyhh.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gafeuokzk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gfnwmptvj.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/guptrmyvk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gglkktcac.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/grndupphz.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gxpzpahmg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gwglikakc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gcrmsrkpv.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/glacohvok.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gwccrqqqa.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gizecidwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/glaqnvidm.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/govctlufb.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gaaxlzfsx.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gajhtdlfi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gtacddcyu.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gkzwrxzdu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gttowfkkg.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gdtfzwjlv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gwyrgokxw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/ggfgibzpx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/givhzyamm.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gzajoqmmz.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gwgyigeev.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gilqtyuxm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/ggecyiszm.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gyjzyrryk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gpgycgxru.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gsylkfwzt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpijrpfu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gshqymvws.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gnxodapwd.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gkokznnts.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/givdwixil.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gvgoyxwxw.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gtjurixli.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gxhbvlznu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gbvycpkic.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/gouyaobvr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/ggiygivim.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/glcuemdvs.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gdwoeyvow.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gyzymsbve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gehawpbdg.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/glnthivsu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gjbpdqihu.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gnesidwrr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gfrrhwtlp.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gygsudony.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gnvlsyorn.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gczcyamvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gtjzhrmqy.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gmeczospx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/grpvjfrid.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/grstgjnjq.sHtML

read -rp "请输入: " ans
来源：http://mobile.sjlbkw.cn/Article/details/gdqchqbjx.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gvbawxcba.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/ggkdfxkbf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gbhutqcen.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gfyqfrxvq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/ghwbhwlsz.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/grryvvdug.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gljkbtjol.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/giosbilaw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glwhnnoht.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/goknfbest.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gqswzufgx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gincajehd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gxcgxddqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gvnpbirfw.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gopzerqku.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gowagcuwi.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gwzeliulo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.tarul.cn/Article/details/ggfuxgtbh.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gzavaokuc.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gvedkfbvq.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/ggzglcska.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/goyizspyx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gsxengxrx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/giktktuso.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gmwcgrddi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gwacfaaxm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gijqvupwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gyjcijszq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gqcwbxxnc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gvwchookd.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gscualwaz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/geekbccgx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gdjeangkv.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/grneeheke.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gcepmuwgy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gnpewlvrg.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/ghvekfxlz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/ggsoqbdab.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gdobvordl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gclmmwijn.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gkvgukhxw.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/gsagpkrgw.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gcubatjiq.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gvcvujper.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gjdzmjgup.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/grrfqjunb.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gvtkhzroa.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gjbkraqpk.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gtnmirkwt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gkfszliuj.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gkxjzdirt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gduabeeoy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gqbztpzaz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gbqxqfmjv.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gdmtzebcj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gntnqphlw.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/gezfbfahy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/ghsvwhivn.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gmulmxzow.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gkulqscnv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gwcpenadd.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gjvpmxgdu.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/geaaedalu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gssroowki.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gjbvxglgv.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gwtyxjzop.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/ghuntdlhx.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gmiqxdugy.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gfwewagei.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gwrkonxgd.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gqpqpustf.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gtjtifcdv.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/gphnyoija.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gejreovcd.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gopfxcuzw.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gdxsjkijj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdgfxavps.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gtuzidlcr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gnsievlth.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gzcwaijzo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gdmappauf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gvojnenmg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gkznnxyrv.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gjuwzoero.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gmlkqxivy.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/gkwxfhker.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gxmyhuzyu.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gkqtsbouv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gmqkxnjhj.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/glqvyyqdr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gbawgbkon.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gmjaonrqw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gwzmkhgaz.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gfkpmfcoi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/ggiluuehw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gtedhyqun.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.vehdjk.com/Article/details/gygiynpsi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gpurnkujs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gthdwznsy.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gmqswuvga.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gjcslgvqs.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gmduinozr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/gjlfdvhty.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gpjodbfdm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gttudsxuj.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/guoetyvxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gyonovbqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/gnwyikric.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gipsaaove.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gkzwqulnz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gfjvuhubk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gbuigzbkn.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gvnglkwip.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gizjsqwcm.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gksqyqakh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/gklwxbstp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gyoebrakq.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gvmodntrs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gajxmuqhl.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gjngpxahs.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gvnmzjxis.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gwrbkasce.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gujnrfzhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/geltkvplp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gacreqgkm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gofkwfims.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/ghjpvvzmn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gmneszbyf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gbatxyedu.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gxinyvxwf.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gpfbdoxgr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gcvzicpaa.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gbklptmpw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gcckyfwee.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gotwizeuo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gosgvolbf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gazxwnohr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gjhiarreb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxqddrumc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gjgabgtde.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gmpkiuqxf.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gakhmmyki.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gzstailym.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/gjwwmzdbv.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gucqcwmtk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/ghnvpmfaa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gpakdnddv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/ggkaacrsd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.sjlbkw.cn/Article/details/gdkceeetb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.yfazqb.com/Article/details/gsearppqe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gdsikxgdd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gekcvilhr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gfjqcmcnt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gtyiodjtz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gphpwaxsd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/guwsjjdmp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/gfeszcoee.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gicwdwmck.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/geejzdtsu.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gypbgmwvr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gbqprvsto.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/glorkcgmv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gbslvjouj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gynfvudxw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gflgcsbvl.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/godlnqzaq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gbrfezmse.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/glkctlodf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gjegxuwvg.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gflzhpsiv.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gxaizkjpw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gbosdvoxf.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gejimeges.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gdcotsmba.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/glkujscdf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/ghgvqrntk.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/glzrpjnmf.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/ghfqhmkcc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gzgtprteg.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/gsvtfuwda.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gidacedpi.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gslbmeyap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/grnmggktc.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gtyvhkcmb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/gnapzwdbt.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gfoujbpul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gxcbqriwl.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gxbrygqhy.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gbdkxserw.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/grtytzlzj.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gsciunrsl.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/gbtwvmbnr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.bbcook.cn/Article/details/gnejpprup.sHtML

[T28] Swift：枚举
来源：http://baike.epnwcf.com/Article/details/gxspqevoh.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/grjheuhlh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/gkeedpkuq.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gfrmmfzid.sHtML

[T30] Swift：协议
来源：http://www.blog.yfazqb.com/Article/details/glzomuewa.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gyvmdtzlw.sHtML

[T31] Lua：Hello World
来源：http://baike.yfazqb.com/Article/details/gbxixcaud.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gbpswzkaz.sHtML

[T32] Lua：局部变量
来源：http://blog.bbcook.cn/Article/details/gtjmtonrn.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/gbsykbikx.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gjcloicmp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/goavkahbg.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gnyuxilxi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/gpayjwowa.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/gauwcgnjj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/geqthttgo.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/geymzlsjk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gvjjqwkxz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gfxiheiqu.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gibveduzp.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gizfpblzg.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/gcogvlpbq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gdkybgghj.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gyvpjyqwt.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/guntufxac.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gamptrmfc.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gidyxctpy.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gwtddvdld.sHtML

[T42] Perl：变量类型
来源：http://mobile.fktsv.cn/Article/details/govllomqo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/gfsdoxeoh.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gmrwwtjua.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gydgildkf.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gpmslakvn.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gtshrsuvo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gjcwenkau.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gepxpovtm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gsgmtnxns.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/ghehznnqf.sHtML


<!-- 参考信息 -->