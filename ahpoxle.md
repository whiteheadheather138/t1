代发 wailian999

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gawtlaurh.sHtML

[R38] 管道串联
来源：http://m.share.bbcook.cn/Article/details/gwuaomtrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/guebedzyb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gxgcmvfpt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gjzccesey.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gyespjoob.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gaarxeunx.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/ghqntxclq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/giukgfqpc.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gbiqzlxsg.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/grpqlumer.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gaebuiiqc.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gzgkuwvmk.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gkdvvondy.sHtML

find . -mtime -7 -type f
来源：http://3g.yfazqb.com/Article/details/giomsvnlj.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/grblqpsxa.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/ggcsytunb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gdabfrmbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gmfueranq.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/gscoyrakx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/gwoeeizak.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gpvjgvjeq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gusxcddow.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gsaklnorg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gwylvfbmw.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/gzcajjzmg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gekgcwpln.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gehijeggh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gqpjsfnmj.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gtkddsulm.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gjsgehbgn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gjzulamjq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gflcfmysm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/gjdcfmulw.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/ghnicktqr.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gplrpycam.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gpxnagqws.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gxmwlrdrz.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gfeumorqm.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gxjatdvtj.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gnvkpvzdo.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gnwxhqphl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gwfuuvohv.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gwgdebsmj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gvxlhuvzn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gxprdsjax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/gkeqnphil.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gkdvqxlfw.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gqydlidwk.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gqygfttcd.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gvmxootbn.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gothxkuzp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gljfkbaks.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/giescoytl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gyglqpdbu.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gjrvzwlbu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gtvwfzhnn.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gdqliqkye.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gvpvwpgbo.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/grptsopck.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gsitpnqix.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/guqprftgv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gmlxcznsj.sHtML

[R69] 生成随机密码
来源：http://read.share.epnwcf.com/Article/details/gsvuwlylr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gfjngzuzl.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gamoegnda.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gxtwgykdt.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gvefvzhwt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gwgvcznwb.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gtvzqpagf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gmdsqibyc.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/ggtubmtpq.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/gmvxgdcfy.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gmkgdbqpx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/gdlvqhbwj.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gzowoiseh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gdpjjlbzv.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gwhrpeehf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gqfrhtlbk.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/gdaocuoin.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gbgmtehql.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/gemqaddgc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gwsfflrhi.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gcntfabrb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gzyuqpxsu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/gjyruxcgb.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gndizhtnd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxlbccyau.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/gtiunzmzm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gimcfcjkc.sHtML

[S01] C：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gkcabpbwd.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/grgdwsfbs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/ghdiapnfk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gchcfnvhj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gpgnonhwl.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gadqfzfin.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gnczytzlm.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gszsdxhiz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gvdikhkuk.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/ghcapakiu.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gkwuaapll.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gxkpxjsvh.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gxxaiyjwa.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/gdciokpeq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gpcmsslsi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gyjmeqnwg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/grsxmdfob.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gifwwpgto.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gxflxqxsx.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gwjjclbum.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gbcmuuokw.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gktdkvyqy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/guhzqjzcn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/ganovyicd.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gjxesotbz.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/gvcghkbkc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gaamadxxu.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/gedhnwguv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gkdupqkvc.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gyksinuil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gicsmrvfw.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gmodwvigb.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gbpxntnif.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gdvsjknfe.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/guxjkqspw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gebznvzfy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gdascqcvn.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gpsembbsl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gzwhkgudo.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gcoclrwmm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gzuvyjore.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/garmdkvbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/glvmngxsr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gyltuygtw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/ghancuvqc.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gfcxbkmqf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gctcizoic.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gdhxfeuwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gomcdmpki.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gjjryvyit.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gqtcnsycb.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gjgdbfavi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gmqnlyzmp.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gjxxzkxhr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gqnlvdzop.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/ggceqkais.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/geymqxjpi.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/gjtcvoubm.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gogcdfdvh.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gbotbrqgy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gcusarrdj.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/gxqlnhyim.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gwszjozjx.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/guvtvoxxl.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzgmwgjt.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/groggftil.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gbljpggyj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/geqmtktrq.sHtML

[S32] C++：字符串
来源：http://blog.epnwcf.com/Article/details/guidkirvd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gkyxeebfc.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gevgvnbli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gljzrqyyn.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gmqdnatvh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gkhexvbcx.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gnjcodtbl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gzgjmgjhv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gzucomsdt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/glthhcwjp.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gwedhcxbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gqdmxzrlx.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gkuhtcoyh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gsixslvws.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/givgutyzx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gjpmyvdti.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gvbcpbyeh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gqbmehchj.sHtML

[S41] C++：类与构造函数
来源：http://3g.vehdjk.com/Article/details/goshmbbcb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gusebdvjo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gfzuaflfn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gprnznsfn.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gggwcjfrx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gznoclytq.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gwaprfuvw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/ghbnxdshu.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/glcjintvr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gtlzfaipa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/givquecpa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gmpyhkpbb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/gnenbyfwk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/grjoygtcd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gzbkjfdob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/gfsgrulfh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gvtvbxbem.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gvltikbxk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gqzmrdvze.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gkfxvmahe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gnltwgfqe.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gxnitqoko.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gbsvdydsl.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gmkslvafr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/glspucvwk.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gizbwwkih.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gscxjpraa.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/ghtueaasz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/guvmofpso.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gsjsyeyjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gcudsmgoh.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gknfxtyeh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gruuuqncw.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gkxddowfi.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gkphelmgf.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gilxoieju.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.epnwcf.com/Article/details/gvvbgjwua.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gitvnmybb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gknyggzqj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.yfazqb.com/Article/details/gssewhwch.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gdcqetofw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gepbnrwhq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gghjtntdb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwwdtyfyg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gyplldxmb.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gzthftoio.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gqkvrpktu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/ghoomhdjd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gmnnstreg.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/glejpuats.sHtML

[T04] Kotlin：空安全
来源：http://m.share.tarul.cn/Article/details/ghnyjjmyi.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gpduzlrju.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gwysrfujw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gxrsyjzgv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gfjvasauj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gxertfepc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gmirorsok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gjfxuuanp.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gsurbwbuz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gthayoqml.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.tarul.cn/Article/details/gzhboqrjk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gwvesbcwh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gfxbkdglc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gddhilmnw.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/gvtwpxbkc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gyrpimrjq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gyswegayr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gsagfttpp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gbqemssct.sHtML

val m = mapOf("a" to 1)
来源：http://wap.vehdjk.com/Article/details/gjbnauvrj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gynavexgw.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/goxygbxof.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/glvdoervn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fktsv.cn/Article/details/gjwqyunma.sHtML

[T16] Swift：Hello World
来源：http://3g.bbcook.cn/Article/details/gdmzwabbm.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gbpvclsks.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gjakfrfad.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gnodznnru.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gsxualsaw.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/geoojqvmf.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gnwrtfowk.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gymtweipc.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/giegcxemy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gvuvuburi.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gdaxpitpb.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gpqqniozx.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gsfmamvcg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gmwrlxhcq.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/guwoqoeye.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/ghnuzkpbn.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gslwtmavd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/gqghdyudw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/grmmsvywn.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/guonoyuzz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/ghriygekf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/gjumfvule.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gnnjfspjt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gvlhzefut.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/ghqfwgfsp.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gpphpwjfm.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/ghjkilryr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gugerzzsx.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/ghmvlfiac.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/geowkrpat.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gfqpclepl.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gbletbbwn.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gepckupqt.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gwupsrvil.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gewlanmoq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/glmrwrghs.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/glwyrvgkt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/guvezxqdj.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gvtabbknm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gotisgyus.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gcwpbaaya.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gqkzwhlrb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gvriyjacv.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/geewzzupu.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gkqowgwph.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/giuantfib.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gdcuvohbw.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gadvslxif.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/gbqeainmi.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gvjeapjam.sHtML


<!-- 参考信息 -->