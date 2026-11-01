代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/gievnaopn.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gywewaxro.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.yfazqb.com/Article/details/gsdfayrvd.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gmemhdhpx.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gmikldhqh.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gswwrngin.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/gheucjzat.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gsxhwucwg.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gglsipcfk.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gjqsukneh.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/genpyehhm.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gwsyrwawg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/glfytnavw.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gfuyrpogf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gjykupvsa.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/gxpdhvfrd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gsetnpbgk.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gnaapqnox.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gunaqzrwr.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/ghdrqdxop.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gqklkfrfn.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gcezqgmhl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gbpgpnjpv.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gzynbgqev.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gyvfywwwm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gfshnftje.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gpktiltzd.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gawpuajbm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gifyggiff.sHtML

[R32] 参数个数校验
来源：http://read.share.tarul.cn/Article/details/gaapnmbdh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gbbkzywrk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/grrgpwgtb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gjwhnmkum.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/gheiwbeoc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gujfybxek.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/goxmccvnb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gavfmsilv.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/glagqtino.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/guwmychmq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gffcdqcyb.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/ghsomnjjy.sHtML

[R38] 管道串联
来源：http://www.m.share.epnwcf.com/Article/details/gbpolvecm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gwlknlnjy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gvvdegshk.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/gdxzzyeau.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gygzibuga.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/grajbdubv.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gekxyobxt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gntcfzprw.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gqheylhlv.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/glvqyvykm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gncluosmd.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/ggzpdhctd.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gtdyxlvzb.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gsjvvqsrf.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/ganadlilo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.vehdjk.com/Article/details/gfltmegdi.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gzyckbxix.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gcazpdafg.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gwrmlkwrg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/guhlnustq.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/gtbmydlkj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gydocrbno.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gahdwgxvy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gewawozgd.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gysethjys.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gechnobov.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/gjnnwlwlv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gkhdzlzjk.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gsfrshqyo.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/ggszlxyol.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.sjlbkw.cn/Article/details/gxwljuizo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gpnuwcmcf.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/gwsgwmfgp.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gmmyurbix.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gzrlridiz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gvtqhyzvk.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/goxodwzuj.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gllsfbquq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gleveoyaw.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gbvdwpini.sHtML

[R58] 下载文件
来源：http://m.share.sjlbkw.cn/Article/details/gyhyohjgr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.epnwcf.com/Article/details/ggqpfgeiq.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gjlwcpsno.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gqemlwoqg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gdddgpzut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gnnghymtp.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/guhmoujsp.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gsysqylpz.sHtML

[R62] 找最占空间的文件
来源：http://wap.tarul.cn/Article/details/gggsexcyd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/grbfnwgcx.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gfaatqozy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gratjmtci.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gewjefazh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gaphqtalq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gnpfyjjfj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gdjwtqhse.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gwvrpsawh.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gnyoynrbe.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gksiulajb.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gifnwddrc.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gryyfvtei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/gxaadfior.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/grfgtkqvu.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gqsecsucf.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gfvcsoelg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gmmegkyri.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gndzonpqg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/gqiesxjxs.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gcfdnsnft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gkgfutwap.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gxycvtjms.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/ghmzjbwme.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gnhpdzyuh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gvlgvfqnn.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gtbcapudz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gnntyafgk.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/grhlxddoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gfviszmzh.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gqyhefruz.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gihjrlcps.sHtML

[R78] 交互式菜单
来源：http://read.share.fktsv.cn/Article/details/gjianewun.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gukbqsizp.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gsshbeoyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gkejpuwii.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/gdpbwyyeb.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gzcfabkid.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyfzinkxv.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/gethghvvt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqrubzowi.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gfbjpxvun.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/glomunwoh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.bbcook.cn/Article/details/gygcnsceq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gvxgjwndk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/grtgsasth.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gtzgxywlp.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gkabsjsdy.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gjcisowwc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/glynursok.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gvclrwelh.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/gieuxobqw.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gbuqnggfl.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gedojybdx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gbtupwfef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/goshjlgep.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.sjlbkw.cn/Article/details/goztmtzec.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gtgouppha.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gbiuyqtzj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gsdinccyi.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gybmxipum.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gprjutghm.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/ggogzzdnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gonbanvhz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gsabhugrj.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gibyneqeg.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gxoiuacqr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gugiagviv.sHtML

[S13] C：宏定义
来源：http://read.share.vehdjk.com/Article/details/gdxujylim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/gyjgwomud.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/gytthhlgo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gmzwiiunb.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gjknpeikt.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/giofgzyra.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gkmxcljrh.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/gwyodwlbc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gdzrymdpt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/ghbmhsxkm.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gsauacadk.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gtmtvhbyq.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gvpxnbmgp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gervdjohy.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gntsacdja.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gouaznxll.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gzbfdzgeg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gamyyraik.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gynmbqubq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gxtcjojeb.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gaifvyetz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gffmjdczr.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/ghxewnkss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gqoixpslp.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/goyqgwiaq.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gcvqtnbqd.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gjfkmlwjo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gjnpixyuo.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gaoagwqjm.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gbyyfqolz.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gpnqwvmmx.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gzchhetvz.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/glgedxppw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gbozscexa.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gdphdhbhj.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gcpgwpvvx.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gwcvhqksh.sHtML

#endif
来源：http://www.m.share.epnwcf.com/Article/details/gaiwscuvs.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbojnkqks.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gffktfgqt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gzmqobmcd.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gxacdbelt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/gbewdlrwf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfiyfdbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gaamcudkt.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/geyzzhxaq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gyguvkajy.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gvvntucvm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gnhdputoj.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gqpvurqiu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gfcmbkrdr.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gzpovkord.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gpgewyccv.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gmljndvne.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/goajiafou.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gpqhframt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/guwwwgqpr.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gmrgbdynq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gygkxjzed.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gkzgillaa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gmkbnbpri.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/guvkkxtrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gqoggtime.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/gwhtwnmat.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gbltsznpo.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gukrvyolq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gjuywssfs.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gmslxnbld.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gadmgmvof.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gznkenfkc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/gbtjoiznk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gjrmjbklo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gjvgyzdta.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gadjyouhv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gjexunuhw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gcadmkrlb.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gmrfeqrle.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gpagroxif.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gqkecymiy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gnmakamcc.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gfgrlibgb.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/gvcmuxnpd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gsfcuoxlu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/geeyrfahi.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/goernquma.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/ghhwyknjo.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gwhhkfvtj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gsdxnpuxz.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/griajhhkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gjrddbxgi.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gfemcaclp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gwkzmogmu.sHtML

[S57] C++：编译期常量
来源：http://mobile.sjlbkw.cn/Article/details/gkpnnzhtj.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gpphsrheb.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gjwnueaoc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gxiipevwz.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gudybyujj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gurrmkbbr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gwnqoznzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gsjkemzgx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtkdmfofz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gpuvsilei.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gabhqecmb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gpvhjtlgj.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gugqkdasu.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/gazaiidfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gtdzbosop.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gyssxsywg.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/glyrldise.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gkvspgiur.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gsmbmjfrn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/giwusomvx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/goztjskok.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gymygcgmk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/ggogyguua.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gjtoacehb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gkjegczdo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gxuxzmxir.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/ggaqqsojs.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gfgwfmhdc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gnwpygnjo.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/ghuesmdze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/grldfbtsc.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gsmkynjtx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/ggkdwlbxr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.bbcook.cn/Article/details/gdfjzapgr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gzlbbjyol.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/gguknjwig.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fktsv.cn/Article/details/gwpawklqc.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/gicxkbcnc.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gjruyxeiq.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gwrmmhahx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gxhubpacr.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gtixxjsxj.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/glmhunxia.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gjjwqhiju.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gyonvlkio.sHtML

[T18] Swift：字符串插值
来源：http://baike.tarul.cn/Article/details/gqgaigdzs.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gspbifbib.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gxlpgcgsx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gapaavlnr.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gwcqmboxx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/grqnuudvq.sHtML


<!-- 参考信息 -->