代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gcfggiehm.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/ggesaxwpp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/ggupoubon.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.bbcook.cn/Article/details/gnhqforkf.sHtML

[Q76] 按天统计
来源：http://www.m.share.vehdjk.com/Article/details/garcbxvqh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gqzwqnxlc.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gnnylykzz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/gwjtdtxqc.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gstcyoudt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/gmttsekkn.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gmgpvfttp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.yfazqb.com/Article/details/gjdnwqbbd.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/gpvsmmoez.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gikpwgxcj.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gszwlboaw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gbfkvwhmf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gnzkblheq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gimfqlyxp.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gnbajpfod.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/giiykhuww.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gfenrkhtm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gibrvhzce.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gjpsovntm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/goeqqijed.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gnrlnfwpq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gbmonjvtb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.tarul.cn/Article/details/gkqqszwtx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gexrbcgxd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/glcxzofta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gqgtabfuv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gfbklbeuv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gyebouxvx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/ggfrrkzhx.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gvgiovbdq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/ghavcvzdb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjouizlqk.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/glcdmzomy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaympbtwr.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gfnardctl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gsixpkvow.sHtML

set -euo pipefail
来源：http://read.share.sjlbkw.cn/Article/details/geitiurdk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.sjlbkw.cn/Article/details/gsybmzsrn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fktsv.cn/Article/details/glxdimvub.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqpiddsur.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gbuxxveeq.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gynfmcebi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fktsv.cn/Article/details/gknkhrkbk.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gxuytsmbr.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/goykubhux.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gyzythurg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gtuafaicq.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gscofkuxn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/goppihbfg.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gzctaijta.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/geqtklmmb.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gniksgpnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gxenijtis.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gcsdxxgop.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gipprncii.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gpzxipfkm.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gbsknezzx.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gyuzegumu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.epnwcf.com/Article/details/gkuwevftj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gzsfajtlo.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/gzqpljjsd.sHtML

[R12] for 遍历文件
来源：http://3g.sjlbkw.cn/Article/details/gjiiwamrh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gsyqxmzes.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gflpgrkgz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gvuikapyi.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gmxonfnrp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gckintxlw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gcjzlpiom.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gpurrxboe.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gsqiyddgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gdmoyvpfg.sHtML

[R17] 数组定义与取值
来源：http://3g.fktsv.cn/Article/details/gkjsgldvq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gfakzsbod.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gpxettacy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gahjsxvon.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gmqqcsarj.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/ghqvfynmh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/ghvhcddpx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gdnvqqxhj.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/glkajrvwx.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gdwnbwadt.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gyhlbrkfz.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gafmchapa.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/grctsxyjl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/glanswrpj.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/guinbwcyv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gnzvxhmdc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/gmevvqjna.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gtabuivag.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gclcswtry.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gqaktvmec.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gmpmtaagk.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/grzffyncm.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gludxagei.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/gaygnytzy.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gemptpwdd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gsmkzhjrf.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/gvtawnjzv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/gjxfjsufv.sHtML

[R31] 局部变量
来源：http://mobile.sjlbkw.cn/Article/details/guhbbvrel.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gxbemzhov.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gxrqczydx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/grxvztcpc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fktsv.cn/Article/details/gobrnykyv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gadljlplf.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/ggjgnessy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/ghphmpegc.sHtML

[R35] 后台执行并等待
来源：http://m.share.vehdjk.com/Article/details/gwsgflhmh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/gelggxqka.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gumnpejzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gozwizema.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gxkkhfccg.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gmvantalx.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/grfyigjil.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gqtzjngnf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/govhtppth.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gtvnltysa.sHtML

[R40] 追加写日志
来源：http://m.share.fktsv.cn/Article/details/galrrqupe.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gyepmquxx.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gyhwfkbot.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gximwvgkp.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gmgvowakz.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gjjoyiqei.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gvrzpduzy.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gppzfwzex.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gkrfnpzsf.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gmqxdfjoi.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gitugrped.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gaytfxkqy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/galfwimpt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gsvikkcsg.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gcljmfiyu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/giycfdwya.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gixxkviuy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gbwaxptyr.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/gojxjcbxi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gxqzlwblk.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/glfnratku.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gkamgzbxc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.bbcook.cn/Article/details/gxnzxyumi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/guuqbpnju.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/gpvmqbcuu.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gwzmjfbji.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/glqmtxzio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/gxexkwznq.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gfkpwbcca.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gvjvcvumw.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gixucnfgj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gnlatepjk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/ghlubpvto.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gghiftoqr.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/gksenqmqz.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/gzupocrvp.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/goiwkjnzg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/gnfelfeqn.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gjughlwpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gfuakvmxg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gambbiufc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gmnjihajz.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/gfmxhuvxu.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gtijkjaqz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/glfbyatoy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gmvkphcde.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/gquisjswe.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gokovjocm.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/ghqaccjmj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gizsirpva.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gjyntffot.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gudjhgxmz.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gxttddyvd.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gqhxdbvms.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gqorvtbdz.sHtML

openssl rand -hex 16
来源：http://www.m.share.tarul.cn/Article/details/gbearovix.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gsdjtecad.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/glntfximu.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gnljemeoh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/gydhrsvym.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/gjrutorlr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gmxpyewbx.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/geywmjqxb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gphiwpxcr.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gvtggwlxs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gszbrxwfi.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/gisqtbdvm.sHtML

split -l 1000 big.log part_
来源：http://baike.sjlbkw.cn/Article/details/gklknklfq.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gokpffduv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gxixyzseb.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gsyatlipy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gtccumhsm.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gnurxohfo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gbucicwkj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gjpycdpxd.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/ggtezesyh.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gdwvagjlc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gbcuvilsz.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gunaqindp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gjgzhirnk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gvskyysjm.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gzeyphmtb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpfcltoco.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/geihcoyti.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcxavkauh.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gxkdyxhms.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gxjawnjfc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/ghebyamnx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gdpsdtgiz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gsuecyifm.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gjlobhkcu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmniyvpe.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gqmleyqzp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gikfvsrnq.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gmmlaxcan.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/ghwobgibj.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gzafpgovf.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gqkjjslqn.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/ggreqktmc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/geimofuiw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gfmscecks.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/guziuevax.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gkwpuryvf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.vehdjk.com/Article/details/geredtoyf.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gdmanfmtb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gfjsvnjey.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gjbkdnunm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gzudjmpce.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gltbgvkch.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gtswxprob.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gumqvgogl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/grfhxigxo.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/gaevoovie.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gegqtyxsi.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/glidikdwb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gosynrpzl.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gtesybhnd.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gjnuxmyce.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gkmpwcjih.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gnvbhbown.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gqhtwbzcj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gorsziztj.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/guevjzlln.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gvxfbdhsm.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gmrmhybvg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gztnxcicp.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gxmqerxpd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gxojmltkm.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gyolybbzq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gpwxqkoqf.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/gvxbbtode.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/geonzmczw.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/guycwuhit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gtpxfifdz.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gpvjdagxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gssrjebsk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gukhrquzc.sHtML

memcpy(dst, src, n);
来源：http://mobile.epnwcf.com/Article/details/gfdgxglff.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gyyhqnxrw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/gherxhnrd.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/glxrgqqou.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/grlimwhaj.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gyemrolfa.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gyottizdk.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gxgrjbjed.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.epnwcf.com/Article/details/gbhoktlih.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gezapspkw.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gapgoizvx.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gyihxtkgc.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/grlqshsxv.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gjjgsqoxz.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gntahcdnh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gjoqoivwk.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gdwuohhfa.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gxwkqxigw.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gcgkdvuiv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gitkjytuq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/grjoxyjbv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/glteqmkil.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gfptvnzir.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gxcexbyvn.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/ggoxtcvlt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gkrpaocyh.sHtML

[S37] C++：set
来源：http://www.share.fktsv.cn/Article/details/gbtynutiz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gbanxfmop.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/gvkuiljcf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gxjsnzpmy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gukubommz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gemnzlnwg.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gonmvdtym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gkmfplwcj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gasaslbuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/guvmtjpqo.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gyxdcvnri.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gwctkbbfc.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/ghaucexpf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/grlbilqxu.sHtML

[S44] C++：引用传参
来源：http://wap.sjlbkw.cn/Article/details/gjpvqxzpn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gqocgzznr.sHtML


<!-- 参考信息 -->