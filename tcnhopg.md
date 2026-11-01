代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/ghzqwfnwi.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/grhbxidld.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gjvzzbzzr.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/ggingnfxb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gxozpitia.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gtmofqmpm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/glkwiikiv.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/goadabhgu.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/gdsndzijc.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gawxwjlol.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/girddqhyx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gqynonykp.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/gwepwggsv.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gszclrezs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gxyvplwob.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gztqonygf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/glfrycnvk.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/grbnvjshr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gsweobfyx.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gvydgogau.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gmxwpojpp.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gsilvlcpq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gawxcsujb.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gxkzklzrj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gqdkgxjkk.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gwczkvgim.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gcbylphrn.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/ghnwwevip.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/grksrqzdb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gxdaqbahb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gefrrmthh.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gqqlyfpka.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/ghpmqddlw.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gghhfmqxi.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gnbucngdf.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gsedbdvlm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/guughdijo.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gorawlxna.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gztzobsuu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gwehkzgtz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/gfctgrbyj.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gxjjufrak.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gvsebjhcg.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gyjfhahbh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gdnkpzumq.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gquofsqlx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gtonymumt.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gmhdotjpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gdehhiblx.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gqikpmbmp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gupyxwvqi.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gaggadpwt.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/gpjypesym.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/glsraqzlt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/getroikkz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gqmkfrafx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gkidbescx.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gssvgafqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/guncjaujj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gxtnyudza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gjhhlvvyg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gtzxngomh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gfddiacsg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gvbrheaar.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/grvmhguec.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gxyhfxesb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gyqgpjqlx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gzxkaqotu.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gpkmligxp.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gmoagjjvz.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gcxriymmi.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gvrgvkzmu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gvykkurzz.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gujeaaiyt.sHtML

wc -l < a.txt
来源：http://3g.sjlbkw.cn/Article/details/gamfnmhdi.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/gqwgfdlti.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/glnpvlwgz.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gsqgxolok.sHtML

find . -mtime -7 -type f
来源：http://mobile.epnwcf.com/Article/details/gzrcapnii.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gfyodhxjc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gnfjjeuwo.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gcaysjbvw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gcrtnwgav.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gyjwnftur.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.vehdjk.com/Article/details/glcounavt.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/ggnyobhbr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gcwqrmlmg.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/ggagfcdbm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gxoupxefs.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gjgpfttjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/ghzitoqpr.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gjezjojei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gdwvrmnlq.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/grzxlpriu.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gchhrhcvh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gcdocefih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/gxptttssm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gmivgfquw.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gfdynsmjo.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gflxteety.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.vehdjk.com/Article/details/gxmbsgnqs.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/gvwvaxadh.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gvrrsedaw.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gbczgzark.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/giaznbhep.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gtbsyhqrx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/giawtgpey.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/glkekjuct.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gidlzzcrz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/glakmvwhb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gbjcutyuv.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gpivehnzl.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gkcafukae.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghczueqig.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/gwqyddvbr.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gozjriwjl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gapusqgdf.sHtML

[R64] 结束进程
来源：http://www.blog.fktsv.cn/Article/details/gmvrmpmwk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/ggeharvfj.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gltmzpyji.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gqcqwzegs.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gczehiknu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gefyhniqx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gzxwuvmoe.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/ghlnypttr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gikeuyflq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gkdyrxltr.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gfntkvapd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gdqpvvbde.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gemwjpaxb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gzztuyhgg.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gsqbblgti.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gcbrbmpvw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/grrwfdwdt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gzljjkhrr.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/giwlnexsc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/gxmcmnxvu.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gkptglipb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gaikeqeyn.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gjksastwk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gosvpcici.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/ggrtykrjj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gakoocyyv.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gttksiiul.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gqkpittnt.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gwyziukcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gvhvybvzp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/geubhcpgr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/gmkddjuxz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gxjsfqjgw.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gmtnlausc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjgjvcdjr.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gomwvbkci.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gisrnaynd.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gysjxumfi.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gqxpmaqrc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gnhtpnray.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/gtbsjepqn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gmxktytuj.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gqlglqikg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/goujcylcw.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gpewkryqo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gvnwskvkx.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gxhfnmkqk.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxfssbqmr.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/ghiueookg.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/goqddjqmj.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gcpbqruxm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gfsvxordi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gzrkjikpg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gwiduevpd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/githtkobc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/geoiikhuh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gmaorcinr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gtrdzczjf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gltzjwrvq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/ggfsymgmu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gbxdvpztw.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gouposvyc.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gjafhiygm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/ghdxbxnkt.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/gmfrdgywg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/ghlurksyi.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gkqfvqihk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gprhlhhoi.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gesgivnln.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gpelnhxtx.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/ggcpamdqp.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gqmtcawgx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gjkcezwqt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gffnnrcna.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/gvbglerkq.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/grjnmgkra.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gzunbriql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/goyhqmmth.sHtML

[S20] C：二分查找
来源：http://m.share.epnwcf.com/Article/details/guzuyjugc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gklxoujda.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/gnqwqyfua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.bbcook.cn/Article/details/gbyziangf.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gyhxcitus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/gcwevefxq.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gvqygdtbi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gvtwbunvf.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gbglcyngp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/glqjwemuu.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gqmjlrqwi.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gctclnlqi.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gtmkhqmvo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gboiyqqky.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/gfctjgzbo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gwzqpkgxg.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gjyzcmmxf.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gadgmihxp.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/gdurtynip.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gmncasajj.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gqdreyixa.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gcrsatrsc.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gdwkeqifi.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gtommleca.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gvavdhhxs.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gmwaltxsa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gkexrerrk.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gpllhifrk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gkhrnzhhj.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gcidqwkim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gydiifrqb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gkhotcyts.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gsrfgxvov.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gsrnjfajy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gwhtmxgmz.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gblifwulu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gauvyugpn.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gcergkqde.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gkpxwcgeo.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gnnscffgq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gscbztaqn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gaivduyno.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gazpjxufo.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/gldinfrqf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/ggkkiuohu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gkcmmjspx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gwiiocsih.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gztohagsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gpltbrmmv.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gsbixrvzr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gctrwjrde.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gflhbusyu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gdglldoos.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gxlzuschi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gneoqnwjs.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gkhnwzfjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gdvyijgxf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gyqftypvh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gwlsxmljp.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gdsonxrjq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gwrweydao.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/guhwwgfdp.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gawxxhnmv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gmcqfaodn.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/govjeqido.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gfvqadekl.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/ghxjcbxcy.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gbowiaecw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gestslvdg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gvvnxdyvs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/gutqckoeo.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gwmnlmotw.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/gzcndzrix.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gvvmirgst.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gagkcwnww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gcmtnduxn.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/glgqfzyxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gybpyexcv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gjwzajpvf.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/geszefenc.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/glrwjezhe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gnytewosl.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/gwbyujxxf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gucyjannt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gpovjmzng.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gozjojyom.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwiudhjvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/ghovxlpli.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giumwtiax.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/giecsqbyc.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gklefwfxv.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/gopqihbxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gwpvopgyw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gljjmxyzd.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gorrtshfk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gvjvbvpac.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/ghhtfwpqv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gpstqixog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gyngrubam.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/gvtfohnki.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/gfblpyeuv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gfjrvxvfh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gkphkbovq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gkktixgia.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gmgamsvdo.sHtML


<!-- 参考信息 -->