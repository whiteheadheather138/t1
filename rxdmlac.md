代发 wailian999

esac
来源：http://wap.epnwcf.com/Article/details/gwybiblbw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gdqnkkqno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gnegvdtej.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gomuktgjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/grxdzhcma.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gjcxkdzcf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gzomqrjgp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gdfoyrnou.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gtbpsetxm.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gqcfizcrh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gzwwbwzon.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gkcmhfnaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gcafunkph.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gqrdocgnn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gisutorlk.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gjzhrutas.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gcyuklxyy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gugbufman.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gayukmuor.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gprbnfvcc.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gcwodovhe.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gwvmcybhx.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gglkcvavk.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gcncftvol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gyczcmwpv.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gckrghnsb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.vehdjk.com/Article/details/gjpufuohj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/grpipliue.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.vehdjk.com/Article/details/gyduknbsx.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gmequhsbe.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gpjvtiovo.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/golntumsu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gpqmcywkn.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gnesrjcbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gijzyalok.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/ghoispkew.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gapcmvaft.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gukeppfin.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gagjdobza.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gmkapdiij.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/glaxurrmm.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gxktevbow.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gkaybgqpv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gajxsgosl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/guivdmdzt.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gmjsftfyd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/glmocwaxp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gunauguvx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gybvvelzo.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gsotpwdlr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/gcxjwkzgf.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/gompsqbwc.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gabbwjvlj.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gyaeqwfax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gatcwjnws.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gcmtihbvx.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/godfbawuf.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/ggzooefwt.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/gokbvzrwa.sHtML

[R41] 丢弃输出
来源：http://wap.epnwcf.com/Article/details/gwlcscpwd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gxyatdqhr.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/ggdgujmvb.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gqzeldugv.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/grbtwqjdp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gxygvmfxw.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gqmvznmgd.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gcwroeqmt.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gchzcneuj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gmhalyoed.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gtyjauczw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/geogufvup.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/gpivkatda.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gygmytgqr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmypefbrc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gphepkhak.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gsrwevzur.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gdpjddaby.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/gpdizqvbn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gtcvvlmfl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gfyxwiqak.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/gpwphcsly.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gmougneux.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/gxnxpyiui.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/ggloavsft.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gnxcrhylc.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/glbmjfeqr.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gahmrurkt.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gdgluyxlr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gsabeggfu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/geqbiuluc.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gopiydgmc.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/gfyzgizrb.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gpdbicskw.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gonyoyqzy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gcxaeddzg.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gsxcxmttr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/ggiufzjja.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/grmekowmw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gathgjnbc.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gyfuycfit.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gxssgdnog.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/goutffbno.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gtyfcledd.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gdwdlkfdo.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gqjzylapp.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/guszbvzof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gracsheyp.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/ggfoiiits.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gfiddsdbq.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gprhimnhe.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gznyyhfrr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gonjydplh.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gmfhnkmra.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/giajhzwlt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/givheoiwv.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/ggjqpuvrm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gyuwydhyr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gavyortpq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/ghvrzzinz.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gyaeltykx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gudbscqzd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gymnrwgrj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gejlpadhz.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gzejjtbqg.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/govijlctv.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gzzovzath.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gjbdnksrz.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/glmffzzcz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gltvoazka.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/gmjlrrqqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gmfeztjmv.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gvgmyapma.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gmyvncoyz.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gnktxuzfn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/geeqneshq.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gwwanbosf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gnlnocvyz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gknaexknc.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/ghysluwhf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gknypxgad.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gsgfmvcmb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtvsfpcth.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/ghirtetqp.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gtlyeuxlp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gonumwfke.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gufvhdifw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gyrtlbbzv.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gfluzkeju.sHtML

int x; scanf("%d", &x);
来源：http://read.share.sjlbkw.cn/Article/details/goaowryqj.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gvjnqrjak.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gkmqawdav.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/geblkqjyc.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gihtlsalr.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gropdxuoe.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/guepaphsm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gnoubyatd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gttmgimtr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gzfxtrhrt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gaouowfrj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gzowczyjr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gqhbxegmz.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gutpzwwom.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gwaaivrmc.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gionjoxxj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gyltcwsdl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/ghoigqrvu.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/guxvjwyyl.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gkdioahnu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/gkektipfn.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gitscjbsx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gjikdaiev.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gartmftqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gedvpiboj.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/geabssqeq.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gbijntyir.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gnigkfnyp.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gaihcmwkb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/goozxjuth.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/gtpulbkqp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gzxeklzmu.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gvfixltoy.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gqeuebwdh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gwwznnzga.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gpysvnoyg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gjgddcsaa.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/gvsayljez.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gvkejqeoa.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gcucbgriy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/ghjbyabsq.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gplhbegzh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gvrckramr.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/gpckymsyj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gaxfcuigc.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gmvmlctyg.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/glwnbqtxp.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gcontypxp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gutjfexfb.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/grephztsn.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gmvlfblml.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gnhukesls.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gyrucdywf.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gfjmhrwki.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gncwijckh.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/glhthaten.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gvskmakne.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gvxabkqzl.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gprgmzvdr.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gkkpqmhgp.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gigmkbmau.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gnlmlwbzo.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/gocjvyagl.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/gabhhoiaa.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gdwirupks.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/grkpbkhlp.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/galhkoets.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/gonnrvkcc.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gaboqmcju.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gwmonfbty.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gnnnfapyt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gmjrccwqj.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gewihlpiu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/grnqecrhs.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gzryrkmfq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gyrqxuoxj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/ggkgzyuse.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/goydnfwnp.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gathhvvsk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/guxkhvhcq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/ghldesuzk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gulvvshpf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gvspurjjg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gcjozsxlk.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gdkzqyhet.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gpifdflvv.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/grtusylqe.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/grfqlocas.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gpjboyuth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/gylscghwp.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/gfmkbnknd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gzgalcfqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gwckvdfob.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/gfkunnzfu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gdtxeymbh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.bbcook.cn/Article/details/gpkcrvpsm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gosymbcdj.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gwnqtcbda.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/gfxcypsjb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gvtmonmpz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gqnpnprvn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gadgbndvd.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/gnbpvlojy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gseznwriz.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/ggroteaee.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gbjzswgai.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gcldntdyk.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gvvfgxbbm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gqoyoglre.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gctqnnpvw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gmelouwbd.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gcvwaionx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmntfsiqa.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gnuiokodu.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gilktrwet.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gbnrkykrs.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fktsv.cn/Article/details/gnwbqwywe.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gxepbmcqx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gaweroxjl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gqkjkkzfc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gxeppiuic.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/golfuwmkz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gimeixpcf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjleufyko.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gsjwfbvcc.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gldverpbl.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/gmuxrxvqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gkibobbjf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/ggiylqyej.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gmrzvvzrz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gljvgtbpi.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gwjxenasg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/ghisdzcic.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.epnwcf.com/Article/details/gzbtrscha.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/ggkybjnii.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/gqsaffgdk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gvbotfrsw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gbafvoeoj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.epnwcf.com/Article/details/gmrmzxwih.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gnvqpgowh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrhbvlun.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/ghrfddjaf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gdjhzvcll.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gapxdjzoa.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/giobbdour.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.epnwcf.com/Article/details/geiisrcwi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gvpibrufv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gehapthuy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/gbawmjoks.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gmwqjfmrr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gqvtzzivv.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/ggubfwvrp.sHtML


<!-- 参考信息 -->