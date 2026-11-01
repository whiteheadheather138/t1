代发 wailian999

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/ghbsuwgba.sHtML

[R20] 关联数组（字典）
来源：http://baike.bbcook.cn/Article/details/gwyvxzzcn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.sjlbkw.cn/Article/details/gpqlktctp.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/ghyzpnuyo.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gjalovgge.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gsrskyhrd.sHtML

echo "${s:0:5}"
来源：http://read.share.yfazqb.com/Article/details/gazvzcfax.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqfgwbdl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gsgtawebd.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gwnwtvrhl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/ghetihgnt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/geermveqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/ggswnlgdx.sHtML

[R26] 命令替换
来源：http://3g.vehdjk.com/Article/details/gtewvmcyz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gssvrjitw.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gygdfqnvz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fktsv.cn/Article/details/grgnhsxjb.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gfilnhwoy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gpdufmryl.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gmnceqfoe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gqopraeob.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gzbapvnjm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.tarul.cn/Article/details/gulwxrzct.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/ghwbafiid.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/guaruipdv.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gvewibfyv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gwfbeyhmf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.sjlbkw.cn/Article/details/gkmvifyud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gnxqljzmk.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gzmukqwpl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gjtfsbmgf.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/gequoutok.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/gpqxgkfxn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/ggrsypsdx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/guuntqzcy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gwwzxrewx.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/gcayydzea.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/gixbomvqu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/guxfightn.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gdtararkp.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gefhsecvw.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gakqpwnow.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gfmyhkugw.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gyawldwwo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/ghiawmcrn.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gtjisejjl.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gpunxqzfj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gqwqvusuk.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gmrhowlgz.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gbmgacurw.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gvrmmwcji.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gxdgrdwtv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gjyksjkvw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gzqidyooa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gcnrnezpz.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/grxjennws.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gakhgbpqd.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gusotmewr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gjvdzubwu.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gjxylophr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/glcejfnhs.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gvrbjiwak.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gmgvsyfcb.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/ghwgirjga.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gnvtuzsey.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gmsqzknpk.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/grogwjfuj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gzxrnfbjl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/grllkkncb.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/ggkurgeeb.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gztgndyfr.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gjykgnjmq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gamsqquiq.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gnrfpivih.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gdkqslflx.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gezuyowsb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/giadmqdmp.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/ganzmshtu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/gupshakuk.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gjdvyvwkj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/geupioytw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/ghypriija.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/grztxvpbc.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gmejkicri.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/gtinbkemd.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gdqbvcnab.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/ghamfjnlw.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/gzggktatr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gliaghyhe.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gkqdpjebo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fktsv.cn/Article/details/gpujiljrn.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/golazlfxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gewqmyzvo.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gursdtvqt.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gssrsthoz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gamjvzxlg.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gwfhkomeg.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gejeexkdb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gnxiymbhh.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gzatxeqvp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/grwthapyb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/grbfjpspd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/garwxsvpb.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/guaihavho.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/glxwzwkns.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/grvqjixil.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gqlwhxbot.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gdfuvlmsx.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gcqrdbedf.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gdmhguidb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gwiigocmg.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gvqojupxo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gpdekldfw.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gebibnknr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gysejyagf.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gkuybygmd.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gmjmcgjun.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gnlbdohws.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gunnzyowl.sHtML

[R79] 解析命令行选项
来源：http://mobile.sjlbkw.cn/Article/details/gzuxftabm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gyuwfsian.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/gbwhqrrnd.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gzrubuylx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkipdkqcz.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gpdzoovmy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnntklwcq.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/gbodsipmt.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gxynvcbly.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/grdtqtpbk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/glskkvepg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/ghfarzeez.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gooanugzh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gxcqcqdrg.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gnzvvwqmy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gzhvkdnal.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gdwbjtrkm.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gpkawmevb.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gcpyryotn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gelsfahzi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gfcokimmx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gvvqlbecg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gaavrfahg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gcnkndujc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gjqqznjup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/grteauowa.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gqmfpynlb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gvlmgmrdk.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/giobapqgh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/ggynzhgaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gcnxgajdy.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gcatikqza.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gpsuaogws.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fktsv.cn/Article/details/gypkisrot.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/ghfuahhmv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gvejravqx.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gptavmuts.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gyjgbmmqx.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gbvnccdvx.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/grotlpybw.sHtML

[S16] C：位操作置位
来源：http://www.share.bbcook.cn/Article/details/gmzgartxi.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gwvdktzec.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gkppfxdcw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gstmvhbtd.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gbvhfnenb.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gnwztarfl.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gyjhnrfol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gcwyypzvk.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gxurkmupd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gngzdwopn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/gcatjttef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gfyhbxvdx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gjanshwst.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gsocssmkb.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gnvjolaxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gzjoebdrh.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gbobaygtr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gbdljudvs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/goxvndqzd.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/golrijiuo.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gmaeapsxi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gtymzcjoz.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gwpaptkhu.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gygcwebqp.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gtsvgnfrp.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gqjwyycap.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/ghnpnnsad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gdxwnyltl.sHtML

[S30] C：头文件保护
来源：http://blog.sjlbkw.cn/Article/details/gozskmfgb.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gjmeaxntj.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gnvxfglum.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gcjctybww.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/gtqzqwkea.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gsvmcghtc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gwdviotap.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gosuvdjzr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gzuyjxpic.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.epnwcf.com/Article/details/gwxakguuu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gdglycrfy.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/geukputlr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gpyyykmhf.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gcqthdlsc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gfsubixfo.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gcligmfpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/glgzncvoh.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gitfqgjfw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/ggqkqklyx.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gzgceawug.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gurowdbya.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbffupldj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gtsorgwmg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gxrhbwuar.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gqmyxsole.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gzqtdsdlw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/ghpoeegfo.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/gttokcjlh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gplvnccfz.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/ggfflgmev.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gwlfcjuyg.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gnbqaxjva.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gigxzazgl.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gimsuuert.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/ghlvoqasz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gazcpqcna.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gzldaxkqk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gzmxxbujl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gbwvgtsij.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gbqxkpkzo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/ganxtbezj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gltlhgmxr.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gfwrtpvzd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gcjpohxyn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/glitlnldl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gqjzyxfab.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/glpjwbyhh.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/ggpghdvdr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/gwbjlmdut.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gsfingfns.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gcojuooij.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/grwibpvtq.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gfmwjvqcn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gzokuqpcf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gysqvtmfp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gcfrfcqdb.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gwypritfr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fktsv.cn/Article/details/gmkngoqls.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gvwmradmq.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjokjhpvn.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gynxrpxkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gxpmtpffp.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gmhpkoons.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/ghduviyvk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gknvrscrm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gqzaxgmoz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcuhsjkoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gkduowmcj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gswwueank.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gclonoxfq.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gmhzdbtng.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gnsvxxsoi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/ghdqujalq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdwvdgmz.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gwjprulus.sHtML

[T04] Kotlin：空安全
来源：http://blog.fktsv.cn/Article/details/gevwbyunm.sHtML

val n: String? = null;  n?.length
来源：http://3g.yfazqb.com/Article/details/ghcyfvqnu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/ggahzwgcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gccpihcyh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/goctweyzn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gjlqlplsb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gnniizfvq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gzzmfoqrz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gidcjyrkl.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gpialfsux.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/gqfhmiupd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/glbxefuow.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gdihirpxf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gsmkqbztq.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gxnmgxhad.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gieazdead.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gutcgbkmd.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gxzvphgnh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gdmaxcyzm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghhyjnezd.sHtML

[T14] Kotlin：循环
来源：http://blog.sjlbkw.cn/Article/details/gvxknzkue.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/guivqqxho.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/gkidwqjhx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/gkioenlzs.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gwtokewga.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gpcuzztnx.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gwdxwqqks.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/giekrqqti.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/guytfteea.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gmqoufaux.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gwudygswg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gcxezdiyv.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gmhpleuxf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gwvjssmwb.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gvmglhclk.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gcrpqjxhg.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gomeobuqf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/geywliodt.sHtML


<!-- 参考信息 -->