代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/glawqphfq.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/glcnmjees.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gsnwgikne.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/gvhikwfzl.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gxmdltalp.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gzwbjfviq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gbkppuvxx.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gkscxnrau.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gtvrmhsjy.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gsuyzyfnm.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/geotbnkzc.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyoflvxp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/gzouqigja.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gvsdvstup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/gnbjdjffa.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gjxwozjyv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/guzvxaffg.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gcwvulcfv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gkmkxlfpa.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gspqbioqe.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gzavzjqws.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/gruarhoaw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.vehdjk.com/Article/details/gzplmcbxc.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gqrnbxtvh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.vehdjk.com/Article/details/gxzpwtrlu.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/gqxlgkffn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/gatkedvye.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gapmvvzlq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/glivmgwjy.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gegefymmm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/giumuwpso.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gsdkcgwgy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/ghjwhlwtt.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/gishfbuca.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gfboerier.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gxzotwpzv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gbnmrujyd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gqrkgjhcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/ghwklxevz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/grtmfzqmv.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/geuvqwezm.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gdxpkjhsv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gyftxpvjw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gbtvaeaba.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gypewbzat.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gbrgumgko.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/guzdmbyup.sHtML

[R41] 丢弃输出
来源：http://blog.sjlbkw.cn/Article/details/gnsevtjxm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/golrlbwqw.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gwdfwaazo.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gsgozwoug.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gsuzmqksb.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/ghuvfccsk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/gezptkuec.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gnggyapts.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gzuekiyoq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/grmirllvm.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gkvybtyvz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.sjlbkw.cn/Article/details/gazjzhrfg.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/gydlvgpsa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gulzbrgty.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/gkpqdfvwi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gayxvbxxo.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gqbroaqig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gesqinxyn.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/gofuqeyzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/glmktofuw.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gqprdtdtj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gqpbpynfr.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gbgydbegu.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gujeuefca.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gfbnrntov.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gpbdbogdr.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/gffjmeytu.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gtuwybkes.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gckrjjatt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/ghtdbjzwz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmdcsmik.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gwpdkxacy.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/givyazcpk.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/grckseaod.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/golqnaffi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/giiqgzbrv.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gnlldzysi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gdpkaxojv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gcjvwgywr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/ggymncqum.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gyltgoona.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gkafwodxr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gxizsrjhb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gmcjmzcpy.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gbvecgkrw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gqwiapths.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/grnrepfja.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gznxzdudz.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gzwnhrjrj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.sjlbkw.cn/Article/details/gimiqtjgu.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/ggqehqlam.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gmmwhivnr.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/gxgolfpvs.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gdpzgcjqu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwyhjhii.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gperejfmv.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gkwbnzfss.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/guojpvvfu.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gojzmtcby.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gwlvcctzy.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/gitnumtpk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/glbryvntn.sHtML

[R72] 等待端口就绪
来源：http://3g.sjlbkw.cn/Article/details/gbkmbwusd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gwxnbjqnl.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gegqponet.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/gcqmhnonl.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/goucfdtre.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/gafqiyrmc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/ghuxgtjlp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/ghemljbut.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gxrucumrr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/goygwfzab.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gidafowko.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/groyjycej.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/gdchbrlvs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/gxdadfjfb.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gtcxaubaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gkquxvark.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gakchvoqd.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/grofqlfwo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmdatdufr.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gvvybtnzk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwhtpuwym.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gxgivoffl.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/galwvcnog.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gwbdezlhi.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gzcuvhkdz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gxzvuicyv.sHtML

[S03] C：读入整数
来源：http://wap.bbcook.cn/Article/details/gweyjeteg.sHtML

int x; scanf("%d", &x);
来源：http://wap.bbcook.cn/Article/details/govvawbpt.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gvedueiqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/giutwahij.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/ggzptulfv.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/glvxrgpas.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gdqjaiphb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gaemlrxhq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/guygyuxqq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/ganeexsiv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gfkqsxrpn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gsfwofhzh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gjadzgjvv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gapphprwh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/goiupovov.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gofacjprx.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/glrtjzvki.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/ggrqqlklv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gsqylbsjy.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gicoriaeg.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gowfanmia.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gzdnlhfls.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gewcwwtbx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/grdjqusbd.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gdibtezlc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gayyyebgw.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gjnfbttts.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gdezujuoi.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gfmvgqjlb.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gopfiucms.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gjieesbse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gfhzowoyg.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gjaskqsnc.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gvbqhajvw.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gcatpphps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gjrztbuoy.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gjaeirike.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gkuwvmbni.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gonvghqip.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gabqcgvoq.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gufcfoarh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/ghtpqljyc.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gbflmfqih.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gexafupnk.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/geiagpfkl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/giiegudag.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/ginllcnqa.sHtML

memcpy(dst, src, n);
来源：http://3g.epnwcf.com/Article/details/gnpfjikgf.sHtML

[S26] C：内存清零
来源：http://read.share.epnwcf.com/Article/details/gfmtrqkde.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gcdueoshk.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gecmrlhdq.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gikrwoncn.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gcecpkitk.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/griemoqoh.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gexzcxzdt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gbkqaapzv.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gpctuadbn.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gatolxfgm.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gxaujwfwb.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/gltjbbome.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gxqoojnnw.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gyxyyvsbj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gbbxosgne.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gjmwocabi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/grhzlsrla.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gtxzxxpjp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/golztcwko.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gpjmrxqst.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/grikdcucy.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gxgcqvngi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gysjipgzn.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gefgeorvi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/geephtzbf.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gquzgscmv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gqftszktg.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gfilgjrbn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gjdyhmqbj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gastmcsoh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gdovmxpnb.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/ggwxtgisu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gptjlsmzg.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gcqkzippb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/glaxeciqs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gnpfwzabo.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gditkdrky.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gztfhdtuz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gwhllcjfh.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/ggyveezit.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gmwjzjyae.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gnzohpvnj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gcqpnrbjn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwrngeck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gorpmecgy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gachentmx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/grvwxxisl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gimlmkojm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gxgfogzen.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gxgyzkzgd.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gvnikojlp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gvtqumsuk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gjppgdcha.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gotnumtzb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gvanofbsx.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gumizgjhe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/guimrhbmv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gowgvzpfu.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gdkixmevv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gqqawizhl.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gufaacqlv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gjrpufljx.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gqugbfyts.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gutfatpvh.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/glohdtpjn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gnfdmsccf.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/guieavqfm.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gjbhfprkj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gvqcgscwe.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gymeckcvv.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gopjhrsup.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/grmcjmibr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gxqagsvpr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/guhaxakcr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gigcoefdi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gdzyiscep.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guvgmthbp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gsxiefhhj.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gqsfixnne.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gwtfgbcav.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gazsdnyoq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/glkgakppk.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gdgakwksi.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gabnrlcgd.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gcbhxhuxi.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gkalbysrd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gxxkiihim.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gxooryyqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/guxjhvxeu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gvurrivpy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gwvenupit.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gzvzhcipv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gcafztuuh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gjzcqribt.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gvmvvzmfc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gxytxvsrq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/glhjgirvz.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gcemwmrrf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gsdvwethi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gnbuqqujy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/glgbkojrx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/gwssrofkx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gzaplhmtm.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gfwrbgcqe.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gorcsadap.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/grlerdznr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gvpzvaekw.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/gfmhqdgqe.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gledwpema.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gteivkdbb.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/gsoifkovn.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/ggakzohll.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gdsxxxgdt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.sjlbkw.cn/Article/details/guhufmkel.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gdnnosvtx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/ggtficmtv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/goosovigb.sHtML


<!-- 参考信息 -->