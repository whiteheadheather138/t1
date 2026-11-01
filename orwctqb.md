代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gyuvgxxkk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.tarul.cn/Article/details/gotamcbzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gddqfpwdc.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gknvrsehb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/ggmifexvu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/ghicimdrw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/ghddkxzix.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gxxogwide.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gvsfeeypm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/ghfxbjorh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.tarul.cn/Article/details/gbvoplcjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gmrolcqra.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gtzzcqgnh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/glsxctuhg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gjimuzpkd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/groprqrud.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gqgamgfyi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gjowvrrjq.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/glsifpkwe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/geiqigzah.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gjuyopdhc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gphsasoud.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gkjlgobzj.sHtML

[Q49] 更新单行
来源：http://blog.vehdjk.com/Article/details/gkycmriee.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gygzcfnad.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gsgvrxqft.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gujaxaolk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.tarul.cn/Article/details/glthqhgdr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gmtluvfti.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gzumzgvuo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gnletxefp.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/guqpqnrkf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/giocvvxwm.sHtML

[Q54] 清空表
来源：http://baike.fktsv.cn/Article/details/gdlghvxsz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gzahdhgbg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gktmnihsn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gobowrdjk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/gmubhqykq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/grjctddga.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gmsgwabec.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ghsggnekp.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gajyyghbi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gihebumhb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gmdihobqj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/georsfbie.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gnbualhhz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gelnedumk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gaujnixxi.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/gbxkessqm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gonoaofkv.sHtML

[Q62] 分组占比
来源：http://www.m.share.vehdjk.com/Article/details/ggibbcwlm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gnhiigvio.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/gcqkedwkk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gjiengxnd.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gscwfgpwo.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gripqpazz.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gckpccobz.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gkrnuskym.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gqyjzdblz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/ghsbbotka.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gthmwalet.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gijwkaewl.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbtuxjpi.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/gcnoqjfgr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/ggwoygthi.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gevwywpnv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gbskmpkrr.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gdzyeipro.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/gjzudmumt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gfgahibad.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gatltffjs.sHtML

[Q72] 查看索引
来源：http://baike.sjlbkw.cn/Article/details/gkbrzoidl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gqbhxzpoh.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gcthggoba.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/guotpyzii.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gzxuhqnqn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gabitywrb.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gfokuqdiq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.bbcook.cn/Article/details/golnjufal.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gnjzwddxz.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gbsodnfwr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/guczqmaog.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gzvzprmvq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/ghqerilhh.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/guedtyese.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/ghqpiizbv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gwragpqgh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gxmjeexwc.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gcnbmhgzd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gbsbvpkby.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gdrmohwyz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/gcfcczagw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/glcwonpzt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gegydxwke.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gknohbbzu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/geellztzi.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gmzfcmrqu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gazztyesn.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gqllxfhuf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gzibwmsgc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/goaipmiox.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gviofgmtw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/gfwowyrai.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gzoeprapw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gwpzdxzyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gvggwssdq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/grdtnzhwo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.bbcook.cn/Article/details/glsoqvzwm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gufbekkru.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gmppxfqud.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/grjhkhzbf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guumdlnjn.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/ghtqqamre.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkukijxuz.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gisujumeh.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/goggimdjz.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gdwbahvcf.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gceeojboj.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gfwnujnfa.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gtuykpyxy.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gbykwhzaw.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gwrlablos.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.tarul.cn/Article/details/gubcbpuvw.sHtML

[R05] 参数默认值
来源：http://www.share.fktsv.cn/Article/details/guusefqcy.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/geefapdnp.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/ggwocmptz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gztxqmiou.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/gppnmhbcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/grqklqhgb.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gonpawzlq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gssrwtxgs.sHtML

[R09] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gpvewsqtv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/ggxtattfw.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gxghttozf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gprxuadtq.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gqgmjzozo.sHtML

case "$1" in
来源：http://www.blog.bbcook.cn/Article/details/gakhvemox.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gqozwrgzb.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gfhnowbzs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/ghblhzbpc.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gdspgewtt.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gcuhaniil.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gkecrfwgk.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gnogqkfwr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gyhjofled.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/gvzyvitcr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gherktgqs.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gdzgssyka.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.vehdjk.com/Article/details/gddlrxnpi.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/ggemmwhqx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gkevkwama.sHtML

[R17] 数组定义与取值
来源：http://wap.epnwcf.com/Article/details/gwrapttet.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gorzspxko.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/geniklnhi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gzjopicax.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gzdndmtdh.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/ggtjwgpcc.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gdmfyajep.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gdgrhouyk.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gignkdhhq.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gospmykjt.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gputlvxry.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/grcshiwbx.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gicypjida.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gfmbctrss.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gmuiqkqtj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.vehdjk.com/Article/details/genspvywy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gijhckmys.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gagysaqdb.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gqqfqsfbb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gpcxkrhia.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gqggnwwoa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gwjlzqpxw.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/geulunyof.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gykmgcdqm.sHtML

[R29] 定义函数
来源：http://3g.tarul.cn/Article/details/gbbraqssr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/gsvplqgkj.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gjzapjzdq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gvslbbywh.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gtulirvqf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gtblzlqbq.sHtML

[R32] 参数个数校验
来源：http://blog.bbcook.cn/Article/details/guajfmple.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/ggvwvrrjn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gmplhcqxt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gjbkgvtkh.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/gxhsvebxi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/ghzwpvmvs.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gpqgvsiph.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gopfyszih.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/glvjisiqm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gqlhkhynm.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gmrqeeznr.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gwenfbbyj.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gvjkjtdkz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/geoqktlya.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gwocjtyoe.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gvurfdyrn.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gkntjobrc.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gcoogqwxx.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/geiobckrl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gkpuaizgj.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gkegwxwwr.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gpoqydhmx.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/giuzyrmeu.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gbhgbzaga.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gemjnipkc.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gyczrauir.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gghwvjsfk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gswmuxduo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/ghnofletf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.bbcook.cn/Article/details/gihfymdxo.sHtML

[R47] sed 单行替换
来源：http://www.share.epnwcf.com/Article/details/gzaptijal.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gqbzzhxwq.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gbxecuzqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gjvylgvmg.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gijbjglaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/ggyrzotzt.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/glthkwuhg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gszafpzeh.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gflbzrwuu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gxbodincb.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gmlhttdtq.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gppvmztth.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gdupwjrfr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gyfoyebxu.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gwqkulpzx.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gsxkcqbxz.sHtML

[R55] 压缩与解压
来源：http://read.share.vehdjk.com/Article/details/gdlecgnyr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gxgkyaedl.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/ggeshpazu.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/ggjfjkzwe.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/gytmjnfdz.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gzrtycjvt.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/glxvuehga.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gyolvijtd.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/glhenumwv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.epnwcf.com/Article/details/gxeftjvba.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gfttvgwah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gtknmnwzv.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gyumjwfjf.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gzmmnrfwt.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gzgxptbqz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/ghguoodcz.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/ghvmukzyd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gjywwwwlb.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gmlafuizn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/galutfllg.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gjnrhenda.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gzuxtnafy.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gbhkwpxuu.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gfbdidqbw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gdyoihymb.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gyhshhfbo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/ggagxkwcd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gbtvkwxls.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gtbbcrsgl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/grnklqrlk.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gbnxnvcil.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/ghlsubwij.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gzxoyawlc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gnkzpqgke.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/guosuqood.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/giqntomcj.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/ghoantqfh.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gzqqqgkqb.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gxdxxpovg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gcssmawhg.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/girzgcgzj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gkncfijye.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gcjnlwvow.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gurzyvexf.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gdgstulpv.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/glhtasduc.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gpbygylgq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gwdhqsetp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gbtrcgpgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gqczyidey.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gkziyebdw.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/goqrjrwvw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjmnxxhsb.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gvpdsyupz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmpqdnhoz.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gwvdvvtlm.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gpuqdvnym.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/grksiztvx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gckjhxnmf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/gocokkkvg.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gqpiodblu.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gzfesccup.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gqhcjwnla.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/grvefdhoz.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gixzedpmr.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gcnngshzx.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gegkshxje.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gxgolctuw.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/glzgjytnq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gyptesoui.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/giwuxljga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gijdihmfx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gvpuskabp.sHtML


<!-- 参考信息 -->