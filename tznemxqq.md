代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ayp.haohaochexian.top

C#:   if (x is null) {}
来源：http://lqk.xuetiantiany.cn

[P07] 防抖与节流
来源：http://rpd.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dfd.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://zou.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iku.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmi.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pzn.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rbd.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pcw.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zgq.xziqi.cn

[P08] 处理浮点精度问题
来源：http://mwr.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hrl.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://swm.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sfb.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://byy.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vwd.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qjv.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nlb.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zxw.smart0.xyz

================================================================================
来源：http://zcz.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tch.smart0.xyz

================================================================================
来源：http://vqi.c1oappe.top

[Q01] 创建表
来源：http://wqz.havefunace.top

CREATE TABLE users (
来源：http://qjm.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ayv.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://ojr.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://bcp.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xrc.feifeiyinyue.top

);
来源：http://rzv.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://wgj.yj20258888.top

CREATE TABLE orders (
来源：http://ara.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cge.xylfe.cn

user_id INT NOT NULL,
来源：http://xlp.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://gwe.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qzt.zhaomingkeji.xyz

);
来源：http://rsb.meibo888.top

[Q03] 增加列
来源：http://twx.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qne.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://bww.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://njs.jinghuilouyu.cn

[Q05] 重命名列
来源：http://otj.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kjh.birdmap.top

[Q06] 删除列
来源：http://kxm.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://fst.yj20258888.top

[Q07] 删除表
来源：http://eag.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://ywk.svipenyu.cn

[Q08] 创建普通索引
来源：http://yfd.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kpg.tianlin.xyz

[Q09] 创建唯一索引
来源：http://qoh.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ebh.zhijiandao.cn

[Q10] 插入单行
来源：http://ele.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vww.sxryk.cn

[Q11] 一次插入多行
来源：http://whc.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aio.nwbrower.top

[Q12] 插入后取自增 ID
来源：http://zba.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://yre.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bpw.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://bcq.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zfk.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://upj.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nyv.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtb.yangfankeji.com

[Q15] 查询全部
来源：http://gwb.ivvv.top

SELECT * FROM users;
来源：http://qlx.xylfe.cn

[Q16] 查询指定列
来源：http://xhy.yfazqb.com

SELECT id, name FROM users;
来源：http://tyq.andypj.xyz

[Q17] 条件查询
来源：http://nxa.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tqz.cqqwz.cn

[Q18] 模糊匹配
来源：http://jjb.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cbi.gogol.net.cn

[Q19] 范围查询
来源：http://uua.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://czb.feifeiyinyue.top

[Q20] IN 列表
来源：http://rzk.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dih.cqqwz.cn

[Q21] 空值判断
来源：http://hwq.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gox.ehwqpu.com

[Q22] 排序
来源：http://red.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rdt.zhijiandao.cn

[Q23] 分页
来源：http://ggf.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://imf.ydjk.org.cn

[Q24] 去重
来源：http://msq.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://nam.sysykeji.top

[Q25] 只取前 N 条
来源：http://iyd.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qbs.bbcook.cn

[Q26] 计数
来源：http://gic.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://jxx.birdmap.top

[Q27] 条件计数
来源：http://rso.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kli.tanke756.top

[Q28] 求和与平均
来源：http://civ.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jan.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://koc.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dns.shzxlz.cn

[Q30] 分组统计
来源：http://myr.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fpc.yvedp.cn

[Q31] 分组后过滤
来源：http://qbs.bjfxy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xqu.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://wdp.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://utn.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gwp.aizwys.cn

[Q33] 多列分组
来源：http://rje.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jxr.shzxlz.cn

[Q34] 每组取第一条
来源：http://jcs.bjfxy.top

SELECT * FROM (
来源：http://cgk.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vlg.uphjek.com

) t WHERE rn = 1;
来源：http://enj.wangshuangyany.cn

[Q35] 内连接
来源：http://buz.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ydx.shanyushiyangtech.top

[Q36] 左连接
来源：http://mbj.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://luv.sweek.top

[Q37] 右连接
来源：http://pqe.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dip.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://zrf.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://set.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://xxx.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://yrs.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hgq.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://htn.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dpj.fktsv.cn

[Q41] 多表连接
来源：http://qhl.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://unv.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://xqs.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://qli.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://nmz.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://txb.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dzy.ydzc1.top

[Q43] 标量子查询
来源：http://wkl.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lwc.ydzc1.top

[Q44] IN 子查询
来源：http://fln.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nyv.tarul.cn

[Q45] EXISTS 判断存在
来源：http://pct.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mun.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hal.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uzb.aibaodan.cn

[Q47] 与平均值比较
来源：http://uax.epnwcf.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qad.sweek.top

[Q48] CTE 公用表表达式
来源：http://xei.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dpl.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://yfe.ppjwa.cn

[Q49] 更新单行
来源：http://xny.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kfa.xuetiantiany.cn

[Q50] 批量更新
来源：http://kzp.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vfs.jqgufenzy.top

[Q51] 用子查询更新
来源：http://rfz.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://abo.meibo888.top

[Q52] 删除指定行
来源：http://upl.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://jax.c1oappe.top

[Q53] 按条件删除
来源：http://mcj.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ezq.316326.xyz

[Q54] 清空表
来源：http://blo.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://cwb.xziqi.cn

[Q55] 排名（并列占位）
来源：http://blk.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rre.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://cqr.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdo.shangyingyoupin.top

[Q57] 行号
来源：http://pfi.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ide.aizwys.cn

[Q58] 累计求和
来源：http://dns.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vcd.tanke756.top

[Q59] 分组内累计
来源：http://ulo.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tip.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://eki.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nrs.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yvu.yonumen.top

[Q61] 移动平均
来源：http://sys.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zkr.gaohongyu789.top

[Q62] 分组占比
来源：http://uuo.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ynz.yonumen.top

[Q63] 开启事务
来源：http://jah.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kjb.havefunace.top

[Q64] 提交事务
来源：http://hst.tarul.cn

COMMIT;
来源：http://kda.ctjpmb.com

[Q65] 回滚事务
来源：http://gfp.bbcook.cn

ROLLBACK;
来源：http://gpf.smart0.xyz

[Q66] 行锁查询
来源：http://rtm.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://omz.gotoacloud.top

[Q67] 设置隔离级别
来源：http://glu.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iaj.c1oappe.top

[Q68] 保存点
来源：http://yhr.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://rpu.gotoacloud.top

ROLLBACK TO sp1;
来源：http://qxd.sysykeji.top

[Q69] 查看执行计划
来源：http://yfx.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fui.daria6918.cn

[Q70] 更新统计信息
来源：http://jgn.yuxming.cn

ANALYZE TABLE users;
来源：http://zwj.shuidangran.top

[Q71] 查看建表语句
来源：http://hjn.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iet.redwolf501.top

[Q72] 查看索引
来源：http://zto.jianghu66.top

SHOW INDEX FROM users;
来源：http://tup.hcnkem.com

[Q73] 查看表状态
来源：http://fmc.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ukc.smart0.xyz

[Q74] 强制使用索引
来源：http://glu.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hht.yuanzhike.top

[Q75] 日期格式化
来源：http://ubj.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jcu.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yvd.zhoulong.xyz

[Q76] 按天统计
来源：http://red.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xik.shangyingyoupin.top

[Q77] 时间加减
来源：http://ycx.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zrg.hammf.cn

[Q78] 当前时间
来源：http://owb.yangfankeji.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vro.hfpthk.cn

[Q79] 字符串拼接
来源：http://hfw.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ylz.sweek.top

[Q80] 字符串截取
来源：http://nsg.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://osk.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://uvb.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bzu.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://gjf.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pke.shangyingyoupin.top

[Q83] 大小写转换
来源：http://vro.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://voj.meibo888.top

[Q84] 去除首尾空格
来源：http://rra.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://ogt.guowangkeji.top

[Q85] 数值取整
来源：http://sli.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oln.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://rav.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jfr.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://iwh.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wzp.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://ico.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iqs.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cug.ctjpmb.com

[Q89] 判断表是否存在
来源：http://umf.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sgj.mhx1999.top

[Q90] 生成序号列
来源：http://cmq.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bso.chenzaomai.com

================================================================================
来源：http://yci.nanxinkj.top

R. Bash 专题
来源：http://han.meibo888.top

================================================================================
来源：http://ykq.gzhubu.top

[R01] shebang 与严格模式
来源：http://ecc.fzhhl.top

#!/usr/bin/env bash
来源：http://ufj.jinghuilouyu.cn

set -euo pipefail
来源：http://kpj.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://udo.yueranfly.top

name="Tom"; echo "$name"
来源：http://mud.aizwys.cn

[R03] 只读变量
来源：http://vui.tian-w.cn

readonly PI=3.14
来源：http://sre.xinyue.icu

[R04] 位置参数
来源：http://qtg.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qsv.jlsjyb.cn

[R05] 参数默认值
来源：http://tkb.ydjk.org.cn

name="${1:-default}"
来源：http://tyt.cdnleiting.top

[R06] 判断命令是否存在
来源：http://uuo.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cwk.yonumen.top

[R07] if 判断文件
来源：http://iwp.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ivj.cdnleiting.top

[R08] 数值比较
来源：http://ult.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hdt.sysykeji.top

[R09] 字符串比较
来源：http://qsc.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zuk.wangshuangyany.cn

[R10] 正则匹配
来源：http://sgv.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ihp.tian-w.cn

[R11] case 多分支
来源：http://ddi.fanxiaobao.xyz

case "$1" in
来源：http://zdj.chenlongwang.top

start) echo "启动" ;;
来源：http://pnj.xylfe.cn

stop)  echo "停止" ;;
来源：http://dsv.shuidangran.top

*)     echo "未知命令" ;;
来源：http://hta.yuxming.cn

esac
来源：http://izo.yfazqb.com

[R12] for 遍历文件
来源：http://smn.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://iuw.fzhhl.top

[R13] for 计数循环
来源：http://beb.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://glj.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://ugv.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hhj.nwbrower.top

[R15] while 逐行读文件
来源：http://zou.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lrq.zdbjq.cn

[R16] until 等待条件
来源：http://gtc.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bmd.jianghu66.top

[R17] 数组定义与取值
来源：http://gxt.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oof.zhoulong.xyz

[R18] 遍历数组
来源：http://rin.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ggb.fzhhl.top

[R19] 数组长度
来源：http://vix.bbcook.cn

echo "${#arr[@]}"
来源：http://koq.pycfn.com

[R20] 关联数组（字典）
来源：http://gbq.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mxd.hongshengwenyu.top

[R21] 字符串长度
来源：http://nmk.zhijiandao.cn

echo "${#s}"
来源：http://coc.jinqigufen.top

[R22] 截取子串
来源：http://hbc.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://mnw.epnwcf.com

[R23] 字符串替换
来源：http://tkj.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dcd.sufxvd.cn

[R24] 大小写转换
来源：http://gpt.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://nkg.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://mzy.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://blb.sufxvd.cn

[R26] 命令替换
来源：http://laq.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://njt.c1oappe.top

[R27] 算术展开
来源：http://fws.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://dsq.yongpay.top

[R28] 浮点运算
来源：http://qrl.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://oag.kuanghao11.cn

[R29] 定义函数
来源：http://nhq.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hab.xylfe.cn

[R30] 函数返回状态码
来源：http://wza.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://gxb.shangyingyoupin.top

[R31] 局部变量
来源：http://yem.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://awo.yuxming.cn

[R32] 参数个数校验
来源：http://umz.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rnp.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://flt.52xcode.cn


<!-- 参考信息 -->