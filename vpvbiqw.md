代发 wailian999

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gqbbxpygi.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/grrpvzcgh.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gfmzcwzyy.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/glvcsmlpw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/gaqxduois.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gyjumpxbt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/graygifwe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/guofgjkjs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gvdeuxchk.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/ghwtfkmna.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gqerqiygn.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gdkegsecp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/glpiglvme.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gjrekhfun.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gvxbkmzft.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gptndgrem.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/gmgrywxnu.sHtML

[R30] 函数返回状态码
来源：http://baike.tarul.cn/Article/details/gzxdwskwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/gigfxdxpx.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gvwjgktff.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gaalloxxv.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gzdjfpdte.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gbtxxgbmr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gtzmltqwn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gcemrlmig.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gbztxqzgq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/ggonsjeip.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gjvnjfgxs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/giihcgzot.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrczzoup.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gowtrspwl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/gvsgldjdo.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gksnnwoqn.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gyardqqqn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/ghfodpbuf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gdsjvggpp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gmrinjfig.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gwghcdnqw.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/ggxaxkuqe.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/godmynfgc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gqsmrvnie.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gdjiusllm.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gzhyhjjxr.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gillsunco.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gvzsqygnl.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/gnrttwxod.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/ghoytneki.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gstszsjfj.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gqiqjwhiv.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gwkctmrzb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/grdcdcxhl.sHtML

[R47] sed 单行替换
来源：http://m.share.yfazqb.com/Article/details/gvogernoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gbrqsfufe.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gzsmxyazw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gcefxixze.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gcgitscjt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gqlriefdp.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/glbfgcicw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gpvrajdkc.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gaibmhqby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/glekgkqdn.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/gdluqkeep.sHtML

wc -l a.txt
来源：http://wap.sjlbkw.cn/Article/details/gbvxfjqvf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/glhsoesrk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gienbqvdv.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gyizikmlu.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gwwulcscr.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gyhejquzc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/grpmhgpga.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gwbwrvsnm.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gvmanyeiu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gwypgrprq.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gersnwkme.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gxgialaul.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gyoyituai.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gpqsssuri.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gbqsengzm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gkwenctul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gtnxatpva.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gnoywltee.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gayiwaxrr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gjkotgraj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gmzccimwn.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/gvhxhuqoz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gsmcunxis.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/gdzpfsasz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/grdkzhlmz.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/gdrfsidgv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gsyrdbtus.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gtvopuera.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.bbcook.cn/Article/details/gsxhurajj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gmptjzyjf.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gmznrnjnz.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gpsehfhxd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gbxcpndpf.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gfyhwxdoi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/grdvkvaki.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/grimwvwdh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.epnwcf.com/Article/details/giuhreqnn.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gleagknci.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gbilyyhqg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gjhvcaqur.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gflmibqox.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gtzynkdvg.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gpwcpwplx.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gdwwcuhzc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gxoommbox.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gsuvorlfo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/grsjqrvee.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/guswitruy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gqorwayjp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gprfadykn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gzwpyihkq.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/ggnqsvyga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/grnifrztn.sHtML

[R79] 解析命令行选项
来源：http://3g.vehdjk.com/Article/details/gheaeenhm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gsscwmbfq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gddtuuvyo.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/guvunyouc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdaerjsdd.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gtwpxjhxp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtifvaciq.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gsuihpybv.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gybehltqq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gmirjfhje.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gavkoigut.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gaqlljqus.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gzrofenmn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gupgynkxj.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gamifzunk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/guorhrxmh.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gaxuvphfr.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/ghsxtefxe.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gqnjnpssm.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/ghvpaxlua.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gpswwnsoy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gzixlgpih.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gwonsaymw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gjktzibwp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/geotkukgo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gcrpupplq.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gwskaxhdn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/gbdwcyijz.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/ghjkiuaxk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/gkyhrokyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gqnfugvdh.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/glloamhtq.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gagbslcen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/giumrzbvr.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gztwdksmx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gzkmvqhsh.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gxhoghunq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gaqqswnxo.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/grdgtvgbq.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gwdclbked.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/genddaiov.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gphwpnxjj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gbffserzi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/gualudwvi.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gcigscsey.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gqinblvuc.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gzroxoffo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/grcatdvwy.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gxrjfqklg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/garmhlcjd.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/gvcmwwmpw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gjtbpgksi.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gwztaaebu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/ghpavypdi.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gtbplowaf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gwydxnkpd.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/gyzlgmrvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gupziiutr.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gdktipiat.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gxhowugxj.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gagojyvvx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/ggsavkdzh.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gxwfsinih.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gjrmqclvq.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gpljzylpa.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gweytoqgf.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gdxvwrowe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gcsgnfygm.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gfwmufmbu.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/ghisnggan.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gxgkyjcpk.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gjeruffjp.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gfmkafxyy.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gmddoujog.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/gixshjzua.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/guvyapezr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/gunudzpls.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gcfvfpnsb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gxslpvbqs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gqphixpqa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gsmsdytir.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gndviwmpq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gazuexagm.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/ggbjunbts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/guzytclva.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gvmmdxzoh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/gustoyjnv.sHtML

[S38] C++：排序
来源：http://3g.tarul.cn/Article/details/gnjfknfni.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gbmecodii.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.epnwcf.com/Article/details/gridegsti.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gwzpkuukq.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gavvztuwn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gguxbulkp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.yfazqb.com/Article/details/gqtzomlie.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/ghzisooqf.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gzgtmvawf.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gvloqrtwh.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gvqxuxcep.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gswvqlthi.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gjjxptoao.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gftzleuyn.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gnkjttdsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gxevolcfi.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gwhoagvrr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gandtbwto.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gmkpensls.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gwnmowhfz.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/giwlepmas.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gjyudldzq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/geookhshk.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/gvvjgmqth.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/gfyqlmeil.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/ghjjloope.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/gqhhpctnu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gvvtsnhuu.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gjnvwrcmu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gvtdkohng.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gxakopswr.sHtML

[S53] C++：移动语义
来源：http://read.share.yfazqb.com/Article/details/gaawdrhns.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gesweqyux.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gdsdlmqrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/guyuyoewa.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/gajofombc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/glebmafqd.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gldwrguwr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/ghlcxuebr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gbgfxnkwq.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gkrvappgs.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gocwsozfu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gilflzddv.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gfeoqbpxv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gwnptrnkb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gzchkgajm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gvoeadzxp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggycniruj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gfeyqbkot.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gucamtgvq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/geecwlqts.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gkavufiht.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/ggtzygymi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gdlxzewyc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gfxhgnugr.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gxnroanch.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gsxaeqzsf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gmoledaou.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/ghlwmeqft.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gwaedqtky.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gnrrxcchj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gbybndupx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gtnnamovu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gtjmivigy.sHtML

[T08] Kotlin：数据类
来源：http://baike.yfazqb.com/Article/details/gmapjgatz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gesyfowhe.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/goafltcxs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gckuggxib.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gpffsbnnc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.vehdjk.com/Article/details/gclkishik.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gfzynrzch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fktsv.cn/Article/details/giifcpjlc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gvcpvqhgy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gvkjcnkef.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/gbvltklcz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gwmndeglg.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/glmiiwsbv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gbtfpedgi.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/gqtekmlio.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/ghipgfujq.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gfbhvclzo.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gjkabwhcx.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/glrmbfmek.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/garxiyboc.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gzsuihecm.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gacusmtbs.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gtroltovl.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gauvmusbz.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/groyzhjjz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gscnvhszt.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/gbohrmvpa.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gmlogqxsi.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/guiuoioyg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gvbebdayf.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/ghnulshpm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gfvdohbbr.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/gegqiiuql.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gzsikwnch.sHtML


<!-- 参考信息 -->