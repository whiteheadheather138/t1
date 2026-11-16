代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hmt.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gcv.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bbx.chenjidiqi.icu

Ruby: // fork 块
来源：http://onk.zhijiandao.cn

C#:   Parallel.For
来源：http://alr.zhixingplan.top

================================================================================
来源：http://qhu.feifeiyinyue.top

P. 常用工具函数
来源：http://two.gotoacloud.top

================================================================================
来源：http://rfc.hnxiangtu.top

[P01] 生成 UUID
来源：http://udd.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://gzz.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bcm.mhx1999.top

JS:   crypto.randomUUID()
来源：http://bit.guannengcc.top

TS:   crypto.randomUUID()
来源：http://xow.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://kyj.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://vff.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://veb.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://ice.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://jjz.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://daw.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uyc.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gfh.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dpe.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://twn.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://doi.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hnq.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dsl.jqgfzy.top

[P03] 生成短随机字符串
来源：http://hdn.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pzx.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://snm.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oyg.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rgs.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iag.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iyx.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kru.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://atr.fktsv.cn

[P04] 求长度
来源：http://aef.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ipk.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pls.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kks.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wcm.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://tzj.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://lky.jianghu66.top

Ruby: x.length;  x.size
来源：http://gvb.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://nwg.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://lto.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qrm.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dvv.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://psf.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uqi.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lhe.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://nff.redwolf501.top

Ruby: a == b
来源：http://qrp.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ebv.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://khb.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kvo.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://myw.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vst.hnqzz.top

TS:   if (x == null) {}
来源：http://efg.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qeu.jinqigufen.top

Go:   if x == nil {}
来源：http://iyd.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sqh.dashuyun.cn

C#:   if (x is null) {}
来源：http://jpm.pengpengdd.cyou

[P07] 防抖与节流
来源：http://yse.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ter.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://sog.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mkh.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nvv.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wbo.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qbt.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aap.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bhn.wangdashe.top

[P08] 处理浮点精度问题
来源：http://ljb.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ind.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tyg.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ctf.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zgt.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qjq.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://swv.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sec.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yrs.vqdsnc.cn

================================================================================
来源：http://jux.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://skg.316326.xyz

================================================================================
来源：http://qkv.xinyue.icu

[Q01] 创建表
来源：http://nrc.bbcook.cn

CREATE TABLE users (
来源：http://lxz.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jrs.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://yac.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://hrp.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gvt.shanyushiyangkeji.top

);
来源：http://jtm.316326.xyz

[Q02] 创建带外键的表
来源：http://vet.jianghu66.top

CREATE TABLE orders (
来源：http://ltq.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://txv.vqdsnc.cn

user_id INT NOT NULL,
来源：http://wbd.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://yqh.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wci.gaohongyu789.top

);
来源：http://qot.epnwcf.com

[Q03] 增加列
来源：http://lxn.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qwy.c1oappe.top

[Q04] 修改列类型
来源：http://deb.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wwv.hysaishi.cn

[Q05] 重命名列
来源：http://kbg.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tvu.fehbvm.com

[Q06] 删除列
来源：http://rng.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://jcn.sufxvd.cn

[Q07] 删除表
来源：http://vyj.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://jen.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://zsp.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qxf.yfazqb.com

[Q09] 创建唯一索引
来源：http://ryw.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zth.cdnleiting.top

[Q10] 插入单行
来源：http://awg.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eae.zdbjq.cn

[Q11] 一次插入多行
来源：http://alk.yueranfly.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bwv.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://mej.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://uul.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hiq.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://ecc.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqn.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://wtb.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://srq.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qdf.hywenlv.cn

[Q15] 查询全部
来源：http://xcm.yj20258.top

SELECT * FROM users;
来源：http://vvs.cashguo.top

[Q16] 查询指定列
来源：http://axt.quarkkingdee.top

SELECT id, name FROM users;
来源：http://fhe.wangshuangyany.cn

[Q17] 条件查询
来源：http://ivl.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://azo.xziqi.cn

[Q18] 模糊匹配
来源：http://hwr.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rsp.havefunace.top

[Q19] 范围查询
来源：http://yng.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bpw.ppjwa.cn

[Q20] IN 列表
来源：http://jbs.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fsd.fengsongda.top

[Q21] 空值判断
来源：http://nhn.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://qgd.fanxiaobao.xyz

[Q22] 排序
来源：http://dzb.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eif.yongpay.top

[Q23] 分页
来源：http://cid.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://esz.zhixingplan.top

[Q24] 去重
来源：http://ovk.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://kbh.yueranfly.top

[Q25] 只取前 N 条
来源：http://qsq.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qsu.yvedp.cn

[Q26] 计数
来源：http://hhc.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://syv.9152youxi.cn

[Q27] 条件计数
来源：http://fwt.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://opi.cucudq.cn

[Q28] 求和与平均
来源：http://juf.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nrn.0kj1m.cn

[Q29] 最大最小值
来源：http://ija.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://amr.dianchejie.cn

[Q30] 分组统计
来源：http://jnv.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wzz.havefunace.top

[Q31] 分组后过滤
来源：http://oro.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njn.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://fxl.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cml.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rlj.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://vum.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qcu.vehdjk.com

[Q34] 每组取第一条
来源：http://oej.daxiang520.top

SELECT * FROM (
来源：http://oxm.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uen.hammf.cn

) t WHERE rn = 1;
来源：http://bhr.aibaodan.cn

[Q35] 内连接
来源：http://ufi.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pau.zhoulong.xyz

[Q36] 左连接
来源：http://cqd.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ltb.svipenyu.cn

[Q37] 右连接
来源：http://rfr.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://piq.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://ety.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sew.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://nfv.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uzd.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bcv.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tie.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lvz.sufxvd.cn

[Q41] 多表连接
来源：http://ayb.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pfh.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://jeo.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://ozd.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://iql.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://bum.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fma.daxiang520.top

[Q43] 标量子查询
来源：http://jtq.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lmm.cdnleiting.top

[Q44] IN 子查询
来源：http://bpm.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aao.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://rxo.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://one.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://rvz.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uca.pycfn.com

[Q47] 与平均值比较
来源：http://lom.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyv.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://iec.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lcp.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://ebs.jinqigufen.top

[Q49] 更新单行
来源：http://sgz.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yox.jqgfzy.top

[Q50] 批量更新
来源：http://gbp.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ttp.ivvv.top

[Q51] 用子查询更新
来源：http://fyt.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lkq.hongshengwenyu.top

[Q52] 删除指定行
来源：http://iwv.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://mrd.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://usk.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://khx.zycfv.cn

[Q54] 清空表
来源：http://klx.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://lla.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://iuf.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wvc.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://uth.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ulz.xuanzx.com

[Q57] 行号
来源：http://hdn.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ipd.shuidangran.top

[Q58] 累计求和
来源：http://ggt.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xcg.jianghu66.top

[Q59] 分组内累计
来源：http://sbd.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fgp.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://lhy.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aaj.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vot.jinghuilouyu.cn

[Q61] 移动平均
来源：http://ows.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oqq.snrcjt.cn

[Q62] 分组占比
来源：http://xwy.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ell.aizwys.cn

[Q63] 开启事务
来源：http://hvm.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tlw.ydjk.org.cn

[Q64] 提交事务
来源：http://sdk.hcnkem.com

COMMIT;
来源：http://xhp.nanxuanxn.top

[Q65] 回滚事务
来源：http://awu.shangyingyoupin.top

ROLLBACK;
来源：http://cxh.pycfn.com

[Q66] 行锁查询
来源：http://ift.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dhu.xylfe.cn

[Q67] 设置隔离级别
来源：http://nfa.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kjq.shanyushiyangtech.top

[Q68] 保存点
来源：http://ovy.vqdsnc.cn

SAVEPOINT sp1;
来源：http://huw.tanke756.top

ROLLBACK TO sp1;
来源：http://gjc.nanxuanxn.top

[Q69] 查看执行计划
来源：http://ilr.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bhd.yj20258888.top

[Q70] 更新统计信息
来源：http://udw.yuxming.cn

ANALYZE TABLE users;
来源：http://jif.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://qxn.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xdq.hnxiangtu.top

[Q72] 查看索引
来源：http://kat.cheryme.top

SHOW INDEX FROM users;
来源：http://duw.tian-w.cn

[Q73] 查看表状态
来源：http://nlw.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hwn.svipenyu.cn

[Q74] 强制使用索引
来源：http://rux.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hmn.yj20258888.top

[Q75] 日期格式化
来源：http://zio.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qlq.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qlu.sweek.top

[Q76] 按天统计
来源：http://sud.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gkk.hesvh.cn

[Q77] 时间加减
来源：http://hhj.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lpu.yj202588.top

[Q78] 当前时间
来源：http://qca.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://efe.wangdashe.top

[Q79] 字符串拼接
来源：http://xcu.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bwl.pycfn.com

[Q80] 字符串截取
来源：http://uxf.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lpb.jqgfzy.top

[Q81] 字符串替换
来源：http://xtk.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ibd.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://qth.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pqt.chenlongwang.top

[Q83] 大小写转换
来源：http://ucl.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ezs.ctjpmb.com

[Q84] 去除首尾空格
来源：http://xsn.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://zhp.dianchejie.cn

[Q85] 数值取整
来源：http://cez.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bkq.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://wmn.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vsf.52xcode.cn

[Q87] JSON 字段做条件
来源：http://axz.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qco.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://wgc.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ubk.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://euq.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://fzr.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://frk.yj20258888.top

[Q90] 生成序号列
来源：http://wop.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mjx.wangshuangyany.cn

================================================================================
来源：http://nht.zdqjudy.top

R. Bash 专题
来源：http://xrq.zhengqikj.top

================================================================================
来源：http://gdt.yuanzhike.top

[R01] shebang 与严格模式
来源：http://cvi.hcnkem.com

#!/usr/bin/env bash
来源：http://qkj.yfazqb.com

set -euo pipefail
来源：http://elk.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://hwd.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://hgt.guannengcc.top

[R03] 只读变量
来源：http://nnd.zhengqikj.top

readonly PI=3.14
来源：http://sgm.zhongyouzk.top

[R04] 位置参数
来源：http://awp.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zto.vehdjk.com

[R05] 参数默认值
来源：http://izk.yvedp.cn


<!-- 参考信息 -->