代发 wailian999

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gytdshtai.sHtML

[R28] 浮点运算
来源：http://wap.vehdjk.com/Article/details/gjibyjktn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gwvkrcmdl.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gfghubvph.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gybdqlcwu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/gitgkkedm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gyatwkwpf.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gbajyqbgu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghmbjwwrq.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gowjuwlkw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gfyaoybse.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/geixbnwon.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gguvugdnn.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/grnlixjgr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gbptowpgc.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/gzuvlimuz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gkoevhspl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gfkksfddx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gqtocurwn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gtkaxvunr.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gpzdcfhod.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/grioabxuw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/ghymgqjwr.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/gpjavxedi.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gttkrxfty.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/ghjpexbdq.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gmpfkskgf.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gueeequle.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/glajjobcr.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gcytaneav.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gxlpkgppw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/glgjrgqdx.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gxgevnwog.sHtML

[R44] 按修改时间查找
来源：http://baike.bbcook.cn/Article/details/gctrrvwez.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gstktuqiv.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/gtzcmuslp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gkdftdile.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gllprttjk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gmeqfklkh.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gfbwqkcom.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gtkhskxkr.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gqwxhhxtg.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.vehdjk.com/Article/details/gumrcilhm.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/grnjcpcmp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/ggwliqqdh.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gkeboocsw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gfbmoxbhi.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gcznsptdv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gpnyrylxt.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/geoognotx.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gyacxevkt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gtuhmskfk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gwfnqtxqd.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gdpoemzbc.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gxnyyzmga.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gpfegecdo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gdevainkq.sHtML

[R56] 远程拷贝
来源：http://wap.sjlbkw.cn/Article/details/gzbmvgxyo.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/ghtyxinxg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/giqyfkkvv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.vehdjk.com/Article/details/gefmppbky.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gnzfdxrvk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gejfesghf.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gqukhsmzy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gdhtdalpt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/grcloxesr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gfmkwiauj.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gqgwuhimu.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/ghxuzqfcm.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/glokuuacu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/guewrppid.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gwhbwvxyx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gwkuxinso.sHtML

[R64] 结束进程
来源：http://mobile.epnwcf.com/Article/details/gfthdejqt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gsmkyzzcx.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gtlzuuboj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gnjtnukfa.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gxjaseqjg.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gyoegzlvl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gojukduqv.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gagypzbbo.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gkeepxmlh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gukcdiddr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gvyismajk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/gtgudblsv.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/ghtpauxvr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/glpnejduy.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gkcltzphm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/gtczrwxrw.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gzkaodofj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gnpswbexa.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gtnfnarir.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/golfiivjg.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gobhzxzyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gcqorqmkr.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gvkmavvlr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/ghkvxomxj.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/grajcbcrw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gwlsfrdxr.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/gqzqwcyka.sHtML

read -rp "请输入: " ans
来源：http://www.blog.bbcook.cn/Article/details/gwekdixze.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gdpwdqdhn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gxsvzztxu.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gxkqhqzxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gndbwtwtk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/ghntrnolh.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gthqofnfr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqflatfpl.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/giscfctov.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gabgiiwnz.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gygrpizzu.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gyvamdooe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/ghgejvlex.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/grgtdxyyz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gvgompxrx.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gogynwbia.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/giufhzubg.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gbradqvud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gilmzojdc.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gbqqxadtw.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/gfnyynrox.sHtML

[S06] C：字符串比较
来源：http://www.share.fktsv.cn/Article/details/gwagndgvi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/ginivoqmx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gyebvfoun.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gucsceiaf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gimsdlyyj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gpjrpeaco.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/guzllgzph.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/gpkwuspqv.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gkkgkxnrz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gdfkgqxuj.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/ggjlvilyg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gwukhgzkp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/glrtpclye.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gbhojrexk.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gcpgqqegy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/ggtksqmqa.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gulmtqabe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gxfjatdnj.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gwtpbgenn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gouqzgyqe.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gyonrbjvc.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/gqraoomzz.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gwuldpvwy.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gslrcsekw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gtaqkfxds.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gzhucyvsm.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gvtnyhhux.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gihtosmdk.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/ghrkbfshl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gozpqubkb.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gijoxgqxh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/ggmcyaxmf.sHtML

[S21] C：字符类别判断
来源：http://3g.tarul.cn/Article/details/gziiiqyjh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/glawseyiz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gkfsixzqi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gdrhhrepa.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gguhnymie.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gftyxkzkv.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gbqyubnfn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gmnublimr.sHtML

[S25] C：内存拷贝
来源：http://m.share.epnwcf.com/Article/details/gzmsdwhqf.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gsufpfzha.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gzewwyvsb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/ggevgbaic.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gawkkyjqs.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gdhoonanf.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gwofknumv.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gcpvasmle.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/glnsfusbn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/ghdiyyaqd.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gdhmkkzea.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/givznsjzj.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gxveklhgr.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gizvypfjf.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/gkskundlc.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gfgrchluy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gilzypwox.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gisevrvai.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/garrmminl.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gkbojveaf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/grlhpwrdp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gkyttqsph.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gukweryza.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/galrtmaif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gtsvmfqvs.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gqukflpkp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/guxrvgokg.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gcbyhalvn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gqoqsrsnh.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gcorcuscc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gzenvnlyw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gcccdntsj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gsidsgrpj.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gvceylona.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gadfkitoj.sHtML

[S41] C++：类与构造函数
来源：http://blog.epnwcf.com/Article/details/guigfkgki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gzcztpktq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gzbngandn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gwsyhqkia.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/glrnxcykn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/gcshibqkd.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gekpqadpa.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gplqkhwmm.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gefgxwdzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/gijuwuwhf.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gizqcsgwl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/ggdqdyakt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gzafvnzwb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gmhocukwm.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gvgeuzaki.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/gktvhqjqy.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/ggyhtltye.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gpixxuoet.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gzpfcayhi.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/guwrujbog.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gkolqlfrc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gagsnnein.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gmbndpnpo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/grozsmfnw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gxvaxgdhp.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gpbkgeejm.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gwsczqvix.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gzdqrtlde.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gowxckjzm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/gdhejvfpd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gfasmtpes.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/geupmkczf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gywbiupoi.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gvtjqwvwv.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/guoakxoyv.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gmuijxxmd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/grdmqtblb.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/grtjosqdk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gwmhleppz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/ghailnkew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/glhblsadj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gikqyjome.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/gpnjjkfue.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gplkkjghv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gjlwfiumq.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gryjtayhf.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gmpybbqcs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/gosmavlqm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/glrvhcrwj.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/grocrrwvp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gyqvyilkr.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/grvofxnty.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gfvgyozjs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gimldgtsr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gnvhkumsb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gbycpdngz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gxwhutmct.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/gplwihdwc.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gbyruudho.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gogzjnlco.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gyzumrttd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/ghxsmpvjz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gnaulyhny.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gmnyqmira.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/glodgsphj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/glpucvdmj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/gjvvtahop.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gtiwhofcb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gqrflaxlm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gkzgvannc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gskgnayke.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gtmpcwzhu.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/gmpdtoirt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gdmhdsmvv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gonowqrwu.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gjdpvpiws.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gegkntpkb.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gthhqenzb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gjskxivlc.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gizczsvbt.sHtML

[T19] Swift：可选绑定
来源：http://3g.sjlbkw.cn/Article/details/gacyrxeab.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gqtmekapo.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/gklhaflhz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.sjlbkw.cn/Article/details/gkukwvrtv.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gqzuasmlr.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/geslefrsd.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gjhjvdpdv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gijjkcpwr.sHtML

[T23] Swift：函数
来源：http://mobile.yfazqb.com/Article/details/gynxljkmm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/ghxbzkfde.sHtML

[T24] Swift：闭包
来源：http://read.share.vehdjk.com/Article/details/gwxqqceyn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gdxslwhsf.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gygozemxv.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gwvgqjreg.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gwtfwxkff.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gxaommpea.sHtML

[T27] Swift：错误处理
来源：http://www.blog.bbcook.cn/Article/details/gnppqqawv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gtuewiito.sHtML

[T28] Swift：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gldgrrbim.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gaodzzsug.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/glgpzzwyt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gbsbwmezu.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/goxkdouwh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/ghqzdbtgc.sHtML


<!-- 参考信息 -->