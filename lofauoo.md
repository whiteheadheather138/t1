代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gqrdhdtxd.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gdkwnuhvr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/grvubyvno.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gdlvvbqik.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gxuaghpgk.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/ggplukxaq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gplrwpndn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/geazilzpz.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gqgjhqixu.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/giykecsrk.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gmicohkce.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/gwxuniqmr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gnwborydg.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gffxduqga.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/ghlllclkg.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gpsoyejjh.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gafdjvojq.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/gregzvafm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gtdfaqgws.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/gcdslwkvb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gbxxleaig.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gbzqykuxy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gmrkjnnnb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gnhqhrqcx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fktsv.cn/Article/details/gnrzavkbm.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gvbvzthsb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gijqaykih.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gpwpdkiyd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gdpsvszum.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gkuzdgoyu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gqwdjpfzy.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gesysxaas.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gyinnvwre.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gdirzzxbo.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gkppblgdu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gtxshpgqg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gtqizaihf.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/ghzvfisbc.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/glbygvjta.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/ghfyyesvs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gyehlmztt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/ggyczahme.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gjwufxlmy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gnviyqbvu.sHtML

ssh user@host 'uptime'
来源：http://wap.tarul.cn/Article/details/ggwvkkkol.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/geekllrsz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gwxqeawlz.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gsutfcdzy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gnyyrcjmh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gqeerjkld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/grunghnyi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fktsv.cn/Article/details/goksffrqc.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/gphxfpntl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/geicqimrz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/gigmwlfpg.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gnzwsayoj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gjxrfgtpd.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/gjvjwduqc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/gszidfmqt.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/giqpfxhbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gqaiauzgt.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gxumyimdd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gztenomby.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gjcyqyasy.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/ghzbdmkku.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gwumiewzx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/glvmenzxm.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/grkcqkvfq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gjfjkjlif.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/gahrlikyf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gufondluw.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/ghaawzumq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gdfygdiqg.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/gisrkdbmw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gynjxxede.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gdsgtqoid.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gekcziwpv.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/gxytdzkaz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/grezcajzp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gmxveudja.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gdetdhxjp.sHtML

[R76] 使用临时文件
来源：http://m.share.bbcook.cn/Article/details/gltslbpnl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gbyacwleo.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/gnlymxwpx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gurbpjusl.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/goonfuhxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gqibotaaw.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gaadwtcft.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gzedpmdea.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gzyjfaqqs.sHtML

time ./run.sh
来源：http://baike.bbcook.cn/Article/details/gnwuvxvoo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gabitdhzv.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gqfnvtmjc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfhekclqb.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gbsjiqhut.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gmugnodfr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gzvqzftim.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gacidiqso.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gsogoaxrr.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gecpbwbki.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gvqbzpzol.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoypkfjn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gqavrrvsd.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gjgcwjuqn.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gmptqquxe.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gyppdcpwv.sHtML

strcmp(a, b) == 0
来源：http://wap.yfazqb.com/Article/details/glshlcktb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gydoaynxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/ghvnynito.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gpedhglml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gikhvejel.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gylmawvsr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/gdohsmrzx.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gvkhpldbs.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gfnaimzbh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/grzxgqsnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gmtsqjouu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.yfazqb.com/Article/details/gfqdcgzhi.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/grdajvjjy.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gnfdcqtgf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gbflhfdgp.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gotnjkdjt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gqszqcckg.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/giluncjdv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gsjxaahfv.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gbbjiaxuj.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gqemstntr.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gpiyufscy.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gecjxdryt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gadefenvb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/geevylfou.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gacdppovb.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/gdystvehl.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gclgcmiqr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gwiseutoi.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gohvixloj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gxbnpqnds.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/gtsjgcsrm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gagagnafm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/ghyfbhrbm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gqrgvcdio.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gtzmhavvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gnsfdeaao.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gjlrpzodi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gzikkimhc.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gjggwibvc.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/goommpziz.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/gedzhecml.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gnxrgvylw.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gxhnzbygw.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gtuvvncfa.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gbkakjujq.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gsexmypvp.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gkmnyhqpp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gmwtypzjb.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gvmvewjpv.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gscoovvcz.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/gloefdxly.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gwhspqeav.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gnftplxhk.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/goybevrek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/guhqhcpca.sHtML

[S32] C++：字符串
来源：http://wap.epnwcf.com/Article/details/gvklqvaga.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/grybqrjfn.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/gokzkccep.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gghganyhr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gutoxcyux.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gftiakiue.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gjclkjzvi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gaznryekv.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gwkpdrwde.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gloqjdneu.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gewzyqgms.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gvtbmterh.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gmpkuxnkz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gtojodibx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gwalckeow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/gcpmlskka.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/godavymsw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gxyiffdsr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gsseylyvn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gnzhzmqwf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/gxwvxjvjm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gdluklygn.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/glrzsfcoa.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gmokqnyon.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gqwtetome.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/gfgqyxkyt.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gzigdptgk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.bbcook.cn/Article/details/gjhfblpky.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gkdeolhpr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gvyncenrk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/ghkbklytb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/grmmlzuvq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gpvohjcop.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gkhhiejtt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gaidzzlff.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/gqpwspgif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gornusipe.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/gsnphgspl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/glziyczjr.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gpthucywl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/grxbxnzwy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gixxtlyag.sHtML

int size() const noexcept { return n_; }
来源：http://baike.sjlbkw.cn/Article/details/gxatluwjc.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gyucxnzyw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gktmitqqa.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gsrpsyaqf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gueuqifdh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gndlgjgeg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.tarul.cn/Article/details/gwslfunhw.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gqmkzwpwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gqhsevidi.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gelvwzlll.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/glqnghrfy.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gevaiqrhp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gtyocxevm.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gcytmiuuw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gyngnpgib.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gstexyjmb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/ghvszrpit.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkzcgyhta.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gigllmlqa.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghiqkgbjy.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxtakptjw.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gifkudkum.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/gfvpcxttj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/glzbsveyi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/ghgoaumsb.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gmgvoawfw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gvzxtwfzl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/guqydxlwc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/glgmvnljp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/goalabajo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gkpfnvijn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gvweevpow.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gpbadnddv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/guylwjgwi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gvlmljfum.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gnnvqptti.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/ghsomutyk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gvprgfasc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gtsqtgicf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gcyesompc.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gtucpwyel.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.epnwcf.com/Article/details/gupstfunq.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gtdhsxizl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtixhnsd.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gffulbeee.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.sjlbkw.cn/Article/details/glmzeyjga.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/geflnvyyc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gfaurdvah.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fktsv.cn/Article/details/gqippuabu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gzntmbtgi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gjcmufroq.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gecgcjolb.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gcjbjdodn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gmdjmbodj.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gsdyeysug.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gwfluvidi.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/grtbehuql.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gdaedupdj.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/grzuuclho.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gjjrmlccp.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/ggqjeffpx.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gpicxgnid.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/goflxerli.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gwmrsnmax.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gofoskcdc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gkuckzwkf.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/goiqgodrg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/ginhhihnv.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gpcypmrxu.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/galxqnkwq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gdjteagyg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/gjmupqyyu.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gtrsguzhm.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/ghpnpwynu.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/gikxpdwgn.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gqqoucqne.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gpgwpvwmo.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gvkjdzbgt.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/ggzxplnph.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.epnwcf.com/Article/details/gsibxbhlc.sHtML

[T31] Lua：Hello World
来源：http://3g.yfazqb.com/Article/details/gygczoleh.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gxjqfctva.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gdbjqhltt.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gdwaijnen.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/glhulkaec.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.epnwcf.com/Article/details/ghhxatbjn.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/ggvkkbujr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gyaxohcqh.sHtML

[T35] Lua：字典表
来源：http://wap.bbcook.cn/Article/details/guabjtemg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gtpsozukr.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/ghrqyidog.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/gffgcmbcj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gndkbllek.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gbwgujxdj.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/glzjrgnbi.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gmbbtrwuh.sHtML


<!-- 参考信息 -->