代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/ghpketfep.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gfjuletlf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gnocjflqh.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gmetmmcat.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gnfvbmafc.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/gfhdyycpy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gcpyecqew.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gnupihela.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gvtptuokc.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/grffvwqth.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gsovhnhcv.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gansxjpqs.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gsrzcwuop.sHtML

[R42] 输入重定向
来源：http://wap.yfazqb.com/Article/details/gsfhnsola.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gkybdkxsh.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gdynsfwzs.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gfsvkcfqz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gfdibhozg.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/gkmohijgu.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gvlrwwcnm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/glmzvunan.sHtML

[R46] 递归替换文件内容
来源：http://baike.yfazqb.com/Article/details/ganugztrz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/glwlxinih.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gijdwvzmy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gscgaszge.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/giskdzyec.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/ggfieieqp.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/gpyuzonhl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gxckvrozc.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/ggszcndgt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gvpumgidd.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/ggomjvzoh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/grovoupab.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/gmzlrxkvs.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gvgbbrwfn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/garryhujy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gdduuykfy.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/ggoglbsqb.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gnqnydrdi.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gletmsopb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gfqrzmcgn.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gfzymqoby.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gihsimpwj.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gowojupjt.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gsottrrec.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gdgobdfbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/glkpydyli.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gwixykovb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gmbhkhmqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gazdmrdtr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.epnwcf.com/Article/details/gugvxpgmq.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gsfinqvpa.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/ghjqqfuxq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/gclytffhf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gljlqlsle.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/grzeezqsm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gcjjqbgoh.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gqedsvexl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gnmfkgttf.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gluywcewo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/ggfoudxax.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/geyhhbtwe.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gpzygoaih.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gqhcbhvff.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gvgvogzsr.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gzhproozr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gbqldzfsn.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gvbzburwj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.sjlbkw.cn/Article/details/gpzwojwax.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gmsldwhka.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gqqtwlrmx.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gwpptuoec.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gxynhsgbf.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gjfdmrokv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/ghckmuosc.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gwtlajbyk.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/gzrinmhox.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gloucpuof.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gibomxklx.sHtML

[R75] 导出环境变量
来源：http://blog.epnwcf.com/Article/details/gtslbymmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/ghqhgbdvm.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/glfftfdav.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gvzmxflqz.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gcwgojqgd.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gqbyecmce.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gtykpouwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gzgikuiys.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gpaqsmcod.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/geebqpegn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gjaaxgxne.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gnjqmdprm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdjutwnqw.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gpdllgxky.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbrppxavy.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gmikaoule.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gaiprhyli.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gluaimign.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gbgmhkzce.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gdeggntyr.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gsezgtjct.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gdchcqayw.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gjwohmvzc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gfeedpzbl.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/ginwzymuq.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gvmbgiuab.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gffydsgyo.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gqawjbfrm.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gmndckykw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gqvvczira.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gmvwwfwid.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gpxgdvsdi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gtxeygmwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gucvdiasa.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuiijciq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/gwgofepoj.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gsydrrkzq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gpodhible.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gorfnzysj.sHtML

fclose(f);
来源：http://wap.bbcook.cn/Article/details/gkxccfsxb.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gjpsndibe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gmgssipey.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gotkujlpg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gxuguguxj.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gcnabeeye.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/ghxfkbeay.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gqqahzpji.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gpmgehhry.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gsmknjhph.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gqzrzgrht.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gnzaftobf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gfrlmktlh.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/granusdqp.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gtscjzito.sHtML

[S19] C：快速排序
来源：http://www.share.bbcook.cn/Article/details/gaclaymok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/giesnpknj.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/gsyyubutw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gatwayufq.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gzkeurqmi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gokmkgwzg.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gawcxwqdh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gbmympaqx.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gumwlxavp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/glngzvxir.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gbyoxlueo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gpvbechos.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gcjljgquj.sHtML

memcpy(dst, src, n);
来源：http://wap.tarul.cn/Article/details/gvbmqmbjo.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gxfvdhkoj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.sjlbkw.cn/Article/details/gwceuvxdu.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gfehjkexb.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gwlzplrbr.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gnizcjjax.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gkzrlexct.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gpwxfctjt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gbukdtmmc.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gklgafelv.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gjzjsglzv.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/grgkzizyo.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gihqocdhb.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gjtligset.sHtML

#include <iostream>
来源：http://mobile.tarul.cn/Article/details/gwcfzculf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gldxojmxh.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/grbttwfpc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gbjhxadxl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gucmggxnb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/gcfoouzyy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gtctrbxcu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/ggsgijtjh.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gkawuyxfc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/ghjmubhpz.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gswyuvjzf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/grjlqhtxs.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gighseggm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.yfazqb.com/Article/details/gczxddead.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gcbdmkkmm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/glmzuvxas.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.bbcook.cn/Article/details/gnwriopdv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/geeutgfdu.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gezhtlkhk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gqlhnzkre.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gbvccnbrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gwigxnrsl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gikmjwqte.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gtpedmpem.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gldluedsw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gyvkquovb.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gsykjueoi.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gvbssvdxq.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/goqfxfelk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gjhwaudvx.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gmcjsmexh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gksocvlzu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/gcphchytz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gydxwsnml.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gkrfnfexx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gmspfxkey.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/guowkqyis.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gxkfhihlw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gdtxtimxl.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/grcrqbfig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gzvmpjilx.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gsouhchty.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gldvqwwdt.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gwbqmgcfp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gsdjvgpjv.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gorrbivjj.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gkhebntjr.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/gvcyaawsd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gxcmlcmpe.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gfbdhhnpq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/guibtcbep.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gpzqgeeds.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gnkoxqpgm.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gzenylbto.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gvlbnelpx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/gwufsyulz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/glerylgat.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gbvzlcswv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gehrlebos.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gefyqvyko.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gnapzzvsn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxosdndfv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gciqdcjta.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsffpgcnu.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/gddbmzxgn.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gcudlmotq.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gaylemktr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gnxmhccuz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gabxnmvbp.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/gzxuvepuk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gpkssndoz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gkfkhuksw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/ggvfylevv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gwxpklrwz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gvkckxcwb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/gdwdlyjbt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gidowhidw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/guorpwcbl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gsrbiehoc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gkppxrool.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gzzxohuyb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gckkdpeqv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gkwswapqv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/gzvvoiijx.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/grlzanqnc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gryxnustc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/gefhmjvok.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/ggqbtdryi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gduuzqpiu.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gpsroexft.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/giglkvlpa.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gquaavxvq.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gbrvinqfp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/guoiynuoi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gdneyxzdw.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gyoijxgbh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gzfuuopxh.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gnylaorjz.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gxgllrazj.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/gpibtdmcq.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gizhwkdll.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/grrozkldn.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gbfqgwfkr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gwazcgtco.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gxndhmips.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/gqkxkogju.sHtML

[T22] Swift：字典
来源：http://www.share.tarul.cn/Article/details/gpkkrnono.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/gihndutmk.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/ghgumvaef.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.yfazqb.com/Article/details/gmoiqplje.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/gvojtmtsr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/gxqliswrl.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/glmsdwpwu.sHtML

struct P { var x: Int }
来源：http://blog.fktsv.cn/Article/details/gumthtbtt.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gidkloryc.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/gqvimsumu.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/grzfwszih.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/gvpyhtqwr.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gqrpvzkrk.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/gfhktlgbt.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gyfxrxmoo.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gjjorczcd.sHtML

[T30] Swift：协议
来源：http://m.share.sjlbkw.cn/Article/details/ggrjmztgc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gctjggmdi.sHtML

[T31] Lua：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gkuozmvfh.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gzddzxaxt.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gbwvelbmk.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/ghdvntajw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/getxztptx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gbxkehpsl.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gdvpgkjii.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/gzvnubsoi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/goegdimkx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gzlnaldor.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/grkrmzusf.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gjmjiijth.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/ghwuvmcjj.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gjxtbsebi.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gtsvhwzuu.sHtML

if x > 0 then print("正") end
来源：http://www.share.epnwcf.com/Article/details/gccktrgjz.sHtML


<!-- 参考信息 -->