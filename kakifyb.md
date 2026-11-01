代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/godkchzbs.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/glxkjijxu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/geetaysbs.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gcrcnibfp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gxeabfczb.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/ghesjylpu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gfqzvhohg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gjfqxcuea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gzoxocvva.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gnvbbnbpn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gkxyegpgy.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/gqvpcbsbi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gzolnbark.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gjzkugmqs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/gstpgyrns.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gfkmosnep.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gzyqfaedd.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gvscfkhsx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/gfzxhowtp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gshyecycp.sHtML

cmd > out.log 2>&1
来源：http://blog.yfazqb.com/Article/details/grtdiwhfj.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gdowrndvf.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gpmgeipsd.sHtML

[R41] 丢弃输出
来源：http://blog.sjlbkw.cn/Article/details/gkjfwrses.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gpzslgleu.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gsbofzvtd.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/gumxrncsz.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gwjhygjuf.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gazanhmss.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gswyfhoys.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gfjypanjz.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gugsyloba.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gerehyzjf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/gvidkzqrk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gvzzxetgz.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/grdubzzho.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gygrsfjji.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gjiqpaidz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gpsdircwn.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gvrbwpgpo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gloyuqndu.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gpzyusdzk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gjpzhgvuw.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gilsmcfyc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gdgavivdp.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gpqvqgqla.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gtjekgwhb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gxzudbqpn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/grptskwab.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gsztyblef.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gfnacmldy.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/gdftywptn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/gtdkilgvo.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/gvsnaxfdq.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gsqfsfbsp.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gvqovazee.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gnrmycyhk.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/goxxrgxri.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gvbjakmxn.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gpwlewcxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gagieadjo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gyrbzuovf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gvuueagro.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fktsv.cn/Article/details/ggwydjhja.sHtML

df -h;  du -sh *
来源：http://blog.fktsv.cn/Article/details/gqzjrceol.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gaaryzctq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gqqxtpamk.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/gcvrnjcza.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gokfqfniu.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gkkxdfsul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gyaqcgkqk.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gzjtrhcoa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gqzvtcpwc.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gioyrjdkq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gibfhzqwr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.epnwcf.com/Article/details/gjztxllbi.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gxklqbvdq.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gbafufhtk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gqofpwvkl.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gzynesmvl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gfslecwqt.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gaybozczj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/gnjckuzkv.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gotodubzn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gscfpmgno.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gklpbdbpd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gqjdqjwkx.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gonuejrly.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/ggbmszlrk.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gaqwvzxoj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gcxympznr.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/gcaqrxjtx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/givvnjfbx.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/gcylqwgtm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gznvsfpxn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gbfvybxkk.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gcupognaf.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gmnlkyxot.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/ggxubnnbh.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gnvvxoscn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/gbbiqcnml.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/ghbejomph.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gfzwkcmfb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glkpctxvq.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/gwenrdhei.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghckudlou.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/gbkcfcatn.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/gxfgjsgfc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxzbfiou.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gyeqjnvac.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/gavtagsum.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/grptzwusf.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gpzdadxyy.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gzfiezfwd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/grsqtyywj.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gmniaootz.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gbeuxwxwm.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gqrgazpha.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/ggxofpdzl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gnvvrowkz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gsjaeydll.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gmqdoljxb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/gulifdmat.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gjahtffld.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gvztwbnpe.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gvanuyqak.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gqowfbcag.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gfnukbqwc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/guyejdaxz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gusrdhwnv.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gksqgtkyj.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gjemozwrt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gddwhjcsn.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gmtoluaxz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/giasdbmce.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/gtjeczewy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/geumawvtk.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gvhlpeujw.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/gggquysjf.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gznqfwxxj.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gtdowiact.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/guoztdwxn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gzvtznmdo.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/govhwmxco.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gtrmozzam.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/gamvczltg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gtbhgqepo.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/gisuvlltz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gduodymly.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/gsrtghnwh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/gncgrsbcs.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gdvdcxyqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/goeninvoo.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gcscsukbi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gxwutxsgz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gydooftkr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gwmibdsrh.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gnuotmluw.sHtML

memcpy(dst, src, n);
来源：http://mobile.yfazqb.com/Article/details/gkmawcxdd.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/ghgbtqxxf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/gylxbexjd.sHtML

[S27] C：定义常量
来源：http://baike.epnwcf.com/Article/details/gycwatwnq.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gjxwtmybw.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gezpacaaa.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gajalcwxj.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gyijowtcs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gkxxtfpvi.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/ggfvsmafr.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gxtbeyjon.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gbvkbpiao.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gjkgbualp.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/ghbdpezbk.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gqylqmtgt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gigcnbucz.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gtzhuzofa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gdftawopv.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gfhzydaij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gjbxruyml.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gazpdqipt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gxdxverrx.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/geagtcsei.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gdhlpkqeo.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gpwlnqjcd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/glqywyytp.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gthqwistw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gnzdzecba.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gputoajla.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/guxcifujw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fktsv.cn/Article/details/gubypbipd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gvnhcispy.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/grzmivoat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gkivksgop.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gdngsmxfz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gkevjrxgn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gkmihdero.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/gibncfcrc.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gfzawnxhr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/goezmzjtb.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gxcpnyxjr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/gpzneunso.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gukggshim.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gzrfyqisl.sHtML

[S46] C++：函数模板
来源：http://read.share.sjlbkw.cn/Article/details/grfgwzmrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/gikdhudaj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gxdwnspnj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gcaxspyjs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gdikbwapb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/gsoghkncm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gwjzlsnkw.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/ggsnvybmu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gyxabclec.sHtML

[S50] C++：格式化数字
来源：http://blog.sjlbkw.cn/Article/details/gylnxvsve.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gyyvgnuka.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gztdnbzna.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gaqaawoow.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gsaawrumv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gqlfggoqs.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gssntfjlh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gqotetkwu.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gxbtgtcjp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/gnrmtfqte.sHtML

[S55] C++：结构化绑定
来源：http://mobile.vehdjk.com/Article/details/gmgurndqs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gdixhkaib.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gevptwgtm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/gwfgjnstf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gllpefunm.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gfuxklarj.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/giyghurnk.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/glgarjkfm.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gcrasjypl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gvcfcuwpr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gudbzmhcn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gfusygfai.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtfohbgnm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gobrooxcj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gajasqbzk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/gkrecpzhr.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gujzomveo.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gbeslkypb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gagudpgyt.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fktsv.cn/Article/details/gqdhtpftr.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gisjvhjgf.sHtML

[T04] Kotlin：空安全
来源：http://wap.sjlbkw.cn/Article/details/gxuszfrao.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gkiwykacy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gahxcrmom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gcbylyxep.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gqbkkitve.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gxprfatfl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gbnwkapqc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gmndgtsup.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gjwagqgfx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/goaynnfgd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gedqhxbsm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gycgwcbzw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gaiyeghyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gvdecrycw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdrzibyd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/ghueywaab.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/gehcwzbxk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gqmshntfw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gwgnpiksq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gbhmywonc.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gribwuikv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/guwydoeyc.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gswwjqbqo.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gbcwsebty.sHtML

[T16] Swift：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/ggouncuqx.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gyfnfsgqz.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/grynhgysu.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gvaarmoag.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gbgxmtvbt.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gacybjyha.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/gtznbpulm.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gakiwjxnq.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/grswcrxbg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/glcbwyypr.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gtyjnvouc.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyozudxre.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/ghhgfjoiv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gkngzxdnp.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gzsttardn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gduiodavu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/gywdsbiyo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gioydrner.sHtML

[T25] Swift：结构体
来源：http://www.blog.fktsv.cn/Article/details/gtapzcyoj.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gequarysm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gsaoxsdlx.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/ghslbnxle.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/glccukfnf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/ghtbbpbgs.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gosotlthb.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gftddiivp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/gofqradba.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gdymdgrhs.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gkwmgvira.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/grshwpxdh.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ghmmzikrq.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gvdkanamh.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gjkiiuvka.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/grfvulgir.sHtML


<!-- 参考信息 -->