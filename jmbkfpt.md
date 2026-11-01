代发 wailian999

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gkapuzmvh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gismeymeg.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gfonrbabb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gqhjefbuy.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gppsidbcn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gqeilwxqf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gpxidrmtx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gkwqpnisr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/gsyjtwyui.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gotmumbub.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gfcvdrvtl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/gpkrvecuo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gxiotsujq.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gvuefedlq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/gitphmxfi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gblzwqsyx.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gnzdsffoy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghulkbpdl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.yfazqb.com/Article/details/gimcblctc.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/gsjxtfknj.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/godkzncxy.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gkkbcgcde.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gwrtrigum.sHtML

[R03] 只读变量
来源：http://m.share.tarul.cn/Article/details/gzczwgmnh.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gxahnmjbp.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gdffrspjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gjocmxlwf.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gwzmiitqc.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gfrloynvq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/glqjakcnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gkxjtvwsk.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gdpkeedyo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/gmbxplwzs.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/ghcbzbbqd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gpfxmqlnt.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gqpurcvte.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/gkdxdhmsy.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gsmibdxph.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gehavuzox.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gylrwypfj.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gjguajhzi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gjldadptu.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/ggivlermc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gsscubxtn.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gscsqelwo.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gcknknkrn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/gadoykyaf.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gogpslpuh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gkfyvwxhh.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gbfebihzc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gpkejnrpm.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gsfviubaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gwnbrxqrv.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gajdxnhel.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/ggqvdevby.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gobrgvkjp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/garravgzi.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gklqahmxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gzxziqjnh.sHtML

[R19] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gcexfzncu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/gfggqkraf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gllaylqsl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/gglotmzua.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gojnalqaa.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/grzivoslx.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gcvwhllbn.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gbbsnitar.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gvfravmqg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/gihhlzdpb.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gdqlfxnkl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/gtqowtlct.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.epnwcf.com/Article/details/geucaqtou.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.vehdjk.com/Article/details/gveqzqpxk.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gbnicadwi.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/glomczojn.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gcixbcphq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gbahplafj.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gucrgdclo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gshhagbkd.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gvivjszdx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gmhqjdwfk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/getnogqwq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/goflgxloi.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gghcfvdwq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.bbcook.cn/Article/details/gtjrfqwws.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gphcizirm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gjxefzszs.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/giexepeeo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gvtynlhte.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/giuwxszss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gmmzylvpl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gmhufedhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gfuwrjvpd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/glydlttjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.bbcook.cn/Article/details/gsagmzmse.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gwgqwdrix.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gjffrolna.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gbibnbjki.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/gpjpwpkbc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/gwmgtsfmx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gtkuycxyx.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gkrnhtevg.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gqhmmtluj.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gqmqxdgrx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gkwiikuhb.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gontvuhrt.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gstbknqty.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/goueffoar.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gkttydalu.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gibmmoaro.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gnvctvcfe.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gqxllbemb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/ggrmoougq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/grxqtvdjl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/grxaokwva.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gfxkzsjrw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gspfgxfbr.sHtML

[R48] awk 取指定列
来源：http://m.share.fktsv.cn/Article/details/gstchcjrd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gtcyzysgz.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/glqhusmpi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/goctppofm.sHtML

[R50] awk 求和
来源：http://blog.fktsv.cn/Article/details/gxgpxsjtd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gepetnbsh.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gondbktxo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/ggrqyfqry.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gyuzawlfw.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/ghtrhnhkq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gkqgcipvr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gwvgdytrx.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gjcjkralz.sHtML

diff a.txt b.txt
来源：http://www.m.share.yfazqb.com/Article/details/gyquyjwqo.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gifhupygq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gnzztxtqr.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gdunoxcxs.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gxhnhqcsl.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gphkqgckm.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/grumnzyas.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gxfxupeyr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gaoywvxki.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/ghlfkqvsj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gppclozfe.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/ghpdirdfe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/giayamnrm.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gxutfscpi.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gwtgcinwh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gekjygyzr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gfvubptff.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gsyewsobm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/glbxqbrea.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/gyfshszzh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gfksaastk.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/gwqulfnzh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/ghdfrqexe.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gjtriwejp.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gawpgmxko.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fktsv.cn/Article/details/gwcvpvwbg.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gtxoylxkk.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gwpgptbsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gtymdimwo.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gnxsssmhx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/gewvqhhdh.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gbvstythy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/gvmtwpzuw.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gacspbgbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gvtravvbe.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gfkjyelvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gvotfijmk.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gltrttkwx.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gpdrbwbpq.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gpzkarawq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gkmacprmn.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/guvpsidfv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/glxswnuov.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/grqqyjimm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gnbnisqpq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gqiemtstx.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/gqssazrjt.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gxyunaglp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gwlngzuzp.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/ghibyebwh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fktsv.cn/Article/details/guljvgnii.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.epnwcf.com/Article/details/gnwwhvynk.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gjlohreei.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gswcvuwzv.sHtML

S. C / C++ 专题
来源：http://3g.tarul.cn/Article/details/gdfdjobrr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtetpdmlw.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/gbbgazfqo.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gyhjhngdf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gieyknccf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gdbxxazfw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gvuuwzffw.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gwtflxbfr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gomlxtbjk.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/guzpyzeec.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/grrozsbbr.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/gyndghahq.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gtpmbywgh.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gwhmiquzz.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gfwxtriuz.sHtML

[S07] C：数组遍历求和
来源：http://wap.yfazqb.com/Article/details/gehxzeulz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.tarul.cn/Article/details/gnmxayqux.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/glcflsuvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/geyqedzpn.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/gfgykhphi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/gsmvoigdv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fktsv.cn/Article/details/gjlctvuhl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.bbcook.cn/Article/details/graumjhfv.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gpmtilesl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gphlkdqky.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gogjrsdkv.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gjhgcwrso.sHtML

[S12] C：写文件
来源：http://www.share.epnwcf.com/Article/details/gqbxnjmxd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gmjmbcsjj.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gwrrkmwqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gtfhjhnkn.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gomvgzowk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gtnsulngh.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gctqahlra.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gvzqsyqms.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/ghnjahpeo.sHtML

x |= (1 << 3);
来源：http://blog.yfazqb.com/Article/details/glenpxfrm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/glwtbijic.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gkcytcdxq.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gexnoipab.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gfblzyfdu.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gliinmguf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gbaicofzl.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gmsgvlkpj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gdbautbei.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/guswvcojr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gxvtspjtz.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gtcztzcgy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gesitnlhv.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gvjwfydbl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gemaxmwyx.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gwfawxeqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gdvkduapr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gjvflboom.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gbppilfmk.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gxxpkaxqq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/getjevtau.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gjbwxxdid.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gadfjxjqy.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/gsbddqqlf.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gywsggdvu.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gyfukhvfa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gzikxxrzx.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gnuykyomv.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/glmnokpnj.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/glxqsvhgn.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/geadqbojr.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ghsmgasmu.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gxqiivqks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gynosemmz.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gueucllik.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gtsomxrgt.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gvurkqrfu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gmsevfzhb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/goqsyjrme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/gsyruxahy.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gqtfdbqvi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gpxzkpyzh.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gnnzdbcxr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gqawiynpm.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/gsiiwqfdy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gkddewasn.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/geuiowgam.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/ggfjtkvev.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/galrcjaub.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gpyfjsrww.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/guiofttsz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gfmqgtvzx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.yfazqb.com/Article/details/gumftwyfo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.tarul.cn/Article/details/gnowgiljj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/grfakqgmn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gvwuiyzqf.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/grdvxzkik.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gdwtnlspa.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gtdibmpmc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gwepmqlbn.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gbokpjsua.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gtliyevhh.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/gfbytgyhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/grijlcvxr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.bbcook.cn/Article/details/gujlstfhi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/giusmjfzu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gutwjfwqo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gwxbkhugo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gxvqnvkxz.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gvbroypfn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gfpyoqtgd.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/gkqhbojqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gqrlltete.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/gqslcorac.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gshjptnvn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/gharrzcil.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmorbwav.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gjpjmqrip.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gwshiholp.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/glkwcikhb.sHtML


<!-- 参考信息 -->