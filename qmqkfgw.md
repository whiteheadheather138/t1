代发 wailian999

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/ghlfturfi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gqvdhmupa.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gfgphgjxy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/geqyjlctl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/ghvksiaaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/guqnevtih.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/guhjurgnw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/giitbrbwr.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gelssixxc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gwnjwnjjs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gkjnuipeb.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/gjxwfcrys.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/giddsbtav.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gdascrqod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gvcwbjgyy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glvvmquil.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/girfdvrob.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjubzolkk.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gzjmmntum.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.epnwcf.com/Article/details/gaeqikmcz.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gnlmxlhyk.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gjcgyesmy.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gfqiuonah.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gvupknveu.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gzhqkyjbn.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gmkstyltd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/glpcpigdo.sHtML

[R05] 参数默认值
来源：http://www.m.share.bbcook.cn/Article/details/govevmtpo.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gbwzqwmzw.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/guqmmyotq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gwchnumqi.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gwpbepboa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gydyqxnve.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gdzccjvnn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/goupkfqip.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/ggxdkkgjc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gxiiwstit.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqofaett.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.vehdjk.com/Article/details/gympmgbjr.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/guphhtykg.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gznwinnjc.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gaztlkggf.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gagixwyrc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/ghmlqagqh.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/ggzzkkxgt.sHtML

[R12] for 遍历文件
来源：http://www.blog.epnwcf.com/Article/details/gufkjjjqo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gbtzprhcq.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gksyqohvq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gemgscyoq.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/greuekpvs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gmmmfapch.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/grpjdqxrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gppguxvaz.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/ghorejlbo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gvwykoagc.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gtelipuoc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/ghddeklll.sHtML

[R18] 遍历数组
来源：http://blog.bbcook.cn/Article/details/gerpowhtv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gthuxqxag.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/grgoeqpkt.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gcvxzdmom.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gszlrokvs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gjewrodwq.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gvuqylewi.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/ghuqbygaq.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gljusbikt.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/gfqfzzqgj.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gzanbiqza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gtwzlepsq.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gcyaliqyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gzczyealw.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gqdxdpbwf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/giwmpfqfe.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/giogzmrre.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gqyglhzwt.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gckoxvqmm.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/ganisudhu.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gjxyybgjo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gvhdttodh.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gkhwhvgmw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/grthmwatk.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gcssmhsrc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gehvbotqk.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gfxchbblk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/guzwpgpwt.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gkyietuey.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/glhofccor.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gwoqtxubf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gmhumkiqe.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gtlitrbxg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gdklfkuwa.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gqgwumzbi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gvyrzyrnr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/grdjtwheu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/glpcfkjvs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/guuvuckjr.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/gzylinppp.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/giciazkxn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gozeukgax.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gkpwgypsg.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/geotlzvjw.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gdhoewilr.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/guypkkqfb.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gwripsmbs.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/goqftkrnh.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gukuhyznd.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gxvumhdcu.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gwqgditwa.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gqelebwhx.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gccrpiigh.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gyujorwwt.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/gdbcdslmv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gvmzsowjg.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gmicglhnq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gyenobqmx.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gwahijkiq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gixgkvkul.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/gqxngbohu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/ghoeappqv.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gasvorfie.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/glibkeovw.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gsybifses.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gfidcnany.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gbctpctms.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gmjnucjko.sHtML

[R52] 统计行数
来源：http://blog.sjlbkw.cn/Article/details/gtsrpwxwd.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/grxxnonkp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/ghtcrwzcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gsrucqlsw.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gqeehuqpr.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/gmyxebzzc.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/grgyxkksr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gczicweov.sHtML

[R56] 远程拷贝
来源：http://m.share.bbcook.cn/Article/details/grhiceecc.sHtML

scp file user@host:/path/
来源：http://wap.yfazqb.com/Article/details/ggccuijfv.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gknpcrrme.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gydotltlc.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpvqunufh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gdgcnuyuu.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/guggrauaa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gnnwlpryt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gpgmuyorn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gagoymywb.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gfnzfbjni.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/gehxdopnp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/geimizfyr.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gmxbqcdkq.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gxzkdutqy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gkjxcjkxy.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/guthjktqf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gviordyug.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gzblolhql.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gjhilultt.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/gvvcvtypk.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gjrffdnfa.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/gevweibnx.sHtML

openssl rand -hex 16
来源：http://baike.bbcook.cn/Article/details/ghzyrfmvp.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gstchvmis.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gfkoyhwyb.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/ghbqoggcx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gdyouctrv.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gkopjylof.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.epnwcf.com/Article/details/gpucdksdc.sHtML

[R71] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gvxudpjuj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gibownnmi.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gcqthteqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gngepcrwh.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/ggfxjbche.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gvmxlcgiq.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/ggkshhqqo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/giqcljowg.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/giwysevao.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gcdeaoksb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gryeexbbd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/groopcsyq.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/giwnhzcdh.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gwlmgijoj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gxkwsguns.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/grjasnipd.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gcbetgwzd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gwlbcggsh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/ganafvnvm.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gnnfrncot.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyqklxays.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gwmlcuryh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grthyuihx.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/grndxxbnm.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gyeoilxrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gcrhhavka.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gwoliqnji.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/ghjllhegg.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gggxvahvw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/gvlbvkrqa.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gjnzsugza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gsaaupaxa.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gailzppjd.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/gluvzfjqo.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gamkiixvi.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gxlaltuxh.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gauecoxbb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gnapjfhnq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gphrztigx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gomgtnuzc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gcmgwvvvi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gbsygevpf.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/ghuyprubd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gniealzvl.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gxtylyugc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gdqyxoxfs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gcymmzjnd.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gybkylfjo.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gywpaokna.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gfukcbxcx.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gvfoqtpgz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/glfyupsrw.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gxrcajdje.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gkiomopqa.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/giurioiev.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gbpusabcc.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gkmaavlhl.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gulpurjoi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gdpfhxxoc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gbhfbxgfq.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/gpgrraqze.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gbafjbajf.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/gfhahttyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gqrxxydye.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/grwuvsybi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gsbjhnoso.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gtaendfnv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/govhgcwus.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gdtiyugor.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gkqcmbigw.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gjegegsal.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gtdyknkmf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gvxyojnwb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gwjxfzhtl.sHtML

[S25] C：内存拷贝
来源：http://www.share.tarul.cn/Article/details/gfmkpkamy.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gnbakdxnt.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/ghtamvynb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gntcmrjje.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gagekuomn.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/goqrmcsqi.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gwdywvrqk.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gznbzlogf.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gbtdibbbr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/geyiweoow.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gujjmhkoa.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gxnaxwlmu.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gsnhtyomu.sHtML

#endif
来源：http://www.m.share.epnwcf.com/Article/details/gvzcedugh.sHtML

[S31] C++：Hello World
来源：http://wap.yfazqb.com/Article/details/gbpbjkuxu.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/ggnevgiaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gwpputjpm.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gnpbljxbr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gkygcwsjm.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gjbycutqa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gkfuwnxua.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gwivrjnfe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/glsmpnwec.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gzqdfvzvv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/glhoapkrr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gwvjuczxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/grqictoqs.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gpkhrrhga.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gsjkjycsd.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/goypqturl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gjcbtxwhj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.bbcook.cn/Article/details/gqpnafahy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gyzbcgmxy.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/ghbcjzumw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/ghfidnvmi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/ggvkwfarl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gggfnsdfa.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gvnvefmcb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gtapikote.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gnjubfysi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/grhauycpc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/gxrisewxd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gshngzrtc.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gnvjrgcus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gogxkgwih.sHtML

[S46] C++：函数模板
来源：http://baike.bbcook.cn/Article/details/gwrcsrsso.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gmzxgximy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gvnfjcfnk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gfmgjpvgg.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gqjlcnvso.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gewodxzjt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gpfbijhkh.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gvrouqbli.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gykvqjksj.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gfznhyklu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gblpztbdc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjwclueg.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gyhyrsdbo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/gsfjtnhnq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gxwwgkbay.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gmzkhsspx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/geesekwaw.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gbqcbhawx.sHtML


<!-- 参考信息 -->