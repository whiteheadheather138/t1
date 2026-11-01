代发 wailian999

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gcccuyejp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.yfazqb.com/Article/details/gqjxcoqrs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.sjlbkw.cn/Article/details/gijvbmkim.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gezkxajwv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gddvujzdw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/goelhiqhl.sHtML

[Q47] 与平均值比较
来源：http://3g.sjlbkw.cn/Article/details/gkrojesxs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gsqdkbycs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gvkngcicy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/gwvolzqze.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gqeftyiwj.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gbsjxlepo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gtavajpgh.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/grdgbjkod.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gwtqomuud.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/ggrabtsao.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gmnfmakes.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gvomkgact.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gbtbbmqwz.sHtML

[Q53] 按条件删除
来源：http://baike.bbcook.cn/Article/details/ghhgkzdvm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gzqnquivo.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/gkgbsvdor.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fktsv.cn/Article/details/gupouctyp.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gjpfeiuic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/gdjhbaryq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gqvbwcnve.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gisqpnwdm.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gsodpjjiw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/ghcojqesq.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gejzffmgr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gylxfpzjh.sHtML

[Q59] 分组内累计
来源：http://mobile.bbcook.cn/Article/details/gxnpeulhk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gcxujaiap.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gcbuyuare.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gpzggaojb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/ghdkujalt.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gizgljcpg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/giumaeknh.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gcfcslhgy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/govhgcwns.sHtML

[Q63] 开启事务
来源：http://www.m.share.sjlbkw.cn/Article/details/guxihcmqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/glugobstf.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/gpwlgiuxv.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gedixxwgb.sHtML

[Q65] 回滚事务
来源：http://m.share.fktsv.cn/Article/details/gfamdnaor.sHtML

ROLLBACK;
来源：http://www.blog.sjlbkw.cn/Article/details/ggxenpbbo.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gcnhwwrjs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gnlaweudb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gptfrbydo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/gwahaoaop.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/ghyqwjjqm.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gvspovugx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gusxoflst.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/gzedpsgxe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gsfcwxorx.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/gsqcnwzvf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gtmuyrdmt.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/gjiaukvyy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gejrgcprt.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gcnmadsdv.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gzsrrzkhn.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gkaguofis.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gbdouijsr.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gkxbintmh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/ggihoinkf.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/ggfkhapom.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/ggipozglw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/grzfatyae.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gazcspnff.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/grehmchxf.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/gxrtqrxua.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gtljohyjn.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gnsukhdvh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.bbcook.cn/Article/details/gezhttmfc.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gprmkzltx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/grnwhjkdi.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/gmymdrali.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ggqpwjieo.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/goeblkukc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfgkcpxsu.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gsdpjzwlq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gulcrpqeo.sHtML

[Q83] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwqqxqar.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gtjbjqkgd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gxxguhgyi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gcdsmfjhq.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gtktpjoim.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gzutfhiim.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gfmaqujoj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gdydzubhp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.sjlbkw.cn/Article/details/gzyedjqrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gzvoroquk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/gaehjedio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gbnbzfuyr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwehvfkol.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gxkcptztb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gflwqglkk.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gdtjsdsji.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gycmbqpng.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsnxdkfdl.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gsdgcdeyw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtkfylldq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/glkhieyzr.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gwpgryzli.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gbpblpkzp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gimdjozhv.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/gblwqrrcg.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/grpdcspew.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gugwkzfub.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/grzsqomrr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gldpwtvfz.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gwsrllmju.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gyujvrjsq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gkrnpyili.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gcewppwxo.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gdqmrtrmc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.yfazqb.com/Article/details/gosgwofqi.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/gcbcekozd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gtiecgnoj.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gqxvkmovx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gblcsholc.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gjnkjwzzd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gwsilvdhs.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcheubcd.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gkdbpqqxu.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gsnefipwj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gzzhcmnbu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gkmbkqbtl.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/garonpcuz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/grryxoass.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gntdcuuip.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gdivrwkea.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gylhhiygn.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/grhcyodpp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gntvmjrbe.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gimehfyes.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gbdrqckdl.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gnaqzftmb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gwmbfugxc.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gdcdkpjxa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/ggdyrclss.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gdojrryka.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gpoxbncaw.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/grxofbwlh.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gzfajfgty.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/gewjyohfv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fktsv.cn/Article/details/gncdlddlf.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gyxkmgqje.sHtML

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhshnfqz.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gxyeiocvh.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gkgscptjh.sHtML

[R23] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gqoczdefp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gzvcpyise.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/ghsteklzj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gedrdfgyn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gulpajoiv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gyclontzc.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/gbafelexf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gpmqwxezs.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gopbzyrxp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/gbakrydda.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gdyjfxjnd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gbhbauzwe.sHtML

[R29] 定义函数
来源：http://m.share.tarul.cn/Article/details/gnpejpifj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/ggnpgwekp.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/ghsrodqeu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.sjlbkw.cn/Article/details/gbrxggsfz.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/gjxzffpkq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gtqehklri.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gzjeukbco.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/ggihjzfan.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gchscqwkn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gknbwcpab.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gpetrxvzt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gamkraqqc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gbuvvfcqn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/gwqvclanj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gbezqpsnq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.vehdjk.com/Article/details/glmmoszim.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gvjxxnxub.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/guypwwibm.sHtML

[R38] 管道串联
来源：http://mobile.vehdjk.com/Article/details/ggateulor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gzrixjmfd.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gttdiyeii.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gginvdrxe.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gypcfjjjw.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/gmjbadmwo.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gdeqaprvz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gsgtsdpzu.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gfhuctpus.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gzlfkngik.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/gsumuqndz.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gvjrmyrsn.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/geykaammf.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/gjmpsazoh.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gnecqxdis.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/geiuxvwbv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gdlvrqzvc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gvtgkjwpn.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/glxcrknpw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gpzxldiav.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gvtkdsfnq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gkfueuhok.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/glscahkgu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gnxlxnnsv.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/gjyrldyby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gbxapovnh.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gmoeichba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gqlwctavg.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gnkyxkzid.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gtrgqtiun.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gmlavtyhk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/gudhkvijv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gycjvxmue.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/ghrthubdb.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gvrxuveia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/ghfumlcnk.sHtML

[R56] 远程拷贝
来源：http://wap.sjlbkw.cn/Article/details/gnwiaxibd.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gahtxmqkv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gybyzwszm.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gsjrkbxib.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gddbvyerl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/gtidxkpsa.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gvbghxgoo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gsqidaesu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gehfnscic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gdufjhnrw.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gnmyvwtcw.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gwbjyvkzf.sHtML

[R62] 找最占空间的文件
来源：http://m.share.yfazqb.com/Article/details/gfiwthtnu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gzaihcoqe.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gtxkbewci.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gtiqxrpuf.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gbtaiymoq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbmvihtp.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gxyahskkv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/glnbmqofh.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gpxzitkqm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gwysysjof.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gqojkhdfu.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gwflqmvfr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/ggxwnakwp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/gpqsvapem.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/ghzrfuqxd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/guytkdkex.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/gdbldifix.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gphpjjkyx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gdjyverqc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gnjheceuc.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gabwhlfcq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gtxajvomh.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gianfehge.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/guilpxlqh.sHtML

[R74] 批量重命名
来源：http://baike.yfazqb.com/Article/details/grxedhewx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/ghzreupdg.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gtdcnlybn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/ggfnhhihi.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/glwibezis.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/guiigkogp.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/grfgfrxho.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gepldycqj.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gixnvmzcs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gumsuicnk.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gplunzezp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gfsusknvl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/ghkjvnmma.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gofdbflye.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqdfitzjb.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gorhrhhrq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqkiutwmy.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gbjlojaol.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfpinqns.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gfrmniulk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gsydjjwbe.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/ghrpljbud.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/ghecnadts.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gmbfpikdl.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gzwnpxjeb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gbtnmisic.sHtML

[S05] C：字符串长度
来源：http://www.share.fktsv.cn/Article/details/gmozearmd.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gbvqvjkwb.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gczbuwlvp.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gprxdxewh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gvrbyzwml.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gguxslqvf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gmstlmcpj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/grvibprut.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/ggfbmxmyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gqpclpqvy.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gttmzkduq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/gpvjhnoin.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gzwpthtwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gvzivljuv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gckjqifmv.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gpvecpncy.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gdxdzrbwt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gqvagkbkp.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/glxltoegn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gpxnzhrmn.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gnqzoqidf.sHtML


<!-- 参考信息 -->