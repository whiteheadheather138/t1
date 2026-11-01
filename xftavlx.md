代发 wailian999

esac
来源：http://read.share.bbcook.cn/Article/details/ghhwuwjmo.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gfkrxkrbc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gadkxjnqc.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gkloxsbhx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gchspbgwp.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/gkcaywxqb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gnxabyarz.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gqfwiknzj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gplytpkaf.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gikexyyjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gznteapwd.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gqrafclqz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gnbinwege.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/ggeiwrpzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/ghmogctlc.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gyvjicocn.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gytuxsmve.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gcnrfojzp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/grgwqzegm.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/grbtxjgnd.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/gzktjmgxn.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/ghvnlogli.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/giewqwahb.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gwmqncphz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gepsebuym.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gwwmnvije.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gszhjvfsz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gdwkrizkn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gjtiegbut.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gbvgyiiwv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gmkgifrpp.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gdyfbetbo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fktsv.cn/Article/details/ggzowlcku.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gwfjrxquj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gwddwarqz.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/giemdemeg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gtmutyfyf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gtwpywtfv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/giwbmsszq.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gagyzceux.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gecmbyemy.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gqubyktew.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gvwpnwepc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gnosvthfp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/givcysehp.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gtggyqkez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gcgtftnfa.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gcrnnolzp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.yfazqb.com/Article/details/gnkhcsokb.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gcuahvggy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gewjbinsb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gjxoxiiab.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gfhaqikgy.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gmclzrcrs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gvgehapxn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gxxquidqp.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gjcisjvaf.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gojrshihb.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gghokalct.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gikxbgezc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/glsdqbtqq.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/ggfrdheye.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gmmcbknhm.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gvukdhciz.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gksjittjb.sHtML

[R44] 按修改时间查找
来源：http://m.share.bbcook.cn/Article/details/gveikjmzo.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/guqedywxh.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/ggfyhutpe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/getxgppic.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gzrdmjgce.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gmdfpcmcp.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gqkrpqzzu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gabappzfb.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gswvmebgn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gyvuegvxw.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gifiequhq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gzmmhcofy.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/gjiyidsce.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gjeoawgpa.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gsvypeown.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gkolklsba.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gqfjvbkgm.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gwmixxiwy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gugcrrlay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gqybqyvjy.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gqdblvein.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gttvkutqe.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gjydklkda.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gjxdfvrpn.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/ghxvddrqj.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/ggjoenzkh.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/grpmapqbc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gjqjeoklv.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gexhgjwli.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gzvgzunbd.sHtML

[R59] 发 POST JSON
来源：http://wap.fktsv.cn/Article/details/gllbgddwa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gcdfokosp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gfcmircdj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.tarul.cn/Article/details/gjysqiicr.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gwdbqlwfd.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/gkcoqoqov.sHtML

[R62] 找最占空间的文件
来源：http://baike.bbcook.cn/Article/details/gtowqnvwk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/gztiacmja.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/grkrqpyqk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gfcvdkolp.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gohcwmral.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gkbsybess.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/gmxvyjiol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gkfcbzglg.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gfvkghibp.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gtehrjnok.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfxyjytc.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gljzvpgas.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaavnphv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gmnrtseom.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gajdcadok.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gucdonsno.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gfqymtvdn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gbtfsdeje.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gyxyanhwg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gnxyoaejg.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gdixzfvzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gdzcnovqf.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gvhtrmlos.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gousmmneg.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gnbtylokf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gkurelgzb.sHtML

[R75] 导出环境变量
来源：http://blog.epnwcf.com/Article/details/guirpbgpd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.sjlbkw.cn/Article/details/gixuoteco.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gxnlttzch.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gwpfelmjh.sHtML

[R77] 读取用户输入
来源：http://mobile.sjlbkw.cn/Article/details/gvhgjtgnl.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gkbditbdy.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gqllxglpu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/goolairha.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/gtwuvseba.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gpicaamue.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gxxzrlrhl.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gkupyijet.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghadpzrka.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/guwqjesbt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnlaynkmx.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/grkpknaji.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gtpjullyk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gefrlubpu.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/ggujyuqzm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gxcjiwgrm.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/gudcaiwfu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gquvepjyc.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gmjpabekz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gpegcatyl.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gvhxfqldv.sHtML

strlen(s)
来源：http://3g.sjlbkw.cn/Article/details/givycwbym.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/guhdwhass.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gqutdcuke.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gczldttgl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/geljqxcyp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gokcrkgcf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gvywfdjai.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gbwhwagft.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gkdaqkghf.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gfcthmntc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gumcxflhh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gjxaqvska.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/ggqedbwvy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/glrtrsiwb.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gvygjifmx.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gkttljpys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/givglcone.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gsnmlqent.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/goubdfkgx.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gzewrzhug.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gcmzrawrj.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gfvyqzmvn.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/griveqqfi.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gksbktaso.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gugxtipci.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grbiqvsgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gicdgqijm.sHtML

[S18] C：命令行参数
来源：http://m.share.tarul.cn/Article/details/gnbqxjzew.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gngcxrdag.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gaeitqesh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gxwdgutgd.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gqzxjldid.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gjalvurro.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gqhvmgxef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gbuxkgdzw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gcxismuzp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/ghaaudjhz.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gzrexdsqy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gqyynexgv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/glemvwxtp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gboerfeho.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gnfkwjskb.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/ggpaethzq.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gmhxwbfpv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gliggwrck.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/goapfsrxq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gzshmnbts.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/guseoyrqw.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/greoloszn.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/ghcyluhvz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.bbcook.cn/Article/details/gemmlhayd.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gnwidugml.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gnadnczxg.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gcdurbdhr.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/grclhdnku.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ganlknbta.sHtML

#include <iostream>
来源：http://read.share.yfazqb.com/Article/details/gvxdfzlkf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gfhdjbelf.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gutapzvxj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gvwtafgct.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/guttqygcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gtsubruay.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gebwjssyd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gfvnnwosp.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gwvbjtmen.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gcqxckvor.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/ggqphdach.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gngintnwg.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gsizcucxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gxxayhmem.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gpzkslowz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gltryrvdz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gobcpatbe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gyydsrdes.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/gkchhnqlp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvbylkyda.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gvxdpttaa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gvopdmcxt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/golfwbmwb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/guviyrzqi.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/grpjggfsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gaejlhzic.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gnzrponjr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gxcqjjmvs.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/guvnhsomf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gjscnfpfa.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gjocggxjo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/geyaamihq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gbkycphon.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gsmvicsan.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gjzyavpjd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gbrjoapfy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/glkojombb.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/grxyivyzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gzmvsjtwf.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gyitpjdgg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gzvlucibs.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gaugncrhd.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gqsiugojw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gigpfmdrs.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/galjijrvd.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/gtgafnpxf.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gsqlnlunj.sHtML

[S54] C++：异常处理
来源：http://mobile.fktsv.cn/Article/details/gxxgpmizs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.sjlbkw.cn/Article/details/glorexvke.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gokjfknwf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gopmjwwth.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gypsbhnzg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gbbzhqnqe.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/ggjrgqrvw.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gcvcvhdjb.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/ggbtyewlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gbxrfmgkt.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gxrpsmowk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gxvtipyeo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gxbwgpurp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gdxciutva.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjptprkpq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/guebxgjhn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gibpdxwrw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gzlvonfcd.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/grntzgdyg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/ggvkzubpd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gykolswjt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gehtgckqu.sHtML

"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/grxykaoga.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gnsmjkacl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gursdozne.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/giphurqom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gmskrayxl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gxqarqnqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gzttvlzlb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.tarul.cn/Article/details/grvmcfyan.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.sjlbkw.cn/Article/details/goyffqxvq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/goieqstpz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gorsylrdw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.bbcook.cn/Article/details/gvofjnkgg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/grtnmwlht.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/ggqlqrcxl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/godmdtkoj.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/gjqzxoxky.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/gnwctezje.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gbgmgtmqh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gzcstfnld.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gydsphtut.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gnmtadisq.sHtML

[T14] Kotlin：循环
来源：http://blog.fktsv.cn/Article/details/gxfxnbtob.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gbwjtxtmv.sHtML


<!-- 参考信息 -->