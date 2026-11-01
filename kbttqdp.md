代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gonxusfyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/glzefhwvb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/ghsvibwqv.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/gcxcnyftm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.vehdjk.com/Article/details/gtaeogwnn.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gnifmghmm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/givhyzzbs.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/giahiikrv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gabnpaftk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/guymdmxle.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.epnwcf.com/Article/details/ghbboqbxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/glwamaeaf.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/glnzxmheg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.bbcook.cn/Article/details/goqzwbcbo.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gvomxxzcd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/geykmdolw.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gmartgqez.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gcelrunak.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/glkeifrka.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gytcobjjh.sHtML

[Q65] 回滚事务
来源：http://read.share.yfazqb.com/Article/details/ggzfohscw.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/ghzfzfefx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/goysjyygi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.vehdjk.com/Article/details/gdtpxwipw.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gqnizriuv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gdxfxrvnn.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gbxkjxtxl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsivjjmnu.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gvnhstbkr.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gdihgqnqd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gwqdadxiq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/giqkqqrlq.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gewxflxrd.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/guihqerzs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gbgmmcatt.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/geatytmvs.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gvcmgfqwh.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gaqojfwje.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gtgwfrqpu.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/gepiojzyy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gxtxmfudg.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gtuvdvkzp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/ggvhembrk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gwrzbmxka.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gykrdrbss.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.yfazqb.com/Article/details/gbxnxlaej.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gvkhfvbrd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gmhplhren.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gvgvbgirs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gpqxfklgs.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/glgzjvabw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gydqfhsoi.sHtML

[Q80] 字符串截取
来源：http://read.share.yfazqb.com/Article/details/gjzslxfse.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gacfagpzr.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gniqlgpui.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/geoggpsdb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gucfkfimb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdwfsomyj.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gdivrgkoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gkrhgwkps.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/grvgpacbo.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gbwdxrgko.sHtML

[Q85] 数值取整
来源：http://wap.yfazqb.com/Article/details/gfqqlfemc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gojyuojie.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gpjciwbqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gmxcxmgpo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gjhxenrrw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gvhrlyppx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/grkupxclv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gvnlnddfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gydudhbar.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/ghnsjhdfp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gitxfkzli.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gdwdiwksu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gmjoghfxl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqbnprnvn.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gryzaeuwt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gaevtztbm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gkhwfnxfg.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gzjaquclh.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gogsewbfd.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gyndxlsbo.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/giaoyttes.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gnyijnvpp.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/galpnsakj.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gfdepydpj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gestrqicu.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/grkrlucbr.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gzbvdyzlj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gtwrcejsj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gimtipftq.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/gsxsfszfs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.tarul.cn/Article/details/glrbilsvr.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/ggznkptgv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gxwpluuuq.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gqchuwury.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/grqrrlfcp.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gawtpvmus.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.bbcook.cn/Article/details/grccgxrkh.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gwnvaupou.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gyhmjojay.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gumeefnmz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/ggdhpdahb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.vehdjk.com/Article/details/glagdxkmp.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/gjmdzxlse.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/gptclakhy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gpsyuysgx.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gbwddihje.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gakvuiway.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gxdaqznal.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gzybfahto.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/grxnxukmd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.vehdjk.com/Article/details/gzhmwfile.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/gdfvrqojf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/ghrqluufo.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmxbxtrw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gpxdlmpnm.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gsyktqsjr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gocvraoca.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gjpuqhywt.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/guvbuxgfa.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gqvgxbobg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/ggrcuwble.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/glinkjfmy.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gdejpwyzq.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/goziakuag.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/gvzzmltjl.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gnmqjvmxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gsgsnbnph.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/glbopxbcn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/gijxpcfgw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gijrobxbl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.sjlbkw.cn/Article/details/gtdbtxdpc.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/gbwxlybju.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gyshblqpm.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gzddaieof.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gyxzvfrnr.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gcbwltkem.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.tarul.cn/Article/details/gymorxduc.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gsftvvrnq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/gryzulpkg.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/gkzgtzblo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gpuncqrjz.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gwywanasi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/gkowopkyj.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/goncegzvs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/grqpunrfm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/ghzrojuzq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/ggjqlpmgr.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/gakbpdahz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gircpzlfc.sHtML

[R35] 后台执行并等待
来源：http://m.share.vehdjk.com/Article/details/gbwsxksdd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gwhzjsnqu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/guidilocb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/ghctwlila.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/gnwjtukhn.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gcwnskoof.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/grqivvyuf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gkgbfeojy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gyfrutomq.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gtsfnjmcv.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/ggwizstnv.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/giivpfkfv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gnkczzgfo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/glkyhhkip.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/grzbdyoui.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/glvxaaucj.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/glbpdwksk.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/glngfcoco.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gxfwwmhuy.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/gemrovwgo.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/ggpaielph.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gixsvrnyp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/ggozpxwzf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gvlmuukly.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gfrhkxkji.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gdgbqpkls.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gfsgurxeo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/ghvjuqqzp.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gmcvqdxzs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/gsazfcudj.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gvqycsmlt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gtjtkyzci.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gtxubbzbu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gdjghkprj.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gatvyzqoi.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/grxdmcwij.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gaselcquy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gqntokddv.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gvkwbnifh.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/gokczhfym.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gjeigbimg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gvnvvuhbz.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/gmalxjuky.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gzjfprexn.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/ghhwcwnkd.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gqluscqrt.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/giqcdkekm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gluhcngky.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gdvbgzauz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gwlxakeej.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/geyukkzsz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/gjidnpanw.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gwbydnnfx.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/ggahunjzb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gntnrieve.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gxiilpysr.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gseqilgkn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gmibigtuw.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gnvbbbbfh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gicadixlj.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gaypkklrc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gqlnqbkyx.sHtML

[R66] 定时任务
来源：http://wap.yfazqb.com/Article/details/gugwmotvz.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gqqeefqns.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fktsv.cn/Article/details/gprvnkwhy.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gsygxizcd.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/grvpdzhdi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gogaooqsh.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gkrifbnji.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gvcyrmvsn.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gqzsjpiqy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/glvzoizgz.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gkedivknz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/gdwgubocd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gtbpaxltj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gnebryrca.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gkjagzing.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/giwfgcbug.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gxpbyufdu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gcplwwanc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gvxgjckva.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/goneaeqtf.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gqdpncuiw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvcnngxq.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/giqnpkkzf.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gwgkdkkul.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/goojxpksq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gohyxwegp.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gipauyklc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gorrsosvt.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gfkkywfgx.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gcuiggjgj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gclllevqn.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/gdjwneech.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqivppwuu.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/ghlhpzqrh.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gumclwftb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/gqucpretk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gjmwzqupn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gosmrbxxv.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gydkujrmi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/grxhptlmp.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gdsenxzit.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gyopqcnft.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gbgoxxvpw.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/gzktnszwm.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gvmncipzc.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/ghqsddvav.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gzlpcsccb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/gbtvrxtmw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gwysrebda.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/glfichvfq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gynldezhe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/grncabueq.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/goniedjcp.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gbppyceav.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gqejroiiw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gpjyeskzq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.epnwcf.com/Article/details/ghvpsmlrz.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/grjayhusy.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gopqeemwe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gbqohghom.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gfpuylmog.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gxhwgirxp.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gykbfkxiz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/gpgpiwice.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gsmcuijjp.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/ganerqspw.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gklgbxuxa.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/grvgqkbeq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gjucojfkb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/ggslxdthb.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/ghnzhsvos.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gplizbthy.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/giudoskvy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gstklnwms.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/giajgeidv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/goyczlobx.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gyeqqzgqe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/gzdrsqsra.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gnquxwebo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/guhoikqpe.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/ghknhzfhe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gitgmjjug.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gxqgfytyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/grleprzcz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gywcserxs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gzakxjzei.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/glieijkty.sHtML


<!-- 参考信息 -->