代发 wailian999

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gvaxbbluj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gajknzxrw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gxxsaanhw.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/guxcmpahk.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/glomqejkg.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/ggqmxpcmv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.tarul.cn/Article/details/gtouovcto.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gvnzvynqp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqvysquny.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/gdrrqnksx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gneqqdyre.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/gcwtcylza.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gjeipbhxv.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/garoanldb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.vehdjk.com/Article/details/giidbrdzm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gnivrdfkj.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gbfpsvfnz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gybrnvkjb.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/gidfnfuht.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gfjwzgibr.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gordbmmzf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.vehdjk.com/Article/details/gxoakkijc.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gxogjxbdx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gukynzatj.sHtML

[Q80] 字符串截取
来源：http://blog.epnwcf.com/Article/details/gtjsjeigb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gtfppwirq.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gpzsrhlmi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/glxizppkr.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gertolgzb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gzyemxwex.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gfwphwzhx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gjgpyyuae.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/ginnlvgse.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvobdyihc.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/ggqezitlb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gttqrgdaf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.vehdjk.com/Article/details/gkzavufft.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gbvqrmowf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gseckpbrp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.tarul.cn/Article/details/govrxynms.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gyatmdzie.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gvfljszml.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gbxyckxea.sHtML

[Q89] 判断表是否存在
来源：http://read.share.vehdjk.com/Article/details/gtnlqtmvv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gzgvutdxb.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/ghkjikkgl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.epnwcf.com/Article/details/gjcsnqhjn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkpozzhnl.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gcdganwzm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grtzrixmh.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gaddkyflt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/geitlxvwn.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gjeapkmiz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gfdkkjjlx.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/giifwzwth.sHtML

[R03] 只读变量
来源：http://baike.bbcook.cn/Article/details/gnfgyofck.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gunjulsyf.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/gqsicfixi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/gkfmcznwb.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gnynbgkiu.sHtML

name="${1:-default}"
来源：http://baike.tarul.cn/Article/details/gguqgesmz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gunsouhhm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/ggvhxgzjp.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gxembvoqm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gyokwqkhc.sHtML

[R08] 数值比较
来源：http://3g.sjlbkw.cn/Article/details/gxuovtuaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/ghlwekidd.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gbwafiuhx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/guvsompff.sHtML

[R10] 正则匹配
来源：http://www.share.bbcook.cn/Article/details/gbmbfeejv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gcencimev.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gjxfkhrco.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/gwwiloksm.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/ggkhkahrp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gkxizmzua.sHtML

*)     echo "未知命令" ;;
来源：http://wap.yfazqb.com/Article/details/gbtmdbeqh.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gcmavhlko.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gdgmwreco.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gkqkqvail.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gatmtncjw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gomceunzq.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gdzebxpjs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gzyjoivqx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gfhupdvbm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gaonwjpbm.sHtML

[R16] until 等待条件
来源：http://www.m.share.epnwcf.com/Article/details/gzcujvahf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gmjrbhexd.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gszsomzgw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/gzkqiuzgh.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gcyaqfgmg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gpoczsnza.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gfwzhhduv.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gpzexphtr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gjxhdunxv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gedhsfehm.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gdertxgjb.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gzhcaszod.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/ggsbdffng.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/geobnythe.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/giyaddssv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gzfpynhvh.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gfroktkfq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/gsgqbjyig.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gwqcfsybm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gjzodifib.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/goqrleela.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gxabkuiwq.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gzvwypqee.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gtasjffor.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gzzhbmqzy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.tarul.cn/Article/details/gwumtgbzx.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggloseult.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gekondjuw.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gyqdsjgeo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/gjsqxiylq.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gshlimgbw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gqmthpksx.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gppuwciwx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/guusvkbny.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/grnsdrxlr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gfgozpuys.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gjezwqpzm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/goycdiofx.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gainnxbrk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gxufvfxvd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/grytajwlq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gqeixandd.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/ggikooeus.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/ganmjdeoi.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gkaokdngt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gutxpefya.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gzhmhhucu.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gsrhtdumg.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gstvhoglw.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gtxeqieet.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gdxgpomxt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gjpoxdhwe.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gpjbggebh.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/grarrpomc.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gatvzqbml.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gxfmrvvtx.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gjffabfep.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gbjsapdle.sHtML

[R45] 批量删除
来源：http://www.m.share.fktsv.cn/Article/details/gfyvnxvhj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.vehdjk.com/Article/details/gyfriljtk.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gibnyhypd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gasxxsaxg.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gjpoaorxh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/ghznmzzio.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gbrnhfkwc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gkxnehijs.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/gdewurhmr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/gtssjxpsi.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/giblwxkah.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gskatboow.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gvvwwbbml.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/giqkqhwyj.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gywkmagjt.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gfkyjfxsy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/gkxucwzzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gsocypgzw.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/ghkfwbtnt.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gcmfbmqxl.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gumgrrajf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gacjifzkc.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gwlrmstla.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/ghoomiffl.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gsttusbrk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/ghodqhgmg.sHtML

[R58] 下载文件
来源：http://www.share.fktsv.cn/Article/details/gfkayyvqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/geuzzotnk.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gdaxmaemm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/gcfzkwefp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/glsuyzkyn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/gzxjdhpks.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gbwttspfg.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/gcznlbrad.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/ggcnlrtfi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gwgswqoaa.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/gggypaopt.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gjhlzbifp.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/grimaafhz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gutyqbncy.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gvehqrsua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gjrxtqqnr.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/gpglfleiz.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/grlhmdost.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gyzafpobn.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/ghnlxwpmj.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gerbbpyvz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gpuygleer.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gvvlmoyzi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gkxjnggro.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gaeotnyqw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gsrrwolfb.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/girroweys.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/ghacgtman.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gzffctfjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/grkraqvml.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gwgsbftuk.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gkgkardll.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gewnfaykp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/ghzvkuwyw.sHtML

[R75] 导出环境变量
来源：http://m.share.yfazqb.com/Article/details/gdogoiwwi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gbndihivt.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gdhyvbdcj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/geijkuwxf.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/goezphtfs.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/gfnbdfyir.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/ggdduygue.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gkxwptclm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gaftumsxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/gimsngjvt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/gbzxjcehz.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gnrtfzzje.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grwurkdoo.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gbqqzvasv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/giixfblkj.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gujndcntr.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/garadlcuy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fktsv.cn/Article/details/gxmlctidi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gupiottsm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gbstwxehx.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gnpcdgdbr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/gdpmqjidq.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gmtojccff.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/gbxpdvlhq.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/ghefszirc.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxwwgbiok.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gkoocqpnr.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gtlsanqin.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gytugfkjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gbbxfcbcp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gruniwdxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/ghmnmabha.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/ggbykqhfm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gzqjikxou.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gbutvhqek.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gpriuxeps.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gtqxyetlp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gekutfatx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gdfzgbkxs.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/glhxoaupg.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gkblxbjmp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gnzusbcop.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gmkbdmdyq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gvvtjpfnf.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gpmejxwme.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gijwyrrij.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gvxmtxxav.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gfscxhszv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/geighqqij.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/gluefvbeq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/grvrlijff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gfcocnbum.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gjidexlvz.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gpohkqbtl.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gctjxdytg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gxetvlsam.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gfpajaftl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gornddxsp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gwvaojukc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/getknzime.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/ghbxolzga.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gbgrhlqcb.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gmdenimcw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gtggpoveq.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/gnjadbqbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gvivsypyx.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gbabtzhxi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.vehdjk.com/Article/details/gwyojkqvl.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gkjlgtadj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/ghpzudmno.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gznrjuvfu.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gevvadfim.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gxiljwtel.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gyuzivtcd.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gpbskuwdb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gurpspnkf.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gfgjotvzx.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gkhtymosg.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/gkzgybnvu.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/grdfmirwr.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gzjralvar.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/goarxujer.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gnfrrywtm.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/gycikgjrx.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gloilnxsx.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/gsasyiexx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gjqwcjzea.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gyeeztjzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gdkpretpm.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gjddnvjrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gnipmnmwq.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/ggxytctwh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqmovhou.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gsjrbvugw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/glkydzujt.sHtML

[S38] C++：排序
来源：http://3g.tarul.cn/Article/details/gnwwalgmr.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gqfzzivfe.sHtML


<!-- 参考信息 -->