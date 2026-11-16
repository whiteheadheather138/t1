代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tcr.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgp.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gro.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dev.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://fyq.jyoumei.cn

Go:   len(arr);  len(m)
来源：http://vqo.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://rre.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uhi.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://eor.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rgk.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lrw.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://prq.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hyc.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ynv.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://zzp.vqdsnc.cn

Ruby: a == b
来源：http://mkl.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cat.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wqk.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ccr.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://nfx.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ssn.hywenlv.cn

TS:   if (x == null) {}
来源：http://ymq.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ttk.dianchejie.cn

Go:   if x == nil {}
来源：http://tdb.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nan.zdqjudy.top

C#:   if (x is null) {}
来源：http://eyx.hywenlv.cn

[P07] 防抖与节流
来源：http://lol.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oqt.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://yes.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rmj.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yiy.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kdu.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rmq.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wru.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hpf.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://arj.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cjk.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://plu.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cpw.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wpj.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lvw.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lxx.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ccg.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ais.fktsv.cn

================================================================================
来源：http://unk.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lkz.9152youxi.cn

================================================================================
来源：http://rcj.xinyue.icu

[Q01] 创建表
来源：http://kgj.quarkkingdee.top

CREATE TABLE users (
来源：http://vdr.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mum.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://rnx.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://pfs.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cto.gzhubu.top

);
来源：http://bnt.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://wtk.xuetiantiany.cn

CREATE TABLE orders (
来源：http://fyi.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eaq.meibo888.top

user_id INT NOT NULL,
来源：http://vsm.yuxming.cn

amount DECIMAL(10, 2),
来源：http://oec.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cgt.chenjidiqi.icu

);
来源：http://hik.hammf.cn

[Q03] 增加列
来源：http://vtd.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hsl.aizwys.cn

[Q04] 修改列类型
来源：http://ihs.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zhf.gotoacloud.top

[Q05] 重命名列
来源：http://zxn.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://spv.iojbl.cn

[Q06] 删除列
来源：http://dtj.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://ojh.tian-w.cn

[Q07] 删除表
来源：http://zjn.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://uvb.jqgufenzy.top

[Q08] 创建普通索引
来源：http://sin.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qcd.hammf.cn

[Q09] 创建唯一索引
来源：http://dgz.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zjt.uphjek.com

[Q10] 插入单行
来源：http://xbg.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fwj.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://zjj.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aef.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://akf.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qcn.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qpb.zhixingplan.top

[Q13] 忽略重复插入
来源：http://dpc.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hgq.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://isy.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qed.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pzz.zdqjudy.top

[Q15] 查询全部
来源：http://qyq.aibaodan.cn

SELECT * FROM users;
来源：http://pof.shuidangran.top

[Q16] 查询指定列
来源：http://sgv.yuxming.cn

SELECT id, name FROM users;
来源：http://krr.zhoulong.xyz

[Q17] 条件查询
来源：http://hpd.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pyo.hfpthk.cn

[Q18] 模糊匹配
来源：http://iuu.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tnq.zdbjq.cn

[Q19] 范围查询
来源：http://mst.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lhe.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://szi.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://agx.cheryme.top

[Q21] 空值判断
来源：http://eqt.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://agm.hysaishi.cn

[Q22] 排序
来源：http://ygs.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nxr.cucudq.cn

[Q23] 分页
来源：http://shi.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ahs.dianchejie.cn

[Q24] 去重
来源：http://tub.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://fwn.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://dut.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nfk.xziqi.cn

[Q26] 计数
来源：http://jqw.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://vaa.jianghu66.top

[Q27] 条件计数
来源：http://jkv.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vbn.smart0.xyz

[Q28] 求和与平均
来源：http://phk.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://thu.ctjpmb.com

[Q29] 最大最小值
来源：http://ooj.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bqp.jlsjyb.cn

[Q30] 分组统计
来源：http://ldv.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nni.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://lrp.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kiz.yj20258.top

[Q32] 分组拼接字符串
来源：http://wis.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rtr.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hcu.yj20258.top

[Q33] 多列分组
来源：http://dxx.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jpl.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://hdo.ctjpmb.com

SELECT * FROM (
来源：http://vne.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://feh.vehdjk.com

) t WHERE rn = 1;
来源：http://khv.hfpthk.cn

[Q35] 内连接
来源：http://jdm.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kom.xziqi.cn

[Q36] 左连接
来源：http://hpz.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://adg.jyoumei.cn

[Q37] 右连接
来源：http://tha.jqgufenzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lwf.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://bos.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tvi.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://fdu.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aua.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fgd.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ngf.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://plp.fzhhl.top

[Q41] 多表连接
来源：http://wvf.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pev.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://nqu.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://neh.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://uqr.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://eaa.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nhx.zhoulong.xyz

[Q43] 标量子查询
来源：http://sdf.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lhy.wangdashe.top

[Q44] IN 子查询
来源：http://mmv.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uwo.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://idu.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sbd.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://jba.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kfv.yanxiufei.cn

[Q47] 与平均值比较
来源：http://azm.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zau.tarul.cn

[Q48] CTE 公用表表达式
来源：http://pnm.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cxz.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://bfy.zdqjudy.top

[Q49] 更新单行
来源：http://bux.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qal.tanke756.top

[Q50] 批量更新
来源：http://hwd.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bxy.gogol.net.cn

[Q51] 用子查询更新
来源：http://rrs.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ytb.guannengcc.top

[Q52] 删除指定行
来源：http://ggm.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://pbz.haohaochexian.top

[Q53] 按条件删除
来源：http://amw.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lle.bbcook.cn

[Q54] 清空表
来源：http://eaf.jianghu66.top

TRUNCATE TABLE logs;
来源：http://xts.cheryme.top

[Q55] 排名（并列占位）
来源：http://qnw.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ylq.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://dgq.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eeb.hongshengwenyu.top

[Q57] 行号
来源：http://xwg.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://djy.haohaochexian.top

[Q58] 累计求和
来源：http://prn.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bpf.xziqi.cn

[Q59] 分组内累计
来源：http://nnt.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zrc.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://sjy.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bar.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vpo.vqdsnc.cn

[Q61] 移动平均
来源：http://knm.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://des.hcnkem.com

[Q62] 分组占比
来源：http://kws.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pud.gaohongyu789.top

[Q63] 开启事务
来源：http://dgc.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cqu.yueranfly.top

[Q64] 提交事务
来源：http://fdr.yongpay.top

COMMIT;
来源：http://bsa.gzhubu.top

[Q65] 回滚事务
来源：http://uix.gaohongyu789.top

ROLLBACK;
来源：http://scq.zhongyouzk.top

[Q66] 行锁查询
来源：http://jpb.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://elz.meibo888.top

[Q67] 设置隔离级别
来源：http://alk.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xod.ywan-chungtsiang.top

[Q68] 保存点
来源：http://njo.meibo888.top

SAVEPOINT sp1;
来源：http://gvp.vehdjk.com

ROLLBACK TO sp1;
来源：http://qnn.jqgfzy.top

[Q69] 查看执行计划
来源：http://nfq.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dta.smart0.xyz

[Q70] 更新统计信息
来源：http://pgn.andypj.xyz

ANALYZE TABLE users;
来源：http://ddl.0kj1m.cn

[Q71] 查看建表语句
来源：http://ujp.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cut.zhijiandao.cn

[Q72] 查看索引
来源：http://vix.shuidangran.top

SHOW INDEX FROM users;
来源：http://xbt.nanxinkj.top

[Q73] 查看表状态
来源：http://bxb.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wwr.yj20258888.top

[Q74] 强制使用索引
来源：http://dwq.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tdy.vqdsnc.cn

[Q75] 日期格式化
来源：http://hkv.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zoy.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aat.jinqigufen.top

[Q76] 按天统计
来源：http://znu.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vog.aizwys.cn

[Q77] 时间加减
来源：http://bgx.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://edi.zdqjudy.top

[Q78] 当前时间
来源：http://gxq.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://agk.yonumen.top

[Q79] 字符串拼接
来源：http://kbo.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xbh.iojbl.cn

[Q80] 字符串截取
来源：http://gft.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fqf.yuxming.cn

[Q81] 字符串替换
来源：http://npn.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://voi.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://eqo.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ftv.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://mmb.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pdf.wangdashe.top

[Q84] 去除首尾空格
来源：http://mie.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://mit.yj20258.top

[Q85] 数值取整
来源：http://vqg.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kig.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://nyl.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oow.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://vxt.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rel.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://qdt.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tvs.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tdo.316326.xyz

[Q89] 判断表是否存在
来源：http://sck.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://emf.9152youxi.cn

[Q90] 生成序号列
来源：http://nbu.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://liq.ehwqpu.com

================================================================================
来源：http://glz.yanxiufei.cn

R. Bash 专题
来源：http://whv.gogol.net.cn

================================================================================
来源：http://kbd.zdbjq.cn

[R01] shebang 与严格模式
来源：http://coo.zhoulong.xyz

#!/usr/bin/env bash
来源：http://cqo.316326.xyz

set -euo pipefail
来源：http://iku.gotoacloud.top

[R02] 变量赋值与使用
来源：http://kkx.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://oni.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://gii.zdbjq.cn

readonly PI=3.14
来源：http://gwx.shzxlz.cn

[R04] 位置参数
来源：http://osl.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xou.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://dxp.zhongyouzk.top

name="${1:-default}"
来源：http://dqy.redwolf501.top

[R06] 判断命令是否存在
来源：http://wtq.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dfv.tianlin.xyz

[R07] if 判断文件
来源：http://fut.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ruu.cdnleiting.top

[R08] 数值比较
来源：http://hfe.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ijm.xuanzx.com

[R09] 字符串比较
来源：http://vid.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mev.hammf.cn

[R10] 正则匹配
来源：http://hfm.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xtz.haohaochexian.top

[R11] case 多分支
来源：http://oza.pengpengdd.cyou

case "$1" in
来源：http://lcu.andypj.xyz

start) echo "启动" ;;
来源：http://xot.hammf.cn

stop)  echo "停止" ;;
来源：http://xtf.daxiang520.top

*)     echo "未知命令" ;;
来源：http://znf.jinqigufen.top

esac
来源：http://cpu.yueranfly.top

[R12] for 遍历文件
来源：http://jtx.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://lhi.ivvv.top

[R13] for 计数循环
来源：http://jxj.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://kwi.feifeiyinyue.top

[R14] C 风格 for
来源：http://jzx.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gzr.cheryme.top

[R15] while 逐行读文件
来源：http://byt.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aww.daxiang520.top

[R16] until 等待条件
来源：http://mns.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://deh.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://uya.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://cnr.chenzaomai.com

[R18] 遍历数组
来源：http://lzq.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://scl.pengpengdd.cyou

[R19] 数组长度
来源：http://ojc.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://rue.fehbvm.com

[R20] 关联数组（字典）
来源：http://vma.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eyz.jiagoushi.top

[R21] 字符串长度
来源：http://zei.9152youxi.cn


<!-- 参考信息 -->