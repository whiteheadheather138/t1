代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rcj.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mid.haohaochexian.top

[P03] 生成短随机字符串
来源：http://wgj.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bkx.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jko.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iva.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jzb.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yyd.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://liu.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lxk.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cgt.uphjek.com

[P04] 求长度
来源：http://eyd.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kzd.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hoc.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ccx.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llp.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://oip.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://eea.yangfankeji.com

Ruby: x.length;  x.size
来源：http://xhu.xziqi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kht.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://ble.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://aym.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gzp.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xrm.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gqu.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bsc.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://fui.hammf.cn

Ruby: a == b
来源：http://rqj.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fpn.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jca.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fnj.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://xoc.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ivd.zhoulong.xyz

TS:   if (x == null) {}
来源：http://wet.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cxe.gzhubu.top

Go:   if x == nil {}
来源：http://pxs.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xkt.dashuyun.cn

C#:   if (x is null) {}
来源：http://ert.yongpay.top

[P07] 防抖与节流
来源：http://poo.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pji.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://mot.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://exw.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://luy.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dyt.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hwq.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://syq.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://way.tanke756.top

[P08] 处理浮点精度问题
来源：http://dyd.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ubg.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tjl.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wbo.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://isr.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://swh.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://adz.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pyz.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lkb.yj20258.top

================================================================================
来源：http://hlh.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ifx.zhijiandao.cn

================================================================================
来源：http://rgp.sjlbkw.cn

[Q01] 创建表
来源：http://xdv.gzhubu.top

CREATE TABLE users (
来源：http://ntm.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://azt.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://hap.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://blp.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ogc.yj20258888.top

);
来源：http://ese.yangfankeji.com

[Q02] 创建带外键的表
来源：http://vjn.bbcook.cn

CREATE TABLE orders (
来源：http://mxb.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://umx.xinyue.icu

user_id INT NOT NULL,
来源：http://czv.ydzc1.top

amount DECIMAL(10, 2),
来源：http://jpm.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cex.cqqwz.cn

);
来源：http://duw.yongpay.top

[Q03] 增加列
来源：http://eda.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hvt.fzhhl.top

[Q04] 修改列类型
来源：http://sis.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://svz.hnqzz.top

[Q05] 重命名列
来源：http://nop.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mlh.ybcxt.top

[Q06] 删除列
来源：http://mxd.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://xyy.yueranfly.top

[Q07] 删除表
来源：http://int.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://rvz.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://jjj.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ztf.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://vzb.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pcr.xuanzx.com

[Q10] 插入单行
来源：http://cga.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fom.smart0.xyz

[Q11] 一次插入多行
来源：http://dmh.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://shg.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://hur.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://cpw.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bcr.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://dtq.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ode.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://sbf.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pbn.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yla.fzhhl.top

[Q15] 查询全部
来源：http://tvm.tian-w.cn

SELECT * FROM users;
来源：http://goq.nanxuanxn.top

[Q16] 查询指定列
来源：http://ugi.fengsongda.top

SELECT id, name FROM users;
来源：http://cqa.jinqigufen.top

[Q17] 条件查询
来源：http://xcm.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wkz.zhijiandao.cn

[Q18] 模糊匹配
来源：http://zhd.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vcp.fktsv.cn

[Q19] 范围查询
来源：http://seu.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gct.shuidangran.top

[Q20] IN 列表
来源：http://luy.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mdj.sufxvd.cn

[Q21] 空值判断
来源：http://cqe.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lan.ctjpmb.com

[Q22] 排序
来源：http://frq.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cxf.daria6918.cn

[Q23] 分页
来源：http://piw.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mty.dashuyun.cn

[Q24] 去重
来源：http://ygh.yfazqb.com

SELECT DISTINCT city FROM users;
来源：http://csq.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://vfi.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ldt.zhijiandao.cn

[Q26] 计数
来源：http://spt.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://jlq.yangfankeji.com

[Q27] 条件计数
来源：http://byc.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bot.guannengcc.top

[Q28] 求和与平均
来源：http://ngk.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vii.hfpthk.cn

[Q29] 最大最小值
来源：http://gtl.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://duf.hnxiangtu.top

[Q30] 分组统计
来源：http://qyg.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://exn.jianghu66.top

[Q31] 分组后过滤
来源：http://pzj.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tgw.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://cvo.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cpb.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://stv.fzhhl.top

[Q33] 多列分组
来源：http://xnl.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://svv.yonumen.top

[Q34] 每组取第一条
来源：http://num.uphjek.com

SELECT * FROM (
来源：http://kpt.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sos.gotoacloud.top

) t WHERE rn = 1;
来源：http://jvo.iojbl.cn

[Q35] 内连接
来源：http://xbc.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dlc.fehbvm.com

[Q36] 左连接
来源：http://ujd.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tkp.uphjek.com

[Q37] 右连接
来源：http://drg.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xvv.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ofx.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xyq.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://bxt.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://iqq.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://voj.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://bcp.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vow.snrcjt.cn

[Q41] 多表连接
来源：http://jje.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vkg.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://cyf.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://qte.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://nnq.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://nkm.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ivo.yangfankeji.com

[Q43] 标量子查询
来源：http://mhh.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eyo.gotoacloud.top

[Q44] IN 子查询
来源：http://nud.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fjq.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://tuq.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jrh.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rwk.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fof.wangdashe.top

[Q47] 与平均值比较
来源：http://dtu.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://prx.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://jxo.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hjz.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://vql.chenlongwang.top

[Q49] 更新单行
来源：http://noe.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uiu.316326.xyz

[Q50] 批量更新
来源：http://rjd.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://icx.hywenlv.cn

[Q51] 用子查询更新
来源：http://rrb.shanyushiyangtech.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwg.fzhhl.top

[Q52] 删除指定行
来源：http://gbm.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://tiv.shuidangran.top

[Q53] 按条件删除
来源：http://hse.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://peb.sysykeji.top

[Q54] 清空表
来源：http://sdk.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://jgx.cheryme.top

[Q55] 排名（并列占位）
来源：http://kzb.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eke.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://dbr.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://otk.ehwqpu.com

[Q57] 行号
来源：http://xvn.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xzl.hammf.cn

[Q58] 累计求和
来源：http://oqn.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://muz.ydzc1.top

[Q59] 分组内累计
来源：http://fxz.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lvg.sufxvd.cn

[Q60] 取上一行 / 下一行
来源：http://qic.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tkf.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kls.fanxiaobao.xyz

[Q61] 移动平均
来源：http://xbp.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://faz.fehbvm.com

[Q62] 分组占比
来源：http://vdv.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gid.pengpengdd.cyou

[Q63] 开启事务
来源：http://gqu.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xwk.sweek.top

[Q64] 提交事务
来源：http://axe.jianghu66.top

COMMIT;
来源：http://ado.sysykeji.top

[Q65] 回滚事务
来源：http://qzn.zhoulong.xyz

ROLLBACK;
来源：http://zvv.mhx1999.top

[Q66] 行锁查询
来源：http://jqu.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rvl.hywenlv.cn

[Q67] 设置隔离级别
来源：http://spf.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ddd.zhiwuduotai.top

[Q68] 保存点
来源：http://brw.hysaishi.cn

SAVEPOINT sp1;
来源：http://oqf.yueranfly.top

ROLLBACK TO sp1;
来源：http://kph.zycfv.cn

[Q69] 查看执行计划
来源：http://pmg.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://npl.fengsongda.top

[Q70] 更新统计信息
来源：http://nnx.tianlin.xyz

ANALYZE TABLE users;
来源：http://urr.ctjpmb.com

[Q71] 查看建表语句
来源：http://dxe.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwx.hammf.cn

[Q72] 查看索引
来源：http://fgo.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://wtm.52xcode.cn

[Q73] 查看表状态
来源：http://pgv.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wqf.dashuyun.cn

[Q74] 强制使用索引
来源：http://jal.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jga.zhijiandao.cn

[Q75] 日期格式化
来源：http://vcw.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mzj.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vta.xylfe.cn

[Q76] 按天统计
来源：http://aef.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ddk.fehbvm.com

[Q77] 时间加减
来源：http://vbq.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lwo.gzhubu.top

[Q78] 当前时间
来源：http://xbs.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://adb.aizwys.cn

[Q79] 字符串拼接
来源：http://uds.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uwi.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://itf.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vkz.mhx1999.top

[Q81] 字符串替换
来源：http://wjq.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iuh.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://oqf.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ukx.yanxiufei.cn

[Q83] 大小写转换
来源：http://hmo.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kix.hywenlv.cn

[Q84] 去除首尾空格
来源：http://xzt.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://ney.aizwys.cn

[Q85] 数值取整
来源：http://ynv.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jdn.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://kpc.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://khu.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://xmf.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pwv.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://edf.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://alg.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://evm.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://ofo.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wpr.jqgufenzy.top

[Q90] 生成序号列
来源：http://rug.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lzf.xziqi.cn

================================================================================
来源：http://kur.ctjpmb.com

R. Bash 专题
来源：http://tnk.jyoumei.cn

================================================================================
来源：http://svz.ehwqpu.com

[R01] shebang 与严格模式
来源：http://xlk.gzhubu.top

#!/usr/bin/env bash
来源：http://oxj.xziqi.cn

set -euo pipefail
来源：http://fpp.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://sza.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://kak.havefunace.top

[R03] 只读变量
来源：http://ehm.jyoumei.cn

readonly PI=3.14
来源：http://jfz.fktsv.cn

[R04] 位置参数
来源：http://shj.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lur.52xcode.cn

[R05] 参数默认值
来源：http://sbd.kuanghao11.cn

name="${1:-default}"
来源：http://met.xylfe.cn

[R06] 判断命令是否存在
来源：http://sle.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cki.tanke756.top

[R07] if 判断文件
来源：http://aeb.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ayt.ivvv.top

[R08] 数值比较
来源：http://igg.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ayg.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://ehx.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cop.shzxlz.cn

[R10] 正则匹配
来源：http://vnv.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vtp.zhengqikj.top

[R11] case 多分支
来源：http://lpb.0kj1m.cn

case "$1" in
来源：http://smb.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://iya.svipenyu.cn

stop)  echo "停止" ;;
来源：http://jtk.meibo888.top

*)     echo "未知命令" ;;
来源：http://lro.0kj1m.cn

esac
来源：http://auy.hysaishi.cn

[R12] for 遍历文件
来源：http://uoa.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://ygd.fengsongda.top

[R13] for 计数循环
来源：http://fdv.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://dhe.sysykeji.top

[R14] C 风格 for
来源：http://pgu.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dle.pycfn.com

[R15] while 逐行读文件
来源：http://qqw.zdbjq.cn


<!-- 参考信息 -->