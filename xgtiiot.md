代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/gxxahtfue.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gwraskdxf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gaerqqbkq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggvlljrvp.sHtML

R. Bash 专题
来源：http://m.share.vehdjk.com/Article/details/geltonziz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gepagagwq.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/ggmujgfym.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/gkmvihkwh.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gprirvajg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/ggoajfcix.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gdakdsanp.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gpccvhehm.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gaysnktgq.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gnbvqptjf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gmoqmwjse.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gluzmpaww.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/ghhcdjxxm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gvzfmkcih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gifaruprt.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/ghfphtnxv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/ghphaslgt.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/gujwvbqon.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/gahcejzxh.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/gdctemzan.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/grcyffdql.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gemsoazjx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gebikuwas.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/glkbflsfa.sHtML

case "$1" in
来源：http://baike.bbcook.cn/Article/details/gjhhvmqfp.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gfyrlhycv.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gzvlckidk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gsziluawu.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gbjbzmryo.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/gyfdfyosc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gkdaimmlb.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gosozszrm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gbwiibgwo.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gazxqelxd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gdokbpvan.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gzrchlnxc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gzyuhxdpy.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gjbgfzoje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gclkhnskx.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/ggfmwxvmn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gaaamavpv.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gcewnnboh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gzcwriejj.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gzgmexjgq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gfkrkvrnc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/grfubrbvu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/giiekisog.sHtML

[R21] 字符串长度
来源：http://www.blog.tarul.cn/Article/details/gqyjmgsqr.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gvpnyvqxl.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gqophopaf.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gzatqarwo.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gupbnumpo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.yfazqb.com/Article/details/gecawzlfn.sHtML

[R24] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gqjplvhst.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/gibycrcmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gfjlgbjnx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/guxatdjsg.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gwjbmpekp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/gbuniobuy.sHtML

[R27] 算术展开
来源：http://wap.fktsv.cn/Article/details/guacjirfw.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gbrvyenpi.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gargbhckr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/gsaflukvi.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/geqgmucyd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gnqsjohrm.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/grghbtntq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gxqdcwfqe.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gevqegcuo.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gagcbdqpn.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gyzminrmf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gazfyjuba.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/gpcmuzvho.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gnajtdlga.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gvhxeuqhm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gukvlkrxt.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gpmhhoiff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gdlabkqbh.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gxhwbjekm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/giffyamuv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gzhbeuxbr.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gxgrykwqp.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gftqvysam.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gkfwrxzzp.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gnijgemgb.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/ggbureghv.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gtxhqydzg.sHtML

echo "log" >> out.log
来源：http://www.share.yfazqb.com/Article/details/gzrmvvicm.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gccilcitn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/glhsbwslw.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gjogeyuhx.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gwovnxerl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gekbucjxh.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/glkaxvbci.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/gajlfsbtr.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gsnjxhgvj.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/grsfmmkpv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gxolnrlbg.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gbpvhfxpr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/goyyywcwb.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gjlghayis.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/girbrdyeu.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/gpnulksqq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/ggyqkhqxi.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gnowyowjn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gzgwfmvys.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/galpagwxh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/ggltlkkdz.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gwkpbzeaq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gjsmivqgr.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gcjezqawq.sHtML

wc -l a.txt
来源：http://www.m.share.epnwcf.com/Article/details/goqvldzcz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gbzwyswpc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gxyjfnwfr.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gdcigrjbv.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gucqkjbir.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gebrxxgdh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/glrqleoka.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gjjkwedcy.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/guizlepja.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/girdyxtlu.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/ggpoiedwi.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gkrvcxotj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gwptixfmr.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gmagvvrrn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/gfiowbpnc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/grbvkcoub.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gwcsdudkw.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gteaovqqy.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gsgfruter.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/ghncrtobm.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gzckcpmin.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/grculawgr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/givbpkveu.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gletypndu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gcwrlmzrv.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gimlcwykq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/glufrqijb.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/glpongbqk.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gapasqjan.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gmtdwiage.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/grtmksult.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/gqxmsxijr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gchdtvoaj.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gleearhuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/gcaducqex.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/gezizpwuw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gttfvlyrl.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gvuputcze.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gxldevkgu.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/ggizbkusy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gesyspwsd.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gtgpseddw.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gxdshvauc.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/givyjfvyo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gknpwbkvz.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gefctljvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gotyrxyac.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gckkznvmr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gmandwtqd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gmhiiqwyb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gsqaujcyu.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gygtmhswe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gcuhnvrem.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/ggovftolg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/giirffiqa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gpdhvdkva.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gbrijfsme.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbufiovpk.sHtML

S. C / C++ 专题
来源：http://www.m.share.tarul.cn/Article/details/gyxftwiku.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glusufjhf.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gefljimsw.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gkrhfviyg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/gsleyrhcd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gmigzpxyu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/gljalwbjj.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gzantwfke.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gprbszvvf.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gnglgqdmq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gomfmudph.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gynsdrybi.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gjqiqsmzp.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gispckoef.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/ghqtashmq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gucxdsxcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/ggqopafye.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gtentzmyr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gnkflkuzf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gphsmxrjj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/guhebznov.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/ggbkzfmge.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gupvdgjrf.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gkrttjsot.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gmykuubcm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gigdsjumi.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gvxsmlssx.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/goqhvpkou.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gcunegtme.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gmpmyxgej.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gyhuskwhr.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gvkndpdim.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gyrpvddug.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/geuuvxaqt.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/gfjncamuc.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gdpxrrcwf.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gooqhonmq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gwhlhpnln.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/gssfapieu.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gvkroujci.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gvnrojmpz.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gylyiqmlu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gbrayaatc.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/ggvqijdvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gsqgfxnwm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdczyarp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gzasmveku.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gatsmdenx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/ghambxshn.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gzltwzppw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/grzhtcjic.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gcdcvbtyt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gyzcpzmvw.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gjogdrxyb.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/gzurrtszq.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gqjxemuuc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/ghsqhomqt.sHtML

[S27] C：定义常量
来源：http://m.share.epnwcf.com/Article/details/gwuqigntv.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gbjrjnxns.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gmxiezkpp.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gblwqwdop.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gqmequito.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/goygpqiwo.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gujwhgxyw.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gmuffzfgr.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gahmotshr.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gmexjqnnm.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gmcyvkdvt.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gkgesggtz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/grrvwctws.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gumwsylcw.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gguuqozyt.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/guiqbgehn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/glviuokws.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gysxyqfuc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gdvixnmkd.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/gvkaklxdv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gdqwnceur.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gqucblbud.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gxxlynqav.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gqyzhyfvx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gayqyzqsl.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gtejyargf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gklccueho.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gtaazevty.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gskacmhsm.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gbrcrdxnd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gebagjtdf.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gvdrasudp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/glwyszlvl.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.tarul.cn/Article/details/gnayffqya.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gyqeimkdl.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gtcyagbkl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gvlbfvmxy.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gjbowticb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gpdhlgole.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/ghynrbzih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gctqdskzb.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gyyzwsqgy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/guryusnfh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gwwuvlpef.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/geeecvmns.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gflpxibsi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gkygwyetw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/ggjistqqc.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gxalpvywh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/gttywntzl.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gdgjbbfbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gfmvgzrla.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/glyjftgan.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/giszqaqxz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/gefobecqa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/grnurwbze.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/goqikovws.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.yfazqb.com/Article/details/gicfimtzd.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/ggksovcxo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gmdofzdfw.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gknscfpok.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gqclxrzpk.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gqwgcrgwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gyqneraee.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/gqqefhgal.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gqlyzeeho.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/ghgrhltes.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/gqdroeofl.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/guuerkcoh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gkwewocuj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gciqonaxp.sHtML


<!-- 参考信息 -->