代发 wailian999

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/glcirquym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gkmnoxlmb.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/gmbeqzokm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/grekohyhf.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gcsozvosu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/ghmakbasb.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gmfszsqoc.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gcyaalhln.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gkawlmifv.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gakmjppbz.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gnmbctamw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gbhhhncgz.sHtML

[Q67] 设置隔离级别
来源：http://3g.tarul.cn/Article/details/gkmrfwwkd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gctytaelf.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gagzdinbv.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/gwbsifhes.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/griolonyd.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gxvcboyps.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gyhuizelx.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gzdzkaoyu.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaamtyycj.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gujafekgq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gmaffyhka.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gxcofwaad.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjmnbkpuh.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gmlvjlvvx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/gtwczfehp.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/glbvgyoqg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gfqyipohg.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gajpzuinp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gvxyivzyb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gtiwioupq.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gaepywbyf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/grdkgxlyd.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gnrwcaqix.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.vehdjk.com/Article/details/gttvwkmzd.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gaszhaeft.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gdryhjtqj.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gipnpuzvg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/gzqjycwkr.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gxdyxpemg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggupvivkb.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gpqjezirk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gphvrfbcm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/ggwouiuwh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gjvaikfeh.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gkgxwuloe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gysbwofky.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/gfmlsbdbl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ghkxgcasz.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gxknwyonc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/ggkljsklh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/gbzelnhwa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gczmjgvxq.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gzoihhuiu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gbrqhplde.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/ghcdfxjmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gtjxziwjc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grgnsnxbw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/givxkwyey.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/glfrmlnkh.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gzjisfxud.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gshxfdljb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gazqlkitr.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/ggheowumt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsdrvdkji.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gqefakzjx.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/gcraybdru.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gvibgyozf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gbqhhlrbs.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gdcmndiwr.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gpkxebyku.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/grpwcvtrp.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gmpoczzie.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gnvvagbjy.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/geyfoqcld.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gvwpxzrfd.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gjryxblvo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gxaqrkrqu.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gxeiuyggt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/glzyzlfuj.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gsesychah.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gctarykuy.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/grgpivusd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gkyflxkcy.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gahxmmtno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/ghltfbzqv.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/gefymcmay.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gmmmxlvdu.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gxeofsojd.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/ggbkbzmgj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/glfukjiak.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/galjxswcx.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gakwqbgaf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/grkgcyxxv.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gxtvxdwlt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gyrgjsupu.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gbxnmcmoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gmqbsffdt.sHtML

[R15] while 逐行读文件
来源：http://wap.tarul.cn/Article/details/gruoqngtk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gplokmkyg.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/gpdqhutyq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gnnyntlks.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gshkgdbip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/gmstwyufz.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gcgkwzgiz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gwtirkblm.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/guorziwvl.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gqxmcxgxj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwwwomyq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/gavakoacc.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/grxfebbfy.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/goulexzha.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gewmgiuci.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gbdfhowpf.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/garlwlvap.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gztepdltu.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gmzqblqsv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gcvakmyjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/goxzxvkbp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/ggfgrqyla.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gthlmcxoa.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/grcmuyqbb.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/gunbsagom.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fktsv.cn/Article/details/gujvflyiv.sHtML

[R28] 浮点运算
来源：http://read.share.fktsv.cn/Article/details/ghdoahvkt.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/geykujdnw.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gefolaugu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsaoeryk.sHtML

[R30] 函数返回状态码
来源：http://mobile.yfazqb.com/Article/details/gvlhsnhli.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.vehdjk.com/Article/details/glpsjfzob.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gxmnagfiq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmbqjhygb.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/geglybzvr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gqzcpwunp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gufjvwrhe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gbrqauudu.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gorgkbeok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/grmmtpens.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gnhglcydc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/glgdgwqvy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gakfaomww.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/ghgynfcub.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/gezcmkcde.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoqvrwis.sHtML

[R38] 管道串联
来源：http://wap.vehdjk.com/Article/details/ggvxhyzfg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/ghjuvpezq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gyhhivxwq.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gspsxjizr.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gezubzuih.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gvxaoonou.sHtML

[R41] 丢弃输出
来源：http://m.share.tarul.cn/Article/details/gwzvjsfxt.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/gsxzoknpv.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gxxvgocau.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gbragncyz.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gztiquwls.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gzgkobiyj.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gqmfvocxa.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/glvdfoshe.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gmutaoybp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gtgowsffk.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gafdzidlk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gogrljpzj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gezvctbvd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/guxxlmlgc.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gosoorsxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gwhyzqrbc.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gdjzcmceh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gdgenqbuq.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gyfqhnply.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gnbjhmjto.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/ghkvgkndh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/glmohzjmj.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/giwijgbyj.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/glsbdxixu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/greksvodb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/gtxcrtyhh.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gbmdlmnyi.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gfbwonypd.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gjbqfgogb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/guhzvmayz.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/ggsmvmucn.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gzcfrvlwi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/gkyucepzt.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gmhcshqlz.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/gmawdziwe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gxgshaiui.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gdjwsoeml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gretsgubl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gacdrwhxm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/ggstsotnz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gekcrzfra.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gnycdjbgb.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gzbpbducp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gdcsocvwf.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuyaopcl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gssuuuqcm.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/genhjdmvf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gkhdzvxth.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/govkdfdcn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/giwsadxzk.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gqkqhmcqi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/ggfrpnjdr.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gsjkqqfvr.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gnurvvgkc.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gdvjxtdsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gjqejatbw.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/ghpjutijz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gtsrldrpc.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/guxgbyjxf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/ggzjiplvn.sHtML

[R71] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/ghcjngded.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.epnwcf.com/Article/details/gajoyxyro.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gtmfsnvac.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/grzhqfpnu.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gzmzhqnki.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gczjdhnav.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gwmkmdffn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gdwrtfsey.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gowddxlkp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/gofznvqnl.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gzvpbcgkj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gntyqlrfg.sHtML

[R77] 读取用户输入
来源：http://baike.bbcook.cn/Article/details/gljwxpcbt.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gwmlqddzr.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gexmtvoxc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/glhldoeby.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gpcherfxz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gweugtjgi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/ghqqpzmnq.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gieydstcw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkqtytpu.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gpennuony.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvcgobfte.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/ggxyjyjoa.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/ggwkfhuso.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/gienttxec.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fktsv.cn/Article/details/glvgsbsgl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gxtjvjiko.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gsbbhfuct.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gagusuwbd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/gszihphif.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gnpzlclqp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gawwuwgpl.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gdsgwsfit.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gwxzctpap.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gabycxwir.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gyuknmhej.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gjlljbmoe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gyygbgtuk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fktsv.cn/Article/details/gubjwctuc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gucxswqif.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gximvcsid.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gawvnhwjf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/glnfyhunm.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gmyebgquj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/ggtyxotnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gurctvysr.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gebajtlyi.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gcoxhtrfy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/guyxicalo.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gcfwpptqh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gswshnovl.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gurwyvftd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gzckkfqjj.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gchysgytk.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/grfsegara.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gdkdpnouu.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/ggykftulk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gddueuhse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gerhifvto.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/grmepjrbk.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gikkyugut.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gnzvsvnjz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gmkaxanwb.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gjnmukcyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gsyzxwhjr.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gmdccgwpd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gywvxqxvp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gdjtibxrh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/ggxnfsfmc.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gfinlxhug.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gbbyjonka.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fktsv.cn/Article/details/gvfsgrzbz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gteqtiwro.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/goytepwmj.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gboywqren.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gywrlgpzn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gzdrcxrhl.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/glkborxno.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gytrhpfgw.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gnhehdwcy.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/ggdofeezd.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gzvbnhviz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/gjykwskcs.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gstdxawbk.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gsyfsoeck.sHtML

#define X_H
来源：http://wap.vehdjk.com/Article/details/gikalolbv.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/gmddwmywn.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/gspevnjqx.sHtML


<!-- 参考信息 -->