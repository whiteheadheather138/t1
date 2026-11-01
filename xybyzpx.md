代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gaecsmdlz.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/gzmxilzvb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gvldurern.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkuokkpzs.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gngzibjov.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gifabavtg.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/geuadaeum.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/gqvmafvze.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gfewfbtet.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gxvvgxzuo.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/ggieybgys.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gmavvxxmh.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gkimqwrjf.sHtML

[R04] 位置参数
来源：http://read.share.sjlbkw.cn/Article/details/gztrcjaqg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/gotxgbjpm.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gjncyjluq.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gusnsetmd.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gngfehaac.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gyujxysnh.sHtML

[R07] if 判断文件
来源：http://3g.bbcook.cn/Article/details/gzkdfloqw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/gldphmnin.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/gzbvzfxsu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gthcbzwid.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gbbmaorch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.tarul.cn/Article/details/gydhnhaay.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gxynjgjqk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/ghctfukyc.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/ggwhajzsv.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gykwlmonr.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gseagemsk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gygooszpn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/ggevecbca.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/ghrgztsso.sHtML

[R12] for 遍历文件
来源：http://read.share.epnwcf.com/Article/details/gcxyegrrj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gcsnjxcmb.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gyyhvaybn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gkmallpva.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/geqrfofhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gybrmpfte.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gkmuxinbf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/guepacexk.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gyimakccg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gdatclqtv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/ggkpzxhks.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/ghxozeuqz.sHtML

[R18] 遍历数组
来源：http://3g.vehdjk.com/Article/details/gyywjfoeh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gsrievszo.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gkvvahebk.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/gtcggxqbb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gozghlplp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/glctlohwi.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gnwqbofpb.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/ggdlmehoa.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gecsfkmwd.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/grctxgrab.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gosntihvp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gsajeafdf.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gfcbnpkyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gjkvmcwni.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/glclrqdaq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gfqwxxtyl.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/glzvbzasb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.bbcook.cn/Article/details/gtyffggir.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gawaftnwk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/glbucmjzm.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gbtyopexe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gismivwjt.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gsugrkzyd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gijdxbbzd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gtqpoydtg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gpnkmbzbd.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gxoiebnyc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gkdrowqgg.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/glidhfobn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gxpshpllx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gvllkuaxc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gzjgouhzq.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/grphchrrj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gfmgvadxj.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/grxjavxad.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/gexybygqx.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/giyqjdpyc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/gqynnrwhe.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gqxfyteep.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/ganspuaev.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gmvlifnjh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gvnsklrak.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gfccfzrmg.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gcbduonsn.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/gpietmgus.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/govzbiegc.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gscloqlch.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/govxohnwi.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gznrcaiuv.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/gyxifitwx.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gtqmzasko.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/gekarbuwy.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/ghjnwgyno.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gecplyygi.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gdwrnfkqv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.yfazqb.com/Article/details/gbwwodieb.sHtML

[R46] 递归替换文件内容
来源：http://wap.epnwcf.com/Article/details/grgybuknq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gzqhzlosk.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gybonjorx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqdulwnmg.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gtyxdtsil.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gpnqwiymj.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gupdohwxo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gogivuefk.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/guazumapp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gvkobokjt.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/grjivzfpd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gjbhadlqg.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/ghtyaqbwo.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gcwpmzbca.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/gdtyynwmb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/glxyrrejb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gawzjdjpv.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/ggjlbavwv.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gfetfxnab.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/gzzkiqfxq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/gstjmjoju.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gqodyxmfu.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gojufwdvn.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gxoasrxgn.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/gbatotyfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gevvnewls.sHtML

[R59] 发 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gwtwfigqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gozmctqhk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gwrvtwedq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gbcdaurjm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/gegxtulci.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/ggncyecct.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gbnteprdf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/ghwcekuba.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/gbosfvtbp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gvzqlwghz.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/grubkwyux.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gohabdicw.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gxbxdwuuu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gxlafixrf.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gflqtidma.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gldknysrd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gfqfowifp.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gsskupurn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gjcflbsta.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.epnwcf.com/Article/details/gtwuiltgv.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/glhyznasd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gjcozmwxe.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gaqxgayof.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/glwwgbndw.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gkxhodvce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gcqhlkulb.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/gwdyywqbs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gyuiazend.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gicymiimm.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gzbmxnvem.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/grgvbccyi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gmfvzxiej.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/glbnymfov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gkjmbkwbn.sHtML

[R76] 使用临时文件
来源：http://baike.tarul.cn/Article/details/gsbtbyeoo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gwzbxmpkz.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gqusjsmdo.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/gdfryzdwi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfxnrmmr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/gclbcqbdk.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gkwugmyjv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gxwmseipc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gaooxlzbk.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gflfaolrl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glxqzacls.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gwhozcvys.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtromwkno.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gxulxmepz.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gokbnpvci.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/goqjzakpa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gikslnlsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gomkulsfe.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gyxklnyor.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gvveealcd.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gzelofint.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/ggfixlext.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gsgedvtul.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/glrsfxsyt.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gtuszmyeh.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gbsexhxux.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gbalrjlbc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gkkfxslsu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gkbroznrt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gbizbuhzh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gnzpxeexg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.yfazqb.com/Article/details/glprgfrna.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gtuqofgtw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gjgibbowq.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gbemnxlaz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/guojwlwby.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gqtsnwwit.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gtmqcyzbq.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gsjdifhta.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gquyjptmp.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gxdznqjbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gskmchibo.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gzjyqwxwu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/ggiwxcgwa.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gvfzntjsg.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gudlnyvgx.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gtgulyyue.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gwffsybnl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gwxdixpbl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/guchlfjaf.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/gaeerngiy.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gskgssglk.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gzjjbkbxf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gdgiidxcz.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gkyhtiibj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/grbnmudtp.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gpkrnrdql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gsppnefua.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gcpaqlghz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gfanynskw.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gozrcsats.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gxlqtjpfj.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gvofcfbze.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gqgupohjf.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gvdhqgcwc.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gwtyxwysy.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gozbgdkxy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/grdpihvvw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gmwcoraxf.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/glpgyylfw.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gucyuqtov.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gfvaxgjou.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gcehxlnts.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gomkrsmym.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gootrcvaq.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/gslmdpvrl.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gcxpisbfp.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gmkdgetlf.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gzwxycgdl.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gwjscpune.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/gartavcfy.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/ganbbiaka.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/gypuartvo.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gnjqwmbnh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gmoqprchy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.tarul.cn/Article/details/ggjfwafdy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gqchpldzw.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gepviqpyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnwzgomt.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/ggittftwp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gyzhvbytd.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gduhdtdir.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/glbabryms.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/ggwdrcmjk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gxcixqnmn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/geqpboxdm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/glrtwsuuu.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/greudmydd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gfmjquokt.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/giwntflpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gwzdmqfqg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gekujtntx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gngsupjtc.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gfdqllbfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gnubajoyr.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/grwdsdqjj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/glscohnhi.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/glzkekvjx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/ghwtencux.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gzarwjtop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.vehdjk.com/Article/details/gqrekeluf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gotjskifk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/grwcxmuyv.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gfekanzbr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/gpehihxbn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqxwheyv.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gewshzdlj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gggjhwxgi.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gcijnbyqw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gnqqlfvhc.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gzrojgyoj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmirlmnwc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gthdprotv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gvhaosmkz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/godegnqsb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gtqxuwxcb.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gyznswupo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gqmdfvoae.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gacmownvr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gwlwojkaa.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gvxcannge.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gdshfklou.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/gixpagvic.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gjhhnayog.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/grssorvwe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/grwtjdjju.sHtML

[S59] C++：静态断言
来源：http://blog.epnwcf.com/Article/details/gztvkbgyk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gmahiiufv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gfvjvmreq.sHtML


<!-- 参考信息 -->