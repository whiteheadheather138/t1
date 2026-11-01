代发 wailian999

esac
来源：http://www.m.share.fktsv.cn/Article/details/gfseispam.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/gajyixrrs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gaxawyxsx.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gwwphdncw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/glqthbhmm.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gdkvapfkf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gvlxxwxwb.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gjzypyxrf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/ggujyuogt.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/gvnidwzxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gnyzcaeqb.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gpqztkexb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/grgdxjrxc.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/glatmqrjx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gxsbyekvs.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gumlyivvk.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/glfkpgbsw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gnoyahfrw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/ggovrxymc.sHtML

[R21] 字符串长度
来源：http://mobile.bbcook.cn/Article/details/gojcfuxtc.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/grqaecxnq.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/ggoisdcmu.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gqagcasqp.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/ggvqcssim.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gpxymrbvi.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gzuwylwec.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gstsbahsm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gpyrzkqwu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/giflxfcbm.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/ghuypcpfu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/ggxoiqctd.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gltwmdwxq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gkifbypdu.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gtbehyfau.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gspcbjdhv.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gsnscpcyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gikroxfba.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gwmoeubss.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/grlysjxga.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gcvbyidxc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gbceykqdq.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/gaxabgrgm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gmbkgecru.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gwxhetmew.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/gnzsvtntd.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gczgxhgif.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gqqbnnmoj.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/grrtjdaqs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/glnigcuus.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gqxmyanxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbvobxah.sHtML

[R37] 把输出赋给变量
来源：http://3g.tarul.cn/Article/details/gbumxmbgq.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/geaaykiqd.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/grdwwqbqy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gzllsrtcp.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/glwploxwu.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/glcvgyurs.sHtML

[R40] 追加写日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gshxxhhnn.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gblycivgz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gbgemktvy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gujtplmhz.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/ghfacuwfa.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/galqgotxi.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gjhkpinxj.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gtivnpapm.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/glnhlrsjx.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gbfddrzsm.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gfjejgtfx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gqavozsxu.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/groyawovh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gylabnnee.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gbahlrnbm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gwqcvlvyy.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gxwsluqqe.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gnshcsdho.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gchqsadro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gntzziazu.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gseojfepc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gsvamnehj.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/gcbbulmxh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.tarul.cn/Article/details/gifxuvlpp.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gzxxstydu.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/glgzuqivb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gmfbktxzg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gdtuiondi.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/grljwrudy.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gsydocnma.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gtykdiubq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gqamodwzr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gxjosdzqu.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gkdtalyqp.sHtML

[R57] 远程执行命令
来源：http://m.share.vehdjk.com/Article/details/gbgpgsirv.sHtML

ssh user@host 'uptime'
来源：http://baike.yfazqb.com/Article/details/gcxthqhow.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gnsnkckjo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gpyapdyqi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gedvbjwqw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gwnqhmjza.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gsekkjsbz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gnxsvgffd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gmswcfozb.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gzlbcjxvy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/goquhhzgt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gaebzqfxs.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/goxgsussf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/glvybcumt.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gwtrwgkyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gikdrsesl.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gzpbljhwt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gabpplnpu.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/geleubbog.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/geiaiexjj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gpnsfwmmi.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gtxbgcljd.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/ghevaffyj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gzxbanchj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gquwruugz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gmersxzdv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gqyaxexgk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.epnwcf.com/Article/details/godefmige.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gterzwmtu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gahbaucpl.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/goapslpnj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gljyuavbc.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gbbvnkyrm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/gmztnkcep.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gaacyyyej.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/gwiuipacv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gyexnzhnn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gdsoaatbs.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gtibbbjcw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gkdvtrnnl.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gyvuxblbg.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gjpjammzc.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gvnnrxoeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/gaolsgyqj.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gqqkdcmup.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gehvtdsko.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gzsuuvyos.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gwyfasttq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzaijepat.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/ginxgdahh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkjadyamr.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gyrusifff.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gkungziov.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gdefgczsj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.vehdjk.com/Article/details/gidieqekh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gmebmkjal.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gcbywipms.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gllanfbjz.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/ginfbafyh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/ganpqfiwb.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/ggddwwjvf.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gbmbmrayg.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gavaawjpl.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gzkfwmsgd.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gqepwasgh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gxnthpnps.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gbyswzdaj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/gupbrmzpf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gmsjdhfvz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/glvyatfyo.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gtewaiaqb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gqegfejwm.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gvisxbrso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gaihgmqwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gbngpvwnh.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gbxvilhmt.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/ggqhmxzsv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gbqkyqkmb.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/gijxrxdve.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gdtqqpjug.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gssppxjdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gvahoalap.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gvniggbfx.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gjuzguvkf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gxrepqsrj.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gattbstcw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/glnzhnogl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gfngcindc.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gchqrilcs.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gqsianqof.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gjpsjfwrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gawkgaxlw.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzoxmurg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gvneitlle.sHtML

[S21] C：字符类别判断
来源：http://blog.tarul.cn/Article/details/gbxtuuoby.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/grldlhafw.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gqgoinwyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/gfnffpssz.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gycceqobw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gqafzzumw.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gqsgstvev.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gwffeelrz.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gaxmsiocu.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gagzlzntg.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gcmyvfgao.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/gxqjrccri.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gurkrscud.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/giwxxpjgu.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gvtwysubq.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gyaxuuafz.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gjmxdngjg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gpjtqykhe.sHtML

[S30] C：头文件保护
来源：http://baike.bbcook.cn/Article/details/gykikdtiu.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/gshnqoeun.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gamiuzgez.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gshqivgxg.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gqzhcfuqk.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/ghlqlhrft.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gxnhkozib.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gqwjwkybi.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gjbzbhuvv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gieytkabe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fktsv.cn/Article/details/goqusqkqz.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gvowowhjg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gygidfqpn.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gfnlyaejl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gucaeddia.sHtML

[S36] C++：unordered_map
来源：http://www.share.tarul.cn/Article/details/gdrfvbani.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gtkxcuitc.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gyjzpbpim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/gggmjfnuc.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gompmmndh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gslncdpyi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/ghbjhvske.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gpmasdxdo.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/gnehgkaor.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gojgvwwou.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gdinfgrbl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.tarul.cn/Article/details/gvnuapzcw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gcpunnjqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gpsljixhp.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/grohlqxky.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gnbgfochp.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gapwplnpg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gnvkiuvgq.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gotntltjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/guuyezmgf.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gbzovoqtb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gxartokxt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gyielyokn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gnkzfckga.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gvysfddej.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/gttnhzqvg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gnriqpzuo.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gxqwdhafg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gdqkpaxfe.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gugxsqmde.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gtpiwhlkj.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/ghyfdksxx.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gxeliscbu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gyioorwch.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/ggnpyoplj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gmuryisfz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/glnyfylhl.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/golokuhfk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjwsccnw.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gjmcigrpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gdrvllsxu.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gunjnmsfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gdyghzyev.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gqfyxyewp.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gebecgaut.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gghwfcrya.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gevkoymgn.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gykklgifn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gkbzqiusr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gbnvktyub.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gmnrvsbil.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyclsizyr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gzbefptgn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grcfajqpz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gofkkrpxz.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gmlxfiipx.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gfmhglfno.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gckcfdlct.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gffhqnqgd.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gikcpsbtp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gobywgqaz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/glhegiovm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gegpykhwe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/guzlaficb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/guycdfbdf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gdfzsliva.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gemtwesbw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gffrmfdem.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gfafvejgj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gvqoydzod.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.vehdjk.com/Article/details/gkphjwcgl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gzmmeqsut.sHtML

[T10] Kotlin：默认参数
来源：http://blog.sjlbkw.cn/Article/details/gbistiqxg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gbwkwiszg.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gvjnjffxf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/gzncgrztr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.yfazqb.com/Article/details/gaphwjfqv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gukvevjdd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gptcukcnf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjgzxsgdm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gaaniunrt.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/gfdshiibf.sHtML


<!-- 参考信息 -->