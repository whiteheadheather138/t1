代发 wailian999

[P01] 生成 UUID
来源：http://yyk.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://jsi.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jbb.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://uqw.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://tlj.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://way.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://uib.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://nyw.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://fbz.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://jzi.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ktd.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://trz.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lef.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://djs.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://suy.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qxh.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lac.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qjy.hysaishi.cn

[P03] 生成短随机字符串
来源：http://amu.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://axj.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aiv.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nzz.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pfc.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fov.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ffk.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ayn.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dgn.wangdashe.top

[P04] 求长度
来源：http://asc.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://szq.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tpw.smart0.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hud.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bzh.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://bkk.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://dxk.daria6918.cn

Ruby: x.length;  x.size
来源：http://nra.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cvs.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://xmu.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://csz.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jax.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rou.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://itn.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vbo.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qnn.yueranfly.top

Ruby: a == b
来源：http://wwy.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gzd.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kqd.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nsu.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://oqm.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mlj.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://som.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xbv.hysaishi.cn

Go:   if x == nil {}
来源：http://eiv.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://egh.tian-w.cn

C#:   if (x is null) {}
来源：http://gnf.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://fsw.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tlr.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://ple.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvl.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfd.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qan.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dut.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mfz.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nly.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://sja.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yvl.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://beq.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zjb.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wns.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wdi.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yzx.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cll.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zeq.jinqigfzy.top

================================================================================
来源：http://wxe.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mjw.tianlin.xyz

================================================================================
来源：http://qip.jyoumei.cn

[Q01] 创建表
来源：http://iox.jqgfzy.top

CREATE TABLE users (
来源：http://ikl.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://smi.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://vxm.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://ocm.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tra.fehbvm.com

);
来源：http://ikw.jyoumei.cn

[Q02] 创建带外键的表
来源：http://afj.xingfuxueyuan.xyz

CREATE TABLE orders (
来源：http://hgf.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ekn.cucudq.cn

user_id INT NOT NULL,
来源：http://vml.xuanzx.com

amount DECIMAL(10, 2),
来源：http://fwq.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ctc.kuanghao11.cn

);
来源：http://rpc.jqgufenzy.top

[Q03] 增加列
来源：http://rbn.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mmm.meibo888.top

[Q04] 修改列类型
来源：http://jik.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yay.jinqigfzy.top

[Q05] 重命名列
来源：http://lnf.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqv.pengpengdd.cyou

[Q06] 删除列
来源：http://rie.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://six.svipenyu.cn

[Q07] 删除表
来源：http://qbc.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://ctc.gaohongyu789.top

[Q08] 创建普通索引
来源：http://miy.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ezo.yonumen.top

[Q09] 创建唯一索引
来源：http://wmw.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vjg.xylfe.cn

[Q10] 插入单行
来源：http://ycy.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ttv.jianghu66.top

[Q11] 一次插入多行
来源：http://sri.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xsy.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://ica.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://uxc.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fkb.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://ead.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fev.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://haq.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://frw.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gzu.xylfe.cn

[Q15] 查询全部
来源：http://dac.fanxiaobao.xyz

SELECT * FROM users;
来源：http://ttn.shzxlz.cn

[Q16] 查询指定列
来源：http://gvg.yfazqb.com

SELECT id, name FROM users;
来源：http://bde.cashguo.top

[Q17] 条件查询
来源：http://ogo.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://buw.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://hsg.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blz.xinyue.icu

[Q19] 范围查询
来源：http://ssj.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://trt.ehwqpu.com

[Q20] IN 列表
来源：http://hev.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eni.sxryk.cn

[Q21] 空值判断
来源：http://znx.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fxg.sjlbkw.cn

[Q22] 排序
来源：http://avr.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zuj.jinqigufen.top

[Q23] 分页
来源：http://yzy.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bmm.9152youxi.cn

[Q24] 去重
来源：http://rml.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://oki.yj202588.top

[Q25] 只取前 N 条
来源：http://pwm.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vgh.aibaodan.cn

[Q26] 计数
来源：http://ufu.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://sis.epnwcf.com

[Q27] 条件计数
来源：http://fjy.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lok.jqgufenzy.top

[Q28] 求和与平均
来源：http://wld.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cww.hesvh.cn

[Q29] 最大最小值
来源：http://ces.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yag.0kj1m.cn

[Q30] 分组统计
来源：http://jxr.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ink.cucudq.cn

[Q31] 分组后过滤
来源：http://qwl.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zma.hcnkem.com

[Q32] 分组拼接字符串
来源：http://cch.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wct.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eal.jinqigufen.top

[Q33] 多列分组
来源：http://vvr.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hqd.quarkkingdee.top

[Q34] 每组取第一条
来源：http://rcg.sweek.top

SELECT * FROM (
来源：http://viu.jiagoushi.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bsm.zdbjq.cn

) t WHERE rn = 1;
来源：http://lzs.jqgufenzy.top

[Q35] 内连接
来源：http://qhp.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://foq.xylfe.cn

[Q36] 左连接
来源：http://ufd.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vaq.bjfxy.top

[Q37] 右连接
来源：http://lzl.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gcj.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://com.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://szy.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://lzx.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oxe.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fga.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uhy.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xjp.mhx1999.top

[Q41] 多表连接
来源：http://ehz.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://lul.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://gbr.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://zdw.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://cir.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://zkf.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kfs.yangfankeji.com

[Q43] 标量子查询
来源：http://oav.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ery.redwolf501.top

[Q44] IN 子查询
来源：http://vuh.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ryz.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://hde.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azz.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jzu.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bnj.meibo888.top

[Q47] 与平均值比较
来源：http://aqb.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fqa.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://cuu.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fzr.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://sys.hammf.cn

[Q49] 更新单行
来源：http://hst.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nsm.jqgufenzy.top

[Q50] 批量更新
来源：http://ndk.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qoj.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://rkc.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bqp.wangshuangyany.cn

[Q52] 删除指定行
来源：http://vzm.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://gws.zhijiandao.cn

[Q53] 按条件删除
来源：http://bxo.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xyx.jianghu66.top

[Q54] 清空表
来源：http://ogd.ivvv.top

TRUNCATE TABLE logs;
来源：http://wyt.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://ptz.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mgl.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://vvd.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gob.guowangkeji.top

[Q57] 行号
来源：http://uac.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fcv.jiagoushi.top

[Q58] 累计求和
来源：http://jmv.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sjt.feifeiyinyue.top

[Q59] 分组内累计
来源：http://qvf.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ket.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://xxk.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://apw.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cec.yuanzhike.top

[Q61] 移动平均
来源：http://cyc.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mxk.hnqzz.top

[Q62] 分组占比
来源：http://sur.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gbr.shanyushiyangtech.top

[Q63] 开启事务
来源：http://ziw.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tgv.zdqjudy.top

[Q64] 提交事务
来源：http://dny.zhiwuduotai.top

COMMIT;
来源：http://hmy.ivvv.top

[Q65] 回滚事务
来源：http://bdb.quarkkingdee.top

ROLLBACK;
来源：http://rap.bjfxy.top

[Q66] 行锁查询
来源：http://aos.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://slp.cashguo.top

[Q67] 设置隔离级别
来源：http://yof.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hhf.sufxvd.cn

[Q68] 保存点
来源：http://gby.0kj1m.cn

SAVEPOINT sp1;
来源：http://qih.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://jle.yj20258.top

[Q69] 查看执行计划
来源：http://bqh.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dyc.tarul.cn

[Q70] 更新统计信息
来源：http://qmu.daxiang520.top

ANALYZE TABLE users;
来源：http://qdv.gaohongyu789.top

[Q71] 查看建表语句
来源：http://jnb.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mvc.yuxming.cn

[Q72] 查看索引
来源：http://ujk.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://jvx.vehdjk.com

[Q73] 查看表状态
来源：http://qis.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vod.yj202588.top

[Q74] 强制使用索引
来源：http://fbc.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uwx.meibo888.top

[Q75] 日期格式化
来源：http://mfj.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yut.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kud.chenzaomai.com

[Q76] 按天统计
来源：http://fvl.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mst.sjlbkw.cn

[Q77] 时间加减
来源：http://mnq.fengsongda.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ipj.wangdashe.top

[Q78] 当前时间
来源：http://ooi.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gzl.fengsongda.top

[Q79] 字符串拼接
来源：http://zuj.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://szt.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://gct.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tdg.xuetiantiany.cn

[Q81] 字符串替换
来源：http://ogw.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rwi.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://obt.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vff.zhoulong.xyz

[Q83] 大小写转换
来源：http://ifx.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oqm.shuidangran.top

[Q84] 去除首尾空格
来源：http://ivi.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://ftd.xuanzx.com

[Q85] 数值取整
来源：http://mor.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rco.tanke756.top

[Q86] 读取 JSON 字段
来源：http://hja.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wrn.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://vxk.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jpn.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://jtx.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uem.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://med.gzhubu.top

[Q89] 判断表是否存在
来源：http://gpb.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pxt.gogol.net.cn

[Q90] 生成序号列
来源：http://knr.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qdp.ehwqpu.com

================================================================================
来源：http://hrm.nanxuanxn.top

R. Bash 专题
来源：http://gyr.chenzaomai.com

================================================================================
来源：http://ksy.dashuyun.cn

[R01] shebang 与严格模式
来源：http://rjp.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://eel.yj20258.top

set -euo pipefail
来源：http://wuc.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://wpt.hfpthk.cn

name="Tom"; echo "$name"
来源：http://aql.yonumen.top

[R03] 只读变量
来源：http://ofb.svipenyu.cn

readonly PI=3.14
来源：http://jir.snrcjt.cn

[R04] 位置参数
来源：http://umx.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ibc.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://hvk.vehdjk.com

name="${1:-default}"
来源：http://ays.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://iiv.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qwy.cdnleiting.top

[R07] if 判断文件
来源：http://wby.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kxj.fzhhl.top

[R08] 数值比较
来源：http://egh.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rzr.sweek.top

[R09] 字符串比较
来源：http://hmc.yj20258888.top


<!-- 参考信息 -->