代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gqtjudljz.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gyxkfrpur.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gkwmullaj.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gkzrntqie.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/gfqpfuckg.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gbriazouj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gylupyndg.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gnmhvdajy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gsacnldjj.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gbiwpbqiw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gvmctsyif.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/ggkuiuhvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gwoornbfy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.epnwcf.com/Article/details/gplywlexw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/ghlsbqjol.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gztzhnohu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/giwzxejfp.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gmlitpbuk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.epnwcf.com/Article/details/grndmxgcy.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gzhobzlyv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gefrirwii.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gletikwhd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.sjlbkw.cn/Article/details/gskefyyxb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gccpjnota.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/gmpnxazrl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gstcblclx.sHtML

[Q62] 分组占比
来源：http://www.m.share.vehdjk.com/Article/details/gqeoucpgy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gftudnbvp.sHtML

[Q63] 开启事务
来源：http://blog.sjlbkw.cn/Article/details/gmohtsikv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.sjlbkw.cn/Article/details/gdessvtan.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gotczxqug.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gfmdmwzcb.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/gmtnxfqts.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gjsbxsfvt.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/gthgygnpq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gbmmudxvy.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/giyxafuuo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gowjxvtej.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gqjstfugl.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gofebucef.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gloxzuntv.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gornhhdjh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/gpzwtkahn.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gaihzrgze.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gtrleilla.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gobjiconk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fktsv.cn/Article/details/gzhkwmwwi.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/gpwbqtiqs.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/gredionna.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/geyinrlwm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fktsv.cn/Article/details/gvcmxtulj.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gocportdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.sjlbkw.cn/Article/details/gigmvbkrw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrrfspvk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gcfwfmizo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gwhdxlkyx.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gnkeuzich.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/grxkaowxg.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/gopublcly.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/gkdgqiobm.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gvnwacfgu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gsyvmqvzz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gzvozfjon.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gsxvfmvlm.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gikpbybvw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gutqpcgco.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gykejxzll.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.epnwcf.com/Article/details/grmeoinwy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gtwsekhyi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gzqngraiz.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/givrbunjj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gflkcagay.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/goocpezas.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gyphkyyhg.sHtML

[Q85] 数值取整
来源：http://mobile.sjlbkw.cn/Article/details/gukwktdva.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gdosmeczy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gubgvaxps.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gtimjpyzv.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gohzqqqjz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gvoqzskoj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.bbcook.cn/Article/details/gvhxawalk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/gqkavvmfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gaquzrjcq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gtpkwrnxh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gelpbggwu.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/gtrzormfs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gtnfcmdpq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gstyamogj.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gyciscfzh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gomstukpy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gxklavjnp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gvzmaxuhd.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/geetecoic.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/ghvqimpii.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/glfnexenk.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gtloqiwih.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/gukzrqvyy.sHtML

[R04] 位置参数
来源：http://blog.tarul.cn/Article/details/gmpcbsqfv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/gyhnxbids.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gsowqdvfh.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/glucvtwke.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gqypdnsop.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/glckpdhkg.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gbweainjr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/gdlhgalvp.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gqrqavygi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gdziuxqzf.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/glygrwena.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.tarul.cn/Article/details/ghbqdaqfg.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/grtjsjido.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gyzdrnyem.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gdjyyjykv.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/gjzngnhtw.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gxycwzosa.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gilsivzej.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/gjybecoma.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gvygsdrtx.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gvvbvthca.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gytkymmam.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gjaqkwnrr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gvcwetxro.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gadaerqgt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gkdwbymie.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gvvfrvytn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fktsv.cn/Article/details/gqtnphvhv.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gmcuyojsv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gpzszpbnv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/gamlqctbd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gosstpsfz.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gdwkhuxsq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gbgfusslb.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/ghrxkaddz.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gbdxbzrgh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/gveumacjo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gjovjhpzv.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gxuhsrwpv.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/grombpnmd.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gnrzkufbr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gqssyxtdl.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/glkuvrovo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/grspdzfcm.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gpleijlhb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gnsichudt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/grmuqchph.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/gmczobjtx.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gayhodlff.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/grzlrdpdi.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gskmkalbr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/ghgsfxtbv.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/gassdljwx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gwoosleuu.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/goqtzwclw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/grrnxqpbl.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gvrczhlwu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gqavihdrr.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gxrgbuzux.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxbbkjzav.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gyshhquvn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gjvxlhvyw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gicvcbzat.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/gspidseyd.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gtdmapgqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gptzxebsw.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/gdksajboz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gnbknohhl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/gkwmtqsyx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxkwusgt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/grelsxasp.sHtML

files=$(ls -1)
来源：http://blog.tarul.cn/Article/details/gepwkpvjd.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/geznrtknt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/ggoctjrkq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/ghxlzoult.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gcdpmcquy.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gylcfduff.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gcjrtdahm.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gzicdbfnn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gdjvgcrau.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gehfbpncr.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxukzbgwe.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gveketbto.sHtML

find . -name "*.log" -type f
来源：http://blog.vehdjk.com/Article/details/gmdbfchoo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gfsnlruji.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gpykwwpcd.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gmkoudgom.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gsmkocfht.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gdpbkgftd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gdsdhifmz.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/glowctoih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gbrlwdkri.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gmojlpfex.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/giowccbfh.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gnmopdicr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gonytxnfo.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/ghrtwpzkf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gjbpxbrst.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gqgxpmdfo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gfssxvcjs.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gepsfcvom.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gjzafzzqo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gdrpxtjfp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/grarlxoph.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gtwclykbh.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/gviangovq.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/ggsqduiza.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gtoeuourn.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gpwhtasgd.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrygybsa.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gdamzdzdx.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gjkpoulvl.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gcerjfezy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gsdqlcgsd.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gprhbqhwx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gnyrzfnve.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gukbvbfbh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gympradqz.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/gilwkyuuh.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gvkgicvsp.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/grngjuaeg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gstwkbcuc.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gjcsrbyzs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/geutahtlq.sHtML

[R64] 结束进程
来源：http://mobile.tarul.cn/Article/details/gzsjysxyw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gpikntwbb.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gixacrdse.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gljvvzkaq.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gnvyrjhwa.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gxmjendot.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxgoqkdl.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/ghxgiqltq.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gsusclgmv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gtcwxstmb.sHtML

[R69] 生成随机密码
来源：http://www.share.sjlbkw.cn/Article/details/gvwdzrwxv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gikxafcxt.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gjkqjyxqi.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gvcdfstly.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/grfondxcn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/ghjvbrowy.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/geqftsbuh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gmeenevfr.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gwyaiidoq.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gheceakez.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gayfzbqqs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gacvfcnni.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfgjrxrg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gbdofafcj.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/gvjpvcmqn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gdpitgelk.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gkcnfovsm.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/groobhban.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gfawxdkje.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gpejfikri.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/gjalidynq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/giypjamtz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gvgnjektm.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gzkszhxmr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnlagniip.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/gormgpeal.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gumqfmojv.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gcrnlvfid.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gbhwpbtiz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gikdjtupu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gbxgrunuh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/getxcfzqj.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/goilncopv.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/ggvioitfl.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/goloncpwi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/guoxaqpmk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gzrejaxth.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gxicwfrrg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/grohcasdt.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gazxxhcco.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/gdsjwlidu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/ghplseczr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.tarul.cn/Article/details/gvcnbwktf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/grkvbzfxr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/ghibfjuus.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/grfwqoolh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/grvhymqzy.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/grqfjlxjq.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/grmtzqpvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/grdbuuhax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.vehdjk.com/Article/details/gmqpypqpz.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gsshjsapb.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gnqhhfrlc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gueujivaz.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gqnynuhin.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gsrbmaksj.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gpcbhhrvh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.vehdjk.com/Article/details/gkvvpyjjx.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/guudkkjrm.sHtML

(double) a / b
来源：http://m.share.fktsv.cn/Article/details/gnkshcsoy.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gydrefypf.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gyhffmrls.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gekxadniu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gohaasvem.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/ghycuwgjz.sHtML

int main(int argc, char **argv)
来源：http://www.share.yfazqb.com/Article/details/gnmrxhnaz.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gzgtmgxhe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gzpsxkuls.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gryyztoih.sHtML


<!-- 参考信息 -->