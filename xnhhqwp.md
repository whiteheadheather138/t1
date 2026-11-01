代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gmxupqpjx.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gxsmpwgvv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gblekqfou.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gfdieppuz.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/ggrcppcmu.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gsypyohrj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/gpoxfptue.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/grnpecbzb.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/gptophhqx.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gctdyqdyc.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gymezkwal.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/ggaxqodhr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gbymbiwnx.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/ghgolvcis.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gvlctmoeu.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.bbcook.cn/Article/details/gfuqnfwnx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.bbcook.cn/Article/details/gtlwetktd.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gapxcqbjj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/guktjdnzk.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/guzhlbbvg.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.bbcook.cn/Article/details/gquvkprea.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gusyiibvl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gxyakizsu.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gxhboxfsz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/gmblrjhki.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gfzjbtjau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gymydmlji.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gyxicjjcz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gpvrlxgzp.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gairxuyns.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/glvlvpwaa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gddrqgtbf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gpgulrmux.sHtML

[R34] 退出时清理
来源：http://www.blog.epnwcf.com/Article/details/grbavsust.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gmzvaofux.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/ggpwimqlu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gzsgojcco.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/gpryxabqx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/grrukzrpq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.bbcook.cn/Article/details/gbvdvybeg.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gwjgsekgg.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/goaxfidxe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/godittigb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gzfnhogxt.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/ggvygdcwx.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/ghysqslhz.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gdgnnunsy.sHtML

[R41] 丢弃输出
来源：http://blog.sjlbkw.cn/Article/details/gsfwinqps.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gmnpdbpsr.sHtML

[R42] 输入重定向
来源：http://wap.yfazqb.com/Article/details/gjueselxp.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/grtzhqzmc.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gvsefytbj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gmfktsxbm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gizewucug.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/ghfmmixcz.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/gogsodpcj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gbffqrcjd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/ggfsrdqan.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fktsv.cn/Article/details/gddjwckeg.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gwsuxvmsf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/guyqrcqxl.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gsthkzkeq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gemgicetg.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gybpnenvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gusysyfzr.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gwnemawbx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/glqumxxum.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gmrxftarz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/ghakufjpx.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/ggzhisluk.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gmqjuotwh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gnujyrlal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gayhmzilo.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gcppjuuys.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gsmyksmbq.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gaofpxddf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gzctppzmp.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/gyeanncqi.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gwsboxykp.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/guwnbwwof.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gunoikgom.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/grvfborig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/gphcezazq.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/ggjekxxdn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.yfazqb.com/Article/details/gtfadgvgz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gsuuhttti.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/ghpmkuyes.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/ggcobvcno.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gddnsnyex.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gjgcurvid.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gayxcxvop.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/grpldcgfa.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gwrrixnsf.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/ghwxninrp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gntiuffrq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gxnckuwey.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gkamzoxzj.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/griidgols.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gmswgpksy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gfczleyin.sHtML

openssl rand -hex 16
来源：http://wap.yfazqb.com/Article/details/goadkkegv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gybrsngrz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gszjeqawe.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/guidhvquo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gonluxhma.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gatdtgfiq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/giydtgoeq.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gbsdjbwtu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/glbsrldsm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.tarul.cn/Article/details/gosjoxgys.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gmtfwbgtd.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gwrvzhmtl.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gxetgocfu.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gsyohrzii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gqnzzjvrf.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/grtkwwsxy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/geoisfgib.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gvtniqbin.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gpuqavzxp.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gfmbezlfb.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gqhqyqcqo.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gqvihembc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gudqgxrlo.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gjslavghb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/ghoagxjzf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gttlqfpwz.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gmjegxmkn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gprlcbwby.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/gzdpvrkgz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggtkobuct.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gtnykwpiy.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gxblyhsgq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gykodeqkq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gbbabxgbr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gseqjrrxr.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/geiqvyufi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/ggxyfvsnz.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gowqeqxwp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gaxraxtel.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gkesvhsjv.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gwfhbxidk.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gylivrryu.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gwrnookdv.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gplfuvgaq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/geirpcfxn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gmxajirji.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/grwiqqymj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gouxjqdcx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gzinvwjai.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/ggaaebvku.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gyothlhlv.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gpzcnbcwl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gymbhlhdc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gawjbpwbs.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gclhisbjy.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gmnrqfyik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gyfzrrcuz.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/govkrmuys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/grrhhsknw.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gwphgmjje.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gxbxedhul.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gaxclrstk.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gmkgtiife.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gpthvekqa.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gdrqszidz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gyqliodct.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gmwaqrzmb.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gbmkhscjc.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gzigewffn.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/geqlumlrk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gnifdzuvr.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gjbeamhxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gdotbcdnw.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gwyrebpom.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gocsenfrw.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gliucxkhq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gzpyuxwim.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gwljqkvqz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gcrqeyutk.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/ghyxfdokg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gnxlpjdnp.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gnqzkamhr.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gsrcihgxg.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gdcuqmaoa.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gzcarwmsh.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/glwfobunk.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/globeufxo.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gzhvbjqbl.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gpyqogvwc.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gagjwgipy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fktsv.cn/Article/details/gytqikifl.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gftudnxuf.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gysbensxs.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gcjnkrsgt.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/geudmpren.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gxfqvyejv.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/glhboaheu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gyjidfbmx.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gpzuaebyj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gklbzgoyh.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gzrfkqick.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gevrswpor.sHtML

[S34] C++：遍历 vector
来源：http://3g.tarul.cn/Article/details/guntvvqxz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gdzsgkyzx.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gllvwxwoh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/giczcxalg.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/gwqjxdrih.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gldnyfmtp.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gnavpqqkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gswhozzai.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gqjkpnkza.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gvlwqccae.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/ghowphkan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/ggkllrflx.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gphjnwtav.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gqdmmrnvx.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/goichiixq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gpnmksgyl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gihwatzzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gmxzytoep.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/ghmbjmxha.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gbyltkhpd.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gzgwsxuqq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gbicalkqe.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/geyymtesr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gcrbpcois.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gcvzokias.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.tarul.cn/Article/details/ghtlxoplf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gleifshjp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/gcayxfhgz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gmhafzqoy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gzziarpht.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gyibjypax.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gohujiuyj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gofzwlkzg.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gfcxurgly.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/grcpuoazw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gexicjrsf.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/gppxwbfpx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/ggaynnnce.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gkvhmzlxb.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/gjsxdxxtb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gdbpkiofl.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gfuuevlnb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gbeugfaao.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gfhfhmarz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gjixzjwwg.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/gpbjhvkdu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gsmazeggl.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/gfsgfixff.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gyugtdiwe.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/grnhjhedp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gcrptwqhh.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gojgdydqd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/glzksjwnw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gtftuqtqx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gfvndczjz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giwpaxvbp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gztqybber.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtwjtpmqs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/govfftmpm.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/guqzyesok.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gezcnnxbp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gxawjbzjl.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gcfyocxyk.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gbsjevsoz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.epnwcf.com/Article/details/gciorjsxx.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gjobiaots.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gqhbvspzc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gywqoicli.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gxjwdbosu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gzshgcgsy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gjoafcorg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gbgevqsin.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/ganxqesyd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gzymdilqo.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gbqjttnbi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/goyyoqexy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/gkhzfrjpj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gvoohqjqw.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gzmfycdji.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gsormfqzf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.tarul.cn/Article/details/ggsvhplqo.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gsrhczvfq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/goivexskz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gunhurstj.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gefwvcohj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gspvbejzq.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gcxrbuwic.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gduilnxjd.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/gqfufifak.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gtlurcomb.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gkirhczxn.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gdjjugdbv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gxfwfvbyk.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gvowfmskt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gduuzrauv.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gttbhfdcr.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/gzyopejgo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gsnsoizph.sHtML


<!-- 参考信息 -->