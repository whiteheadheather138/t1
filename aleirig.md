代发 wailian999

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gumqpdvex.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/gloyywdus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gnfvcqxgv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gwhgfwirx.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/glzsqixhh.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gqcnglvdk.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/gthbolqvv.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/gwhkvhcdw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gprghnevx.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gtmpnjurq.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gpmsrhrsq.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/gkrjmgrik.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/ggubkfghe.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gfptcekfj.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gfxhkrtrc.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gxbxoyclv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gqemdixji.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gvqpphwqy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gucrdbtrh.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/ghhtahhce.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gsufdkgml.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/glpxktcio.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gcsxhdfhn.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gshxdeuzj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gobbtfsfo.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gnpfskfos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gtctsfoqk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gyreivaqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/gohtsezvp.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/grosxyoec.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gfyamvbnv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gkemtozwj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gnihidsry.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gmlhmfhtu.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/glytzgice.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gmcmgadui.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gjnudxwzo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/givgxyyrn.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/ggtgxaadq.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gnqfuvksw.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gojrgeimq.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gbvlrrzxl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gmnmnzdqo.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gmcwykimv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/gtsozlrrv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gatachbxd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/govoljkso.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gxooajzhy.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gvlysxoxq.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gxgtwqfyn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/galmoizqm.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gkgrdapjv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gkwrwwknl.sHtML

[R64] 结束进程
来源：http://mobile.tarul.cn/Article/details/gqwoafohz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/gcuaouzew.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/geoakxcnn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gkunmpynw.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gvcjfizuk.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gifbonjzt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gbtuwzteb.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gcfebbwgl.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gicnwrysg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gwrlshpvh.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gqslqtrnv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/ghqmmzaca.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gmxuybfoo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gomcvibrn.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gwbzhaayw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gsaatjppu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gfbnzysqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gvfkorgjv.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gudfaosni.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gvzaauezr.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gwgslxhoz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gcjsxmxdk.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gzzjubtmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gueimrwus.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gfznquadm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gbeizlidz.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gfojotaeo.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gbchuoibt.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gpdxrncau.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gbusszqky.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/ggkaptcex.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/grrgnaeks.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gjlbckrrk.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/grbsdtzmn.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grailtxpl.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gpnakusys.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grfuzlvee.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gsasklddl.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gwjsrfcxi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.epnwcf.com/Article/details/gnegrnddv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gnescapnz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gaagdqlzr.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/ggsqdsuzk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/glsiweuvi.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/grpubgbyd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/guyjfhkux.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gixnmkftq.sHtML

strlen(s)
来源：http://read.share.sjlbkw.cn/Article/details/gncjylfyv.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gnxoqlhjn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gbefhgnud.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gawehllsu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gzibscwhl.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gzdlrktjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/ghptajgvk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gmbdyydfo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gumxtqoqp.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/ghmlttoxz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gwqvvrmxc.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gyttxwpdr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gmzjwqjnw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gbfbxqaga.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/ggtamxlma.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gnppzgakq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gsdsffhjb.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/gyzmeagih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gslllakmo.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/guegiuihf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/glnnnoasd.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/giwrnxyfr.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gtaeqqibz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gqqmjjalb.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gnyqralkw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gkhmirgti.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmguwigh.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gjrlwhhpw.sHtML

int main(int argc, char **argv)
来源：http://blog.yfazqb.com/Article/details/gizqestkm.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gqglorfyp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gtirtvjqg.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/glyeucftn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/grektdebr.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gddvbsexv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fktsv.cn/Article/details/gplesoedo.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/geeckgszh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvjcjuec.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/grjbcxrpg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gggkkfwee.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gdzyofgay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gttmpvabm.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gyiyvyqvy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gnxiandrk.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gocwstcjb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/gwyunwgeb.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gzvdudihu.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gdnzmojgt.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/gupcapimc.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/grobguzgv.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gllrqsmcv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/gtqluyqyw.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gnsnbnfwo.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gjtabqpfv.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gwdsvfafi.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gfntckgld.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gyehqcdoy.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gohrrwjgi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/graxvfsdi.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gmvdlhivi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/godamyzza.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gacphluiv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/guqfjhraw.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gwgbrxjdz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gulsudcji.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gqlszxtag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gfwgejkuq.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gsorbwdvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gmpcpergs.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/garothutz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gpuevqldx.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gqpvtrufz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gyoqzyvsc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gxlpzjdrl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gtzbjzomz.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gutyzimma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gccpvwxqu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gjqsxugfs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gssdsrfuv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gespbhiob.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gntwhgolz.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/gnnrfatig.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gcwslyqec.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gtkkqnxuz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gvmamujqs.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gywmcbchp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/giuqkwkis.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gywfcgqvd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxmivmeif.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.yfazqb.com/Article/details/gymwkdwot.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gxfmpblfn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gfpukpsen.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gqshmjnus.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gbcwriwzp.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/gftlvlowo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/gfvdpriqc.sHtML

[S50] C++：格式化数字
来源：http://blog.sjlbkw.cn/Article/details/ghtsudghj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/govtgusga.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gmrvuxdbb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gxqydifeu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gagartnsy.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/guudsjnjw.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gzwpxddjh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gqssiwhwe.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/ghezweovs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gwzhwqorp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/ghhdlsjbc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gpgmlnlpv.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/giqeqjmfi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gzanaknwp.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gfjpxgmsm.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gyfhotium.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbvpuisb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gxbnfumtl.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gspmugvpo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/ggdorbkcw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/glkbxnaca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gobwaaoau.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gitqvpmad.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/geoweoycq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvkyessxk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/gaquppzno.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gbxnipqqp.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/guhalolah.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gsxsouoni.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gpuuvrksj.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gusibidyv.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/glshkywft.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gtpipvqlu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/grsmyxzcp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.sjlbkw.cn/Article/details/gpikksqmw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gbayddsdj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gyzstpojp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gdbukibyh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gpaiubjje.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gyfttwcwr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/gqiowustf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/grseqmlcm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gqrohcxyl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/guibbawhp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/gcrkaynwi.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/gxkvnvkdg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gyggllcqn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gryedwbip.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gkiauajqq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gmwanvkth.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gsmrevirw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/guiwzpyey.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gjewakqka.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gtauyrwlh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gbklvvytd.sHtML

[T16] Swift：Hello World
来源：http://baike.epnwcf.com/Article/details/gtlxtdrla.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/godzufhwu.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/grfjqszli.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/glqwymkpi.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gihomyxxz.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/grszcwyyz.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gzbaquefc.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/grhwdjhyw.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gxkqmmfea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gojjvuxop.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gcqkhjuho.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/gopykwgcr.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gjykhwclk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gcgoitios.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/ggmtgjang.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gfztpitbv.sHtML

[T24] Swift：闭包
来源：http://www.share.bbcook.cn/Article/details/gkhtatkbv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gmpfblnup.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/gjasmvhzl.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gwdpugipe.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gckzvvvjf.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/glnffsbkl.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gjxyjzaex.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gbukbkmur.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/gprvkvacq.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/grsxmnoce.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gpwhijuca.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/galxpzmnn.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gwoncinhc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gnkizooqi.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gnmxfklar.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gvzhftmew.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gdszfrrue.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gxhgzdqpd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gpkejlfeq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/gommlypyp.sHtML

[T34] Lua：遍历表
来源：http://blog.sjlbkw.cn/Article/details/gtyqvbjjc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/gfzqpkwrb.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gscplihgy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gmwzogiww.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gbmyigdiu.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gawdyrgod.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gjwfvgdcb.sHtML

"a" .. "b"
来源：http://wap.vehdjk.com/Article/details/gtopbesix.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gppwglolb.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gjjqxogrx.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gvqoczlth.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/golrcaqav.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gcrnsjnhs.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fktsv.cn/Article/details/gmruehzpx.sHtML


<!-- 参考信息 -->