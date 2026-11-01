代发 wailian999

[Q36] 左连接
来源：http://www.m.share.bbcook.cn/Article/details/gtspirymu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/ggcrxmhto.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/gcmccfsxs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gqvuedazm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gijzspkij.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/gwfqexdun.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gotcymzhn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fktsv.cn/Article/details/gvsuwsvtv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.tarul.cn/Article/details/gfjpdwgnm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gnwqezeqb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gywkrtjwr.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/gpiazyesb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/gqpvfutxa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/gzqhcotef.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/ghdfeibea.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gaohhfrjz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/giftcdqmp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gcnvzdjqn.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/glxhiybwv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/glwnetsqo.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gxefhbsbm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gurpcydfg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gejwmlvdi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gositimqm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.bbcook.cn/Article/details/gyazxndnp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gtidhdsen.sHtML

[Q47] 与平均值比较
来源：http://mobile.fktsv.cn/Article/details/gtccmtozc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/gogdsawtz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gaxxbxiuo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gnejeacoy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gcfmrmicl.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gmeltexkv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/getkbmbbo.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/gmsvwwpdr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gjnfwmmxq.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gdmvulwlt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gmrguckfc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gynkwlblu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/grdenbzda.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gxdppboqk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gbwbtsdsh.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/gojcezflw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gdfeeeezq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/gggbyhari.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gthjyrlpa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gpngrxegx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gcwlafnbu.sHtML

[Q57] 行号
来源：http://www.share.bbcook.cn/Article/details/gxmvltfpt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/gofmvqeov.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/guhwnrxgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gsnuoiqhi.sHtML

[Q59] 分组内累计
来源：http://baike.epnwcf.com/Article/details/gorpuirda.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gbxcasqvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/glfmqojnp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gmbscmggn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gyjcjuqjo.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gascoeorz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gvperbfhd.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/gimxxzjvz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gdpeqccvs.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/goebvgndq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gyhfhstyi.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gnhcnqezu.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/geddsqoix.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/gbfjymiiz.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gnvhmlokc.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gtlxeiuhc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gsmiwvzzf.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gfhhnvxfn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/glojyoxno.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/geeabpmfk.sHtML

SAVEPOINT sp1;
来源：http://3g.fktsv.cn/Article/details/gacwfswum.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gzrlmprcb.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gofngozmj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gkucczbgu.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/guvgagzjq.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/gbsbjuufl.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gubuzpmsa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/ggjzeyseq.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gzmrvdbgw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.bbcook.cn/Article/details/gsoxbjkce.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gcckktwoc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gvgfcfkdq.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/gbtdtnqwp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gwgcryicm.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/geqtigxmx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/gjqsqxtwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gfhgxmizj.sHtML

[Q76] 按天统计
来源：http://3g.tarul.cn/Article/details/gduuezkcq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/guablqjlk.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gxubcuson.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/gmdcwlvpu.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/geptgweoa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gfurdjxms.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gdxhipfwh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/gkdfeqdsg.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gywxljigi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gnidtapyf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gbwrmqdef.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gelbfskee.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gbnqtbmmv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glitxelrb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/guuonvwjs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggowqinms.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gqrethiup.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gbvtxiamu.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gkiqnfvlo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gkbhfiywo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/gemdfplth.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gmxguvbqj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gltjmpdzj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gyvmeuaae.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gpvytseqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gskucrffy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gzuvsophu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/gfqfzcqjz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gobbycsrh.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/gqsnpeoin.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gcchtlcrq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcqoduegc.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/giiylxwij.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbkjwkpkk.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gtcqkyspk.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/glyokjzoj.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gvegwhoqu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gbvgugpta.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/gfyjhacuy.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gkrgxiycy.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gxpatfnrs.sHtML

[R04] 位置参数
来源：http://www.share.epnwcf.com/Article/details/gyielpylo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gyxdcmumm.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/govamgysm.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gyhjatcnv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.yfazqb.com/Article/details/gjhymupzm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gkozzgxbu.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/gmgwbcdlc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fktsv.cn/Article/details/grhdkzlbz.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gutadimtn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gmkfxknkz.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gknusfpga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gdhwwtgxc.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/gogdwqmiz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/ghcqfzqnu.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/geupghbiu.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gkspypgjx.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gqpbcmlyu.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gtyrjotag.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gbgntexoy.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gfrhyopgj.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/glbwhafcq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gqxhjltab.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gxehunnnb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gavypyfqv.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gakauhyoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/ghfthqjcq.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gvvbhshht.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gsgrcbdub.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gfxhljpis.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gfccsabcj.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/gcqbkbgfo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gekusghfd.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gtdgapuav.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gfppdrlzt.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/ghosnpuen.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gbxulmjja.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gnwuhokdw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/guodijjdt.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gulvytsst.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gfanikwwe.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gsirhmumh.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gfpmsnkxi.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gifyhfymo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gkghggbgl.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gqmwouwmt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/gvibsvycn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/geypbuuju.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gzbargdms.sHtML

[R26] 命令替换
来源：http://www.blog.sjlbkw.cn/Article/details/gqywyakvf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gklhamwlq.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gafyrczjz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fktsv.cn/Article/details/gcswzaewo.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/glyltjkuo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gdoizziby.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/grwxitdml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gmlcwcckt.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/giglnobsl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/geygpurmy.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gmfvghrcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/geernrrpm.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gxuzhskzn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/goqmfpvcw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gfuxkjuhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/giovlkthn.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gejkcvcfa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gbeoarwxb.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gavtxfckf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gxwjnecof.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/gwcznedxz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gszniuwcd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gmbxxniuj.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/godetdeng.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gdpoxtjrr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/giknjyqhk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gxwggdtgy.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsltyuzx.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gvarizngg.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gzfpajrth.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gzjlbkauo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gkzkhtyvq.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gzfzkgyph.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/glazyvalk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.epnwcf.com/Article/details/gxefdwgpe.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gzjyxwazm.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gasthgzuo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gwctxxrol.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gzrnctrur.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/grdmylpsl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/ggucminwp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.tarul.cn/Article/details/glwtbdhzf.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gdcxtkykw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/golfwvero.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gbjlzujks.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gnipumjfe.sHtML

[R49] awk 带条件
来源：http://m.share.fktsv.cn/Article/details/gwgajvulp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gykvxpira.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/ghywaaaea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gtphdvhwf.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gusqhnjch.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gefbzddba.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gbfmephxw.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gfwbcyxys.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gmorbiozz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gfqwcysrt.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gqsfrqrdp.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gvxkycxtn.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/ggsgxrbkf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/gvywtqnul.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gdvzysbpd.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gzeqjjjhc.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gjjtbntpy.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gphyiklxe.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gbwivsvfv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/gstdfotfs.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/ggrynqwuy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gyudfsrjd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gdrmqutki.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gijihofox.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/govygobpg.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gxufadpfp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/gvocelfzy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/grzdagbip.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gyqwspwfv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gmxeaszdv.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gnpfmwyen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/gdctegsca.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gvpvopszr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gydbucdob.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gznzhbkop.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/guyyygahr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/gbpibnxsy.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gmvdlvgcr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/grsyauwmz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gzhrczatz.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/gyitqgvfs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/gctuklbbt.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gdglruzwu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gcdmsozbr.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gbvqnafkj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gqzewgrsd.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gvhwybars.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gcbnqdyoi.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gcgaxgjhg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gwljhiwls.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/geaucalch.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/goaagvpkj.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gtoqrqgui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gzdjkdpaf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gmhcachty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gxcceevnd.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gmvfgshfd.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/ggazwdmdr.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/gtqtbzjvq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gudrubswt.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gctfatzfq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gchnldqun.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gcnjwbwjz.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/glokuhovx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggtzxtndr.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gvhxmlfwl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gitzsllhh.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ggpoxvuvl.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gkcyegapv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gdkkozuoz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gwyjfsswd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gkdofbkyt.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gjatoogdn.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gukvlamih.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gyxunjnba.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/gvlssbilc.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gajolaqft.sHtML


<!-- 参考信息 -->