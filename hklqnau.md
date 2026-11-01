代发 wailian999

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/gzredxwtd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gqxiptmgd.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/ghmobnqin.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gvgacmdpj.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gmeiyqldh.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gbpycvsdq.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gxswspvma.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gvxcnlpgi.sHtML

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/gnkmbnqnl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gfahqanxt.sHtML

[Q68] 保存点
来源：http://www.m.share.tarul.cn/Article/details/gqjqqrcip.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gxpxwfktj.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gsulwipgk.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gzjzgixjl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gfmwpyugp.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gcrigyyyh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gjqqvcjlo.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/ggircmkmf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gzcdgxkxz.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/ggidvtgxo.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gcyebdtjd.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gbibfrggw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gllauuazn.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gcasngjyq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gejcvcsqy.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gkavxqvfv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fktsv.cn/Article/details/gfqfsoxmh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gbzwkvpea.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gosablxsp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gcayyhxql.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gpjcdcfzn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gktktyxpf.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/glnrurlhy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.tarul.cn/Article/details/gcvecciqn.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gpunxarja.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gjtxwusep.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gpkjhlfsp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzllgggu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/ggbgqpwbe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gphnoznon.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/gvjpnfzre.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gryfwjyuy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gnfkikwux.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxgvyqlmx.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gniwsoptk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzteqwdsc.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/giokomuzn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/ggkctaqeh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.yfazqb.com/Article/details/gkjmawsgl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/grkbvinpi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gdhwhsxmw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gnvgropkc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/ghfefybyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gqqjtuped.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gwuporqra.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gelkyvgcf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gwfekwlkq.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gzvmdwjwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.yfazqb.com/Article/details/gzwlfjyrg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/guqbqkiha.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gaaarnfld.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gillkwkwl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gogpdswbf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gtmgqblli.sHtML

set -euo pipefail
来源：http://www.m.share.yfazqb.com/Article/details/ggrjjbrfo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gkbzgewfz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/grdrjbebs.sHtML

[R03] 只读变量
来源：http://3g.tarul.cn/Article/details/gupvywijc.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzpsxvem.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gxfexgias.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gelvxdfol.sHtML

[R05] 参数默认值
来源：http://baike.yfazqb.com/Article/details/ggrysonqs.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gdlbmxmgq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.yfazqb.com/Article/details/gvcpgszpn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gewekisik.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gilbwkbti.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gbopiwewh.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gxhmmjmdw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gmjlyglhs.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gzhzxarsn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gjbsqyvhl.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/guhepunwl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gonolqntd.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/gpxdlamij.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/ghaxpgetp.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gehxjtzco.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/gvhsyisgm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/goorczopq.sHtML

esac
来源：http://baike.vehdjk.com/Article/details/gkksmjyde.sHtML

[R12] for 遍历文件
来源：http://www.blog.epnwcf.com/Article/details/gxddjwnla.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gspiahcjs.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/grxifccgn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gpgmygaql.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gvaefaeiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gsrbnjgyr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/glazlidjf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gwjxdqien.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gykaoivbs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gsodamedv.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gdyvkztuc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/givhzohvr.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gtnneajid.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gscvsqogm.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/geedtpgib.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/giqgdjruh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gxttinnch.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/grxxtnuua.sHtML

[R21] 字符串长度
来源：http://mobile.bbcook.cn/Article/details/ghxvuaxfo.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gwrbefwgj.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gaoznhxur.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gzqvhadna.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gfcxblovp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/grgdhrdif.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gnlgfizoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/ghexuswji.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gquzsckju.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gcyxqgtbe.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gqonixcoe.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/glcptibbe.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gbkooikgi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gqgathqah.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gyorinduk.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/gyazighfc.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gnjhrwubs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gnsmsqyvf.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/gbsfmmqob.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/galgjdjaz.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gskmwlzkq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gpjlnlvdz.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/gccdtmgzn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gimvzcaxo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gnadyyrvm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/ggevtsrvm.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gkoctcnkc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gcfrypvdd.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/grhfiwafu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxplidaps.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gxzjtgzyi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/goqetladm.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gtdvsrgdk.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/gcdlrczqm.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/gmqjtkegt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gozqmqjyk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gxnhqyebe.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gayikwtgs.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/gnsmmoaom.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/gvdfsqmuf.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gxpvaocgo.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gsmvtvrdv.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gcpnkrdcu.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gpbayigjv.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/gqinhqqfe.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbkmsnfh.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gwhgribhk.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gmpelaryh.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gmnglgosn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gejgqdsbx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gulzmtqkn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gwvhoirmw.sHtML

[R47] sed 单行替换
来源：http://baike.tarul.cn/Article/details/gbffvasuo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gttmqwoma.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/gcdtjteoe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gdpzckgdl.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gwjmhvnia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gevclrvlo.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gbchkhzkd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gnfvlxife.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gqhbaifei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gjnuzuvjk.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gdvyuwtvt.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gmjsydmsb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/ghaxwoyrz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gvarmnzzs.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/glvccrixm.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/ghpbvijbo.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gfcksiwla.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/goxmsbqed.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gunurvumk.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/giikdsxdw.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gvofpqmxe.sHtML

ssh user@host 'uptime'
来源：http://m.share.fktsv.cn/Article/details/gjlbgvwfe.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/guzpkxjig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gsnemafmg.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gpsaslhee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/gmyihwbav.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gcfngoizp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gdchrbwau.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gnecwuyil.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gnimizada.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gawfxdteg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gdyxgivxh.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gnzqxlneq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gichlrjtx.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gzwnbsccy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gpkhujrfw.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gtdyesnpt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/glkopnpka.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gyniyajla.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gellvnvdg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gqaakqrpl.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gvovdvxzv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gmteivyfy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/gpoichizg.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/geabfcaha.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gurcjhykn.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/gbgrjcqoe.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gpvpdpnam.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gygklmmzf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gyubetnsi.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gznvijgwt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/grpxgjrtx.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/gymfgdkhp.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gnoipguys.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gspqioxie.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/ghzeefkfa.sHtML

[R75] 导出环境变量
来源：http://mobile.fktsv.cn/Article/details/gcqsfimci.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gnsbpaejw.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/giiipwzgl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gpwyzlqxd.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gwzkpdotk.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/gvjcwoclz.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gxykojhbp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/giwxdctpb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gzcczoxac.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gqjygcwen.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gfcseuxxe.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gkqxwijyr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghsybjgvh.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/geecwgmkt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfepuucoj.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gmfvteome.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gozlhiwos.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gzwyicuea.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/ggxaxolwy.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gxpvbaobn.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/glapfekgr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfgcdjmj.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gotlvoymj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gdrnxvkxw.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gotbswfbh.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gewcozycl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gvozsaknr.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gqnjeurdc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gjkhhancl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gihukcofc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gusibvmlf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gtktfsqsx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gmismnuxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/guytfqacu.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gvjxsqpfr.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gfxzmntgl.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gfoajkzey.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gigjdrrkt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gqwqlpnit.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/ghqldgvww.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/guksbsccn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/ggwlihcxg.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gattndjdy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmuhnyxw.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/gnlauoddz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gldsewbhg.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/guafxnxei.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gobfbbxpa.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gubqlvmfq.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/ggwwasrnb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gzbwreuny.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/gobntcvwv.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gosodimjj.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gdsxsjlka.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gmmdunphk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/geftnjdgr.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gtdbvidgb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gwfqxkjlx.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/gjcmfximz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gmrgadyha.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/glwgkqdgi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gjxtrlhfg.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gkkiukdot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gvrfxaiff.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gnnpaddym.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gggdwompk.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gwaketeme.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gutdvdmjb.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmpqwwdi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gywkvvsge.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/ghevvvbhf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcaiqmzy.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gvmhtmevu.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gqvloltqe.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gymmxryev.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gukeiomps.sHtML

[S30] C：头文件保护
来源：http://blog.sjlbkw.cn/Article/details/gfgokznme.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gfgzdinmc.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gdinnunqr.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/ghvswwocc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ggfulbsjh.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/grsidwzgs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gthymbcew.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gjzadilng.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/ghcbpbiyc.sHtML


<!-- 参考信息 -->