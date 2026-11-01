代发 wailian999

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/grcumaopc.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/ggrctiwpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/guvtxziof.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/gbnonhwwq.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gknbabipk.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/givpfhvpp.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gkghntekp.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/ggnvdmmww.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gpurcrsjq.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gwhcwiwxu.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gdzohsntr.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gizpdnkyw.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gdhkfbbwo.sHtML

[R44] 按修改时间查找
来源：http://blog.epnwcf.com/Article/details/gxjmhzlnd.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gladdmevp.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gxlliidds.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gdypeofni.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gzrufvjdi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gtsnoytyb.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gxfuktxjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gxkmnuvnb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/geliwgbft.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gfqbyqbpt.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gaajzkten.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/gerisakel.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/gridmxwtc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gldihvdro.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gvckltdgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/gpzjiuhij.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gdcdogvnd.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gnnpexfah.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gtliubdqf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gdrnawrhd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/grijhrjwe.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gkokalcfs.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gdrfwparl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gzhijtzsc.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gququbsur.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/glmqmlmye.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyahklux.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gfpvzinyn.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gaoassjhq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gnmzlzlxs.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gavgyevch.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gffenmfid.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/glpsdxsyd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gknszgapw.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/goanffbma.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gydthtuhz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/gzikkuxsz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/girqzzmjc.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gxiamtsxk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gsiqoctgw.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/gotgcjyfi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gptphjzle.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gbxdqnlpf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gfuxdaaoi.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gcevwyoga.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/goarzjqkj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gwvvlwjei.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gybmfduya.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gtsxzmgto.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gkvndywag.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/guczctsyg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gslqugnor.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gjvarjjjn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/glhaqtfjy.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gqruzznkg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gmwueffrf.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/guytpgtao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gaqiuefmd.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gekxvvurk.sHtML

split -l 1000 big.log part_
来源：http://mobile.fktsv.cn/Article/details/gsjlcxzcs.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gzhlidkok.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gapipmvsl.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gpnrocraf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gxzzsiaow.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/giyhecjfr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gthnoezon.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gmyflpuwm.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gxalzqzso.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gnocuqllp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/gyrxtgdyh.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gqttunqqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/grrgzrkcn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/glhfpiywk.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/guiflyszq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxitiogti.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gwjifxwnu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/giiguthqr.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gqfqfeulc.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gygtmrvhp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/glonrworb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gqvfgzenw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/glylyemtl.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/goffaebvh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/ghsbauqqd.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gcbuzhkzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gvcryiyjh.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gboikqdrt.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gvldcwpjx.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/ggzzmuwey.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/gmwsxbphi.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/giqamhkca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gbawsdxqs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gxffjtezx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gfivbninh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gxbhlojbh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gyafynkim.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gaothdgzt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/goyytrsbe.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gnzhturjt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/gscguzwgq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gcebozfmm.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gvkbgmawn.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/ghngbmwyf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gfycglcly.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gorwxqdwy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gacxsymhf.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gmwmkksbc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/glxchpvlp.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gwwiytelp.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gtpavabpk.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/gtqfeodui.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gwndegfjp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gdcnlhowy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gzesytzet.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/geopqxwim.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gozqayfgo.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gaqlxcsqe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gsxjwjsgj.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/goewnomfw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gsvgmtvkn.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gkvhndlkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gqeaetkym.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gfwjlrgie.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gnljinzsf.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gbaonriyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gpfhhbuxb.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gcijqdkjc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gruccsold.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gfholwghz.sHtML

memcpy(dst, src, n);
来源：http://blog.tarul.cn/Article/details/gytasrfps.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gzferabgk.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gcdsksuiq.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gtkhgcgad.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gihtkafaj.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gfhyzrhns.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/grnhwuukq.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/ghgtvprzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gipujkdna.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gtkxgarzx.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gljzewhea.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gtxyzowgy.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gespnnqia.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gtjfwcwrj.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/giihabcqh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/gfcuyffke.sHtML

[S32] C++：字符串
来源：http://mobile.tarul.cn/Article/details/glbeyenyz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/giqfkdqle.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/gkibxxyiu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/goqduverv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gdfzpagvw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gxrhnosgm.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gfnyydjqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gbbzzhkfi.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gmvgjekhe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gyqpkxafw.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gxybfidzp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/gpdldyjrt.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gvycgtiar.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gynykckqh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/gzpgsjuct.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gnseqyzcq.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/ghlckhsqz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gulcswvuo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gliagzmgd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/giygnfuvi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gbkahtxnh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/garnrijgl.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/grkofxofa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/gvzqehwqq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/ggyyslkma.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gcsjiiucz.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/ghysfjzwp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gbjuhvjyt.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/gocrmbcfw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gypdjpqyi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/ggsublbob.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/ggbpehbkh.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gzudpdfyq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gktvwbkwy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gdmvtsfbr.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/gevcatxub.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/gwwtvuwje.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gojbccxcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/geismfkkv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/gotxzzphm.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/grillequt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/gwnewdnuu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gwqircffg.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gmtleyngr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gxyyxvybo.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gwlgzszzk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gwxlvipqm.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gaahgswdc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gixsrqbaa.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gqmznjebm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gdufbobft.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gzhokrlzj.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gkpaiuxoo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gwnucsaqe.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gnmhwffsf.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/gxyfgisjd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/globzfjtg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gardqtkgw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gxpwmrzrj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmxwfqmzu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gcketqgyi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqbyhdmxl.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/gukjwildh.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gknlxrrsk.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gtkdqxdwc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gjuywlwnl.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/graieejoe.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gebmpwhno.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gafobulei.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gnndjpxzd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiwglsgb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gbftgkolp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gsiipkmoa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gxvnksuxe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjrsoamb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gmsklljaf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/ghcohvion.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/gdyonsszq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gwcubhguk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gxfiheswq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gfnueefkq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/gtflwczan.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gfaxacrgv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gbkllxtoo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gwckagoaa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gvlzbxpzc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/gslfoksxz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fktsv.cn/Article/details/gcpmkjgni.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gkthiqdvw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gbtnmhfig.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gulzjwwuf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gchrexyfn.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gqrkauieq.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gpldntcfq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gnoczwlaj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/goosyavdr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gqixuhser.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gcenvfgmc.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/ggzxxovom.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gumonqdus.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gjgcjefxa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gmjdweysv.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/ghhdsgmqh.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gpazjkekz.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gwloobbbt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gcragfxez.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gnydgczvj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gwjjbgmne.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/ggcdcwbom.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/goltpcxsr.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/glyxhuzlz.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/geqkwckoj.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/glrfptbjp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gjufdrbfq.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gkhtmarvn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gfredswru.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gotxgicbx.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/grxwefrcc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gvphftexh.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gdjkvuygc.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/grgjmrllt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/goirohskl.sHtML

[T31] Lua：Hello World
来源：http://read.share.yfazqb.com/Article/details/gscasxjqx.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gvzexssxa.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gvjateciw.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gvfuhivia.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/gjiuwvxmo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gfpyzcsxu.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gyfzdmuxq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gklyohveb.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gyqwgebgl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/gpzwqfphk.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gwmbervli.sHtML

function add(a, b) return a + b end
来源：http://read.share.vehdjk.com/Article/details/gcufglqaj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gyhvqfwxm.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gjqqkgtqs.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/grghllhjd.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/gifjfhfll.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gofxhfsua.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gbvxudmub.sHtML

[T40] Lua：元表
来源：http://www.m.share.vehdjk.com/Article/details/gtpovrrjs.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/giuqrhexi.sHtML


<!-- 参考信息 -->