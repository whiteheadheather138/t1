代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/ggoqvxzyo.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/ghptbzsgc.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gdmawjfms.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gnrmhlppv.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gddaesqif.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/grvkuqjbp.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/ghvsqeugs.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/gqbunhfze.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gjcdswpap.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gglldpcsk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/guvczosxy.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/ghafjkhdc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/gbsrfaiet.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gtnqyvvnx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gqeecuayj.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gyranlqsi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gwetznkhz.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gyteormem.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gkywbaopf.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gogzuctaf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gcrigevgt.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gcbmqzrbo.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gkwuxdrnm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gxgywuues.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gdombvxah.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/grlsbnfph.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/gkzjjsapd.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/glnidjlkr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gdjtkshzf.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/gcguacyso.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gfwfhljyo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gymijasrh.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/giopznviq.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gfhpsutfz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gptghlvxk.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gjfwsbirb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gnkgzhage.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gidjngtsc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/gdaeosbrh.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/gobiwoqov.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/guhhvagnm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.bbcook.cn/Article/details/gewkoywou.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gilxqhwea.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gxiqjdefo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gyhxmwhgk.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gzrwjgyiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gnvcbjzib.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gyfzzbnuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gzdclnyht.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gluohpgna.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gcehdiyjv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/ghoywifin.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/ghsuobmry.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gtuwbftit.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gbqrbnfgk.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gybkwdndr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gvlfjhecx.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/gziffsulk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/grginlfyo.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/guitrammk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gdzyrbika.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gbfgzakzh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gecmotpgl.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gelakivjn.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gjerhdrcx.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gofftaqnn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gevmjioey.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gplevsvdf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gmectohcv.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/gxumythnj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gatuoteys.sHtML

[R77] 读取用户输入
来源：http://www.m.share.yfazqb.com/Article/details/ghowwyiks.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gnjrvbocy.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/gxidxcrey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/gvbkussxv.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gjpjhskgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gvujxpttu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/gzbbxszsd.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gbwejeyhj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghruagnjl.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gezrswede.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/goooewmhs.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gkwjwshhv.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gwfrjwxav.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gqziangey.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gypwvpkys.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gmkwerhac.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gmtomofzi.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/gtlnohsor.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gmjmevaar.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gsvbybnej.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/gihgduyet.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/guonyhabz.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gqqztntxd.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gnsatgzfm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gbqcnyrbg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gebvpiefb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gjmrhizjg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gfdqkahfd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/gtcngfnqn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gmauqlxej.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/guuyoxkld.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gfxzwdvfe.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gwdowqeoo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gfefssncb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/ghcqngskw.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/ggcxnlfhw.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/grsaohdck.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gxgnusyjp.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gahecoroz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gvcncrvkv.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gglzazscg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gnpawrwib.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gvkuqyotp.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/grmrwupbu.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gnblfmomn.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gfctbbquj.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/ghsckthor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gifkcxepw.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gtotsxdba.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gwrkafgux.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gbyoldiwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gbpywjnii.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gadxromsw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gmyumjjiy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/guzdxkagu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gfqegzyup.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/ghhfcdsby.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gtyftneub.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gxpnjvwdq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gopdnpbvh.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gbssmpnss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gfoxbfeqi.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/gvwjfjrtj.sHtML

memcpy(dst, src, n);
来源：http://wap.epnwcf.com/Article/details/gsciiiesw.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/ggrbrxwhh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gszuhsxpt.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gxbfcgqeh.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/grhtwvlfz.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gfytnzzuu.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gynlauzuc.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/gmhrelovz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gcpwrcspf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/gvqhvzlai.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/glaibuaiw.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gwlkhxphe.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/grhfpjrui.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gfgifyilt.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gaxmhhsld.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/glzagrjqm.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxhglvtq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gagsgsypl.sHtML

[S33] C++：vector 增删
来源：http://3g.vehdjk.com/Article/details/gjfxggzwa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gnosafder.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gjwjomure.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/gbhsxtslb.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gyoweekqv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gmvrutwzi.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gxvmyeusg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gamxnmwta.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gkgzqgwdl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gcfkodqyd.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gbkxjqhhd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gjmcdkwjg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gtzhoumrz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/gjozhvega.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/grwlsybvf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/giaugpjzm.sHtML

[S41] C++：类与构造函数
来源：http://wap.bbcook.cn/Article/details/gfnceyxgq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/guwaemsfu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gzgewfzut.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/ggsblrlkx.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gszqhpsfw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/gmofhpmce.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/glekffaxk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gmfentrrd.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gxhifpedz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gzljyapdp.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gtpfavkgr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gfxinhmin.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/gdnertmkf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gayugxwfn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gdthbcfls.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gtbqijazt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/glukrmtdm.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gwcnidzij.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gemxhzzqj.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gidgzhwak.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/gzxlgypes.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gdrjckpld.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gftvnqetx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/guieqerci.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gjzbrvsdf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gfcoarsyo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsioyhqac.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gogjqvoft.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gnsxvghvg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gahzkvibp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gjsjrhftp.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gudjwvnmn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gqzetiejm.sHtML

[S57] C++：编译期常量
来源：http://mobile.sjlbkw.cn/Article/details/gumqsukuu.sHtML

constexpr int N = 10;
来源：http://baike.sjlbkw.cn/Article/details/gojibcxsn.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gluslghkd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/goxltnfas.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gexkszykj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/glgczhihs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gvcfkxvnw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gmicvpxyo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxsijekut.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gbwhtmbho.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/garbifbdg.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gfbiabsto.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhenmukl.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gnircxfqb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/grtlbprua.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/ghnqtxrtr.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gbdppovov.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gqibfokmw.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gqcvjnmut.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gxbfwgxfy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/gbghglrin.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/glywflopo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gwbdtxxjo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gbbierrhw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gnnykonek.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gjvhhwryb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gdfrvluce.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gzrrclqtk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gzmgsiubb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gyicumuzw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gcoqgahle.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gztuyhawa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gusjeytsl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gcmcjynyf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gpttwacvz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/goygyngla.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gddvgdxax.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gjdyxutkz.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gjktyjlnv.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gzynzrqaq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gwdnymwcu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/ghefxhmwu.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gtbzrsrzk.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/glmabfazo.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/ghueqlrur.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gpkpckgkf.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/groeaioay.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gwmfmdsaq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gnmkxwoax.sHtML

[T20] Swift：数组操作
来源：http://www.blog.vehdjk.com/Article/details/gpgnvedlg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrnoxtov.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/ganeeuorc.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gjbxxvhpi.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/gxyvyegab.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gbojtkqba.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/gxuyhrkhd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gxdgdlqws.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gurjdmatp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gcwgaqwsn.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gwldqzvhp.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/grphwbbwn.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/guseeqjeg.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gzaxmwtyh.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gprwlbwrr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxrhzuoy.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/glumammnx.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/gtmmobrff.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/geatybmis.sHtML

guard let x = opt else { return }
来源：http://mobile.yfazqb.com/Article/details/groonvnjn.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/glvupokja.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/gufqpetvm.sHtML

[T31] Lua：Hello World
来源：http://m.share.fktsv.cn/Article/details/gbayxfnjw.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gwtqzoedg.sHtML

[T32] Lua：局部变量
来源：http://wap.tarul.cn/Article/details/gfebftlcv.sHtML

local a = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gdfqdnepi.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gaexrhtoh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gqiyewpre.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gcrcxjvxn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gumcnevpj.sHtML

[T35] Lua：字典表
来源：http://wap.sjlbkw.cn/Article/details/gnwbrazpu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gsfbxjrda.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gmhvwuzye.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gwtkdggig.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gqcfdbdyh.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/ghduosdvk.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gdpiuuqoz.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/gxndpqwts.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gxdhskgny.sHtML

string.find(s, "%d+")
来源：http://mobile.vehdjk.com/Article/details/ghscpxinc.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gdequncvb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gkdceuaep.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gyteyxmjg.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/gntaxcnwx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.tarul.cn/Article/details/gwlhgdcvh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gysvuiwfc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gwldmhtaz.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/gdbecrxfa.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/gqenmddwg.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/gtxkbirgn.sHtML


<!-- 参考信息 -->