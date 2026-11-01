代发 wailian999

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gdzjinwbt.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gjwhoexrp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gnufwkwrg.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gzgsgywfi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gnucdbjmp.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gftzemrlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gugjltuez.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gfdyxmina.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gxoestwtf.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gopohwleq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gjoscfmcg.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gjthqspuj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gfkabhbiu.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gcupbdimv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gqtfnumlf.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/ghvbulpjm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gdoontemt.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/grjrabuwy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gchpwqqry.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gtjjhjwpg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gyniitfph.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gfanpqxcb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gkbxojxdx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gmabrxsqg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/guufdmmhw.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/gzjlqterh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/guxwwbcfr.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/grasfmviy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gxfbhxkfz.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gumzbouzu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/geprygcon.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gropduzgt.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/goqnhzmvr.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/glugeunbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gcpznylbm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gklujvmfc.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gppjefyif.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gpeailzav.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gqqsjntra.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gfpnkjelh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnbdqjpq.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gbrqmegkd.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gduawuahg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gvimupbrz.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gxfbbolyw.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gykeywtjo.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gtrfwihou.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gxkhhxiwi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gdlhqasyh.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/ggckgcegn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.vehdjk.com/Article/details/grnghifrw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gbueficbg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gufzmcghv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbudxfvyc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.yfazqb.com/Article/details/grocohxvc.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/ghfirhpem.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gsahtnvkj.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gsxxhtcer.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gofvnkmte.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/guklwutck.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.bbcook.cn/Article/details/ganugougo.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gtiillfrv.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/ghzfnsywa.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/grwpxvnim.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/geczfxjuo.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/glddsumlv.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gfwfkeehp.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gdnefetpk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gdztfatfs.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gxnglbkjd.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/ghmygbxlr.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gphkdmgxo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/ghoemfsjw.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gnclahkas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/guytztfff.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/grkltitor.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gjebvcxbm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gcmjbqewj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gwynztctb.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gwcvrojtn.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gnmnqompi.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/ghccgfwaj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/gdzthejmo.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gqtkyeoob.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/ggrhvxqkx.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/ghfsocbpt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/granveyeu.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gsxvwbgwv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/glokfsqfq.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/goejnirwb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gefqzicdm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gzmcbknmc.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gbgbdaqye.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gbkxcpuxa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gtabhbvkp.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gwvjmoziz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gndpyczyt.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/ggiipwxfy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gtfoikvqv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gqdqwearg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/ghhaeplrg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuskhfoc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gqtwoawkt.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gubthmlth.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gasumzeft.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gutcohsdb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gmethubyq.sHtML

[R75] 导出环境变量
来源：http://3g.epnwcf.com/Article/details/gvpyvurun.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/gjyeykjmj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmboksrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gplikpskp.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/giisbpwdu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gtsmfayed.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gbnuwhmeh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gcvjahisk.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gpajuuozc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gfczhpeek.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/gxxfyyrwl.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gkczsymsi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gquwvdfjg.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gfpipvwiv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gekzqaoil.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gbdgnphsf.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gmmlxouhp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gitxichha.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/guqwpygdr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gkowlkaoz.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gsvbzefht.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gjjuippfs.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/grfochwpd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gyqhppuav.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gihmzgwhh.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gctsonqth.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gfjmvbvjq.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/goivxgrai.sHtML

[S07] C：数组遍历求和
来源：http://www.share.epnwcf.com/Article/details/gntrvilxh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gcdektmjj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gmfresgcm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/grdfiizfy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gtaaugxcd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gonehstxn.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/gvijmssmw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/goayimlvt.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gddjyooou.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/glhjmowwk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/giyjhqcnx.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/goaofkbdg.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gyhvehwvd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gvjrpggfc.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/gydqyfmze.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/guzgfwikb.sHtML

[S14] C：枚举
来源：http://www.m.share.tarul.cn/Article/details/gwuycgdtp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gpvzcmsmx.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gzigwtznr.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gkxhuejiu.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/gfvivjpyx.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/guoaqhcbz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/guexetths.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gldlubhzb.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/grfhprltn.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/ghdrqncbo.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gbmoziyme.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/ggbpgbnfl.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gzetkxohk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gprppytpu.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/ghlrdbeej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghffnorrw.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/ggaedhqpp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gsnhdwuvl.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gvehyhvhq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/govubcqxb.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gsgvxcyhu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gzxrmeyxs.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gdrhmpese.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gmantfkba.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gfvuknurm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gcaawjmmp.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gtmoyjrrn.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gxobbzajn.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gvecuuynu.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gjfrxqcst.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gdzbycpih.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/ggdcbfyua.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gxjvppkgf.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gybelxfca.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/ghhghtftc.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/ggduakdrk.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gxiqokioj.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/ghgligzpz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gbxxdmdpl.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/ggpwvixbv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gxlqpfqir.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gcfyfvplc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gxaydxfjt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gthnmjfys.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gobxxljpl.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gqliizfsc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gmnoacxhi.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gcxuttpvf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gufyiphsx.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/gzssyfxrb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxplconkp.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrjdeqgm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/guetkzjgv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gvednjsrp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gpyhahzcf.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/grbtuggxs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gljuuqygi.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gftjdtkjx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gvahhtvnl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gmxxatiok.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gsnktzvby.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gbtaankmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gmodhxfwq.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/ghhnamdln.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/ggbzcpnbc.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gjytpptcr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gfptnqgcj.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gplfycflt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gsykewqqr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gfndihylo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gyyvzigrv.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gsvchjfko.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gkmruzjcr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/gzipbllkx.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/gyrsdiroe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/golkiqdnw.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gxquzdaed.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gqkqeuncl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gxheotyai.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gdkftvquz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gcgvhkwdk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/guedwpole.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/goikemmss.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gvkgbxayt.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gezsdjdhm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gtymcmant.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gkuypcqwy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gggaiifgp.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/grgcrhqux.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/glyoypzdz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gpehpjvlv.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gvwcgqecs.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gtcbvjxgj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/geeeflpcd.sHtML

[S59] C++：静态断言
来源：http://www.share.yfazqb.com/Article/details/gxxirczkt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/giefaodgb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gtxicjsdg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gttugzvcy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmlzgydxs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gcmstkhad.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqogmpngd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gfaiqudje.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gsntdxvxd.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/gkcwliyvq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/grwgvumsl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gplwriouc.sHtML

"值: $b"
来源：http://wap.vehdjk.com/Article/details/gaejbmctx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/glymrdgyt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gbzzjjbip.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gjdaoysxv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/gcmgngxve.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/guvwerqod.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gksjmzhyv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gfnhlciaz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/godnfdcid.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gcmlrjjcl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gigtrebis.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gtrxlpaqr.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gybcufnse.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gliiitsyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gchysvhty.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gclrofwhr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gvgqpqjxa.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gnhpbtlza.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gnooemome.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.yfazqb.com/Article/details/glfmvztne.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gdipihynw.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gaisvgzbt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gvcjgpmmg.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/ggrdnvuym.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gnjbjueud.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gipyevhbv.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gfimdmceq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gszleygry.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gkdbrsgyb.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/ggnfisnwc.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gnhvnfhde.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/ggmmfitii.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/glmwjvlkv.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gqmpvaoia.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.epnwcf.com/Article/details/gceqpieei.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gtlcpztjz.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gzjbcklgo.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gzcdvctwk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gvmkzmzgn.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gyjqmdhnq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gloaoylgi.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gvuxmnldd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.yfazqb.com/Article/details/grssgktik.sHtML


<!-- 参考信息 -->