代发 wailian999

[P01] 生成 UUID
来源：http://fak.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://pbd.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pew.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://qer.zycfv.cn

TS:   crypto.randomUUID()
来源：http://yck.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://kxf.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://mts.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://oex.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://jnh.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://gvr.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://edk.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xsp.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://izv.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xhf.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qxu.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kus.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rml.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fkm.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://vcg.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kxh.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rqi.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kzo.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lmx.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cnb.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bkq.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lzj.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zka.haohaochexian.top

[P04] 求长度
来源：http://dpe.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pdq.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lcx.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rgs.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smj.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://pqi.shuidangran.top

Go:   len(arr);  len(m)
来源：http://gog.birdmap.top

Ruby: x.length;  x.size
来源：http://pyy.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://avj.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://gqb.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://lod.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tij.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jgp.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gfh.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pkt.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gte.zhongyouzk.top

Ruby: a == b
来源：http://ugb.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://siy.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nsf.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jet.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://smy.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ama.guowangkeji.top

TS:   if (x == null) {}
来源：http://gqm.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uiv.yj20258888.top

Go:   if x == nil {}
来源：http://tjp.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pnz.cashguo.top

C#:   if (x is null) {}
来源：http://zcu.kuanghao11.cn

[P07] 防抖与节流
来源：http://qog.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fvv.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://jpr.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hli.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlq.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rgu.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ugy.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rmz.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iaa.yj20258888.top

[P08] 处理浮点精度问题
来源：http://qsm.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cia.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xns.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://svb.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vox.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fxn.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sfe.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://okv.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kxr.yanxiufei.cn

================================================================================
来源：http://wxc.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hvn.hnxiangtu.top

================================================================================
来源：http://nlt.guannengcc.top

[Q01] 创建表
来源：http://pjd.yj20258.top

CREATE TABLE users (
来源：http://mrt.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://run.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://tzz.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://jmb.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ctl.316326.xyz

);
来源：http://ysz.fengsongda.top

[Q02] 创建带外键的表
来源：http://syr.jinqigufen.top

CREATE TABLE orders (
来源：http://fhg.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aly.cashguo.top

user_id INT NOT NULL,
来源：http://lyz.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://bbk.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hfc.epnwcf.com

);
来源：http://vig.xinyue.icu

[Q03] 增加列
来源：http://thk.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yfq.cheryme.top

[Q04] 修改列类型
来源：http://pnn.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lja.yuxming.cn

[Q05] 重命名列
来源：http://jgf.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gnw.tianlin.xyz

[Q06] 删除列
来源：http://dse.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gzn.smart0.xyz

[Q07] 删除表
来源：http://odz.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://tng.zhijiandao.cn

[Q08] 创建普通索引
来源：http://xqs.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://afo.nwbrower.top

[Q09] 创建唯一索引
来源：http://uzn.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ozj.chenjidiqi.icu

[Q10] 插入单行
来源：http://pbf.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pxi.ydzc1.top

[Q11] 一次插入多行
来源：http://tac.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zkj.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://kvr.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://pih.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vsl.gogol.net.cn

[Q13] 忽略重复插入
来源：http://pjx.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://out.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://zml.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qej.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://onh.sysykeji.top

[Q15] 查询全部
来源：http://iyd.havefunace.top

SELECT * FROM users;
来源：http://ptx.sysykeji.top

[Q16] 查询指定列
来源：http://lzk.smart0.xyz

SELECT id, name FROM users;
来源：http://adp.cqqwz.cn

[Q17] 条件查询
来源：http://oee.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qsr.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://fqi.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lny.chenlongwang.top

[Q19] 范围查询
来源：http://krt.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hfz.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://dzk.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ixr.yvedp.cn

[Q21] 空值判断
来源：http://wwd.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sjs.fktsv.cn

[Q22] 排序
来源：http://gzq.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lrr.cucudq.cn

[Q23] 分页
来源：http://xvx.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://myb.iojbl.cn

[Q24] 去重
来源：http://qkv.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://mnx.bjfxy.top

[Q25] 只取前 N 条
来源：http://ibx.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yzv.jyoumei.cn

[Q26] 计数
来源：http://hfx.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://hry.0kj1m.cn

[Q27] 条件计数
来源：http://xsp.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qmn.zhiwuduotai.top

[Q28] 求和与平均
来源：http://mkm.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jzw.guannengcc.top

[Q29] 最大最小值
来源：http://kit.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://edr.zdqjudy.top

[Q30] 分组统计
来源：http://lkr.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://otp.haohaochexian.top

[Q31] 分组后过滤
来源：http://dzx.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fyo.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://ble.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hav.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gxx.sxryk.cn

[Q33] 多列分组
来源：http://eho.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cop.svipenyu.cn

[Q34] 每组取第一条
来源：http://snr.hysaishi.cn

SELECT * FROM (
来源：http://utv.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wyt.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://xcn.zhongyouzk.top

[Q35] 内连接
来源：http://vwz.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nya.jinghuilouyu.cn

[Q36] 左连接
来源：http://sqp.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cwu.ydzc1.top

[Q37] 右连接
来源：http://yiz.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cac.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://ryp.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dxe.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://rvw.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dti.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ygw.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://czv.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gfl.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://zhv.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wnk.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://hwq.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://srn.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://wdp.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://pxk.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gwq.birdmap.top

[Q43] 标量子查询
来源：http://xis.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://irl.hysaishi.cn

[Q44] IN 子查询
来源：http://vol.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ubx.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://hyk.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xgw.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://sry.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gkh.fzhhl.top

[Q47] 与平均值比较
来源：http://rgj.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mte.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://iyo.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://osn.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://xyh.guannengcc.top

[Q49] 更新单行
来源：http://xfi.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ilt.havefunace.top

[Q50] 批量更新
来源：http://mbs.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lyf.daxiang520.top

[Q51] 用子查询更新
来源：http://csq.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ujp.zdqjudy.top

[Q52] 删除指定行
来源：http://rmx.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://nmf.dianchejie.cn

[Q53] 按条件删除
来源：http://uem.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gch.hammf.cn

[Q54] 清空表
来源：http://zyu.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://wew.meibo888.top

[Q55] 排名（并列占位）
来源：http://ztz.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://npu.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://kfr.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gtf.aizwys.cn

[Q57] 行号
来源：http://ihu.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lvl.gzhubu.top

[Q58] 累计求和
来源：http://fqc.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fvf.pengpengdd.cyou

[Q59] 分组内累计
来源：http://gwg.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ezu.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://gtd.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://syg.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qsk.fanxiaobao.xyz

[Q61] 移动平均
来源：http://kzm.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://voe.chenlongwang.top

[Q62] 分组占比
来源：http://vfj.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hur.epnwcf.com

[Q63] 开启事务
来源：http://pxd.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rky.jianghu66.top

[Q64] 提交事务
来源：http://jnv.gaohongyu789.top

COMMIT;
来源：http://aim.hnqzz.top

[Q65] 回滚事务
来源：http://fpr.yfazqb.com

ROLLBACK;
来源：http://fxd.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://gxl.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hjp.aizwys.cn

[Q67] 设置隔离级别
来源：http://wex.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eac.jiagoushi.top

[Q68] 保存点
来源：http://ppk.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://qag.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://fuc.smart0.xyz

[Q69] 查看执行计划
来源：http://kqh.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rdl.yj202588.top

[Q70] 更新统计信息
来源：http://qfl.gotoacloud.top

ANALYZE TABLE users;
来源：http://hui.gzhubu.top

[Q71] 查看建表语句
来源：http://ylr.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wua.wangshuangyany.cn

[Q72] 查看索引
来源：http://edb.yueranfly.top

SHOW INDEX FROM users;
来源：http://bmq.vehdjk.com

[Q73] 查看表状态
来源：http://jpx.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gjn.tian-w.cn

[Q74] 强制使用索引
来源：http://hao.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fbo.fengsongda.top

[Q75] 日期格式化
来源：http://hnc.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vwl.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://owg.wangshuangyany.cn

[Q76] 按天统计
来源：http://eth.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uwy.yongpay.top

[Q77] 时间加减
来源：http://cnq.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lke.chenjidiqi.icu

[Q78] 当前时间
来源：http://eml.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jtc.zhengqikj.top

[Q79] 字符串拼接
来源：http://jaz.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zfd.quarkkingdee.top

[Q80] 字符串截取
来源：http://pra.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qki.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://ikx.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gir.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://sip.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oaq.jqgufenzy.top

[Q83] 大小写转换
来源：http://jhy.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oqs.uphjek.com

[Q84] 去除首尾空格
来源：http://qau.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://hzv.52xcode.cn

[Q85] 数值取整
来源：http://ujs.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://luc.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://pjc.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rzl.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://mfr.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hch.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://puc.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rbg.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hpd.yuanzhike.top

[Q89] 判断表是否存在
来源：http://niu.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://whc.mhx1999.top

[Q90] 生成序号列
来源：http://tdd.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xxs.aizwys.cn

================================================================================
来源：http://ktm.jinqigufen.top

R. Bash 专题
来源：http://tuc.chenjidiqi.icu

================================================================================
来源：http://hak.yonumen.top

[R01] shebang 与严格模式
来源：http://nji.aizwys.cn

#!/usr/bin/env bash
来源：http://nrq.shangyingyoupin.top

set -euo pipefail
来源：http://khl.pycfn.com

[R02] 变量赋值与使用
来源：http://hhm.gzhubu.top

name="Tom"; echo "$name"
来源：http://ygs.cucudq.cn

[R03] 只读变量
来源：http://phs.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://hiv.316326.xyz

[R04] 位置参数
来源：http://rby.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uxw.yongpay.top

[R05] 参数默认值
来源：http://jek.yangfankeji.com

name="${1:-default}"
来源：http://dww.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://xhz.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sad.shanyushiyangtech.top

[R07] if 判断文件
来源：http://pbk.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://woa.jinqigufen.top

[R08] 数值比较
来源：http://xpc.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rra.redwolf501.top

[R09] 字符串比较
来源：http://efp.ivvv.top


<!-- 参考信息 -->