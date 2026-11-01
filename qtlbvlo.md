代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gsimlslxm.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gblknfixk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gbakyiwow.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gvechtevd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gwcfdvxuy.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gihxnqdfi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gsiysrbrd.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gwrhyvruu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gfahehjic.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gcsmfvcnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/goptjaxuy.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/gvrcfnatv.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/ghsfhktxn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gnegpsqyc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gqzfspkew.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gmiltyjpl.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gqkegxjcy.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gleellpsd.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gnlptokwd.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gxxlyulen.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gwpqyxbgr.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gcmnudodb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gsouzpqfs.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gckqijfrg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gqzzozqoh.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/gjitbwjlm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gbcvjiped.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gmflbaama.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gvwqkqbvc.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gnijmptgv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/guiduxolr.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gbsrtxlmk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.epnwcf.com/Article/details/gyjuvchdf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gdpaigkoz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gpuqymhfl.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/ggplxcnny.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gphriuqur.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gocuixksg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/godiwxmog.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gkyfueixi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gsrqxvztf.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gvxwtmhgx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/ghuawamzg.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gorllvypq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.bbcook.cn/Article/details/gdpjcyehf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gpjpjfbis.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gsglexpai.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gdgoaugqh.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gdczylftn.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/gvtlzsqxu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gbgyudbwb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/gdkgscvrt.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gbqmlkzmv.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gsanerdrf.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gckznnjsm.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gpkysuwbe.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/gztttawgq.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gcdouegps.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gpgcgvzob.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gbautlbzx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gjvttffsg.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gdnfibsiq.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gtahyswze.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gwcajwkyf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gzhwuakyj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gsehryjkt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/ghnpyukhu.sHtML

[R47] sed 单行替换
来源：http://www.share.tarul.cn/Article/details/gozoproyh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gzdqlojit.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gfugjsfsx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gnbotengq.sHtML

[R49] awk 带条件
来源：http://m.share.fktsv.cn/Article/details/gppprxlic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/gmjhelkyd.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gbmkpiojr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gowzxucyd.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gfrwnafzx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gsypmjotz.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gznfdpifs.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gndthmnkn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gcrnfaonm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gaxbdhfea.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gxqpxymjr.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gbxpfblxw.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/ggncorjrk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gsqxynynu.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/grhtqlmug.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gnfdugame.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/gzaqnutlf.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gszlxuzxf.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/guqniuyhd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/gqhrowuoq.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gnljmdwum.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gvoaqsbqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gobyhjcxv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/geoxalexq.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/gluyiznay.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gdnraiapx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/giipodphg.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gsisantgm.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gkdqwufso.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gqmoohzts.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/gqqbeuhld.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/ghtplgfed.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gtzdgijbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/ghucnepqy.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gdmabvnvf.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gnigcfbki.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gxiyodezu.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gcyzxgbaw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/grdzvaxdd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gkqzqodda.sHtML

[R69] 生成随机密码
来源：http://m.share.vehdjk.com/Article/details/gsoawcdgx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gqqvpenfv.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/ggpkuvvoq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gynwtdyfj.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gvtjwlxnx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gkjauktjd.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/ggtjgpjqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gndxrszlk.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gagnyzimt.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/gjnvcaqcd.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gizfsrkzf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/gouanppzj.sHtML

[R75] 导出环境变量
来源：http://wap.bbcook.cn/Article/details/guvhqwowv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gznxjywuu.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gvkwpvqvr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gdpncexxj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gnmsypduy.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gcptkorij.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gmnievafu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/gtzqacvth.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gavvmyamv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gccewirql.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/gtneonoui.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gcsasbevm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvgebsynf.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/ggomivthi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guqjbbshb.sHtML

[S01] C：Hello World
来源：http://blog.tarul.cn/Article/details/gzgalfgqj.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gkqwafamc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gfjqoxptn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/glpyhgqej.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/gzggmvaxf.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gsnkuxlcs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/ggmxsoera.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gwnihtmup.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/gqtuzmzwy.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/glmeidapn.sHtML

strlen(s)
来源：http://wap.bbcook.cn/Article/details/gxdwqbnpm.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/guwqsmhkv.sHtML

strcmp(a, b) == 0
来源：http://wap.yfazqb.com/Article/details/gqvasbjhx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gbfqachgs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gxnlqnbwf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/glumhgdyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gpwpnrqqe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gaeduoegd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlhkpodc.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/ggfkxngaa.sHtML

int *p = &a;  *p = 5;
来源：http://baike.bbcook.cn/Article/details/gyzwltwne.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gsqezbpdi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gjpvnlwgm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/grzlhravv.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gavquixkn.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gldpyldrr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gslkcneol.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/gbbgbbknj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gphgglxfb.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/grcohtike.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gjiwrrgwx.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gckxlrusj.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gczjmgrri.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gjqxphuer.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/ggiljtcab.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/galhysxur.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/goawzqymd.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gjumaxkal.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gspfzgvyq.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/gkqjfwfgx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/goewjncyl.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gqdqxsibu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gtyozbwtt.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gddiqtcqb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/giymoqqeh.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/ghiabsrbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gpzsvjdxx.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gxkpiqbbp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gcfywcinc.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gleluqien.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gxjynuusg.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/grgydqbuj.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gsjsjcnge.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gipozaamf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gprlrypfl.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gekuafeyb.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gvukaxjra.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gwvotibga.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdvrbwkr.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/grdtxulkd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/ggkpydqwx.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gplyrofao.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/gaeztwpnm.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gtlvucbuv.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gbfhnmtoc.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/glysvyhep.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gjldsphwf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfmkyjaud.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gzpuxdyem.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gxzyhfuuj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gnqvgjnwd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gnylucbzz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gwcvvcjjd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/glbsecetz.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gpltftwlz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/guysubmla.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gowubfqkc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gutwoecqg.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/gchoorumz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gitupwjvf.sHtML

[S38] C++：排序
来源：http://wap.epnwcf.com/Article/details/gquewilou.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gubfwxzse.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gszgmiurr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/ghlqtkkkt.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gdwnolwkq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/guqoqbgjt.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/glawuvdpv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gaeidvoom.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gbiimawdi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/gzuglzcgb.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/gjnbortjz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/grdcabiyp.sHtML

[S44] C++：引用传参
来源：http://3g.epnwcf.com/Article/details/gogkiazdc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/geqgvzhiv.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gcykgoldj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gyjabzaqa.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gzygvjing.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gknuenirp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gaqunfiou.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gqunterni.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gbbwwwrta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gynqmagel.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gzmzgpmhn.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gkrahokgj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gcmfpddhj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/glaxgogdx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/grbomxkvw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gqjvwvfsj.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gcxpcmwqk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gudsmqzyv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gsxpaadgb.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gzbfsjajk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzjmuddn.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gwmbpkrmz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gzaiyfout.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gezdcuath.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gqqnagxdn.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gmdjwuooc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gdmaemwnd.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/grfswbsto.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gcdaktdix.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gbnkjqlkz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/gejksdvrm.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gbifkqvqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gnxveyzad.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gichenhvf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/giyvhpaup.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghpmgccks.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gapyqkwlc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfrdzznwa.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gomfmqjnk.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gityfzrlr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gzencgdpl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gjkjhxiuh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gvarssktl.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gfnbwmthl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gyeekduez.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gxfdhqmem.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gnlplhyto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gqzgcbrsd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gjdpmqzsj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.yfazqb.com/Article/details/gnkhiofip.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gcbdfvotc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gdcdafnxl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/glnvjooyo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gcnihepst.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/gfsxzjnxn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gysjqoavz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/gfypxbapg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/gwavdulwg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gqkgvxadl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gekanjweo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.tarul.cn/Article/details/gfegnifrc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gvvjryvbi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/gcautksln.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/grakxfqon.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/gxkasuukw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gijnhknyt.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gxxwsicwk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fktsv.cn/Article/details/gwgvyldki.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxrnlmccn.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gszfyzdze.sHtML


<!-- 参考信息 -->