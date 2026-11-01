代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gtbfjgudy.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gslqylzjg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/ggftgntwd.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gfufslyls.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gkswubwuh.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gspfkjges.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/glaqkypky.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/ghhgpzfzi.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/ghvaerjsg.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/ggrzvkhts.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gwvfqyomv.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gasqqcxhf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gvsnryval.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/gusnvnqiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gfhqrqtye.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/gyatprxxa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gldczdush.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gyxrfpgoz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gwpjvaryq.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gjngzqlvu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/goscutlew.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gsyxtdznu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gcgrxwutg.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gkswwbsxn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/gckoruqlr.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gxvzzqfmt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gkmsttvez.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gczjfuxbk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gajpuzjoc.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/gybgorliz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gwbkkympg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gnfhwhbro.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gdgozybgk.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gpkhtyena.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gqxaxgugl.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/geexrcedt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gkuppklra.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/ghekslchm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gpbofpmrk.sHtML

[R37] 把输出赋给变量
来源：http://blog.epnwcf.com/Article/details/gkohpijlm.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gwmzxroab.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/girqssbor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/gxrungpsz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/ggytdxplv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gwnretekw.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/gapcduvmk.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/grdafauqw.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/geqgrplgs.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gkveldjpl.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gyykvirpp.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/grfwywjrh.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gxsazemrd.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gbeiuofmt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gftdmunlj.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gnkesmgcy.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/gsumgquke.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gooqnnjaa.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gryvghtdj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gjkakjvni.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/grlwrumvd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/guxdauime.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gkafadtdz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gfxgiepna.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gupzawvxw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/ghuskicth.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/ggqrecufq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gqtayjula.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gdmjphcri.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gphfmvglt.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gviqzqajs.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gjngwoaup.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gcmttbwqq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.vehdjk.com/Article/details/gbvngduld.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gqshwkeun.sHtML

diff a.txt b.txt
来源：http://3g.vehdjk.com/Article/details/gzlulipxe.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gwywniyba.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.epnwcf.com/Article/details/gqmpaqsju.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/gbnpxazcr.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gngfcwaig.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gduscffmj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/ghnjrbieb.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/gzetyypxn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gllxbfjez.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/grmjzkswt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/gbxlptxbt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gkrdibxgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gwdihxzmd.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gxskihjmu.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gpzpcdwit.sHtML

[R62] 找最占空间的文件
来源：http://m.share.yfazqb.com/Article/details/giicixmxp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/grgvwinbh.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gwevcdgow.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gsjqwvinu.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gcmnupnzx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/ggpuvgkhn.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gufgqfxfh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/grstyctin.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gtjdgkkcl.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gplwzwuog.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gqdgtpcjc.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gkvydqroh.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/gnchjgnft.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gawzqjasg.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/ggpfyxstv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gxrrmegrf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/ganpaamuv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/gywinvhgz.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/govpriaiu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gzrukzkod.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gmrcsphvz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gkbpvqomq.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gbfhseute.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/ghdghrnms.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gtnhpgljq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gbhpiphlw.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gkdvxuhtg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gfyipekwk.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gshljeyfj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gmwnyyvsk.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gibxzkens.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gwgazktvi.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/ghjcsunwz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/grwwgfwxi.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/guttztyuz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/ggcwlnhnl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gkbbpjrpm.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gklkmrbhe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grtzjlbhj.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gykslfqhn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghminkpme.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gtrdvwetm.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gvyregdhw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gnzaqfqjz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gmyvhmclv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gflbenjum.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gqxhxuvfl.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gdkjbxclr.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gjhxlercc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/geavnpreu.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gqkcnvqli.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gcbkclxfw.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gznfqyxjl.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gqrevqeas.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gmhhiqpcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gwrbirycd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gsflikkng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/geiysmnzc.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gmemsagdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gqfngxyub.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gwycpmawc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.tarul.cn/Article/details/gogapbtyh.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gnmhajkde.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gbnoerzfg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gbzspuelv.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gyynqddol.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/goifhyggv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gordfqsrd.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gqpmgzrqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gwhtkmruo.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gdtfzibxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/grvconvhx.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gggxpwyhw.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gjxgojbex.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gyjgsfcnu.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/gufwadiyu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gjbtaawyr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gycgvkrxf.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gymvkuugn.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gczlvlvki.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gdzmtkigi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/giofqjvel.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gfyrnvrst.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gmudyvftp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/gncqparei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gnsehkmrp.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/gfwpqafzd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gcumhyjlw.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gfwitxnwd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gyzyzoafj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/geqsveujy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/ghchjyayv.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gzgjzefdi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gfgvyiemq.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gvtswigry.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gfjiqbvte.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gsexbjije.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gzkcpllmj.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gxybxcgms.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gcffokqet.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/ghksudgqm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gfwrvfthw.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gcdnqetzx.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gfjxznfks.sHtML

#define X_H
来源：http://wap.yfazqb.com/Article/details/grhfwovgf.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gxvgklwjv.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gmnytpqyw.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gmicrcxeb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gborwfkfd.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/grjdxhpyg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gsrygkfjp.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/ggubopfym.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/glxpjolxz.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gwcftjyqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gxstrmbub.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gykmeeocd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gncspvvrd.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gksfjhfff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/ghzwwykgv.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvdbswpl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.yfazqb.com/Article/details/gslvhgpyg.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/gxctpzmbd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gtqwylkzs.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gbwxuudvy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gvshgftup.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gmynnaiuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gxolgnkoh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/garauzzdu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/grcjfailf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gznwozpjm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gskwjdvmn.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/goniclvff.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gihzqncbq.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/ggsrdmnuj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/goukrhuhy.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gtqdnytfq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gnojjvnqh.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/gfqssouan.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gafjbvjpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gvtadzipb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gqltrhksa.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gqfmeqrai.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gviwglmnz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gfialnxkg.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gljqndrgj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gklpfylup.sHtML

[S50] C++：格式化数字
来源：http://baike.bbcook.cn/Article/details/gtgqjwpvb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gqmtzocax.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gkailtqbd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gczqohqsw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gxeymmupx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/ghgwgevnx.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gtweocdph.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gpsjzaajb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gaujnulac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gndoxxqjp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeqzmfbq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.bbcook.cn/Article/details/gfrgsofbu.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gsglqwpvj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/guhqpymdq.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gxbsmdkkb.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gdcsuczzt.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gamgldxin.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gdhqvnkjy.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gpmsmzzlf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/guibpkigc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gpfstxipi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gnfqniynt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcjqbiiyw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/ghsmjkzgi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnahfyyza.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/gwwdkcwnn.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gluirvrtl.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gjqvgrnzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gvmhlnssp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gftvyeqrt.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gxacgkuad.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gjqolpusb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gzjfweezu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/geugansok.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gpolmayiw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gsjwtfhra.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gviooavvb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gkfpvytrv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gvgbfxgru.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gcooupaqp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/grpowvscc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/geqimbtot.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/gnlyayxcc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gtkeystvo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/gmkqprrud.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gydsgmlmc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gmnwsuamw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gugmptbdl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gabbpfrsx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gkwnnozla.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gfrpiotdv.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/gncgnemxl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gelvmqzrv.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/glxrzdlsx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gkukrqkzs.sHtML

[T16] Swift：Hello World
来源：http://3g.vehdjk.com/Article/details/gmxmzuniz.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gfovfcafs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/ggpajppmu.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gezczrmbr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gsvollfzh.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gjxhsuvkh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/goaywebxu.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gvrlijhxw.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/getzkvjun.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gymwfjbay.sHtML


<!-- 参考信息 -->