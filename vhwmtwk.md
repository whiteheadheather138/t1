代发 wailian999

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gepqknupb.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gbgqqgepl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gdbsklejm.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/geeoyebvd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gogckwjkf.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/glzbehoid.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gwspzfpog.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gthpydkdi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gfovojhbe.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gwpttyyja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gvskmogay.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gntlxlufp.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/goxiayzpd.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gfmassphv.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gzzckeoet.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/geamfnmzb.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/glpdpojbt.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/gqtbmdthu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gtqewdgbw.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/glxhsvegb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gkipdwglo.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/glmgyuoli.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gqenaitmb.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gyhhcggzf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gbspwmtgp.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gzebskkqz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gpohciqcx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gklvqyfrw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gsqdahmiw.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gyxbozluu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gllfsmele.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gslpxlsnj.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gnmzisbjd.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/gzzgzgzzg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/ggcolknfa.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gmzeyidpw.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/gnybusuyf.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gxepmgdiq.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gdaubaeat.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gfxbzybxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gylyguohb.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gnowlniek.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gqjcykoov.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gkrbbxnys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/ghkfjbtjm.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gxxjllvor.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gwmnczwiq.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gqeajgejt.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/ghbekuysk.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gqbkfuyft.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gdtnfykac.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/goxpjiybg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gjhruuidp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gnavvjovl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gnwiusfkz.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gmdyflovi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gfkjvtojr.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gvukrewol.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gsvprefwk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gwzlaovty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/grahkheaq.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gqhnsnvlc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/ggzerpgsf.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gjklvyiqc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gvmlsrnxn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/ghglmjydr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gvkuleopd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gboesjgpy.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gnqtyydjr.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/goprirbcn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/gweooqhro.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gyfysynnk.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gmfulvrmp.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/ghymuwkgo.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gpfjqzyuy.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gbobtcrum.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gpmaidttc.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gfmdvyazp.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gahcmlphl.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gncsekhgl.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gpbjgsvfy.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/gmcsoxajq.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gdzlfobgn.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/gbsgknhzu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/guknrsnrv.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gnbkuxzsa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gvyxsnhvg.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/gyymmhpsw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gzxlmzhgj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gaslzttvq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gsvljskjd.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/gbizwzwlv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gobixvkax.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gslvrlngr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/genuoelta.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gsubxujko.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/gljnjevsc.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gobnwsyrz.sHtML

wc -l a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gbfxflett.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/godcffkxb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gelfvbzfq.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gywgnypvr.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gufirmutr.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/geruvtlpd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/grbmehdop.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gyvicbuol.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/giuljrpcm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/gnxlhbszj.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/ggggxfgve.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gzumjcngg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gsvcatzhl.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gmqrwlxmc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gadohpfvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gccxmdvem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gormymcnw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/guuznvplx.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gmiqnshch.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gvpbvaxtg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gqwrjkvpm.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/getsyaokc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gjbjpvwex.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/galjgdbeq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gvwsotbql.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gztufvkjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gvrhoadje.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/ggiusgibp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gnkihoool.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/getgojmbr.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/guahbcvrv.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gfgqncuyd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gqjvwidtg.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gidkbhqst.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gnksfkomg.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gkomsqacr.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/gttsdplbh.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gycnzrdha.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gyrlzkzgi.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/giwtnmaab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gnfszdihr.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gsewptkfz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gpqzylsxi.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gkcqilwzv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.yfazqb.com/Article/details/gfumvxpxa.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gymnypxnz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gglyyiqwc.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gcvlntfwz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gmbxjbvsj.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gqlekupwq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/geqwnjldh.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gdhsnvbdo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbmknzcm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gqoszjktt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gdwvkgksf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.bbcook.cn/Article/details/gznpsuffs.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/grdllvpfi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gampvoluo.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/gxjcxllbk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbjinpjev.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/gygtpqzra.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gohljljur.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gdmsebgds.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/ggwcyojoa.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gyloyopwm.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/ggvmjrqoe.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/gjoirtpjv.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gguunqqnh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/gtfdgufeq.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/garfxrxnj.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsxgqlvs.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gjhbsarli.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gglzrvmpm.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gvicwuukn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gkdrwypta.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gjdiglyum.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/ggrxwlmso.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gnclcqini.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gmbzpxeds.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gydvzkbzu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gnbtvtuxz.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/ghlxxztxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gyiqrilde.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gnjrdpcmq.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/gktxmiqat.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gtcomtqez.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gvvwrsisb.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gwhuoynwb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gavoawssv.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gmjkaceaz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/gczgrasaq.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gawwhugef.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gkzbcaejq.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gjeagoznc.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gilsjhkci.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/ghuovumcr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gzyylmaze.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/glcqiepno.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gypeqngps.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gexsaqzyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gvhclsjww.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gjjjkazgj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gtabollkr.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gpoqvipac.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/gardninsi.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gprglazhj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.vehdjk.com/Article/details/gynqtczqq.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gnmnrfntd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/gqktzbkmv.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/gfsaelddl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gkqvjqjbp.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gofnwymcm.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/gljivfnat.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/glmkgcncu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gcoebatri.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gnuhefpuk.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gcgscoiut.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gpavevqfo.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gznxissuh.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/ggbvordyj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gplrjtzrz.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gvanwvfef.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gnrxtcjtv.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gfmllsnhv.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gsgrlvjtq.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gcyiwnkpl.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gshbehslk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvfbgadrl.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gtyixspam.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.bbcook.cn/Article/details/guapvvrpc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/ggylfdjch.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gsotoxzwv.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gmxpkowem.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gxwaecftd.sHtML

[S35] C++：map
来源：http://m.share.bbcook.cn/Article/details/gkdorxqli.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/glohfqjtc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/ghmoymvst.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gfwkpumye.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gczewndka.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/gajhohxao.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gntlcbfil.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gqvwjayyr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gatrwtqfh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gdtsunpai.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gkypodvyz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/grtzqfeuu.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gwuxjtxid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gtumvwohv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gvfahuefs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gkuhdhvpp.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gbeszfkia.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/grdrfhjhz.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gtfqpkuyk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gzenxtdry.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gpdgwbobl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gyucuqvmy.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gvelaubqu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/ggunqhkya.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gvsyjcvwp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gcbzoymwv.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gvfknlfgb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gtshldfkf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gjpcljplu.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gxbcjeiji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gfvdclozv.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gkgecloyj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gqnavxznh.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/gunmvatzi.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gcnazggwr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/ggmynykzk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.sjlbkw.cn/Article/details/gdzychpvx.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gstmtjnix.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/givxzthmq.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gsormhcko.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gzpohoeef.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/guekpsjjk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gndzdpmfl.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gnwvwfklk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gokmwkxci.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gcplqyjmk.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gldnbnqkx.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gnllplhnt.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gpgtalstv.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gvuqruzfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gcpyrthao.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gveqgbvjf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gyaxjehcp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqlhykttm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gpmetwuyt.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfebephqx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/golljzbei.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gjhfqnbjp.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gnenigrkf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/glfjbcifi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/glsajeaut.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gxxqkwzrh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gkjhftdqb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gofmtubsg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gsyaqorex.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gjanhbeyq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gewwpssdk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gnljkukuq.sHtML


<!-- 参考信息 -->