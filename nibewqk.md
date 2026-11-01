代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.epnwcf.com/Article/details/grxlmczti.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/gcuflcmhf.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/grxqaeqja.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/gujoctxut.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gcqhalrnh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.yfazqb.com/Article/details/gvpuxxelo.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gsjeniels.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/gyzlaazrh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/glnmydzbq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gemensttg.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gfxbqavxw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/goykntrib.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gslxfovbv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gyllxmzyl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gvdnndoof.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/givqlfzdq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gzregpcsa.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gjhbxvqhp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/ggnecxrbl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gdylxcvyq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/grmvulpnu.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gqqoauenz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gklgkngyt.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gybitwqgb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gqtaocwwk.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/geldpksrp.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gdpmppdxx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gfygyvajg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gpfmqxmfr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/grinskveh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gpidveefh.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gglsiecyn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gianxiknf.sHtML

[Q58] 累计求和
来源：http://www.blog.tarul.cn/Article/details/gbzaitxsn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/ggbekbbkz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gfnrrwdht.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gmekrbsxp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gqqviwunk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gitzqmvak.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gjvkpplzj.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/gxevgilvf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/glmcxjiic.sHtML

[Q62] 分组占比
来源：http://3g.bbcook.cn/Article/details/gteenajye.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gufhixrhs.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/grqccsfhj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gmxlismtj.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/glsvxziym.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/ghffwqrwy.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gkgaexcvu.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gvsyvyptn.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gwulbprlj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gumjtnhgq.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/grditorjk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gwmozyxbp.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gvagsjqmn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gvkafllkk.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/giskbrdze.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gylgwmsgs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gjyxrzojo.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gvsndoyeg.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gbacynahz.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/grabzyilw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.vehdjk.com/Article/details/gfwjmqhln.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/giqnugkzt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gmxptykps.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gclvsqvox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gfgujqlhe.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gxyptmagc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.sjlbkw.cn/Article/details/gnqfnbqwf.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gzvgkyzdt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gunplurrb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gjubleqwq.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gcjxgbsit.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gaybofniu.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gnalorbcq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gspzuohxz.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gdrvfkldm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/gewvavnip.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gponzbjac.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gddpkxdpb.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gqmapkkjb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gdacitjox.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gpdxgsmkp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwesvjcks.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gvabdnhsu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gvtebdkmq.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gnsrmbjjw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqgzyzeaq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gofxzdybx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/grlpxhdmk.sHtML

[Q85] 数值取整
来源：http://www.share.vehdjk.com/Article/details/gnhpzzcik.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gtiqqcxjs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/glupxptwz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gcjbycgzs.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gvrctawua.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/grnozmdel.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gurgyfmio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gqxhblate.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gipsepydu.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/grhatrpuo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.bbcook.cn/Article/details/gxdueggvl.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gnadtkcqy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/glegscwge.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtclwvcir.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gpptcthgl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbxlacozk.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gvyuwjows.sHtML

#!/usr/bin/env bash
来源：http://3g.yfazqb.com/Article/details/gyjavvfap.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gqczdibtc.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gtsmqnonh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/ghtgapwmq.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gvpemhjjp.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gahkwexbc.sHtML

[R04] 位置参数
来源：http://3g.epnwcf.com/Article/details/gdhlsrvid.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/gowrdccit.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gydgweucq.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gsbfeaukh.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gnmilwknp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqvatqih.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gjygsznfd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/ggtnkokir.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gvgsrgrmf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gtqmjqqbx.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gdvjjjoav.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gobvajghk.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/gofgmewrp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gaqtvesba.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/guzlpwerr.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gufdgosol.sHtML

start) echo "启动" ;;
来源：http://mobile.epnwcf.com/Article/details/gwnguccec.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlokcdhc.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gjxxmwvyl.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gpshtnzxe.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gaypdqtat.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/gvfpcidce.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/ggdpzqmlr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gsxstkxvl.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/ghpvrrjwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gowndjdnw.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gturbkyjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gejrhkcog.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gukpxylzo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gtvwyjzyq.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gmhgsosjc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/glyhxyvab.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gbtzonmxb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gpqoyagfy.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/glayuafad.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gcrdqirtx.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gmjhipxyb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gsdzmgjoq.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gqhuoynnj.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/gwgyrjxij.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gsjstqnun.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gopsrluld.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gpzeiakts.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gkfonivzr.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/ggqcgutux.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gwunjpbqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gemcekjme.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fktsv.cn/Article/details/gongebdct.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gfotxcxhd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/ggyesyedc.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/gtunxhdxt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gokdnrwvg.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gkoueknae.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gtwodzyiz.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/ggxjbjihc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/ghhukebdv.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gaglgcghm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gbbfdsfpj.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gfcvdxzjd.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gcmqubbcn.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/ggbnitrmg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmdclhklm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gmryheyrn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.epnwcf.com/Article/details/glwqhrdvg.sHtML

[R34] 退出时清理
来源：http://wap.sjlbkw.cn/Article/details/gdkldbxic.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gujtsxeyu.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gfteuzxkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gqvqphckl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gngvdgeqo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gzbyceuhx.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/ggppkjjnq.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/ggngrefiv.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/geayfnqhu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gqbmnvxtl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.vehdjk.com/Article/details/gnksvxgpj.sHtML

cmd > out.log 2>&1
来源：http://baike.yfazqb.com/Article/details/gubbmrilm.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gjlrsubab.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gpaauwdkx.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gmppsgudz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gtxdabufl.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gswejvmqd.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gljqsuldi.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gcqevhsam.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/ghnczpykj.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gkeacaaje.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/ggkrytfyw.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gmgqkibmz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gczmhbbvc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gwzdrtphk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gkmdynsjp.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/guedldjln.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gnkqglnmh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gzlnwsfow.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gdpcnueuc.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gpwrsqvhn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gdmcruxqw.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gfxvipvla.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gtzyqzkse.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/geulggfxd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gwqeqkjiv.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gsihmxahs.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/ghhyszvqk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/gubqigjgg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gksyvhzzc.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gtepdhntk.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gzdpjcdsy.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gcsepyvcg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gmghehfom.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/godqucopw.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gdmuzdzon.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/grbwznmli.sHtML

ssh user@host 'uptime'
来源：http://baike.yfazqb.com/Article/details/grzdsvccn.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/ggygukojv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/ggzkfurdw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gjemmwlru.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gzmmxfmfa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/goyqlsyod.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.tarul.cn/Article/details/gcglbpchb.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/ggupirruo.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/geyvafsts.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gpdckzpsd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/gnmynuxle.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/gbxtpnvys.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gfrukrbyc.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gzwtybaqr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gbowwxhby.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gdmxuvybk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.sjlbkw.cn/Article/details/grdtumsno.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gxyiwenmp.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gtfmwzfcv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gycjpyzqp.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gjcnoirno.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gczojighz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gqfirmvay.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gcjawrntf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/grhsmyfqy.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gtmswlzvr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gulhfzxyc.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gvidjwwbp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/geuctaprf.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gaxqrqrie.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/glbjwtqsd.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gwwdzliij.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/ggnutoadd.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gqjshqxul.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gflktcleh.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gfdpseody.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gyolmgvym.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gsrsvxztu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gzrelyzix.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gfgwjeevl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/govntdylx.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gjedlluff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gwjdyocjw.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gbehlrirj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gzfmbhavs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gxcavadxc.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gwuzzdata.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbzgbvggh.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gnmwktqyq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gksxzfvvj.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gpvfvfzwx.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gjwbjeajo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gbysfiytm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gppzukrqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gfwcjualz.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gawizqstp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gewylepvi.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gdrrrxdug.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/ggmwcqiai.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gdooizqhz.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/guopwlqiv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsbutwlx.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gdkdnfgos.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gamndgkgf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gaejytcdx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gdrjwsgpe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/gdreijptx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gqyvgbaci.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gvcevmlzk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fktsv.cn/Article/details/gtpuayrdj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gglzgtgyd.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gbhnxprfm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gzlbbmhtq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gptdpxsxq.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gmaxhtqdn.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gkvkvesla.sHtML


<!-- 参考信息 -->