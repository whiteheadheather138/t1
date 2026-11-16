代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hxo.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kgy.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uck.zhixingplan.top

Ruby: // fork 块
来源：http://xdy.gotoacloud.top

C#:   Parallel.For
来源：http://bng.hywenlv.cn

================================================================================
来源：http://ths.pengpengdd.cyou

P. 常用工具函数
来源：http://xwx.iojbl.cn

================================================================================
来源：http://wgp.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://kah.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://gnx.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zxd.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://hrr.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://jmo.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://zsu.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://vgf.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://hdy.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://ime.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://aoe.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zpk.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hpi.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rqu.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ibd.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xvb.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qfx.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wzo.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://daa.meibo888.top

[P03] 生成短随机字符串
来源：http://tnl.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sqv.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mju.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://omq.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pcm.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://abw.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sbw.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nuj.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kjl.wangshuangyany.cn

[P04] 求长度
来源：http://tpa.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kee.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tel.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qit.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blh.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://vev.zycfv.cn

Go:   len(arr);  len(m)
来源：http://iuu.hfpthk.cn

Ruby: x.length;  x.size
来源：http://iur.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cqc.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://qjv.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lfg.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kcz.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bjk.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://riz.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dzj.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://fhc.yj202588.top

Ruby: a == b
来源：http://xjt.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wrh.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oee.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vwf.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://gqn.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kwu.fzhhl.top

TS:   if (x == null) {}
来源：http://xnt.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bjz.yanxiufei.cn

Go:   if x == nil {}
来源：http://gbw.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hqh.sjlbkw.cn

C#:   if (x is null) {}
来源：http://ilz.zdbjq.cn

[P07] 防抖与节流
来源：http://olt.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yoq.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://xko.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwz.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vna.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mtw.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nin.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gmu.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pww.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://yci.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xtg.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fbk.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oyr.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yfq.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ubs.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ybr.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://snj.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mlo.c1oappe.top

================================================================================
来源：http://agr.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ogp.zhengqikj.top

================================================================================
来源：http://orc.yanxiufei.cn

[Q01] 创建表
来源：http://rtp.xziqi.cn

CREATE TABLE users (
来源：http://mvh.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oik.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://zzj.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://ryp.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ekz.hysaishi.cn

);
来源：http://vwn.xylfe.cn

[Q02] 创建带外键的表
来源：http://qrk.jinqigfzy.top

CREATE TABLE orders (
来源：http://cus.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ddd.chenzaomai.com

user_id INT NOT NULL,
来源：http://eag.xylfe.cn

amount DECIMAL(10, 2),
来源：http://ztg.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xqk.ydjk.org.cn

);
来源：http://pwf.meibo888.top

[Q03] 增加列
来源：http://qfo.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lum.yongpay.top

[Q04] 修改列类型
来源：http://cam.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mzm.smart0.xyz

[Q05] 重命名列
来源：http://cql.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hjh.fengsongda.top

[Q06] 删除列
来源：http://lqg.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zmy.shanyushiyangtech.top

[Q07] 删除表
来源：http://vxv.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://gkp.tian-w.cn

[Q08] 创建普通索引
来源：http://enf.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://isj.sweek.top

[Q09] 创建唯一索引
来源：http://uxp.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nmc.cdnleiting.top

[Q10] 插入单行
来源：http://buh.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ybh.vqdsnc.cn

[Q11] 一次插入多行
来源：http://res.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zpi.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://yff.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ugz.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dyh.havefunace.top

[Q13] 忽略重复插入
来源：http://tpr.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ynr.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://yfr.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lrp.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oay.sufxvd.cn

[Q15] 查询全部
来源：http://lui.0kj1m.cn

SELECT * FROM users;
来源：http://uah.andypj.xyz

[Q16] 查询指定列
来源：http://mrd.chenzaomai.com

SELECT id, name FROM users;
来源：http://uei.316326.xyz

[Q17] 条件查询
来源：http://tbw.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wyf.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://mdl.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jzm.fktsv.cn

[Q19] 范围查询
来源：http://qjc.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bxv.quarkkingdee.top

[Q20] IN 列表
来源：http://gfz.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tug.xinyue.icu

[Q21] 空值判断
来源：http://ldx.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xax.vehdjk.com

[Q22] 排序
来源：http://qjc.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wqq.ybcxt.top

[Q23] 分页
来源：http://shq.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jcm.yj20258.top

[Q24] 去重
来源：http://nat.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://eur.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://lfr.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xal.hysaishi.cn

[Q26] 计数
来源：http://twk.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://sfl.tarul.cn

[Q27] 条件计数
来源：http://bmv.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sxc.tianlin.xyz

[Q28] 求和与平均
来源：http://nrw.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bpw.fktsv.cn

[Q29] 最大最小值
来源：http://fcu.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xqv.jinghuilouyu.cn

[Q30] 分组统计
来源：http://ols.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sxv.bjfxy.top

[Q31] 分组后过滤
来源：http://ogi.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ucz.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://laf.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uzz.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qot.gaohongyu789.top

[Q33] 多列分组
来源：http://zom.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uqd.bbcook.cn

[Q34] 每组取第一条
来源：http://dbx.dianchejie.cn

SELECT * FROM (
来源：http://qsd.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wyv.zhixingplan.top

) t WHERE rn = 1;
来源：http://hdq.bbcook.cn

[Q35] 内连接
来源：http://guu.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://low.ywan-chungtsiang.top

[Q36] 左连接
来源：http://ouu.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ffb.fengsongda.top

[Q37] 右连接
来源：http://tlr.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mnu.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://bvw.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lzg.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://aqw.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wtu.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xij.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fky.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jpe.hongshengwenyu.top

[Q41] 多表连接
来源：http://xjm.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://snf.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://ylp.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://jsb.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://isc.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://yys.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yss.jinqigufen.top

[Q43] 标量子查询
来源：http://lfu.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jnc.zhiwuduotai.top

[Q44] IN 子查询
来源：http://roz.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ucd.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://xab.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyx.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://btb.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://riu.yj20258.top

[Q47] 与平均值比较
来源：http://qfe.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sic.hammf.cn

[Q48] CTE 公用表表达式
来源：http://usz.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rli.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://foo.vehdjk.com

[Q49] 更新单行
来源：http://vxy.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iqb.xziqi.cn

[Q50] 批量更新
来源：http://nvi.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qaa.meibo888.top

[Q51] 用子查询更新
来源：http://xxt.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://enh.daxiang520.top

[Q52] 删除指定行
来源：http://okx.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://byp.guowangkeji.top

[Q53] 按条件删除
来源：http://cxc.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://plp.zhongyouzk.top

[Q54] 清空表
来源：http://gzd.zycfv.cn

TRUNCATE TABLE logs;
来源：http://bwi.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://pgh.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ygv.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://zjd.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ffe.hywenlv.cn

[Q57] 行号
来源：http://jib.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bio.zdqjudy.top

[Q58] 累计求和
来源：http://bnc.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eqj.zhengqikj.top

[Q59] 分组内累计
来源：http://dup.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jfc.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://lhf.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bhw.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hhu.jqgfzy.top

[Q61] 移动平均
来源：http://oni.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ele.gotoacloud.top

[Q62] 分组占比
来源：http://rpv.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cfa.xuanzx.com

[Q63] 开启事务
来源：http://abq.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gya.hfpthk.cn

[Q64] 提交事务
来源：http://yms.wangshuangyany.cn

COMMIT;
来源：http://nxt.vqdsnc.cn

[Q65] 回滚事务
来源：http://nri.0kj1m.cn

ROLLBACK;
来源：http://yyl.zhixingplan.top

[Q66] 行锁查询
来源：http://gly.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zop.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://sjf.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sst.wangshuangyany.cn

[Q68] 保存点
来源：http://woi.bbcook.cn

SAVEPOINT sp1;
来源：http://bnq.yuanzhike.top

ROLLBACK TO sp1;
来源：http://htf.hcnkem.com

[Q69] 查看执行计划
来源：http://nfr.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hiw.hywenlv.cn

[Q70] 更新统计信息
来源：http://xzg.xinyue.icu

ANALYZE TABLE users;
来源：http://kdu.yuanzhike.top

[Q71] 查看建表语句
来源：http://wbh.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://djz.yuxming.cn

[Q72] 查看索引
来源：http://vdg.hfpthk.cn

SHOW INDEX FROM users;
来源：http://avv.9152youxi.cn

[Q73] 查看表状态
来源：http://jpb.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ltj.yuxming.cn

[Q74] 强制使用索引
来源：http://yme.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wmi.daxiang520.top

[Q75] 日期格式化
来源：http://bfx.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://htw.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://afk.yanxiufei.cn

[Q76] 按天统计
来源：http://xmq.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ied.yj20258888.top

[Q77] 时间加减
来源：http://fbp.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lnl.shanyushiyangtech.top

[Q78] 当前时间
来源：http://kfm.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gxz.vehdjk.com

[Q79] 字符串拼接
来源：http://yxb.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oey.jqgufenzy.top

[Q80] 字符串截取
来源：http://xxb.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ukl.yuanzhike.top

[Q81] 字符串替换
来源：http://thx.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gqx.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://ruk.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fsd.iojbl.cn

[Q83] 大小写转换
来源：http://rvv.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ayr.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://vgk.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://pre.chenzaomai.com

[Q85] 数值取整
来源：http://lyy.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cph.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://xwx.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gap.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://bni.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oat.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://hfw.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bvd.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jwg.dianchejie.cn

[Q89] 判断表是否存在
来源：http://bpc.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://odo.bbcook.cn

[Q90] 生成序号列
来源：http://uau.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://azw.shanyushiyangtech.top

================================================================================
来源：http://jfu.hnqzz.top

R. Bash 专题
来源：http://lbd.ppjwa.cn

================================================================================
来源：http://dxo.fzhhl.top

[R01] shebang 与严格模式
来源：http://ssj.gotoacloud.top

#!/usr/bin/env bash
来源：http://bxc.snrcjt.cn

set -euo pipefail
来源：http://dgv.aizwys.cn

[R02] 变量赋值与使用
来源：http://nts.yongpay.top

name="Tom"; echo "$name"
来源：http://xiz.andypj.xyz

[R03] 只读变量
来源：http://okd.tarul.cn

readonly PI=3.14
来源：http://jco.svipenyu.cn

[R04] 位置参数
来源：http://pxd.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vmc.hfpthk.cn

[R05] 参数默认值
来源：http://che.fengsongda.top


<!-- 参考信息 -->