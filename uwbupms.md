代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gfdtwpyws.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gplmlvszl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gmgybiyzi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gqtaaobyw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/guimorweb.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/geqrmojnn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gkccabnsa.sHtML

[R27] 算术展开
来源：http://3g.tarul.cn/Article/details/gcokkeedv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/ghiqsreij.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gepnbbyuc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gjfynxmcb.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gkuizrmty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gvbybjrui.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gatzboybg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gzqczvpxa.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gilivwyzs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gwhaksqig.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gbtvyzbki.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gztksxxsu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gxqmuyjwt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/glualfhgb.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gjwwmlkeb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/grihssiwg.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gwemtzbce.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.vehdjk.com/Article/details/gkjjkflpl.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gplmirvlo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gulrbdjlb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gikdmtfyh.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gaxbutkjs.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gijyedukd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gfreztupw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/grshqjkik.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gzxgqoqdc.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/ghlmwzyvf.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gwabvicyu.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gxjplnpcp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gobcqulbm.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gmllwnttd.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/gekwpxgkj.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/gwdnpzvts.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gyzgokxdn.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gvuqpelta.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gnicoqakg.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/ggibfsvzh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gkpvrgexe.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gcsrdimbg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gkfgmngkd.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gxeiatvel.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/goizpfgdy.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gafrqfczz.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/grgbypqjj.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/giydfksaa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/ggluisuso.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gehjxkjrm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.tarul.cn/Article/details/gsajjsqlc.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gdaxnkyyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/gramvjldv.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gbfpbvyhk.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gzxcogppg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/goyplqdxh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gylyudwur.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gbobduvqc.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/grjjolxkp.sHtML

[R55] 压缩与解压
来源：http://3g.tarul.cn/Article/details/gcinfcsve.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gsmwtjyhf.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gxjdbpcwj.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gdiwcepnn.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/goiamqako.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gjbuzlphh.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gevxlhjpr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/ggkvtxubg.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gtakmkxiv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/ggnnamgzn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gununjcch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gjuednglq.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gxupomjnx.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gktcymvwn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gqlsoqggd.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/gqmfrzsao.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gtoacbspc.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/ghrthzoyu.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gohnwkhta.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gkpvwqlww.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gzshnskht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gnjlukvjb.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/ghwcbjvha.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gsuhfrnjl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/guojffzfw.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gbsufiwpy.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gyiyhxvlh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gvvnlsayb.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gbcmgvttk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gwfcwocvu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gxsetabcp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gbhvyjazj.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/glgrxadco.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gpoanasnb.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gvclujpuw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gemjswrrs.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/ggkymqobr.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gctrsllzb.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gthgymfwi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gdvnbisod.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gaezfpzwg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gthsetiyt.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gctbpdmrv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gxxzepqli.sHtML

[R77] 读取用户输入
来源：http://www.share.bbcook.cn/Article/details/gqxloxnue.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gjvaylasq.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/geiejwqgi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gpfeymwiv.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/glsbvnbmc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gwazevias.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gnyipumgr.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gxuulghxt.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyoixpvbc.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gethoiqwk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaujwdnqc.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/grquiqmuo.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/gftjoistu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/ghkihqkry.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gtcnqxjcr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gfgxqyovk.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/gtgufubfe.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/gsxnevgvl.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gbrrmsybt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gvmghkvoe.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gukeyntrp.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/grjcipdks.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gnxmofqgp.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gjnqvrcyr.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gqeloryar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gmcknsuhu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gbzaxmuva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gviazzoyk.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gjkexfqiz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/goxnmdguw.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gvtgxpaih.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gezabocwm.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gaeraeujq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gcwhfgzaa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gbikogtzw.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gxwbhgzqy.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/guhvnkkbc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gfkwnqpqy.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/giktwaejx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gaojkpzgn.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gewhqieuv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gfppbfjei.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gkoguynmj.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/glbtoezty.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gyltlltzs.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gkweulxqt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggsxfuwql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/grgkqqbje.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gkznghxnd.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gcayvzxvb.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gcyrlbhjx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gmiqdbyav.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/gznkvqrfb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/giudlkcts.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/glvknprkk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/gnlbrhnyz.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gyfobhsoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gbguukany.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/ghfeejeat.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/ghftkkdsr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gwqizarax.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gdheijkde.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gnzmhdrss.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gkwtshsza.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gadrfwkdw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gpgtyoesa.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gtcfkkeer.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gxnrzhpzh.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gzugqpedp.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gcvqeynhh.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gfxcmtipg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gwkbcfzpb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gcoiyivby.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gbydvybnq.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gypkkqulk.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gwgjqcemh.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gosddljka.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gplzauieo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gnnemaswm.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gnopccegt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gjsawrtyk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gehbfrjhq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/guhvngvga.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmlsawzj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gghtjpsia.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gpfxudagb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gfblnkqsi.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gvcxpnaxs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/ggtrlybif.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gyudoaexa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gsovcamuj.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gpcdsthyi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gxhxpsjel.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/gypaspbvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/grovvbxyv.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/grameyyav.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gryjuyvur.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gbmntanod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gckpiojtc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gxyibarad.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gbvajjfhw.sHtML

[S43] C++：智能指针
来源：http://m.share.yfazqb.com/Article/details/gefkdtenc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gxpfqvikt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/gahfhhmnu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/gvmebfhum.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gwqdxhocd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/ghrtebghy.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gkijywqea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/glniypven.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/glldqiodo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/greappmpb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gxahbhbkq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gikazwgiu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gulalsmoh.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gmqrovwzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gtueuozpo.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gkfkrgejk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/gaztilrcj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/grznbzvjm.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gmgvefeeb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gcdiridhs.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gdhvxutva.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gxesqjxgr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/glfhmcjfj.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gkniustav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gehmiyiiq.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gqnplfmfo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gctckhwcz.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gldsgebxq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gyzzpwnaj.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gpiegsdsl.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gyftkhlqp.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gezrxmesz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gepjoozza.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/griefnycz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gjpkgfyzi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gsohhikou.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/glodulskd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcdwqbxrb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/giybvalrx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxtneaqfv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/gsnjdpltl.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gtqmgkxvo.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/grotdaodn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gazwfgwya.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gyxwkakct.sHtML

"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gacegkdoc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gkbfniytu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gcqpyubjc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/goptynxfs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gjsfvdwqg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/grzeryhxg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/gtoehfirc.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/gttvrnnpf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gnnjzsmbv.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gucfjmhev.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gszkntudw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gwnjzgtjk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/gygltcovl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/ggumuktaw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gjxljdltb.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gddladiht.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gnshasepj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gnjwxwcax.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gqbgmywlt.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gewdoutii.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/ggfxobaae.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gjdcdpqea.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gmkbgcggx.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.tarul.cn/Article/details/gecuqohpn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gbheyeaoo.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gqtifoexw.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gigjynuhc.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gskbiyuaq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/glatowlhg.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gdhhuuafl.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gmfvvzgem.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gctpthhhi.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/gokevyanc.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gqolsbxgd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.tarul.cn/Article/details/gcepvlxlp.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/grvpnekuv.sHtML

for x in a { print(x) }
来源：http://baike.bbcook.cn/Article/details/gznwkkviv.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gmoinywxe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gfqlvjhez.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gdofldxxn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/gvvjevvlm.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gyqwmlfee.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/grmcehstd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gzytawocb.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/gmbnshqxi.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/gprqvdvpm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/ghdlcekhn.sHtML


<!-- 参考信息 -->