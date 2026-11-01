代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gbpmjnsqc.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gtfmzghev.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gfwicwsvf.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/goabqvgfl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/gmhhquivk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/ghhdahmwh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gyzrxlvms.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gjpdlbsaj.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/gticbyuac.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gbkkbshvi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gxcnqjxdn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gnrmkchjp.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gldbrcoaz.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gxpxkjwcp.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/ghljdwzhn.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/ghppkzvzu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/glhxfmgca.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gvpeythbo.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/gzpmjfeoc.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gjbajqfxn.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gmjhtsleg.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gcwumgqif.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmxmaxrl.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/ggnrzsezs.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gqrgxpeip.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gfqzixnnt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gorrhvlcn.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gjflgkchs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gkmnfrxrw.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gvuptkbls.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gcicckfyo.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gzrgrhvkx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gitemjxvr.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gubzeozcf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gdtfjhfsq.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gekkzqjva.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gjaeutdye.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gqriihqyi.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gcaerbpbu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gkkvfsqib.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gjsefhrdg.sHtML

[R54] 比较两个文件
来源：http://wap.bbcook.cn/Article/details/gbrluycju.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gvykededr.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/ggxvhmfol.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gbsgumiha.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gioilucfx.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gxbkaicfv.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gjrwfgdsg.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/ghtzdzrfl.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gazkadkae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gjrxqftlg.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gucldpbtq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/ghgtsijst.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gjomtbuup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gnyaqbgjn.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gfgopkehn.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gefyvhcoe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.bbcook.cn/Article/details/gcyggtzck.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gqjfaorxe.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/ggvhmapcm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gsmikwmik.sHtML

[R64] 结束进程
来源：http://3g.tarul.cn/Article/details/gunymqpve.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/grofguszz.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/gkqocpnzs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gbbjzgito.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gvujcaunr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gizmvxxxu.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gybhjbxym.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/gdwqplyif.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.tarul.cn/Article/details/gfyvlanmr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/guqrlxzke.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gsemsbofd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gbgwcpxtv.sHtML

[R70] 时间戳与互转
来源：http://mobile.epnwcf.com/Article/details/ggkurvjhf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gqqkyojol.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gpdsbnmvv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/grlobwyci.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gdpxxciai.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gxbulklul.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gfebgyyeu.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gcxchegyc.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gdqfxhqsi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gwjdiamju.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gaengidbp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/giupppmio.sHtML

[R76] 使用临时文件
来源：http://wap.yfazqb.com/Article/details/gsfykazyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gmfulexoa.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/guxvwjppm.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gtwnemtcc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpqvnysk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gfbgjbmqi.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gniksxihm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gomyyltwt.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.epnwcf.com/Article/details/gepcsapjl.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gkceuzdtj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gslcoxbls.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/ggexkurna.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggvnaifop.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gvcjfttzy.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gdxtdumva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gxrwwbiqh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gpauljrue.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gtmlxyest.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gmlmxnctw.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gvuyismoy.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gjmksqggp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/gmraryrif.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gsznbgcle.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gqfcljvje.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/goofmvrml.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gonuortle.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgulpusn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/guwnjgqet.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gsnavgsng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gczyecigz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gpvpgminz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/gqsgvbndc.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gdhbfsqfw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gcolfnyfs.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/ggsxgseqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gzrawugpj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gxqvbblww.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gklirdfop.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/grgvbitqv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gcvdqoenm.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/grpjgjmtz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/gehbshoma.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gbvpkdkve.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gxamajikp.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gleyxwcib.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/ggswokdly.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gnhuuimad.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gmkvkhwkg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gmxhmtpaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gyzauyilq.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gokgwigfl.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gzmlqkpso.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gmvxcardr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gomvnmhak.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/gwnbowmke.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gndyvmamc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/guhxdsxet.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gxgpkyvox.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gkmccqyme.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gneddvsmh.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gcagrdmdp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gvfrsjydq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gputiowvo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gaptdbvuh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gaogncymo.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gvwmsnvpj.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gwcezvmrb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gmsqvwtxp.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gdxxlqsuo.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gzmlgqjbk.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gpsdjkbne.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/guxcjpjrz.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/gvlqkwpnw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gldfzqizm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gpiavwhli.sHtML

#ifndef X_H
来源：http://blog.tarul.cn/Article/details/gqolnrquz.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gwfpcqsea.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/goulyjqkq.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gtexsxlrc.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gcyqeaoct.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gcmyahhhw.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gckvkxqlj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/giiyheyxh.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/guwztluqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gangvgouf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gsufygwmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gjutinorc.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/girwgzdkm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gmyvxmtxa.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gouymhzgk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gpyifyctk.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/glhcavpyz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gfmxcpueq.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gpoyswclc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gdgcablzd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gfruqdqwl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gimwcmick.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gxpangglg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gslyjgsaa.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gjkmetvgv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/guuqfanaj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/grmqlvwqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gingyuhug.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/ggyltilcz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/goeabceyv.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/giljwminw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gcjlflzua.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gjhzjgvoe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/gcrduzijq.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/goxwrqgic.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/guijvazhc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gzwtijemw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gyjdhflzg.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gswbchvdm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gznkkgszb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gkdjseerz.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gcscdgtbt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gymsbscir.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gfhcjpgdc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gzwopnrsz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gsjyraulc.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gncscstxa.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gmtlxjygd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/grcewlazg.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gybowzwrl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gajetecme.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gakytxqal.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gykltwfxk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gyzfxvomk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gcqosgsuv.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gapgwxzjo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gjbsaezlo.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gnzqhsfss.sHtML

constexpr int N = 10;
来源：http://baike.vehdjk.com/Article/details/gshubqlyh.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gaxhilukr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gonoxywzh.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gnrnpisba.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/ghfmlnpof.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gkpxfncjv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gkwwbqthq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtrvvcyfh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gkgvcltfs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvtecaimf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gqnwbanqz.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/glzswkkud.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/ghwbjclye.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gniztdxbo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/glzmkmspw.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/ggwgxvcdr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gnabqunrh.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gsmvztydb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gnlkzirkc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/ghsrlsmcx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/guhaytgcs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gmtufbkpb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gbalweyub.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/geufuopgq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gyryxecsc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/gaxyykvna.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/ggbhjlyuj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gzowxslna.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gguhmbiqy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gsyrsrqos.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gqqdhbjzj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gcopwwhwp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gyugczacn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjkuvcwby.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gxkzvglss.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/grgqxqcyy.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/gzvrpyrtg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gnlmjpfas.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gygwphdbj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gjbategwm.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/gprdhdxjx.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/ghkujmfsl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gxwgrohmw.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/gctvmmzau.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gkjholssn.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gehemilgq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gkzjbhddy.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/gsbgmtuvd.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gmxhiojwi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gqhksrjoz.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gjmfkmkie.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gtqjjwknr.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/glywiwhge.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gifsaxmyz.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gsvmccaxs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/grjdujjig.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gorijwftu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gzjsswdcg.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/gffowbsia.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gtnyoxhie.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gbhnuscbq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gcjzpzeoz.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gihhkhmod.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gvkrovgkq.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gbcdzypdj.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/gibzpvnqe.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gnokvpijo.sHtML

guard let x = opt else { return }
来源：http://3g.fktsv.cn/Article/details/gxamyapgl.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/ghkuntngt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/gzmrrcfht.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gmdcgcfhm.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gbowxotnq.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gqdwabfrb.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gurmdkjoe.sHtML

[T33] Lua：表（数组）
来源：http://read.share.vehdjk.com/Article/details/gzxykmleb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gcqqhncso.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gpqsouajt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gtfmqkljz.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/ggqxqpeft.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/goculowtk.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gfsnbleot.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/grxnnbymc.sHtML


<!-- 参考信息 -->