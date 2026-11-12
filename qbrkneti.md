代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ghg.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zrb.cdnleiting.top

[P03] 生成短随机字符串
来源：http://swy.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mxt.guowangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gvu.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cmm.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wam.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ost.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qsn.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://slu.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://igi.jinqigfzy.top

[P04] 求长度
来源：http://afn.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://spd.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uzl.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://niu.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lws.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://ojy.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://wed.tianlin.xyz

Ruby: x.length;  x.size
来源：http://iai.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ksl.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://cbe.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xxd.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tne.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dqq.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hro.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vsr.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://mja.yanxiufei.cn

Ruby: a == b
来源：http://nrf.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mar.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ybd.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zia.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://pxv.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hjo.yvedp.cn

TS:   if (x == null) {}
来源：http://rkk.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://jvp.sxryk.cn

Go:   if x == nil {}
来源：http://ckj.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ywf.uphjek.com

C#:   if (x is null) {}
来源：http://qxu.sysykeji.top

[P07] 防抖与节流
来源：http://lxv.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sgh.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://jub.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzu.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdc.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://frx.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dze.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fwp.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kjq.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://fsb.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uzg.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qvb.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://edi.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kgn.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://byc.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tex.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://plz.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lom.xylfe.cn

================================================================================
来源：http://zcm.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ott.fktsv.cn

================================================================================
来源：http://hid.jinqigufen.top

[Q01] 创建表
来源：http://ytx.shanyushiyangtech.top

CREATE TABLE users (
来源：http://btq.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xdn.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://jhh.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://yyd.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pjp.dianchejie.cn

);
来源：http://yrv.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://zco.jqgfzy.top

CREATE TABLE orders (
来源：http://noo.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cfy.xuanzx.com

user_id INT NOT NULL,
来源：http://uge.iojbl.cn

amount DECIMAL(10, 2),
来源：http://mkn.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://afy.vehdjk.com

);
来源：http://hml.zhaomingkeji.xyz

[Q03] 增加列
来源：http://evs.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://noa.sweek.top

[Q04] 修改列类型
来源：http://qof.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://umu.sjlbkw.cn

[Q05] 重命名列
来源：http://thf.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eom.ivvv.top

[Q06] 删除列
来源：http://awl.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bpu.tarul.cn

[Q07] 删除表
来源：http://mel.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://twg.ehwqpu.com

[Q08] 创建普通索引
来源：http://vpr.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wjd.yvedp.cn

[Q09] 创建唯一索引
来源：http://phm.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rqd.zhiwuduotai.top

[Q10] 插入单行
来源：http://lnk.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xxy.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://htj.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jws.meibo888.top

[Q12] 插入后取自增 ID
来源：http://lmr.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lpr.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vtk.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://pny.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xfj.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://gfc.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yjn.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tmc.fktsv.cn

[Q15] 查询全部
来源：http://pii.hongshengwenyu.top

SELECT * FROM users;
来源：http://pzu.cheryme.top

[Q16] 查询指定列
来源：http://cbw.gotoacloud.top

SELECT id, name FROM users;
来源：http://mqg.shzxlz.cn

[Q17] 条件查询
来源：http://eax.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xxb.zhoulong.xyz

[Q18] 模糊匹配
来源：http://tpo.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qdj.tian-w.cn

[Q19] 范围查询
来源：http://qsi.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cug.gaohongyu789.top

[Q20] IN 列表
来源：http://hkp.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://igj.jinqigufen.top

[Q21] 空值判断
来源：http://ift.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qjf.hnqzz.top

[Q22] 排序
来源：http://jqa.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qrq.mhx1999.top

[Q23] 分页
来源：http://lsn.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://adg.yangfankeji.com

[Q24] 去重
来源：http://nbs.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://iqj.andypj.xyz

[Q25] 只取前 N 条
来源：http://lsw.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mgx.yvedp.cn

[Q26] 计数
来源：http://kjf.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://ius.9152youxi.cn

[Q27] 条件计数
来源：http://hor.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pco.bbcook.cn

[Q28] 求和与平均
来源：http://egx.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://moh.hfpthk.cn

[Q29] 最大最小值
来源：http://dbi.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kbk.sysykeji.top

[Q30] 分组统计
来源：http://gdb.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ifl.hfpthk.cn

[Q31] 分组后过滤
来源：http://hsd.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ztg.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://upu.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vdy.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tba.hongshengwenyu.top

[Q33] 多列分组
来源：http://ulz.sweek.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dlv.ydjk.org.cn

[Q34] 每组取第一条
来源：http://rsy.tian-w.cn

SELECT * FROM (
来源：http://sbs.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zwy.ivvv.top

) t WHERE rn = 1;
来源：http://mtx.yuanzhike.top

[Q35] 内连接
来源：http://pul.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://erh.jlsjyb.cn

[Q36] 左连接
来源：http://qtt.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jym.9152youxi.cn

[Q37] 右连接
来源：http://hss.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bln.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ioq.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://urt.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://yjp.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rgi.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mzp.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gut.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yel.guannengcc.top

[Q41] 多表连接
来源：http://fmw.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://txv.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://rpj.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://wjt.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://cri.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://upm.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vyj.sjlbkw.cn

[Q43] 标量子查询
来源：http://pbt.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zpo.ctjpmb.com

[Q44] IN 子查询
来源：http://tew.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sdu.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://xdc.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tar.ctjpmb.com

[Q46] NOT EXISTS 判断不存在
来源：http://oao.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nek.yuxming.cn

[Q47] 与平均值比较
来源：http://xjs.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lnm.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://whh.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://urm.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://boi.316326.xyz

[Q49] 更新单行
来源：http://qzg.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vdz.vehdjk.com

[Q50] 批量更新
来源：http://mko.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dbi.gotoacloud.top

[Q51] 用子查询更新
来源：http://shh.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://llm.aizwys.cn

[Q52] 删除指定行
来源：http://hpl.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://uzx.chenlongwang.top

[Q53] 按条件删除
来源：http://qsk.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kre.aizwys.cn

[Q54] 清空表
来源：http://tok.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://znx.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://pdm.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fvk.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://tvw.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gcu.jinqigufen.top

[Q57] 行号
来源：http://oph.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxf.cqqwz.cn

[Q58] 累计求和
来源：http://nta.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fsk.gogol.net.cn

[Q59] 分组内累计
来源：http://hqx.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ilz.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://jpo.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nah.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gtu.cheryme.top

[Q61] 移动平均
来源：http://bns.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fes.yfazqb.com

[Q62] 分组占比
来源：http://huu.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://npv.vehdjk.com

[Q63] 开启事务
来源：http://tnk.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lng.gotoacloud.top

[Q64] 提交事务
来源：http://cdn.ydzc1.top

COMMIT;
来源：http://gdp.hammf.cn

[Q65] 回滚事务
来源：http://qhp.yongpay.top

ROLLBACK;
来源：http://myz.pengpengdd.cyou

[Q66] 行锁查询
来源：http://jdu.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zkv.52xcode.cn

[Q67] 设置隔离级别
来源：http://jje.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://glh.epnwcf.com

[Q68] 保存点
来源：http://fjc.fengsongda.top

SAVEPOINT sp1;
来源：http://gok.cucudq.cn

ROLLBACK TO sp1;
来源：http://lrr.sufxvd.cn

[Q69] 查看执行计划
来源：http://ajd.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ooc.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://onx.redwolf501.top

ANALYZE TABLE users;
来源：http://xjc.sysykeji.top

[Q71] 查看建表语句
来源：http://dns.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tou.zhijiandao.cn

[Q72] 查看索引
来源：http://vwh.tarul.cn

SHOW INDEX FROM users;
来源：http://pja.gzhubu.top

[Q73] 查看表状态
来源：http://wxe.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://xnr.tian-w.cn

[Q74] 强制使用索引
来源：http://kxo.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hep.zhijiandao.cn

[Q75] 日期格式化
来源：http://liz.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gin.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vhn.jqgfzy.top

[Q76] 按天统计
来源：http://zaq.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qjj.yueranfly.top

[Q77] 时间加减
来源：http://rvj.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wyx.hongshengwenyu.top

[Q78] 当前时间
来源：http://hqr.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://svg.yj20258.top

[Q79] 字符串拼接
来源：http://vph.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://trb.zycfv.cn

[Q80] 字符串截取
来源：http://ogw.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nvg.yj20258.top

[Q81] 字符串替换
来源：http://caj.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zse.yj202588.top

[Q82] 字符长度与字节长度
来源：http://xfi.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://swr.ydzc1.top

[Q83] 大小写转换
来源：http://fcy.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ufs.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://xcn.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://hln.guowangkeji.top

[Q85] 数值取整
来源：http://ppc.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eju.yuanzhike.top

[Q86] 读取 JSON 字段
来源：http://uka.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vsw.vehdjk.com

[Q87] JSON 字段做条件
来源：http://xus.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://izb.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://wiz.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tih.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jwd.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://cvl.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uyk.havefunace.top

[Q90] 生成序号列
来源：http://fny.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zza.hcnkem.com

================================================================================
来源：http://yql.jqgfzy.top

R. Bash 专题
来源：http://yxq.jlsjyb.cn

================================================================================
来源：http://hpx.meibo888.top

[R01] shebang 与严格模式
来源：http://uoz.jinqigufen.top

#!/usr/bin/env bash
来源：http://niy.bbcook.cn

set -euo pipefail
来源：http://drm.snrcjt.cn

[R02] 变量赋值与使用
来源：http://tkv.birdmap.top

name="Tom"; echo "$name"
来源：http://sjl.fktsv.cn

[R03] 只读变量
来源：http://ngm.sjlbkw.cn

readonly PI=3.14
来源：http://xpz.hesvh.cn

[R04] 位置参数
来源：http://bcz.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ier.aizwys.cn

[R05] 参数默认值
来源：http://dsg.epnwcf.com

name="${1:-default}"
来源：http://pkb.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://zui.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://msq.yangfankeji.com

[R07] if 判断文件
来源：http://hld.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dnv.zdqjudy.top

[R08] 数值比较
来源：http://tcg.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ron.zhiwuduotai.top

[R09] 字符串比较
来源：http://pgq.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pjn.yonumen.top

[R10] 正则匹配
来源：http://mkd.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://acz.cheryme.top

[R11] case 多分支
来源：http://eho.jinqigfzy.top

case "$1" in
来源：http://hmg.smart0.xyz

start) echo "启动" ;;
来源：http://ypd.jiagoushi.top

stop)  echo "停止" ;;
来源：http://tmt.cheryme.top

*)     echo "未知命令" ;;
来源：http://iyr.wangdashe.top

esac
来源：http://gez.52xcode.cn

[R12] for 遍历文件
来源：http://bib.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://tau.jyoumei.cn

[R13] for 计数循环
来源：http://gds.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://juu.gotoacloud.top

[R14] C 风格 for
来源：http://omt.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://arn.hnqzz.top

[R15] while 逐行读文件
来源：http://keq.zhoulong.xyz


<!-- 参考信息 -->