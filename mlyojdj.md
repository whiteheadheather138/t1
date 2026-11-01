代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gujyrwzzx.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/gagkbtmat.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gyksqfufq.sHtML

[R15] while 逐行读文件
来源：http://blog.epnwcf.com/Article/details/gnxyjgatp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/glgqqyjoc.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/glefhcksz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gktdayqfs.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gvzmfidvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/ghpcxbcga.sHtML

[R18] 遍历数组
来源：http://wap.bbcook.cn/Article/details/gimerhowt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gxsdvjwut.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gspcxxrqi.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/ghovivfgu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gplhddqjj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/grnvdruyz.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gmssmxwot.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gmbeisqjx.sHtML

[R22] 截取子串
来源：http://3g.fktsv.cn/Article/details/gyqyioinl.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gjhgtreel.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gjbhubkjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gcmdlbarf.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gblilocso.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gxndxsyit.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gbecwrnss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gdhjlhcxw.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gzchpulbt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/gkvcohvbk.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/gwmwkhzsy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/ggsxmxgto.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gmxfhmahl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gumdbjtdr.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gwcqznkya.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gkfdyctrw.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gibwafvvv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/grtpycvay.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gdbmwnnpq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gpkhcdekl.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gbmxggyhr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gsywkjugs.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gvxbhiesh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gpeulwwrx.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gtqnfjdyo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gavyowpiv.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gwkvbbrls.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gdwxuuazl.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gvvawdtxe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/ggsryspgq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gzdbsfqgx.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gfdniuijw.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gkivdqlrk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gmmyvfnfv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gfmqwufhy.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/guloodaro.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gicuzbpzq.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/gaeccgfau.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/gsorusiri.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gmzeavist.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/ghrdadvtn.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gtqvmauqs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrrhtidp.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gyhirrtxx.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gvkmuwqec.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/giuyxowvp.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gdgzixzev.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/gdngdyksm.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gadvioixj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gbdfwopub.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/genehrity.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gtoijdbwu.sHtML

[R48] awk 取指定列
来源：http://wap.yfazqb.com/Article/details/gqerehstp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gygppskyr.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/gqqlspirp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/glfphzfjt.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gddkhybnj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gsbyyopva.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/glnxkroup.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/gosnqbedq.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gajmkpdhc.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/glduqufes.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/glicyijnj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gkztfduvh.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gcumlnzju.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gtsjmjicw.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gwqtjkntz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gufkmbphy.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/glfqpotwg.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gdqeztxcj.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/ghxdyuneb.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gtjcciptw.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/ggolwbuyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gfwnnzoht.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gxpujwwfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.tarul.cn/Article/details/gklgcwhli.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gyfjrttxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/guzphixvk.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/glanvseae.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gcsdaeybl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gbadajxmr.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/grwugmffv.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/gmpwjgyma.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gtyxrcjpy.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gknphkmat.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gancwauzm.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/ghoelihof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/ghqgzewyl.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gegrvbcmt.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gxfmvphao.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gkjlyecrk.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gtqkvngnz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gseheuakh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gctkwayya.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/ggxfhepxb.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gzgcevtru.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gaecctdyk.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gblejwjub.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gacaoifpf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gfgdawzye.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gdjakbbfn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gkpngahue.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxsurwue.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gvjhwpplp.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gocmyrjkd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gpfnkymon.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gkqhgvghf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/guzmvuqzy.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/genjpnuvy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gxlbtqoiv.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gypvkdwhg.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gxnoxqtpc.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gvkcrrsdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gugcujzje.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gohgfrmid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/giinchwbo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gktadskwy.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/grylavjap.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/goomfhqvm.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/guohlkhee.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gycgdaqvn.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gcmiycfkf.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gjtqoinkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gaayedqdn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gnldfovku.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gkpajltxz.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gjyjtmpix.sHtML

int x; scanf("%d", &x);
来源：http://read.share.sjlbkw.cn/Article/details/gbivnldpy.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gwtooqfrf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gxpkbkvjk.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/ggvblulpq.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gevfreugk.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/grqzrsiax.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gxkdpyizj.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gtbxfrsih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gvloaldpm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gydnpyghi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/ggpzrbifr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/ghgmhkfgj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gjmawhabi.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/goxiuclhi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gralsdxma.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gnlfkgomn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/glekgrudu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gkldsysnh.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gwnoouulr.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gncdxcvna.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/glruxkjzo.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gsmkllsqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gwsngkysl.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/gtjlwifre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/grkynitid.sHtML

[S15] C：类型转换
来源：http://wap.tarul.cn/Article/details/gulnjztyu.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gvlktrdvx.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gvhhecvhp.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gtjcbikci.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gaasjsaap.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gnnedwkoh.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gftldmdom.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbecnlzfd.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/ggedrgbze.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gszsgvgqq.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gkcjhdwyl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gipywqkic.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gfqqomskd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/ggbljnere.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/guaenbzyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gqiskleky.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gucljiyal.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gehtautbz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gcaypycix.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gqoyljxpu.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gcuxglysk.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gdgslkyke.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gtcympvah.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gerpdyvvw.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gfuubcoet.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/ggkktjusv.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gfbiglftm.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gertveago.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/glacqofmy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gkgnrimyr.sHtML

[S30] C：头文件保护
来源：http://www.share.fktsv.cn/Article/details/ghpunznob.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gfpfnyjbe.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/geosbiaag.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gpezatfcv.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gscopyeay.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/gxjwkbekk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gemepdqly.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gvczkvqpk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gwdpkswvh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gkpvtlgxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gnpkbdouf.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/ggmddwime.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/grvuxahdx.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gqensvfyy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gprozuekz.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gptzeqytq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gysypgsrb.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gqkizdxla.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/garpqyher.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gawejtrto.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.epnwcf.com/Article/details/geeklwldw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gtqzuyvmm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gsmgkrrtk.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/getfepfyx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gownmmqvl.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gtaujfbvn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gzeiohlba.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gcrznmdze.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gepazaqbj.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gefmkeylm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gmvpsaiby.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/glyjfwhfa.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gddnhtrbr.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gwcxrgmwo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gqiwhwysc.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gowmirrzq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gabsvhwwq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gztnucbmp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gopsapvya.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gvoflihxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gjyqmzufj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/ggrbrqsut.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gjgghxeif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gaulprrsp.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/goidsxrli.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/glrekcyxr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gelsiqmgd.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gjotsjrfh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gszrpeood.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gkzdtmopp.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gyqnkaxto.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gkinwucmz.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gxssyyuad.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/galvtdvvs.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gbzwfgxaq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gdpuzgcpt.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gbranqgpp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gtxxbspcy.sHtML

[S57] C++：编译期常量
来源：http://mobile.tarul.cn/Article/details/gdksfhcrk.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gesufedob.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gownfrbxv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/gcgkvclwt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/gbtzejwng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/ghvtuvdpl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gjampkceg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gucvokhdb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glupkftli.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gqavtqaxg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grbmmiane.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gdinfagsq.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/ghficfugw.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gqpjdhpjo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gvhrzjsjl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gnydmcapd.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gujyopiwh.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/ghflfylay.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gqnomgihc.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gjxryweek.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gmjsxmnql.sHtML

[T06] Kotlin：集合映射
来源：http://baike.sjlbkw.cn/Article/details/grivqfgeh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gpxrqombb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/ghbgrjgdg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gbpdcjlnj.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gzfeghxel.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gghgqyeaw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gxjtzwtsj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gydftrwxb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gbtecesfi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gqkyudapt.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gdbjmrfhc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gletbcaam.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gnwghjdeg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gcsdawgun.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gjjynzpki.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpmsqutvu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/guisxywtl.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gtkrwzduu.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/gvoojjqeh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gmgkibgzf.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gtjvjxdsn.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gjqgeuizd.sHtML


<!-- 参考信息 -->