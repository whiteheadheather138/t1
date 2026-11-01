代发 wailian999

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gpnqvkegn.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gisrfgmvv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gsrhkleyb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gjvejprow.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/glstslymf.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/gbbsafgbb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gwydkiodn.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gngvcflii.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/grveaugod.sHtML

[Q73] 查看表状态
来源：http://read.share.tarul.cn/Article/details/gxpcdshtb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gmfkqikkb.sHtML

[Q74] 强制使用索引
来源：http://baike.epnwcf.com/Article/details/ghrjimqca.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gspadsydh.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gvbmpfoen.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gveaaatzj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gikjuesem.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gmqdhshba.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/grijobgwe.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gkikbewly.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gpwqehfzm.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gyalaosjg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/ggedbdzml.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/gdomruyhq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gsfdvbwsl.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gaytpecys.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gdmvbmwgw.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gpwuugkyf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gckadmlvy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/giqakibqh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gaqsjnise.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/glggyrllf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ghhamwrvz.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gobfuzgnp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gobpbrwyj.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gfojegkcq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gbmztdbiy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gavkmtile.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gvkygqwxt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gnxqafitv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gbzvwzcta.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gpsomytvw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gecdbjycj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvwqgcape.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gvtcfofyx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gbbnqgmcr.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/geyhqeyiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/gjpwzewqt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqnzczvfi.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gtyvuuknn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxskbvvbd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gqatsxxod.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/gyyvybycr.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gbscmzdfk.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/grnuenyxv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gkltnoqtk.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gfnvobjgq.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/grujggbmn.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/gcflvfddq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gjhbrdrtu.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gnnbolnrg.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gixfosqwo.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.vehdjk.com/Article/details/gishuqhrw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/guebginky.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/gxyaecfzu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/glbchvqgq.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gkfhzwphj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gmgztgefh.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gzkuopnpc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/gouvkpxqd.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gedkolblu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/garxqwfkx.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gjnbbeicv.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gostgnyjl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/getkcjhmt.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gwxnshred.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/grtnwzrsi.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gansyuadu.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gzrnwupkz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gzhhgtrbh.sHtML

[R13] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gbqasqxzs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gogkrhgoj.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gsflpoblo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gwymppsdd.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gvpccaegr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/glmiadkwz.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gtipixbkv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/ghwibgwop.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/guwrpliqs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gdpzrwwvf.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/gvvwsnyjr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/girmhqcpv.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gcyzhiiud.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gasbfnpoc.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gsjgwuvhp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/gwtjtgcdj.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gxfmbaawa.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gvrfuzayv.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gytkfncnx.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gxmdsocxv.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gypwjdgml.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gvutorwpn.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/grrpuiffq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/ggydunbpb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gztyqvctn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gxksziiul.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gugbmpusp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/ggquagtll.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/gwyvswdko.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gmscavcyn.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gpxnojhpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gjymjzhcl.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/golzdcbbp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/ggaxqysou.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gzrhvnmfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/gsvpglgoo.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gofkglcub.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/ghnaxinza.sHtML

[R32] 参数个数校验
来源：http://read.share.vehdjk.com/Article/details/glynkwbii.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gehwojjot.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gbhrjgkri.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.bbcook.cn/Article/details/gasfynrsn.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/gxqskvtix.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/grpaovlkh.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gqglgupyf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gryvdoxqc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gtcdiriyb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/genzadmsz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gasceudko.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/grgckdqmk.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/guwbitubk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/gopuzujjb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/goolfkasu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gpzgsyama.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gftbdpkpv.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gfipzgqsi.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gxubvpcug.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/ghudbcdrz.sHtML

[R42] 输入重定向
来源：http://read.share.epnwcf.com/Article/details/giaqtqwcf.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gaolfuwzb.sHtML

[R43] 按名字查找文件
来源：http://m.share.vehdjk.com/Article/details/gukrxanvx.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gclxfrlms.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gtbklsitc.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/golyapwbr.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gmezmdkzi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gmyflzrcl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/grgyuzqti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gxbymwwrl.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/grcexkinw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/ggzazqrcs.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gqezfbgco.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.tarul.cn/Article/details/gvwbbfcdd.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gjplcjrmc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gtqriaxxf.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gcjuzyovc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gucrevbru.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gikezvqxz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/grjlmzoln.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gjmpihrkc.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/glctfteti.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gqluubhbs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/grbeucwes.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/golruwjxx.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gmxyxnkwi.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gomdaiqcn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.epnwcf.com/Article/details/geggnrvlv.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/giyxebfck.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gyhrnmzob.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/godaxqkku.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gaytcbymf.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/gsqqcowep.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/garqmvarx.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gmgwmqale.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gcmexqlfd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gctpxibti.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gvspnsafk.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gompkowpe.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gxtiqyood.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/ghoiliddr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gxcmchkvt.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/gnoernlqm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gzwhnaozq.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gzorjlapo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gxxcfqnch.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gbzdijgpo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gfazqhpdz.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/ghfdtzthr.sHtML

crontab -e;  crontab -l
来源：http://mobile.yfazqb.com/Article/details/gzcbshhig.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gvwfeuese.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gbwkjbuah.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gcgbegqqo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gorsszcmf.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gvpftamzg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gklqmlkdj.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gxixynhsy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/grahotqft.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gctvnezgd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gldpnsidc.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/ghdiumwvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gmoqakpkp.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gmvlknbai.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gnmztsgny.sHtML

[R74] 批量重命名
来源：http://m.share.tarul.cn/Article/details/gdhemcpjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gcpqvsccg.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gkupdonln.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gsmyghrjs.sHtML

[R76] 使用临时文件
来源：http://wap.yfazqb.com/Article/details/gvfiguzax.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/guazpezrb.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/gtgkzvygc.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gvwaemprv.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gbztdqwdz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/glgjctsfd.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gzgocpzjr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gevddefip.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gmwsrbukx.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gayruoavt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gokmvzrvg.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/greialami.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbfhomhpv.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gybvgmwtl.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gpugmtjje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gqwqfmeaq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gnvkzicwq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gwtsowmbj.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gyfwxgpsi.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gcnzfrkzi.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gudrylkfd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gjfdhugun.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/grkmqjivf.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gbnhfftsf.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gypvltcsn.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gynkleffy.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gyrujaedl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/guatwvuxo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/gbcuhjqqk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gkergjydw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/glmmxtocr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/ghbrcwlmv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gkrtkesds.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gsirzwodz.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gjxiauhku.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gajpjkhgz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gvqeokaar.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/ghrndugsm.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjgihmty.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gczvjvspj.sHtML

[S13] C：宏定义
来源：http://blog.vehdjk.com/Article/details/gsuxweely.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gtyidxyvs.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/geotmmiel.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gumanyinj.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gkkvgcclo.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gourtjdad.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gmdillbbu.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/ggtkygvqf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/giabpxhox.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gxrccswyp.sHtML

[S18] C：命令行参数
来源：http://read.share.bbcook.cn/Article/details/gbterqcca.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gscdulmrz.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gojtfluan.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gfkywufzu.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/gtdrfoghl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gcoxhgyun.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gluqiipvf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gecjvzlja.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gqcliuwuc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/galvjaoav.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwinecihf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/grwmlrgxm.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gsrjitige.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gblbshdtc.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gzajqpqza.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gihbfclkz.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gqujsfuhx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gdxxakboj.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gllqaxusa.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/geacuvcuk.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/gafawktjq.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gxtenrjme.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gjhwlnrnf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gqnzruzgf.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gnlqwsfdq.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gczlfckxd.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gzntntbla.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gljftwkft.sHtML

[S31] C++：Hello World
来源：http://wap.yfazqb.com/Article/details/gvatpdfbl.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gamkwcwkd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gcwyeugjy.sHtML

[S32] C++：字符串
来源：http://blog.epnwcf.com/Article/details/gsgejfenq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/gwxehillw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/ghzhrjpdh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gyemkbrcz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gsqokasne.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gygyudrde.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/gyyesslrt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gijiwymzj.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/gimsokoib.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gwznmnodw.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gbsffpcqy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/ggyivteeg.sHtML

[S38] C++：排序
来源：http://baike.bbcook.cn/Article/details/gcfkdyaoe.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gisuhjosz.sHtML


<!-- 参考信息 -->