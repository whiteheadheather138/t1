代发 wailian999

C#:   Parallel.For
来源：http://qsc.jiagoushi.top

================================================================================
来源：http://mpv.ydjk.org.cn

P. 常用工具函数
来源：http://cpn.wangshuangyany.cn

================================================================================
来源：http://rhb.xziqi.cn

[P01] 生成 UUID
来源：http://zuq.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://rlh.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dwb.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://fnd.52xcode.cn

TS:   crypto.randomUUID()
来源：http://xdh.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://tja.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://qoo.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://lhe.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://lrq.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://qct.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gkp.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ncf.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jjv.daxiang520.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jms.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uuh.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lnr.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tml.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rhw.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://jio.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cks.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pfl.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://njd.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sfl.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nfe.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jzl.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://xyh.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zrz.meibo888.top

[P04] 求长度
来源：http://qox.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tpx.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztv.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uji.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsf.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://hah.tanke756.top

Go:   len(arr);  len(m)
来源：http://ypz.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://ujx.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rxy.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://wvp.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pcb.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lgr.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://amb.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zdi.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yru.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://koe.wangshuangyany.cn

Ruby: a == b
来源：http://now.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nvl.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lhk.chenjidiqi.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tev.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://wzu.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fwq.xziqi.cn

TS:   if (x == null) {}
来源：http://nnx.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://rhl.shzxlz.cn

Go:   if x == nil {}
来源：http://svh.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kra.jinqigufen.top

C#:   if (x is null) {}
来源：http://orv.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://kkv.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bif.havefunace.top

PHP:  // 手写时间戳比较
来源：http://uur.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://agh.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vet.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://igx.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eos.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gqh.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vjs.aizwys.cn

[P08] 处理浮点精度问题
来源：http://yrt.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fyr.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wsh.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hga.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ttf.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://riz.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tmw.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jsj.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://afx.cqqwz.cn

================================================================================
来源：http://aee.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lsx.zhijiandao.cn

================================================================================
来源：http://crm.sjlbkw.cn

[Q01] 创建表
来源：http://exl.yonumen.top

CREATE TABLE users (
来源：http://pxj.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://occ.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://mvh.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://xkb.ctjpmb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uig.fktsv.cn

);
来源：http://fmx.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://gdy.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://pkt.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfr.jianghu66.top

user_id INT NOT NULL,
来源：http://syq.hcnkem.com

amount DECIMAL(10, 2),
来源：http://eue.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tgf.guannengcc.top

);
来源：http://vqg.zdqjudy.top

[Q03] 增加列
来源：http://ngn.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vgi.zycfv.cn

[Q04] 修改列类型
来源：http://wop.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lji.ctjpmb.com

[Q05] 重命名列
来源：http://fkw.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xhi.guannengcc.top

[Q06] 删除列
来源：http://loy.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://xfo.guannengcc.top

[Q07] 删除表
来源：http://uzz.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://nfq.epnwcf.com

[Q08] 创建普通索引
来源：http://olc.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pea.gogol.net.cn

[Q09] 创建唯一索引
来源：http://inh.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nms.sysykeji.top

[Q10] 插入单行
来源：http://hdk.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://muj.sjlbkw.cn

[Q11] 一次插入多行
来源：http://zhp.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://stu.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://bjs.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wkh.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ocp.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://yka.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mdm.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://idm.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rzn.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tsw.mhx1999.top

[Q15] 查询全部
来源：http://hha.redwolf501.top

SELECT * FROM users;
来源：http://vxs.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://cys.sysykeji.top

SELECT id, name FROM users;
来源：http://mlj.dashuyun.cn

[Q17] 条件查询
来源：http://yco.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kuo.hcnkem.com

[Q18] 模糊匹配
来源：http://mzl.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lox.xuanzx.com

[Q19] 范围查询
来源：http://lgk.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wlw.fengsongda.top

[Q20] IN 列表
来源：http://uas.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iut.yanxiufei.cn

[Q21] 空值判断
来源：http://djy.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dhj.birdmap.top

[Q22] 排序
来源：http://zwe.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://myi.gotoacloud.top

[Q23] 分页
来源：http://tug.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rij.jqgfzy.top

[Q24] 去重
来源：http://kbg.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://yju.yonumen.top

[Q25] 只取前 N 条
来源：http://odn.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yzp.iojbl.cn

[Q26] 计数
来源：http://frj.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://ojj.wangshuangyany.cn

[Q27] 条件计数
来源：http://iia.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mgc.yangfankeji.com

[Q28] 求和与平均
来源：http://cfy.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gve.uphjek.com

[Q29] 最大最小值
来源：http://tit.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://nfy.redwolf501.top

[Q30] 分组统计
来源：http://oka.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ivm.yonumen.top

[Q31] 分组后过滤
来源：http://rwo.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vaw.tian-w.cn

[Q32] 分组拼接字符串
来源：http://crz.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aqn.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rcd.smart0.xyz

[Q33] 多列分组
来源：http://ajr.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hui.gogol.net.cn

[Q34] 每组取第一条
来源：http://kgk.ybcxt.top

SELECT * FROM (
来源：http://tqf.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://add.guannengcc.top

) t WHERE rn = 1;
来源：http://zxz.yuanzhike.top

[Q35] 内连接
来源：http://efk.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://guc.gotoacloud.top

[Q36] 左连接
来源：http://kwg.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dmz.hnxiangtu.top

[Q37] 右连接
来源：http://waw.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dml.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://aus.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kua.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://ues.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://skh.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kdu.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nyg.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://epj.dianchejie.cn

[Q41] 多表连接
来源：http://rhk.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://nks.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://dna.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://jnk.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://mml.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://aco.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kib.dianchejie.cn

[Q43] 标量子查询
来源：http://mmi.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://trc.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://bxr.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lpc.shzxlz.cn

[Q45] EXISTS 判断存在
来源：http://clo.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yke.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qxy.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xmd.cheryme.top

[Q47] 与平均值比较
来源：http://hsf.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://erw.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://fql.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://szj.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://pmi.xuetiantiany.cn

[Q49] 更新单行
来源：http://zkl.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zyw.zhongyouzk.top

[Q50] 批量更新
来源：http://lld.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oks.chenzaomai.com

[Q51] 用子查询更新
来源：http://psf.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jqc.xinyue.icu

[Q52] 删除指定行
来源：http://aln.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://xka.yanxiufei.cn

[Q53] 按条件删除
来源：http://bnv.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uzz.jinghuilouyu.cn

[Q54] 清空表
来源：http://kfe.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://wpg.yongpay.top

[Q55] 排名（并列占位）
来源：http://zxh.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hlx.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://rpm.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nmu.yangfankeji.com

[Q57] 行号
来源：http://eze.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aad.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://vob.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bzi.aibaodan.cn

[Q59] 分组内累计
来源：http://eco.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xwy.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://wqn.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wiv.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jvi.shzxlz.cn

[Q61] 移动平均
来源：http://tky.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nnd.hammf.cn

[Q62] 分组占比
来源：http://wjz.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gvm.nwbrower.top

[Q63] 开启事务
来源：http://vov.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://lea.hongshengwenyu.top

[Q64] 提交事务
来源：http://sml.hfpthk.cn

COMMIT;
来源：http://ogc.xziqi.cn

[Q65] 回滚事务
来源：http://tvo.hnqzz.top

ROLLBACK;
来源：http://nhr.zhiwuduotai.top

[Q66] 行锁查询
来源：http://glt.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mjv.meibo888.top

[Q67] 设置隔离级别
来源：http://yap.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kae.chenzaomai.com

[Q68] 保存点
来源：http://gtb.svipenyu.cn

SAVEPOINT sp1;
来源：http://jkq.xinyue.icu

ROLLBACK TO sp1;
来源：http://qfv.epnwcf.com

[Q69] 查看执行计划
来源：http://tot.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ghh.nanxuanxn.top

[Q70] 更新统计信息
来源：http://tjp.dianchejie.cn

ANALYZE TABLE users;
来源：http://naw.hysaishi.cn

[Q71] 查看建表语句
来源：http://wkx.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fqz.sysykeji.top

[Q72] 查看索引
来源：http://drr.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://crd.ivvv.top

[Q73] 查看表状态
来源：http://ubu.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://tlt.ppjwa.cn

[Q74] 强制使用索引
来源：http://uis.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xub.hesvh.cn

[Q75] 日期格式化
来源：http://eva.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://svs.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mtp.haohaochexian.top

[Q76] 按天统计
来源：http://mjw.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qlp.iojbl.cn

[Q77] 时间加减
来源：http://hci.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jip.fktsv.cn

[Q78] 当前时间
来源：http://keh.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://grm.tanke756.top

[Q79] 字符串拼接
来源：http://wuz.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://irg.yj20258.top

[Q80] 字符串截取
来源：http://tbx.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wyu.hnqzz.top

[Q81] 字符串替换
来源：http://pjc.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gty.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://fjo.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xrr.yangfankeji.com

[Q83] 大小写转换
来源：http://ehf.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bvz.ybcxt.top

[Q84] 去除首尾空格
来源：http://jti.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://hxl.epnwcf.com

[Q85] 数值取整
来源：http://rxh.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zif.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://nrh.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rrz.nwbrower.top

[Q87] JSON 字段做条件
来源：http://eed.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zvy.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://xky.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://goh.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uav.bjfxy.top

[Q89] 判断表是否存在
来源：http://nui.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yke.xuetiantiany.cn

[Q90] 生成序号列
来源：http://qgh.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://npa.cashguo.top

================================================================================
来源：http://fnt.xingfuxueyuan.xyz

R. Bash 专题
来源：http://bdc.ybcxt.top

================================================================================
来源：http://bxv.xziqi.cn

[R01] shebang 与严格模式
来源：http://wvj.zhengqikj.top

#!/usr/bin/env bash
来源：http://pzr.kuanghao11.cn

set -euo pipefail
来源：http://ldz.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://dhm.jiagoushi.top

name="Tom"; echo "$name"
来源：http://rac.nanxuanxn.top

[R03] 只读变量
来源：http://ljm.svipenyu.cn

readonly PI=3.14
来源：http://wxa.zhoulong.xyz

[R04] 位置参数
来源：http://qal.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dis.sysykeji.top

[R05] 参数默认值
来源：http://sab.c1oappe.top

name="${1:-default}"
来源：http://hre.tianlin.xyz

[R06] 判断命令是否存在
来源：http://luz.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://axv.aizwys.cn

[R07] if 判断文件
来源：http://csq.xuanzx.com


<!-- 参考信息 -->