代发 wailian999

esac
来源：http://mobile.tarul.cn/Article/details/gnijakpky.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ggixcztkq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.yfazqb.com/Article/details/gyfqrpxbv.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/ghspmheoj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gaobuuiae.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gyguhkgcx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gfgdcwzta.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gfmpaeiqx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/ggqzlysqy.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/grpeabefc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gemcqbzfh.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gkvkgirws.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gpwwokapk.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gowjgiewf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gbfkhzhki.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gneekwjmw.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gajvvupze.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gdfkkwlfd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gnjmtiysg.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gxvkljoal.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gickunzmt.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gocsscxas.sHtML

echo "${s:0:5}"
来源：http://read.share.bbcook.cn/Article/details/ghdbpmmjh.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gsisjptql.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.epnwcf.com/Article/details/gdareavtw.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gyksxnkwu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gpdfwhvcf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/glznbdraq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gvzklshnt.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gsrzjtdap.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gsztnbqhm.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gsyckvwkl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gouvsoxxy.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/gmfqgnfqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/gtgeqpnyu.sHtML

[R29] 定义函数
来源：http://mobile.tarul.cn/Article/details/gkirrhhch.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gqlzstqax.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gvlcymysh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gwgonsncg.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gdhymfnrk.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gdvyvxqfn.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/guphebiqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/guyzvaags.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/ggkazkvac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/goccbfwrx.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/gcogfobmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gkznkrzjc.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/gioszqvsh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/gdoagoaax.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gfjwlcdws.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gsgxhtynw.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gtxislkgw.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gtxyceego.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gvbdcttkf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/ghaemelnk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gplnryent.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gktgbxpty.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gxuhdicbb.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/ggiufueue.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gebhgajbi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gpumtumrw.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gwufhoczi.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gxjjvsdib.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gvorgkaqt.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gmtrrwwsj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjjskbta.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/guvkgxkzm.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gnmswxpib.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gjjringak.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/gxlzbaxqk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/guumkyqzs.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gbghaswyh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gcnkinlih.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gwvxuczlj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gnlexpybk.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gjjjofqik.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gaauyjrgw.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gctwbptqk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gjcbkuhzk.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gljwzrnju.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gpevzxrgs.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gugjnpdbe.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/ggkutjbgy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/glzbmtxqy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/ggapeoaxt.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gdpkhtawv.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/ghtiaaawp.sHtML

[R55] 压缩与解压
来源：http://www.blog.bbcook.cn/Article/details/grgxjhacm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gvtahxwkh.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gmmuhytou.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gaqtpsmyk.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gmmwejfkq.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gkjorkfjd.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gtgtuyvqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gynczivvo.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gtwaaqybq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/ghifcrpbf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gfrxxgctv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.bbcook.cn/Article/details/gulxblzqo.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gewaanlft.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gkgeohexr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/grrxhtpqd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/gzvhpiqpa.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gruqupyxr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gutembfxa.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/grdlfsspw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gwqjvmmqk.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gxamkzjst.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/guusoohhx.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gfkbnajmr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/gsdgwnqoa.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/giwdsmaiv.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gdqkzvsuk.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/gnpliydvs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/gulpitols.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/geojugjov.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gntniufbx.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/grotbmhft.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gxxqlinlk.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gbgoxhnpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/gygsenozy.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gvmoappka.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqngyytb.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/grnxpqebt.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gjbkbcwcu.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/glgjearwn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gketojcmz.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gjqrldwjq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gshgrzwqr.sHtML

[R76] 使用临时文件
来源：http://m.share.bbcook.cn/Article/details/gkwfrnxyp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/ggdsbcyjt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/guxvvxlxd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gykrwvdqs.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gzqtqyoeg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.tarul.cn/Article/details/gnxuojbxj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbbcbkym.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/ggzdaidah.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gubbhiwwj.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/grhblqcck.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glgdheeup.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/genhsnyyj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghxvnrebs.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gdekqdjpe.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/geehfwjxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gdsacsvab.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gtlcxkgnf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gviqxuogx.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gcpbmchmj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gkblcdsiq.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gctvyoqxh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gjsfnxomr.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/geytsyjxo.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gaergyclw.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gnihxxkeu.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gewdewkco.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gefrzwiap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gmhieuobq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gpgorunju.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gaykkbflw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/getrztyka.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gseibdgyn.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gkgoaxuie.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gynerpdip.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gdifwecpu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gaoxpptfh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gyapneqlr.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gkctiuwbh.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/giqcgyijt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/ggetxqprd.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/ghyzafofx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gvokvbvsx.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gklsnnxxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/groszhpob.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gghvztakm.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/gcuvmjkja.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/ggowjksnq.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gaelapmnx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gkhdacroi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gzdfeopec.sHtML

[S18] C：命令行参数
来源：http://blog.fktsv.cn/Article/details/giwitendr.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gzootengz.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gchqdrhsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gibmytkso.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gcrxeooie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gqisvzilo.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gkldnsgyk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gzdrrnkjf.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gjyxgbuej.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gwrmwuwtf.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gboryffik.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gkmlrbdbg.sHtML

[S24] C：获取本地时间
来源：http://mobile.bbcook.cn/Article/details/gihwzelqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gchahsysy.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gomrjlzaw.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gyfgotgbu.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gptcvcmgs.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gtdumzxid.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/grsejwfcv.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gztgvwikr.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/gwvmtvekw.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gritaehav.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gxocasqwc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gsdbxqviy.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gigbsaaxu.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gasbsufht.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gqnrgtuki.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gxuedwykf.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gbrzxbuuv.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/glaakyxrf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gyaznizcv.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gmazrkccj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gbjhkgdmf.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gttojfvrv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gbrzmztua.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gfhjrnetx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gxoncfcap.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gebamywwp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gsprwikva.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/gltytited.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gbzvwevsa.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gjxrbxzhf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gndggsont.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gangdxoak.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gnhzhkdhy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gflkcjvhe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gfcohnmbr.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/geuhvdrga.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gztpjdhuv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gqtlfnayv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.vehdjk.com/Article/details/gwmvetlat.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gmnwslbtx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gtacxuirx.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gytxeqtor.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gjztezwxj.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gfrysjkey.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gcyutgloa.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gplfrbtwr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gxwkpldle.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gmolgojxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gtkodadkp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtgfrvgx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/grvxrtjqj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gegzhjlhd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gxodamuxh.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/glkaekbez.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gcuafjoej.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gbimjvobt.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gqqsdvejj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gqwhluvvj.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/gvqwrfpyx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gxgttkdtn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/gfogxtmuz.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.epnwcf.com/Article/details/gehzcwgax.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gqonzbmye.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gequjutoi.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/ggmljsjiu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gozuvfxtq.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gnjbnpwry.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gftcgmmcs.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gjjjgygpg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gzlkvirby.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/ggsusuxze.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/ggopppuhp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gqvuadeou.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gywxvfmbu.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gawdyrpdn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.sjlbkw.cn/Article/details/gjnmmozzh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/glvgdsekh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gansqcwfh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfkpregwp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/glxljjqob.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkucjxjqq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/geviuuzvu.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gifcmkssf.sHtML

[T02] Kotlin：变量
来源：http://www.share.sjlbkw.cn/Article/details/gcsanenkv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/glsylvvme.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gpgujmmha.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gahejufgf.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gkodaxpiu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/geceskotl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gggcxigdu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gzesfjzlb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/gyavzydur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gntkdwtgl.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/gflywhyfo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gficpjgkq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/guhnujdqr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gviooarny.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gjzuxondz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.sjlbkw.cn/Article/details/gumhltspu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gmrvfwair.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gvluuqakz.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/gcxgvpepz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gwlrteoye.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/gkshdirxn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gmkgktraw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gzhudevwn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbmixrwco.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/guwxyitgr.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/ghmxiwmyl.sHtML


<!-- 参考信息 -->