代发 wailian999

C#:   Parallel.For
来源：http://atv.jianghu66.top

================================================================================
来源：http://sfe.sjlbkw.cn

P. 常用工具函数
来源：http://dss.redwolf501.top

================================================================================
来源：http://efx.xylfe.cn

[P01] 生成 UUID
来源：http://mrs.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://ulz.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lzg.smart0.xyz

JS:   crypto.randomUUID()
来源：http://ykd.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://bek.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://rba.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://rhz.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://mus.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://fyq.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://rcr.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lzq.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://akq.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lrq.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fjo.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qjp.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bae.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jxo.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vrw.yfazqb.com

[P03] 生成短随机字符串
来源：http://yax.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aav.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://imu.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mlo.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ihq.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lrc.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://adk.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tsn.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ggf.zhongyouzk.top

[P04] 求长度
来源：http://hij.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mzo.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://drd.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hsg.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubh.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://lts.fzhhl.top

Go:   len(arr);  len(m)
来源：http://sen.gzhubu.top

Ruby: x.length;  x.size
来源：http://gdw.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://iae.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://roi.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pmf.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://apj.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qie.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ced.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eeu.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://txj.yuxming.cn

Ruby: a == b
来源：http://qht.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nvt.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://say.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bjt.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://alj.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rpn.xziqi.cn

TS:   if (x == null) {}
来源：http://env.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ixz.svipenyu.cn

Go:   if x == nil {}
来源：http://vdo.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://usb.zhongyouzk.top

C#:   if (x is null) {}
来源：http://dha.cashguo.top

[P07] 防抖与节流
来源：http://neg.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uxq.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://ngk.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbg.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lnb.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://atj.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pcu.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sdn.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://afm.daria6918.cn

[P08] 处理浮点精度问题
来源：http://iuh.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hpi.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fyc.cheryme.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qje.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zig.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lpn.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eal.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cpf.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dgw.shuidangran.top

================================================================================
来源：http://nrw.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zsg.chenlongwang.top

================================================================================
来源：http://mxb.nwbrower.top

[Q01] 创建表
来源：http://std.hnqzz.top

CREATE TABLE users (
来源：http://okv.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://isv.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://qix.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://qgw.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pko.sweek.top

);
来源：http://cyx.snrcjt.cn

[Q02] 创建带外键的表
来源：http://rqe.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://auj.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://anx.quarkkingdee.top

user_id INT NOT NULL,
来源：http://mul.smart0.xyz

amount DECIMAL(10, 2),
来源：http://vit.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jyn.hnqzz.top

);
来源：http://dkz.sweek.top

[Q03] 增加列
来源：http://bdf.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mev.dashuyun.cn

[Q04] 修改列类型
来源：http://pke.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kbi.nwbrower.top

[Q05] 重命名列
来源：http://mxv.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rxg.gogol.net.cn

[Q06] 删除列
来源：http://lnd.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://zmr.0kj1m.cn

[Q07] 删除表
来源：http://sqw.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://mda.nanxinkj.top

[Q08] 创建普通索引
来源：http://sah.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://txr.jyoumei.cn

[Q09] 创建唯一索引
来源：http://ald.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lax.snrcjt.cn

[Q10] 插入单行
来源：http://vvk.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fes.birdmap.top

[Q11] 一次插入多行
来源：http://jde.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xop.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://nhl.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ske.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://edp.ydzc1.top

[Q13] 忽略重复插入
来源：http://egx.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://quc.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://gxc.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gbc.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lks.tian-w.cn

[Q15] 查询全部
来源：http://ytd.tianlin.xyz

SELECT * FROM users;
来源：http://vyq.hfpthk.cn

[Q16] 查询指定列
来源：http://hgd.guannengcc.top

SELECT id, name FROM users;
来源：http://gtx.chenzaomai.com

[Q17] 条件查询
来源：http://hpk.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hqz.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://xtw.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nmc.yvedp.cn

[Q19] 范围查询
来源：http://shy.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vzz.ybcxt.top

[Q20] IN 列表
来源：http://hig.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tvh.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://bil.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ybv.redwolf501.top

[Q22] 排序
来源：http://rma.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pre.nanxinkj.top

[Q23] 分页
来源：http://jwl.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uza.dianchejie.cn

[Q24] 去重
来源：http://gpz.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://nqy.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://igs.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pnv.pycfn.com

[Q26] 计数
来源：http://diq.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://rtu.chenlongwang.top

[Q27] 条件计数
来源：http://tmg.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cpr.yanxiufei.cn

[Q28] 求和与平均
来源：http://ehm.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://civ.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://jpu.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rku.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://ywy.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ker.jinqigfzy.top

[Q31] 分组后过滤
来源：http://drf.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ggu.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://frs.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ccm.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zag.gogol.net.cn

[Q33] 多列分组
来源：http://dfa.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iiz.nanxinkj.top

[Q34] 每组取第一条
来源：http://vhs.jqgufenzy.top

SELECT * FROM (
来源：http://vgl.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xih.yangfankeji.com

) t WHERE rn = 1;
来源：http://nyj.jinqigufen.top

[Q35] 内连接
来源：http://myx.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bug.hcnkem.com

[Q36] 左连接
来源：http://gfp.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ylc.fanxiaobao.xyz

[Q37] 右连接
来源：http://ght.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uoi.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ixj.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jgm.tanke756.top

[Q39] 自连接（查上下级）
来源：http://lic.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fzs.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qja.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sfv.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fik.shanyushiyangtech.top

[Q41] 多表连接
来源：http://ohq.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://atm.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://lwv.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://ijd.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://zlr.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://iya.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ylm.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://juw.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lnx.zhiwuduotai.top

[Q44] IN 子查询
来源：http://mne.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nrn.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://qng.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qeq.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fix.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oof.yanxiufei.cn

[Q47] 与平均值比较
来源：http://pyr.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bfn.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://ckg.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hvo.guannengcc.top

SELECT * FROM t WHERE c > 5;
来源：http://iev.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://xvy.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qed.gotoacloud.top

[Q50] 批量更新
来源：http://cpn.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jet.gotoacloud.top

[Q51] 用子查询更新
来源：http://mvw.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://phb.yuanzhike.top

[Q52] 删除指定行
来源：http://coj.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://oyl.hnxiangtu.top

[Q53] 按条件删除
来源：http://bcj.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://clm.ydzc1.top

[Q54] 清空表
来源：http://sym.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://fhc.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://yya.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://edz.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://gfq.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jkj.yuanzhike.top

[Q57] 行号
来源：http://vwo.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wzf.birdmap.top

[Q58] 累计求和
来源：http://xds.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nun.nanxinkj.top

[Q59] 分组内累计
来源：http://jdc.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fal.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://del.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://psh.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oxh.jinqigufen.top

[Q61] 移动平均
来源：http://xpv.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lcl.xuetiantiany.cn

[Q62] 分组占比
来源：http://jmz.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uct.pycfn.com

[Q63] 开启事务
来源：http://nlp.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lap.feifeiyinyue.top

[Q64] 提交事务
来源：http://crq.yueranfly.top

COMMIT;
来源：http://ffj.jinqigufen.top

[Q65] 回滚事务
来源：http://qkv.nwbrower.top

ROLLBACK;
来源：http://qho.chenzaomai.com

[Q66] 行锁查询
来源：http://zlp.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://byj.shzxlz.cn

[Q67] 设置隔离级别
来源：http://plu.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kpg.bbcook.cn

[Q68] 保存点
来源：http://ptd.hcnkem.com

SAVEPOINT sp1;
来源：http://fac.9152youxi.cn

ROLLBACK TO sp1;
来源：http://lxu.yfazqb.com

[Q69] 查看执行计划
来源：http://bri.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tev.zhengqikj.top

[Q70] 更新统计信息
来源：http://mdh.chenzaomai.com

ANALYZE TABLE users;
来源：http://bir.xziqi.cn

[Q71] 查看建表语句
来源：http://gyj.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gjp.bbcook.cn

[Q72] 查看索引
来源：http://oun.ydjk.org.cn

SHOW INDEX FROM users;
来源：http://bgr.yj20258.top

[Q73] 查看表状态
来源：http://ctl.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lez.yangfankeji.com

[Q74] 强制使用索引
来源：http://jeb.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kyj.yanxiufei.cn

[Q75] 日期格式化
来源：http://xfq.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ouz.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://abw.yvedp.cn

[Q76] 按天统计
来源：http://ftx.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pak.zhijiandao.cn

[Q77] 时间加减
来源：http://qao.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xks.daxiang520.top

[Q78] 当前时间
来源：http://jao.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iky.yuxming.cn

[Q79] 字符串拼接
来源：http://jyr.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://byi.jlsjyb.cn

[Q80] 字符串截取
来源：http://jhg.hysaishi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dup.shzxlz.cn

[Q81] 字符串替换
来源：http://xwo.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kcp.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://vpd.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://btb.zycfv.cn

[Q83] 大小写转换
来源：http://rsl.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bos.shzxlz.cn

[Q84] 去除首尾空格
来源：http://bcu.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://cbh.feifeiyinyue.top

[Q85] 数值取整
来源：http://qje.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ste.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://ilx.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vqt.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://mdu.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lfn.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://dic.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tbk.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vyp.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://zfc.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://crq.jyoumei.cn

[Q90] 生成序号列
来源：http://fvs.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tel.xuetiantiany.cn

================================================================================
来源：http://qto.chenzaomai.com

R. Bash 专题
来源：http://uds.ydjk.org.cn

================================================================================
来源：http://sic.zhixingplan.top

[R01] shebang 与严格模式
来源：http://ljn.0kj1m.cn

#!/usr/bin/env bash
来源：http://gxx.hywenlv.cn

set -euo pipefail
来源：http://ewq.birdmap.top

[R02] 变量赋值与使用
来源：http://owm.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://xqn.hongshengwenyu.top

[R03] 只读变量
来源：http://awo.kuanghao11.cn

readonly PI=3.14
来源：http://pfp.wangshuangyany.cn

[R04] 位置参数
来源：http://sho.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uhv.hywenlv.cn

[R05] 参数默认值
来源：http://yhc.guowangkeji.top

name="${1:-default}"
来源：http://btl.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://swq.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xke.zhixingplan.top

[R07] if 判断文件
来源：http://fci.cqqwz.cn


<!-- 参考信息 -->