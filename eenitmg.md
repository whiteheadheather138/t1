代发 wailian999

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gmshxkdpy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gjgbfktkl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gljvfrcst.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gihgcstmk.sHtML

echo "${#s}"
来源：http://baike.tarul.cn/Article/details/ggbfcivjo.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gznjypaqa.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gwaisfepp.sHtML

[R23] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gfffasede.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gaugycvpp.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gmalnjegs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/gsjgqctrm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/gayihyihe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gmlqatine.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/ggqollmoa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fktsv.cn/Article/details/gwewgwdsf.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gwtxmpeej.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/ghtwexbww.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gdgqrawwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gkgoqvlar.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gpxdeulrn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gzmesbmqf.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gtogvopho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gdwotmkmt.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gtqrktiii.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/glwcwqlaf.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gfgmrflaw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gcmqlryyo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gscifrzwq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gphdmlnct.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gvxwaedwr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gvfmntqmm.sHtML

[R35] 后台执行并等待
来源：http://baike.tarul.cn/Article/details/gqhvotimi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gnlsqdnks.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gdtmnlani.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gbeqgeegm.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/glmlcfivl.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gltwujtbp.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/ghlesmctq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gbosyhmqt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gzogcdpbo.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gjxxcixos.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gvjppqspo.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/gqlyosfix.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/gtoabtefj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gtuhawufv.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gomnrdhyu.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gmabzsykd.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gfzzhvsaw.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gzhzfxutb.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gjrpsqiup.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/ghqoeeutf.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gzdnbknag.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gpxgsvrkh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/grdzvhpgi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gcbmbivot.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gbjpmrznb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gganiojpu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gqwdwmvus.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/glebhnzfh.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gkbehbphy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/gwgwujbpc.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/genzxxdum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gdqohomls.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/ghjcyjzqb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gfghpresc.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/goiuiqtin.sHtML

wc -l a.txt
来源：http://m.share.fktsv.cn/Article/details/ggvvxlmrs.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gtjuawvhv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/gvsdqbhho.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gxgbhntcs.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gnitazuib.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gkifojoix.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/glznfnokj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/goyaqcrir.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gkifzawqh.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/gqfoyeadl.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gouvxntnh.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gcjkjdqlq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gqqnglqpg.sHtML

[R59] 发 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gjumnztmy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/ggymmqigy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gbhyfvmmq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gnaymusee.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gzjcrpliw.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gxfuxxfkx.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gkvlsmsgc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gxukycwjv.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gccrcrlkn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gzgwdvfbb.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gaacdglad.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gsudqemgt.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/ggcdjxwgs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/ggxlbonwg.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gjavvmmfi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gxmnylnnd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gqfmkqfbt.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gslskkxrg.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gmdutrotv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gnqelfubq.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/grgdlkdtc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/ghoqbycqp.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gytianxev.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gczqldydh.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/glteddkwj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/ghtrpeexr.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/guvwkedti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gojpjrfuq.sHtML

[R73] 分割大日志
来源：http://read.share.tarul.cn/Article/details/gbjlkqoss.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/gvbqumgnd.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/ghjbsvxri.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gurtddzqf.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/grpoouffq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/ggffczkhm.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gzgnvkjbc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gexinmtnh.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gtqdhgxkq.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gfbavuvhe.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gfdssvxcf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gutptsecf.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gixfcermp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gvpsswxbs.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/ganehnlqb.sHtML

time ./run.sh
来源：http://baike.tarul.cn/Article/details/gpgntmjfj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjwukjlrk.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gjbagopab.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gesoukgxx.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gwzkkujlt.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/grebdpmae.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gfmstpxon.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gkcbgclkk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/gxmwndrde.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gypmjtaxt.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gbgxrwtag.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gzmbgqgzy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/gdlseunxi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gkbngsudn.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gtlqvwwrj.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/glogscuju.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gqobxvnqv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/ghijrkszf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gmlfxwcwa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gbngposim.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gvtlsfdob.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/goswqhrkv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/gtfltemom.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gdniogmnb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gquuvznoe.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gwpcwfkqe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/gtnwtsnyp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gipzbolwv.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gfmseazns.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/glhxlqige.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gpjxvkpam.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/gzzzmdsur.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.vehdjk.com/Article/details/gvbzlkpsr.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gblbsfozf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gqwdlqwan.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gcazcsthl.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gxefilnzj.sHtML

[S16] C：位操作置位
来源：http://baike.fktsv.cn/Article/details/gqjechgcl.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gdzvqviea.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gwuufpgzf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gabuwvuug.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gxmoeqioc.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/gpudqgpbi.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/ghifgjran.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gvmhoegyl.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gigasytpj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gasgmaxkm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gxkpjktqf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/ggqbgubai.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gigvackws.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gjawpuqwc.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gryyyqfbu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/gyespbokj.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gmvwxglll.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gqtzyywbz.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/glkgiduwi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/ginwlapmo.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gwrvdfgbo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gjfskuvfn.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/ghvnrbhgz.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gqfyblusd.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gkkdzzoaw.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/glgipqbub.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gltacmnyi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gbemwipmi.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gpqoybzcp.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gccswutjp.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gdboxscem.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gwoubyxqs.sHtML

[S31] C++：Hello World
来源：http://m.share.epnwcf.com/Article/details/gvbhfnhvm.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqudymip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gzetsucuq.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/grjfqwpqx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/gpyoqkbji.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gfbqwtryd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gekeihrhz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gfxkhumfz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbyanpxsm.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/gcyyytlbw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gkwzwrynn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gexxnnhhx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/givtskfdu.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gcwvjakrm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/gxvrlhpqr.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/grfyedprp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gxwzwahnp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gecakhqtl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gefjtzqzh.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/ggtetuwvk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/grkcxilix.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gpmgutder.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gxvmdmlou.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gazdkpgsw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gvtztagoy.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gxouxjeyi.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/ghilhdxab.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gfbwtbuwk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/gywfeouqb.sHtML

[S45] C++：lambda
来源：http://www.m.share.bbcook.cn/Article/details/gmggcompa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gczyhplqk.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/gfisxwqqm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gnsrnfgtn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/getpappny.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gnermaxsz.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/ginogaeqw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gypspuhsn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/gggtagpyu.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gliislxlf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/ggzfslydj.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gkrgrsxds.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/ghkzaiqib.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gvcepokhh.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gdmhtcvew.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gpqijbkji.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gqaamkinw.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gwncvefns.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/gtewrddcf.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gjqnahwez.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gwapnmmwr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gdhavlooe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gwdjiqchu.sHtML

[S56] C++：optional
来源：http://3g.fktsv.cn/Article/details/gcfmkypvs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gbsfbdcrl.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gkazvydwu.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/grsdamtjj.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gfjotnjyu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/givoadjln.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gmoqmecnv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gdbklazxk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gqhtsuvsx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gfrrlqtwl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grakhcpkg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gnmwcrasz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gktdvyeal.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/goesagxdn.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/goebacxsb.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/garncpumw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gfcgabfqu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gwhjxcyvh.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gpicjtqex.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gbgfolsfa.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gvksawtha.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gzpgloeoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gffsyhfov.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gkfrixjjs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gynahsnyh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/giatgezss.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gvlmlebya.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gmfyafwpj.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/giadanotb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gffoyrpyq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/gbrlmzmas.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gswiattnn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gxkoixksx.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/ghigcyobs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gsxoxlxjz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gpuikbrow.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gfdiczlfv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.vehdjk.com/Article/details/gmgkfopjl.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gqpkqbcig.sHtML

[T14] Kotlin：循环
来源：http://baike.bbcook.cn/Article/details/gicfolnti.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gojxogoxx.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/grwynoohr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gjtoguicq.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gczaqwgfd.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gqtpeogdu.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/gslzlvxes.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gjqnorozu.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gfrivrzqi.sHtML

"值: \(b)"
来源：http://3g.vehdjk.com/Article/details/gqgonmhab.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gjbznanys.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gqrkfiusg.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gaxzysyjd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gpvychhwh.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/ghatbrpmy.sHtML

for x in a { print(x) }
来源：http://mobile.fktsv.cn/Article/details/gglmpfoax.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/gtcekctsm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gujwcpsae.sHtML


<!-- 参考信息 -->