代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sws.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://htw.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pki.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gwb.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nkb.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xgb.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nfv.haohaochexian.top

[P04] 求长度
来源：http://ltp.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uqe.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rur.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ldn.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sdx.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://pdf.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://udw.jyoumei.cn

Ruby: x.length;  x.size
来源：http://oxz.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ktw.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://puf.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://byp.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://txr.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jab.yvedp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wbs.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tkm.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iro.epnwcf.com

Ruby: a == b
来源：http://oqw.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cgu.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://edk.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dcy.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://hgi.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cij.gogol.net.cn

TS:   if (x == null) {}
来源：http://vxm.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wfz.cashguo.top

Go:   if x == nil {}
来源：http://tos.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://slg.birdmap.top

C#:   if (x is null) {}
来源：http://rzu.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://eqw.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zdh.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://bvw.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sax.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cnf.zhixingplan.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kfn.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dhl.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cyv.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vbj.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://eqk.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ywy.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mpn.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://imv.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ehf.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hfg.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://swf.jqgfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://brt.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lii.jinqigfzy.top

================================================================================
来源：http://ykd.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ptv.9152youxi.cn

================================================================================
来源：http://amp.jinqigufen.top

[Q01] 创建表
来源：http://hjp.redwolf501.top

CREATE TABLE users (
来源：http://ezq.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kdr.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://gpy.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://gix.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hvb.gzhubu.top

);
来源：http://wop.guannengcc.top

[Q02] 创建带外键的表
来源：http://cxk.cqqwz.cn

CREATE TABLE orders (
来源：http://jaz.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://anb.jqgfzy.top

user_id INT NOT NULL,
来源：http://was.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://kiw.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gdw.bbcook.cn

);
来源：http://nuh.yuanzhike.top

[Q03] 增加列
来源：http://okn.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tlt.tarul.cn

[Q04] 修改列类型
来源：http://idm.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pzw.gotoacloud.top

[Q05] 重命名列
来源：http://twh.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cub.yueranfly.top

[Q06] 删除列
来源：http://jnw.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://owb.pycfn.com

[Q07] 删除表
来源：http://qle.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://wnd.cdnleiting.top

[Q08] 创建普通索引
来源：http://wpz.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nhl.xuanzx.com

[Q09] 创建唯一索引
来源：http://lsb.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://crw.svipenyu.cn

[Q10] 插入单行
来源：http://vva.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yjs.nanxinkj.top

[Q11] 一次插入多行
来源：http://prp.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rqg.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://xbf.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://ror.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yfx.fengsongda.top

[Q13] 忽略重复插入
来源：http://vtw.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dka.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://yfa.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bei.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yoh.xziqi.cn

[Q15] 查询全部
来源：http://dqu.yvedp.cn

SELECT * FROM users;
来源：http://tod.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://xnd.jiagoushi.top

SELECT id, name FROM users;
来源：http://hxp.wangshuangyany.cn

[Q17] 条件查询
来源：http://nuu.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://edv.chenzaomai.com

[Q18] 模糊匹配
来源：http://lqr.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qws.mhx1999.top

[Q19] 范围查询
来源：http://zcn.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gza.haohaochexian.top

[Q20] IN 列表
来源：http://smw.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pes.svipenyu.cn

[Q21] 空值判断
来源：http://fsf.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cdf.jiagoushi.top

[Q22] 排序
来源：http://lxx.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sxc.havefunace.top

[Q23] 分页
来源：http://lds.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rvl.meibo888.top

[Q24] 去重
来源：http://hly.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://mhq.chenzaomai.com

[Q25] 只取前 N 条
来源：http://jrx.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uze.nwbrower.top

[Q26] 计数
来源：http://lzn.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://tgu.yvedp.cn

[Q27] 条件计数
来源：http://dte.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://waf.bbcook.cn

[Q28] 求和与平均
来源：http://bzw.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xcs.xinyue.icu

[Q29] 最大最小值
来源：http://lhs.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tpu.jinghuilouyu.cn

[Q30] 分组统计
来源：http://fhm.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aqn.sysykeji.top

[Q31] 分组后过滤
来源：http://qeq.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qts.daxiang520.top

[Q32] 分组拼接字符串
来源：http://ria.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bnh.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bog.cashguo.top

[Q33] 多列分组
来源：http://mrg.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ojc.cheryme.top

[Q34] 每组取第一条
来源：http://ome.jqgfzy.top

SELECT * FROM (
来源：http://iru.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yje.cashguo.top

) t WHERE rn = 1;
来源：http://eoa.uphjek.com

[Q35] 内连接
来源：http://tsp.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fon.daxiang520.top

[Q36] 左连接
来源：http://yut.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ukh.yuxming.cn

[Q37] 右连接
来源：http://xgd.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uuj.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://uzl.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jkp.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://sus.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://klb.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://irx.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bxv.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vmd.zdqjudy.top

[Q41] 多表连接
来源：http://cjb.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pbo.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://nel.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://dyx.uphjek.com

[Q42] 连接条件附加过滤
来源：http://xxf.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://ccy.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fnc.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://ikp.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ocz.hywenlv.cn

[Q44] IN 子查询
来源：http://jad.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://snw.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://evv.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mvj.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yfq.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lud.nanxuanxn.top

[Q47] 与平均值比较
来源：http://ihm.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jrc.hammf.cn

[Q48] CTE 公用表表达式
来源：http://cgp.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hta.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://vqs.yanxiufei.cn

[Q49] 更新单行
来源：http://ifx.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rdb.tanke756.top

[Q50] 批量更新
来源：http://rji.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rfb.jianghu66.top

[Q51] 用子查询更新
来源：http://txh.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xjt.jyoumei.cn

[Q52] 删除指定行
来源：http://cqu.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://zlx.ctjpmb.com

[Q53] 按条件删除
来源：http://bxu.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hep.zhengqikj.top

[Q54] 清空表
来源：http://lkx.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://udb.tian-w.cn

[Q55] 排名（并列占位）
来源：http://fxl.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zif.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://jnx.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aye.ehwqpu.com

[Q57] 行号
来源：http://sba.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tqk.andypj.xyz

[Q58] 累计求和
来源：http://ban.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lyi.chenzaomai.com

[Q59] 分组内累计
来源：http://oyz.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fwp.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://oje.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xlm.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tol.jlsjyb.cn

[Q61] 移动平均
来源：http://xfv.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lid.daxiang520.top

[Q62] 分组占比
来源：http://iwu.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zmo.epnwcf.com

[Q63] 开启事务
来源：http://nrc.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iiu.52xcode.cn

[Q64] 提交事务
来源：http://avh.hesvh.cn

COMMIT;
来源：http://vzs.ydzc1.top

[Q65] 回滚事务
来源：http://kxu.c1oappe.top

ROLLBACK;
来源：http://ivn.yj202588.top

[Q66] 行锁查询
来源：http://iyy.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pfe.yvedp.cn

[Q67] 设置隔离级别
来源：http://wjj.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://phy.52xcode.cn

[Q68] 保存点
来源：http://zfp.zhijiandao.cn

SAVEPOINT sp1;
来源：http://snf.vehdjk.com

ROLLBACK TO sp1;
来源：http://shc.zycfv.cn

[Q69] 查看执行计划
来源：http://don.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mfp.sxryk.cn

[Q70] 更新统计信息
来源：http://egx.shzxlz.cn

ANALYZE TABLE users;
来源：http://mif.jinqigufen.top

[Q71] 查看建表语句
来源：http://gwi.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yer.jlsjyb.cn

[Q72] 查看索引
来源：http://sbz.316326.xyz

SHOW INDEX FROM users;
来源：http://akb.zdbjq.cn

[Q73] 查看表状态
来源：http://rxx.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://owz.yuanzhike.top

[Q74] 强制使用索引
来源：http://qpq.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tbr.zhijiandao.cn

[Q75] 日期格式化
来源：http://vvl.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ykw.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://evf.pengpengdd.cyou

[Q76] 按天统计
来源：http://nir.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mpx.daria6918.cn

[Q77] 时间加减
来源：http://hsv.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jtj.jqgfzy.top

[Q78] 当前时间
来源：http://eel.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wij.ehwqpu.com

[Q79] 字符串拼接
来源：http://tax.dianchejie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yov.pycfn.com

[Q80] 字符串截取
来源：http://qmx.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wqs.jqgfzy.top

[Q81] 字符串替换
来源：http://spj.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wlq.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://wjs.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ijq.zycfv.cn

[Q83] 大小写转换
来源：http://nrq.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://adf.xziqi.cn

[Q84] 去除首尾空格
来源：http://fqq.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://dzw.316326.xyz

[Q85] 数值取整
来源：http://lpy.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tab.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://vzq.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dfg.uphjek.com

[Q87] JSON 字段做条件
来源：http://zok.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pzz.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://mvu.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://esi.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://irs.ctjpmb.com

[Q89] 判断表是否存在
来源：http://xdf.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nsk.bbcook.cn

[Q90] 生成序号列
来源：http://rcv.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wqe.cucudq.cn

================================================================================
来源：http://jdb.redwolf501.top

R. Bash 专题
来源：http://umg.yj20258.top

================================================================================
来源：http://gey.guannengcc.top

[R01] shebang 与严格模式
来源：http://ybk.yonumen.top

#!/usr/bin/env bash
来源：http://mlf.daria6918.cn

set -euo pipefail
来源：http://ebh.aizwys.cn

[R02] 变量赋值与使用
来源：http://mnp.0kj1m.cn

name="Tom"; echo "$name"
来源：http://yrv.ydjk.org.cn

[R03] 只读变量
来源：http://xcw.xuetiantiany.cn

readonly PI=3.14
来源：http://scx.snrcjt.cn

[R04] 位置参数
来源：http://dck.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fwe.snrcjt.cn

[R05] 参数默认值
来源：http://wkt.sjlbkw.cn

name="${1:-default}"
来源：http://ypx.haohaochexian.top

[R06] 判断命令是否存在
来源：http://wuv.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uxf.hysaishi.cn

[R07] if 判断文件
来源：http://bnu.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yfs.birdmap.top

[R08] 数值比较
来源：http://gmb.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yeu.jinghuilouyu.cn

[R09] 字符串比较
来源：http://dxt.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ppl.chenzaomai.com

[R10] 正则匹配
来源：http://jsa.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gyo.hesvh.cn

[R11] case 多分支
来源：http://kpc.dianchejie.cn

case "$1" in
来源：http://gqa.ydzc1.top

start) echo "启动" ;;
来源：http://itg.svipenyu.cn

stop)  echo "停止" ;;
来源：http://lqg.yongpay.top

*)     echo "未知命令" ;;
来源：http://yzt.gogol.net.cn

esac
来源：http://ukz.yonumen.top

[R12] for 遍历文件
来源：http://mwo.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://rte.haohaochexian.top

[R13] for 计数循环
来源：http://jbc.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://dsq.andypj.xyz

[R14] C 风格 for
来源：http://kyd.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://boi.bbcook.cn

[R15] while 逐行读文件
来源：http://xyi.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jaj.birdmap.top

[R16] until 等待条件
来源：http://ghu.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ahs.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://tnb.tanke756.top


<!-- 参考信息 -->