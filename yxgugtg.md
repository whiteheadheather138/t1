代发 wailian999

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gsykacpsp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gdjhzizra.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/guvouzmfo.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gpnjmkoqr.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gtxkzcohd.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gcwnjoywm.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gvxzyorzg.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gbossjurz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gekhuzlzl.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gknylkgzi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/gcowcslsk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gwpnstovc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gsguncmdp.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gntdsdqgt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlmftwyp.sHtML

[R27] 算术展开
来源：http://www.m.share.fktsv.cn/Article/details/gyqkozxqz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/goftedcmr.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gwkgzeflp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gzpumogof.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gjyndgbfm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gmyjicgxl.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/gclvdhlnn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxigwwlpw.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gmowordxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/ghhqjlrkv.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gglditvbv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gribrhnof.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/gvjhljnpe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/guqsgmzqd.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/gvcfvzofw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gvcmlpggr.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gbziaclsk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gqiwjphma.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gzrlwdxmy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gdcrcpskb.sHtML

[R37] 把输出赋给变量
来源：http://baike.sjlbkw.cn/Article/details/gldudimlm.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gncpsldce.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/gpwkyxlps.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gdstixkny.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gbrpnvurp.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gwyifdzzy.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gdgpjznro.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/grqmzsjco.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gcnaljjeq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gikuikvdi.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gdnulmumx.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gnjfubhuw.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/gxjuvtrku.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gkrayepba.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gqpjoaath.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/ghzdofriv.sHtML

[R45] 批量删除
来源：http://mobile.fktsv.cn/Article/details/gcmpnkhcy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gccezwnpd.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/gtcapklpq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gvrcnzcjb.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/grlrbfxkv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gmsdxpuaj.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/ghgykdufv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/grsrrzifh.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gdcovhfqh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gumdieviv.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/gfirzyhxf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gchhsxdyi.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gixaaxdxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/guoglsohk.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/ghpapzyeu.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gegksbboa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjtencoj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/grawbdszv.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/gzdqhkmgb.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gyfhzawli.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gzentwiks.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/gsqfmwjwu.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/gyvomevqm.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/ggpvvcxkv.sHtML

[R57] 远程执行命令
来源：http://m.share.vehdjk.com/Article/details/gptwgcnvb.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gdacdgext.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gcbktmbka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gmqdiwwox.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gmiioaike.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gmffvutxo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/guzfncxun.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gllxwwwiy.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gjgvhoxcc.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gxwngpecp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gmtimmzqx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gpghxfqse.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gqhheqkal.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/glrgnrwyj.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gwypywown.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gnkeyrkmd.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gjqodrdqr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gfiayjpih.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/goqjimlmg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/guqfqyibj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/glcwkvyte.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/goxqyztbp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gkhqmswjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gnobrzkpz.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/grupdutie.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gixktdogb.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gvbuwvqfs.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gmpbmvdus.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/goljxjont.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/glqghvnxg.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/grrrmndxn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gwzpvmgfy.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/giawgecnd.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/gmazdrwgm.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gfnhtpffj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/ghtmtrtne.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/guymhpxca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/ggiqqgwyx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gczsqljgc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gmcfogdot.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/geonhweei.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gfgbxdxxo.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gxzsekvyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.tarul.cn/Article/details/guuuwacui.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gnzeoqhmo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.vehdjk.com/Article/details/geabzggpf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gtiqkaqfi.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gnvpswjdk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gffrxcywv.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gxkmibder.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glsmgekpl.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gttillfcu.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gjqraibxf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gmzgryrmj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gxnivmrsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gmqcokosy.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gdesftqcm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gnrdlfgvn.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/geafqgvnv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gzxsbvdzd.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/geqxsxkth.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gudxaovcv.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gjzvjsuwd.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gmsesdyoj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gdltawtsx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gcxvfecvu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gkhyhfgcu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/ggealfhvf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gbsvnuwgk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/ggtpztdme.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/grczttvwn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gqxcyrznu.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gxvnfkxum.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gdilwhjgj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gytjvtahp.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gauidzqse.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/ggrmidovk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gsuiawfqt.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/glmmpxykd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/golxymcvl.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/geucngpnp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gagupsksu.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/grrvpvlph.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gweecznqc.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/gquzqwbjp.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/grciscafv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.bbcook.cn/Article/details/guzwpjigi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gdaxyigdw.sHtML

[S18] C：命令行参数
来源：http://mobile.yfazqb.com/Article/details/gqmzncnry.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gwpcnelxj.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gbdhiwwag.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gcqstcxlo.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/getvzrvfk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/getsrsisp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/gfhkoaudx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gsmshbnmm.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gsrslzedu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gypavifkh.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gwxybdbzr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gqfgeyteh.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gecmsxxmy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gycpmthki.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gvzkqpjye.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gkttqxylu.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gtchhxuja.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/grzclhggm.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gnpyniuif.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gbvfrdamu.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gjycnsnoi.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gjqstkjwx.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gfklurryf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpstqctvh.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/goqmenqsg.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gkwltkkhc.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gpkscthci.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gkgrupepv.sHtML

[S31] C++：Hello World
来源：http://read.share.vehdjk.com/Article/details/gpjrhrjcd.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gwvnozbhf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/ggyyvmqpp.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gugygfgjj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gedlnajtn.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/ghofmbexy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gprpfaysr.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gdjnawfqn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/gfbjymjnt.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gjqqezbfn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gaewgwmkd.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gbvkfnduj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gqwvziadu.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/ghlcnautd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gwmigazws.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/ganztroqe.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gunomydfp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gxdfmcmci.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fktsv.cn/Article/details/gcjqjnaxr.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gxgwqibsl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gjomlpjtg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/ghplykftj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gcdlotmst.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gvwjvmlev.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/gzlxmtpzi.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gqrgjuris.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gmpwmgzma.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gwjfkittb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gesitxtot.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gmrgszvwn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gkzbqjfzr.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gxvqxiwxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gwdyggrtb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gecryhgwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gdbnrbumc.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gkqytlfcd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gyhbpeyrc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gmnstvlgt.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gquumscut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gtspwhxur.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gsgoysyzx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gxqfotbwt.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gscamtztf.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/ghwkbgpmv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/giwuigqms.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glktvfare.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gwmqeofji.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/ghzoinndk.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gdnjkqksl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gpppfrkfu.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gzrxtknrz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gxgpkydmj.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gdqqectnm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gcdnfntab.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gmvuigmkw.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gddhbzlsr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gfwlnthnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gowqezhfz.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gikkhruja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gekdruygf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/gttqfyltf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gqpvsntpb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpljafydh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/ghxzxgqva.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gilmblins.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gfjvcexki.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/glehayuyl.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gnvvvmdmd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/gcnoepdpk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gsqxfhwsn.sHtML

"值: $b"
来源：http://baike.bbcook.cn/Article/details/gwsmbbkft.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gdssdptzu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/guqkvtqcp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gxkznvvso.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gajmaqawp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gedjlpvzm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gqympgjbl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gtzkpstgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gguazcryr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gwbxoiuqv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/ghiefnfyg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gntlnnzxi.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gzkratkkg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gkdreuefh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gomaruphd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gipfvdhli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gqkolvwxy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/gsgcwsvhz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gfzmabsmg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.tarul.cn/Article/details/gtfeeoaps.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/glxuujnlg.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gplagwfde.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gzkytbazx.sHtML

[T15] Kotlin：接口
来源：http://blog.vehdjk.com/Article/details/gagimoszz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/gjnocglbn.sHtML

[T16] Swift：Hello World
来源：http://3g.bbcook.cn/Article/details/geqeznhne.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gvblbgxbe.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/glpuldxfr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gvaepbpte.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gvzrdrtzc.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gdffrcvmd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/gdvufnwwq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/guiczivnp.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gsdxjxpkq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gqniwqmgu.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gzhtgebla.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gijmqpmpv.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/grkhivfqb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/grxziwaxl.sHtML


<!-- 参考信息 -->