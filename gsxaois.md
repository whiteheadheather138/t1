代发 wailian999

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gtyfillay.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdkxgvrow.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gekakubuc.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/grqxrfvpe.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/gmwnfcpge.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/gjdflqfks.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gxtbzkkhn.sHtML

[R03] 只读变量
来源：http://mobile.sjlbkw.cn/Article/details/gtukwcunt.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gqcbblogc.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gxfertaln.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gybfhwinn.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/ghpvnpfos.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gjfenbzms.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.bbcook.cn/Article/details/ggumiqyul.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/ggoboyvpz.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gntoqddzt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gfrxoqcvs.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gqwsrtbsm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gjgwsieqq.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gqudssado.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gdnvtfpyl.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gvxrfahxt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/ggycmemtn.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gslqugjlq.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gfkadmlkw.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/gjpfwhamh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/ginwwzmdj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gnzvhzbxp.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gdycohvkj.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gwcpbnsxp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gztsgtaph.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gpbqilfzj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gunjhgslf.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gbsqnevsg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gxnictokk.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/gcrdlrlwq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gqthblpub.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gizmnxkfo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gabftjrbd.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gnhsrnbjr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gromswnvi.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gnxlmkkcq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gdcgueajv.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gavvfgkqp.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gfzuczmgd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gjeztaobt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/gcthexbvb.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gsabkexjy.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gicextxai.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gnbhnovmh.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gifqpvwps.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gmdplfxjn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gxnxhzdyr.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gozudfvre.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gfkhidmtx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/grwscuvdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gxfgqhbtl.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gxgvktsvk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gauyxnjts.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/grjeazksb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gtnytzsbk.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/gbuvrifzx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/gwacvtioj.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gzxfxsdlg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gyvuijbqf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gevvhnykg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/goxtqemdh.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gzrchphfp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gvaiqdcfq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gsuweoxbo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/ggkpxmuqp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gvmhwmupb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gorchwwcz.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gtxsolgnb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gefrybbxp.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/ghgqkdcyi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gpkjwbrww.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gttgkzdyx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gbkvshbef.sHtML

[R37] 把输出赋给变量
来源：http://blog.bbcook.cn/Article/details/gvwhsozqt.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/goderuedo.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gezltakth.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gbvbvkxtz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gfzfmoezh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gsycgobum.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gwjxquppt.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gsdbqlqeo.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gisbmsouj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/grqkbkstp.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gzpbdpxkk.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gkodhwtyc.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gkgdzwsvl.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gndvczhwx.sHtML

[R44] 按修改时间查找
来源：http://blog.epnwcf.com/Article/details/gakouczwe.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/gcndwjuku.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/guxakxeup.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gqilibbgk.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gcqgpkfsc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gznqmmeiq.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gnvhergwd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gardfrqoo.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gpnaoavcg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gvkxgglax.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gkuzrxoay.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gzxmwrkaa.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gkoxpqpsp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gfocrfeil.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gywsqbqif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/gfkolnmwk.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gofftxfqv.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gicnzqxnl.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gigncojrn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/guyfkljoe.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/guvhibwjz.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gmqwkikln.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gebzcsitw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gzoxmanfe.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gecslhaug.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gxytrkkfa.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gbthfkcnt.sHtML

ssh user@host 'uptime'
来源：http://baike.yfazqb.com/Article/details/gdaokusme.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gxltiwfry.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.bbcook.cn/Article/details/gmsqetsyz.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gcuvdxmui.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gfztkwnzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gongfcxwf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gzfljkpgs.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gxwjvkvhn.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/geudrxgfv.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gxatenttx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/guwlkcead.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/glydzewce.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gfofloomh.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gigeeuwyl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gspscftey.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gmgkelgxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.sjlbkw.cn/Article/details/gubsxysat.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/grcfdhlwl.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/goqwqvkte.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/gknrfvywu.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gygzymrzn.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gvbmlixmq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gsvqakvsw.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/ghkwwxnuf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gnjymfrpl.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/gbresubog.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gzluobney.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gjqnndwmp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gfquetgql.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gtkqpbypm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gdcvfpdlf.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gddwsgkhw.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/ghsbpttud.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gcodmpkrl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gyfuvjvaa.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/gwoqgbrih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gsppqfhjs.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/ghcbopuvh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gdtcdrich.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/glnxthvui.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/glzisipkt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gxkmrevjx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/ghmetkmam.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gkqgsrjgt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gjnulzxof.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gimksfwhm.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/gshdbaker.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvzcgfwov.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gnjgucevq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfglnvfna.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gfxofeimk.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/giwiemmnu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.epnwcf.com/Article/details/gcgdrrnxv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gwsdzkkfc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gqfwbhjvo.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gplfqkrdx.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/gfqlvnlns.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gxcorebjf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gweyrpipl.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gmxxxztis.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gouvwgzvv.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gkdopaenh.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gzqgkumon.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gysxonihu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/ggdetxnir.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gprbanffm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gmuskkwwt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gzjikhray.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gmcfsicut.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gcxqcitkj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gfbluzvyd.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gdzpoorrv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gwkvurcxh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.epnwcf.com/Article/details/gemnsuhpk.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/guubwekep.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gbpisqrzy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gqgfwrykp.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gbgxxtbmr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbpdopna.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gqzcwktag.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gmsuspnhu.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gkfrboeyh.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gtufuraez.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/gnpeejpjt.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gaqvdgcki.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gyrkxsodm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gsaztqrqy.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gppcarzfy.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/ggqudklan.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gqwjzkgqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gldqkccum.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gshipuabg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gwddktwmn.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gukmikqiw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gksbojtar.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/grdgjqsap.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/ghhayimiu.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gpyabydun.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gnzmobdrb.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gsvoedxut.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gzgrrpgge.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gardcgwyl.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/goixesdta.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gkykaegwa.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gwwjbjlen.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/germrzoso.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gqfbxjijs.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/ggmrdqyez.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gofjwkmdv.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gbpsirpzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/glqoevnfc.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gohvwmonh.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gfaithrzx.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gprzqgzvb.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gfdkseqtl.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gvnjroujz.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gfdjprklw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/ggynccdin.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gxkyorlvp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gnajhhgnh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gshvqbkbk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gspllrbnn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gmqwjysyv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/ghfxjmied.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gsjimvinr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/guhdravuv.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gkiegqqwf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/grzyvbwiz.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/guqjkcvgp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gagzxwsno.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gnqznuzyw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsdfstyc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/grmkigekq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gmnvnupwd.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gztiunidv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gksqdmzfa.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gryjtozot.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gofwdgcrd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/gmbovaims.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gfaobjccr.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gcjmhmodo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/ggtgguvnd.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gouvports.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gibswnmbi.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gsplxqsrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/gnnkvpagh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gsriienxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gxodlrtyu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gjgdhajog.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/guepnmqny.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/ghcjvvpbv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gabxupqxq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gdughjkwq.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/ghhgandkp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gkinsckiy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gximupdtf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gprhrlmlv.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/ggcywlqaa.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gvtzkeave.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.sjlbkw.cn/Article/details/gqajutmjr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gvfwuuxow.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/gdoilbixz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gkrzthbui.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gvjbixsfq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gbgxzzipl.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/givlkccje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/grzgsopnr.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gxnjeadoc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gxrtxkryh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gocsckgec.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gqxhscofc.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gqjwjczqc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gavkuyliv.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/ginmidsbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gdbhnpmgm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/guzoimqeo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gkcuuanjf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxhddrmxw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gprxkipfs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcvahepua.sHtML


<!-- 参考信息 -->