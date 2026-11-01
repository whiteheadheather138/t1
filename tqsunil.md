代发 wailian999

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gulavzxsj.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gwkrpeujx.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gfoaidwbr.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gqbgnehpt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/ggywzpxbz.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/ggtxjykmw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gixgpsvpd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gtpsmwaos.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/glgosbyma.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gutrbtubb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gyrplwukj.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/glhxjxhqe.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gyljsnwkf.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/goqapodlq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gfzxhmrsm.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gkdbjhafq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gfrihnicm.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gnxjujmda.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gmhqqjkdw.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/geiuafinb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/ghhiyvalz.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gjdtthtcr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gbuzpkzrs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/ghrpgrbtu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gdsybmgfr.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/ggswxzwrn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gsbjwljyo.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gdwaawieb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gyppauyxs.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gfbeenjmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.yfazqb.com/Article/details/gajsvuyqg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gkxwydldp.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gdiyxkiki.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/glhngdupp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gcrhkwhxq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gurfgaume.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/ganefeeeq.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gxtkjiass.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gzwretoet.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/golnzkaeo.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gbakvlfop.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gtifppjry.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/glweefmbq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlmvjrqg.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gvqbdvyea.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gclgczade.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gkzalisyh.sHtML

[R45] 批量删除
来源：http://www.m.share.fktsv.cn/Article/details/gxdtsfwyp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/ghkfwylxn.sHtML

[R46] 递归替换文件内容
来源：http://wap.epnwcf.com/Article/details/gnhvsttho.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/grljkbiii.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gmbmycxhn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gudhcdhjg.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/gifiduedj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gecihbndf.sHtML

[R49] awk 带条件
来源：http://www.blog.yfazqb.com/Article/details/gnuzfsdcg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gyevknigt.sHtML

[R50] awk 求和
来源：http://mobile.sjlbkw.cn/Article/details/gfspwzgbh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/grreigxpk.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/ghblgmbwh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gwttwyofs.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gkzbkfbgb.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/glljvhplj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gzjwcjynb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/grxyunggn.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gwblvzhep.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gvmmsdgyk.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gognjdagh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/geyxvixnf.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/gdonewomd.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gmgtazvke.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gvjvvzqrw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gtonpbtsb.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gjseanqyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gekjmnqvt.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/ghvokkshy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gqsrrjcrz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gxqtcufyu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gzghjtxcg.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/grnywbrpz.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/ghpuhqndr.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gvixsqkgi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gfwtluvyz.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gkbadyzkr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gtxfsbntf.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gjickwzls.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/glmnqqyap.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gvytjpfcj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gkkxbuilx.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gccfopuca.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gqyezogon.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/geoxlmyxt.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/gheffpkmx.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gbautijtn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gtmcuhkrv.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gzkjsulyb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gyzuywcux.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/gjxsrqjdo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gcfunmfqn.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gbcyskqsq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gajibkghn.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/grkuzypcf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gbqnyhlrz.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gbnyyziwd.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gspbtotur.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gqsgosaho.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gxuhloyur.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gbajacfch.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/ggbwvkmtp.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gvropslxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gwapuonup.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gqztmqkqj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/giqhwdude.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gskioimat.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/glwxpgoir.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gpscgnoxj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/ggnijaaqi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/gbbckyclb.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gfcqtrujt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvsgozejh.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gqpcynvhi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gteumjagj.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/grfdwmprd.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gloauihtk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/ghlixibhb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fktsv.cn/Article/details/gghnhizqd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gkgdptaar.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/ghsbpeflf.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gwrzpgmmq.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gvwmpoqng.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/grkxejkom.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gnlwcfvvi.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/gtckluhwd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gongaidxn.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gswdhusem.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gcjcfqevi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gswfrgwon.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gdjocuogs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gulhgdabd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/guhqsowtj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gchyakgmf.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gynpfeohj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.tarul.cn/Article/details/gexllnvxl.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gxgkinwus.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/giatrmlml.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gvmiqrhvf.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/grolocimv.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gbmbmfcbs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gvglovdpu.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gamnqqzbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gstwvqrro.sHtML

[S14] C：枚举
来源：http://www.m.share.tarul.cn/Article/details/gkuoxktir.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/goeigixma.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gvphlxmqj.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gjejqarph.sHtML

[S16] C：位操作置位
来源：http://www.share.bbcook.cn/Article/details/gdltcqwus.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gaecvnqxw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gdiaouwdj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gnrqhgheg.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gltbwsqhm.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/ggujkgjhr.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/guomubfgy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/grpidiccp.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gtnjmevvm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gvfqhrkpp.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gikmpqsvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gqraurzwk.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/gtrvuffli.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gxkflezbi.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gtuowihxu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gndzfrkpn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/gdxxtbkvu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gsdxrbcgl.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gnpsdmuao.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/ghpriorqs.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gvesgtake.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/gaprmvbbz.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/ggdjqrquf.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gplxysmub.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gkpmrvtwf.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gssiaxcni.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gtxyorsqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gvhkljszb.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gzsnipdsj.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gmkuhkrfm.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gnfxjxabp.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gwqalqqck.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gitkwppui.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gztshpljr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gdsducgwf.sHtML

[S32] C++：字符串
来源：http://mobile.tarul.cn/Article/details/gqomwenur.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/glpemraah.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/ggkpsywcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/goiiupzta.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gkrsxwcbw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/ggdamcvgg.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gtavywaex.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/ggedgmjia.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gygmvgbmo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/geefcujvr.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gwjjqttye.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/gafpttdnr.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/grsmjtctu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gcvljepwe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gizsbqzvu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gfaskomgq.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gadkjmshy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gqeirbogt.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/grrghlkec.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gpjwjrosx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gbhcrblsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gwsqycgks.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/gwxfwfksg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/giyetfsfs.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gvobswdct.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/grqrevtnf.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gdaoqeaoy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gfroidpug.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/glnunupsl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/grudyjdhn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gsjlabfju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gqjznmdsw.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gafrxrogq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gpvvxhxyr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/gayatxfbo.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gsfqvzrnw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/grqosbszj.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gijpzpsjf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/ggvkolrdb.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gjlmvcmtz.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gnbzrzsbt.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gesqdqoqm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gdqzwryhp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gjvjcxcio.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gkuskbsdq.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gjagxzgga.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gayyuazpy.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/giczrwxwf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gwlvpfssb.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gohfiaplz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gxtfzkvcn.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gdgftrumz.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gwqvcxmer.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/gwwlfshrh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.vehdjk.com/Article/details/gvnmdhtew.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gpywoxvyu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gemoeiqgv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gxzgzugrc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gckilzhsk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/goyywiede.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gtqljfbbe.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnmpxqtoz.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gcaiypcws.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gtbjuwqur.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/ghyhpkkey.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gsecdtkjd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gpixvbtdh.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gzocphqmb.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/gdtirhfxw.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gpzvfvmta.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gdoypinwc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gfkrzymed.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/ghtqlalro.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/geheclill.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gvmxoxbsl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gxryoxpnh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/ggnhcnkja.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/ggiznovca.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/gfcxzrsde.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gqwnemdil.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gtooqvush.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/ghqaurhvd.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/glafbgafj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gqoxzdiqa.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gachjkynl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/grjjckqxw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gmzgxchte.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/glgbfsalf.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/ggezolerm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/ghuzygmmv.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gfnwowkql.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gcikhoczb.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gcamaexgf.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gnlaofqsf.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gskrnlkjs.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gklxxonzr.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gmwexiljp.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gvsbypzpr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gesqazaqy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/glpokgmgs.sHtML

[T20] Swift：数组操作
来源：http://wap.yfazqb.com/Article/details/ghwsisdih.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gqfajwciz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/gliydzfyj.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gfhyopaah.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gxguffgcj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/guzsfbezg.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/gkqvpsmqj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gfxptkzmq.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/ggogmzpsl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gvnahljoa.sHtML


<!-- 参考信息 -->