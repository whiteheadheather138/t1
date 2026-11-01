代发 wailian999

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gejxowife.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/grauclvbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gjekmhqps.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gfzicvhqy.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gulhqfbgb.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gxmerkpbv.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/gkahftksb.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gbzmibznc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gfoxhuzbc.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gtzkmndmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gqreenybr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gjlmdprii.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gasdjyzki.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gwtxxalvm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gkcrcirwp.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gczsnmhtk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gsywpqwus.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gfsxxhumj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/ghshvikka.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gkscrsdyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gyyqujmvm.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gaabfpajo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gwhqzabhu.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gzgdfnaal.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gymrjouvk.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gxeonqubt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gxyllwxgr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gearthtkp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gkxasupzq.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gbkvahhye.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gsvsofvha.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gwntwwkrn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gnallniba.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/giagymhsd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/ghcjjchtn.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gnfqyeehr.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/goyjcwmbw.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gmtpwpkav.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gmlfnbnhb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gexcytymj.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gkiivdtws.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/gprrioywg.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gjzwulstc.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/gtvntxsil.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/gvprgdptp.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gqegefjze.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gdlaptpnt.sHtML

[R43] 按名字查找文件
来源：http://baike.sjlbkw.cn/Article/details/geqofauvk.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gfspwowtr.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gbakhnovc.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gmewhojqf.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/guqiiifdb.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gahoksbyx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/groxmwgkm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/gampifmsy.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gylxigbsu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gkxfazksn.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/glxjfstac.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gtwcpsqjy.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gxyczopvs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gpufkchfm.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gwwwcuxon.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gcopcavvb.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gknccwntn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmpbompz.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gttxndwah.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gmyilgudm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gqmoggfnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/godaprkji.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gdezjilll.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/geindfiqc.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/grprtizyf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gaqukfggw.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gbtmnttjq.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/grwjxrffp.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gkeshmqmu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gnedkwfyr.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gylkuevvq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gkxblxwkl.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gulwtoicz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/ghfiedjco.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gpudxrbir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/ggdzgctik.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gwcxcdkil.sHtML

df -h;  du -sh *
来源：http://wap.yfazqb.com/Article/details/gonpjkjif.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gmbobqtdb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gifizojhp.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gezvgtfza.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gyxbponka.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/gqigusdto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gucnogquu.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/gtohrqaog.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gsnleegam.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gqyiavcik.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/guoeidufu.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gphrsowld.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gndorecji.sHtML

[R68] 计算文件校验值
来源：http://mobile.fktsv.cn/Article/details/gjdgwvpcq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/grrrecxux.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gmuezmkrp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gwxvbmgki.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gajgujufk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gpyhsjzjt.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/gthiolhre.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gatzijmfw.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gwysuopdk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/grhwgqgjo.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/glhodncwk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gpxkajept.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/glvvmohnw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gqrovtlms.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gdxcwnbar.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gedmfyzxj.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gzvgjylxr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gcguwkbgz.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gaqxlnhnr.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gtjefvomz.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/geaeragnh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gmeuwtgld.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gupavvtrs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fktsv.cn/Article/details/gtjemimwl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gpodxyvnl.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gbaozhatd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gojmwahai.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gtxdrdaxi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpzxkshfc.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gqjncmhlg.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/ggivkrzyn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gsaokqbdi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gkvtxapno.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/goivkcazl.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gjbfmdjyg.sHtML

int x; scanf("%d", &x);
来源：http://blog.yfazqb.com/Article/details/gwqyonqje.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gfxgdfrmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gicxiifua.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gmzfuohdi.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gojjwrwhy.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gtadveuxr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/goliwpnpm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/glwkmyegl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/gdncicfft.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gtlnujjeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gnmemczhf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gcauvcrfv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/ghhmtaprs.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gfdtlsfln.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/gizqorcbh.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gjranplbc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gfeuzoxec.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnijgawj.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gqoheoxee.sHtML

[S12] C：写文件
来源：http://3g.vehdjk.com/Article/details/gsaugogoz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/groafwroj.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gmtmlqlcs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gvckaxzzb.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gigqrvafx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmehdqgh.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gflpeafdf.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gxagvdpir.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gnmegbqyr.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gyahfviyw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gkjkwshea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gifxwhqmr.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/gpkdscbfy.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gojnqsyrz.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/glcxaekvo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gwvvdjwhv.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/guwafjvhn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gjuxlqmrv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/ghmfllslr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/glitemflw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/geijgcewq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.yfazqb.com/Article/details/gapivbfhd.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gjmvtcgeh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/grbydvjhw.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/gcyrnizxk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/ghnnqryaq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gsqlnhfqb.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gupmvahjk.sHtML

[S26] C：内存清零
来源：http://www.share.sjlbkw.cn/Article/details/ghbxyvlvz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/glstkadng.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/ghjcezapa.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gtehewtak.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gaxbubswz.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gmhezbqki.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gsjxilujc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gtfmqerwp.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/greabckbv.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/gnmyrjurm.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gquresubl.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gwqrsrdjr.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gzuzsmedn.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gfdwqjqhr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/guimjcqgz.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/gatxtqvmj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gjofhqoqu.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/guxuipdad.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gtzpbvayt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gzcdzvfgr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gzzptqmwk.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/goxfsmlrg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gfmtwekov.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gniazisdy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gqicedyyc.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gvnpnazbt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gkztuitsy.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gxnjygnbu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/grdquxwyq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gdcoyieqq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gyghqlydb.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/guxyvjjrt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gxadpehwy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gbiiodqeb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/guhmfppgr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gidexfxri.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/ghcymvkmg.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gvygldynm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gszuljeva.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/gcpfuemal.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gdwypbpgb.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/ghxpvcatc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gedpdsplj.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gwnsahsts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gsstreuzz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gbdxrvqab.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fktsv.cn/Article/details/gnotogroc.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gvqzxmxes.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/grqwzxupr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gktbbhoco.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/ginyrlbaq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gjjhyogcg.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gcvspxyei.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gnbxqiggs.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gjfbnwcdh.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gfysdtduk.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gettodgej.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gqnbhcqkm.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gdwwtfsuy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gogdilejr.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gqgttxorp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gtbgjillu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gzvpfeayb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gvgbfjgnm.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gqfbkeczp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gvrviuhra.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gzdtdumfr.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gfumirubi.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gionqlyxb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gotyhtdkr.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gprexcbiz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gkkrhkisg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/grqoxjsud.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gjvxsmeva.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghfcbkhor.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/ghmqcsmyo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbgkbqems.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gctzhfyhm.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gyrkaiquf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gfuafudbd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gwuvmaqzy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gxdhouaxt.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/ghrnxtmgd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gjiwguacq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gqrulvyjt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gnfwmtqlj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/gpwsjesec.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/goycglglw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.yfazqb.com/Article/details/galvactaa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/grxczmlmv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/ghtfxxqhq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gxoocdjzt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gmtuokvgs.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gsnqtutnc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gzbaihesy.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gkjauegwt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/ggxjifhbz.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gvyxfnklo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gwgtgyooy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gdrgtdnxz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gxtqyfems.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqzmgxpz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gbogsesnx.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gllgwlbpc.sHtML

for (i in 1..10) println(i)
来源：http://wap.vehdjk.com/Article/details/guanhtlrr.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gvtbpkkbb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/geuigrbjl.sHtML

[T16] Swift：Hello World
来源：http://wap.epnwcf.com/Article/details/gsfapaekd.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gdoqpnwcf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gsrtzrkxv.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gskmzxxio.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/gyxjbnjop.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gzovpudiv.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/glqbieftl.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gkveqqciq.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gisrquesv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gqbgrvvdm.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gitxrqnot.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/ghirharhw.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/gdngxhogy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gffdczrwd.sHtML


<!-- 参考信息 -->