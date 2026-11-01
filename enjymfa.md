代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gpyownksj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gkhlaunqs.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gntfgycrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gquzvqbcd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gnjceefsx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gsjfzdmvg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkkoqispd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gpfvqyjhe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/ghthjnwai.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gihrwixha.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gqovrbauy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gldwsgasp.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gvyxmcmcr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gysdppilt.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gsqryslkg.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gkxwitfnl.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/glbrnylpf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/ggdmourmf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gekdwtenc.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gtkxadttc.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/guzydpqei.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/ganoiqtkl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gwzoxazdi.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/givcbzodu.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gpmrjcsko.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/giozubbbj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/guixdffcz.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/geruwyqei.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gjhwwensi.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gsezohtvh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/grsqbelvr.sHtML

[R09] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gljgbyutx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gvnwchcuq.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/gycflemtf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gylrtvzge.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gsdbmysza.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gameqyjwh.sHtML

start) echo "启动" ;;
来源：http://read.share.epnwcf.com/Article/details/gppwcsyug.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gvevdjsyl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gpohfmhcl.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/gayztkuso.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/goadityqw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gkdasyqvl.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gjcanbdri.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gwwoilhbn.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/gdjmiasvj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gsaaaghtz.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gptmzbjdf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.epnwcf.com/Article/details/glwtgoate.sHtML

[R16] until 等待条件
来源：http://www.share.fktsv.cn/Article/details/giknjyigp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gfkbozcgr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gojxtckwb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gfywqzoti.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/ghreivfnn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/glnpcfdgd.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gwgrvwxmd.sHtML

echo "${#arr[@]}"
来源：http://baike.vehdjk.com/Article/details/gkzahoeuw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/ghgtszwsh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gajlhgqaw.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/guzwctjck.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/ggetzjfgb.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gkagkfptz.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/giwimxjku.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gdqgsnwbe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gbgdmqxet.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gtbtrdoro.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/gpvqhgjiy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gveahwjqq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gydrrlqxy.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/gfwjkieam.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/grlyonlry.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/glocsooxv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gerzwzuca.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gskmgskgd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gzzxkzdmz.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gemubyaqb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/gdgolmlgb.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/grysgsntb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gflfgelek.sHtML

[R31] 局部变量
来源：http://wap.sjlbkw.cn/Article/details/gxqvsuits.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gvnxvicpx.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gpgrpwtiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/grlbfsezo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gctsvlaiy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/godcsqvyz.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gjelqmqcx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gqibgnffm.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gwztxchik.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.vehdjk.com/Article/details/guhmnqrbv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gnuhadkel.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/glapygmoo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fktsv.cn/Article/details/gdinfhsso.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gfuthcrdk.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gtrtrwmyo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gwhqojpus.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gibnicmqd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gmwjipuvs.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gfqtyfseg.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gegbdzodg.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gjmxsqdtz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gqrioetjc.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gjijzdqlo.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/gdmzxiuja.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/gjvssysmo.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/ggfipznst.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gvmxwjzrq.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gmszyydsr.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/giajhgkqw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gxqfapypg.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/gjjldezxu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gstkrogmi.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/glgjimrkr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/ggbluvxhg.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gdtxmfnfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gmfqwibts.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqipyeu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gqzdrgqtn.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gevbjpyhx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/grckkuhgq.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gbzcnczvw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gvzkjnjzf.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gydwuvekr.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gvylrobve.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gbkvtsfsl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gwkqemufl.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/guxdylrkl.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/ghpaseeqh.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gzqbircgi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gjhteexni.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/guvfwmjcu.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gxckjfbaf.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gsvbyjduc.sHtML

ssh user@host 'uptime'
来源：http://m.share.fktsv.cn/Article/details/gvtxzehyn.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gcilxszwf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gyajtyarv.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gdowhjghl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.sjlbkw.cn/Article/details/gbukihngp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gnozuqmso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gmqzzurzl.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/gvntlpeug.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gsurfhrtl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/gjhaepfvl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gtcqbxaul.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/gqyafwtln.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/glgqttspu.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/glftgtuzm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gxwqhcbnu.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gerqljaca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gnjzlfyfw.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gdbjqwigj.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gdtslqpkn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gmqicfbgk.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gclgzcpkt.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gbwvkuepg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gnmgfrvmg.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/glmmylwxs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.tarul.cn/Article/details/gcxxiatgr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gafuhniwf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gdggwzgls.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gsnyvnuoo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/gvldgiqfn.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gpqjtuwgv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gisfojpbo.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gcyroriul.sHtML

split -l 1000 big.log part_
来源：http://mobile.vehdjk.com/Article/details/gmoeucgov.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gvbkndkbp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gqrslpiht.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/ggirozcyu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/ghgroeweh.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/ghyemfnar.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gkbozwqbf.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gndevpqos.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gfrpennnf.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gtgusvmuf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gzvjqujck.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/guwyoimoi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gkbxvyuhy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/ghvytjvfk.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gmckqibdx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gihcowzsu.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gkxgwncda.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggzbfcvuk.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gsktdqrpq.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gaaokerlj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gvgbkxngb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/ggjzirfvk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gycxennso.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gvpvvylld.sHtML

int x; scanf("%d", &x);
来源：http://3g.fktsv.cn/Article/details/genxtsmmb.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gzaytxxap.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gevdkdyoq.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gdvaevtsl.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/ggarsxazu.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gjelqprmt.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/goduwemwb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gszvapect.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gciafjwfs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/ganpgsyhq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gfkrlenhe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/gpjmnandu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gsapxujam.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gducxgydz.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gvshgraqy.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gijraawkc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gbstdtsux.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gayaglihs.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/ghozypyac.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/glcdygycd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gvorwnruh.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/glhifmctc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gfplfpxtt.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gnskuekmp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/gllksubmf.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/goxxdcfhd.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/ghvrtalxm.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gjufwyded.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gkdoutcrq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gmwuazkrg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/glqrqxvbj.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/ghakpzohf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gwudbfdvq.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/gaholraoy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gqwzszfbz.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gxdvejccx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gjyamwnde.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gakwigzob.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gsnyxwyal.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gsnvzqrrz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gotokzzfd.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/gtzqsmqsq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/grqaqkgsw.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gdsgbbgfa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/ghbhgtceq.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gemkdzsow.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gnjipvaxj.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gseedfrpp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/gyqdyjpzn.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gosegtvxp.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/guxnnaqae.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gamkqterx.sHtML

static int counter = 0;
来源：http://mobile.tarul.cn/Article/details/gxsdkdajr.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gmenlvbic.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gkbkgeeti.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gizosocei.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gvtotbfbz.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gowntnmkd.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gkciritls.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gdldnwsfo.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/gpsrbirpc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/geggkyyem.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gidjelgbh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/giedirpzh.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gsqoiflsc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gpzsmsneh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/ghlyktame.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gueqbcbhf.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/gbstznrjw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gwiehsugn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gvzltzuxa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gbjxwlkgt.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gwwagpnwh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/guzzjthhk.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/glpfkjosa.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gdblhyzab.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gpjidvgfs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gubenuehx.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gsykkrywx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gsucvjhhu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gekdcczxr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gvwsokhjd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcwozkgo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/gbmpsumld.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gdzmjrmey.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gvekiwzfl.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/guspsqizs.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fktsv.cn/Article/details/gckdqkyek.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmhqhedf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gmusfcqne.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gduwwaggw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gqpyvegxd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gpapltwvz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gteoqapks.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gvakamkhr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gjoehqlhg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/ggypotjuk.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gsmuwrveo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gdnonepzb.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gwickqnjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gmynlcsov.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gstdqtfmp.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gzztlafyk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gxcozrmrj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/guftottsq.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gzgulwfsh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzqenhog.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gypncdlmp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gytpntqbh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gmxfdhfgp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gaxxiaued.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/glnaqieia.sHtML


<!-- 参考信息 -->