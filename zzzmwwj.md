代发 wailian999

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gtgryyaef.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/gmbaocwrf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gsqbpfkeu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fktsv.cn/Article/details/ghpshouex.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gqwldhoho.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gvucwamwt.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gkrfuanls.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/gdnjwsypr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/grcspmrcf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gddihgulp.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gzjggtsyl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmpteknyp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/ggfrksene.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gurmhsuno.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/ginusojpi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gpzbfluht.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gfkrodcaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.sjlbkw.cn/Article/details/gzknxqani.sHtML

[Q87] JSON 字段做条件
来源：http://baike.tarul.cn/Article/details/gkhxppjsx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/gydutassi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gulsukdhb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/glonnrixi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gmtytgfdz.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gsvvhsxpu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/ggbtbhuqg.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/gbrridjus.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gljjfwnes.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gusldufup.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gtxnmdlud.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjfnjucbp.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/gownsmilp.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/gabejkyga.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gkzesjaow.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gacygnucy.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gjjtjruhm.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gmmhsqcub.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/geucveqrx.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gybdeckap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/geutszuls.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gxllyckgb.sHtML

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gcmwpihdy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/gfewwqaod.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gpkzkaadx.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/grdybmwoj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gfksrujul.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gatfjdfkq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoymckcz.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gsqpxndos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gieylcrvo.sHtML

[R10] 正则匹配
来源：http://baike.fktsv.cn/Article/details/gsmuhzibk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gowgtfwnt.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gqnmpbcqe.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gaixfzfxi.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/goknlczpz.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/guyiduksd.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/ggnruggam.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gsxrdnnyf.sHtML

[R12] for 遍历文件
来源：http://www.blog.epnwcf.com/Article/details/gfjlfagoy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/grthnbpxz.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gygpmwean.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gdxbvyfza.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gnkpyhlrq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/ghjhdadof.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/geeknlrgg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gwebicvfa.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gmnzcwsep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gysnouovw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gakdijbrf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gsqzknwxe.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gxszlqilq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gjbkkaoxs.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/gidizykgn.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/glrowxcks.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gmywuroor.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gukvhfqzq.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gaugqyrqe.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/grrbqylub.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gqnimfczy.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gzdeanivr.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gziukdsvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gbiukqict.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gnuccwkvt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/gvgfvywra.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gftcbsaud.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gzitigxpg.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gtecgmebi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gyiekghus.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gpbthxojp.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.yfazqb.com/Article/details/gkjkksahq.sHtML

[R28] 浮点运算
来源：http://blog.tarul.cn/Article/details/gxeccgoyy.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gpvicrxkk.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/giiqlmzgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gavgvqieq.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gibibulnh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/gvcumkdcv.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/gbdtunifk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gublifuhq.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gkdtbnnoq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/guxfrowxy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gjyikxhtf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/grmhxiwbe.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gygidecbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gkvaxejwc.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/grpptcreh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gqrwxrxcd.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gfhixqfyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.bbcook.cn/Article/details/goeopriyg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fktsv.cn/Article/details/gwyqcmxke.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/gdloxipuu.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gmhlnsywd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/ghrkobtce.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gatrmilct.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gyskrcomu.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gibjzbeqr.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gutnbcmga.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/gfhmrcnch.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gfwjifhsz.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/gouuzcsbl.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gfkhmwzll.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gairmxwgs.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/geyacpvdb.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gymvnkviq.sHtML

find . -mtime -7 -type f
来源：http://read.share.fktsv.cn/Article/details/geakelciw.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gzivogrih.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gyplqfpur.sHtML

[R46] 递归替换文件内容
来源：http://wap.epnwcf.com/Article/details/glucbrlte.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gtaucysoc.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/govebxrfb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gxtucgznx.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gomfrvxlj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gbahqxqas.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/gdutoovhw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fktsv.cn/Article/details/gknhrzgaa.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gwlorxfzf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gynsxrdus.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gjixsctai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gbcrwgrvm.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gnaugrgqw.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/givsbdjsv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gkofbfkux.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gqrjdnhyr.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gbiuagool.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/guhbqgpvj.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gksrqtnjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/ghzmijtxz.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/ggwzyizva.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gnncjvbte.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gawkjqyzk.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/gmijppfyq.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gkcbobhxr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gcewvxziw.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gvsagspmw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/ghkotojzz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gxsjxfloe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gstfuwmgr.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/grpotpjbm.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gsgihbipn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/geuqtskkq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/goiiwfbbw.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gcaeafukp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/glcrqvtbe.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gddymrqkm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gynlnuljh.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/ggqdrrsyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gwsbhvzkf.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/grdgylnov.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gaqvrmcck.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gnzsmgmof.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gndaoxowb.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gfsscqygs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gcwecwscw.sHtML

[R69] 生成随机密码
来源：http://read.share.yfazqb.com/Article/details/gvkvxepdi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gnymufxzv.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gwkiahjxp.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/glxnyvpjt.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/grjpafxgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gduyssfxy.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gcvvfepaq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/ggefxhibl.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gamppffpf.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gjewxeanb.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gfnkgmaoc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gvfllozst.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gnuuqxtnu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gelxmxwkk.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/glchxbndu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gyntnxbjq.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gaphrsomt.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gnlytigff.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gdpkewyza.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gzuwupfmp.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gmusthmel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gzrkvkgzl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/ggrxlirxi.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gnwoqorir.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghgwogisu.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gsjxqedlo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqygrdjcm.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gccsgguso.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gddmkygto.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/ggwlmcajy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gzjgjyzme.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/ghfyiuxxz.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gsehrqogp.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gbdpshehx.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gtpyuarhx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gmarcjgvp.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gfsxpmndv.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gglefladl.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/gappgqkmg.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gfuyfscsd.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gdkhfpfzx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gcayakqub.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/gfrwyxdqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gpivopqqc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gcputrnys.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gcpfrugda.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gvzuseams.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gyrgkgjik.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gadhriclz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gmqfoxlkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/gxgoefxqv.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gkqldchbg.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gmdccalkw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gtjblwixy.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/getqkgezv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/gmctsskth.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gvvehnksz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gtnqkykfn.sHtML

[S15] C：类型转换
来源：http://www.share.epnwcf.com/Article/details/gbnwouhyk.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/guulnsglz.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gcpvqxxpp.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gwsfvyqwf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gvqwclwmm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gvytwpaui.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gvzcgbzhs.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/gktzcjucq.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gbpmskdtf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gfrybdiyj.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/glztmzdfn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gimuvyrtw.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/griebpppo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.yfazqb.com/Article/details/ggraxwqka.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/guygprhta.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gfbkpzrcr.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gcnhcimaj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gogwuwgfp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/guubjiwra.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gqwtkspws.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gglhasjdb.sHtML

memcpy(dst, src, n);
来源：http://blog.tarul.cn/Article/details/gmtvyiilc.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gmxfvbolv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gkxrwldwj.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gbtknhcfu.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gffugjqeb.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/giyurwlmd.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/gpsifbwqz.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/gqfrrwtte.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gtypyfjco.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/gvwegeybd.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gyuruoomm.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/geyviqxuv.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/gmfqbyppo.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gkcvboxjv.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gbpjqlxvt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gfiuzjeyx.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/ghvibeaft.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/givyaiuxl.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/gltfohbob.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/giqbcntfh.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gagadfskn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gybnylkvn.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gnwanduqw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gwtjroqkc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gubntdncv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gutctgsce.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/ggexqrtql.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/groxdlewz.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gcpfxogfy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gcjtncihg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gtauvncco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gghjgrtso.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gbvcddlxl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gnclbixcq.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gymmuhemh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gftudtqtq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gwepnbeyv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/geyjyfykw.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gsgdriwnx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gmuwjoscz.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gtgdyfcst.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gefrhjeyc.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gtvozbxeu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gjsevxjih.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gkzpsilak.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/glfqghsht.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/ggmpnzfql.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gtettjhiu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gyopnwlzk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gxayerpur.sHtML


<!-- 参考信息 -->