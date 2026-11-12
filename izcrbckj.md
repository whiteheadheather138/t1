代发 wailian999

C#:   Parallel.For
来源：http://bts.hnxiangtu.top

================================================================================
来源：http://ufi.yongpay.top

P. 常用工具函数
来源：http://jve.yj202588.top

================================================================================
来源：http://fbr.zhixingplan.top

[P01] 生成 UUID
来源：http://fnd.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://tgl.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wyu.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://zqj.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://vdu.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://hgx.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://nmb.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://mze.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://ksx.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://ejy.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pov.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iwb.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xou.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dpt.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nau.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xue.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://swb.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://duu.yongpay.top

[P03] 生成短随机字符串
来源：http://doj.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://abp.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lrj.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fik.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ogv.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fhw.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bzy.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qff.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://syd.yangfankeji.com

[P04] 求长度
来源：http://oom.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xxb.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rlw.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yae.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://djb.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://qfy.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://opf.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://qbs.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wig.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://nnn.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mez.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ucz.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dsm.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zns.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uey.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wcl.feifeiyinyue.top

Ruby: a == b
来源：http://bkx.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://smx.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ooj.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://quj.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://mre.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vfj.quarkkingdee.top

TS:   if (x == null) {}
来源：http://fss.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ucy.fktsv.cn

Go:   if x == nil {}
来源：http://okz.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gkz.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://ylu.quarkkingdee.top

[P07] 防抖与节流
来源：http://dey.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tsu.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://vzg.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aya.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lad.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fbv.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fkt.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://max.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gvz.bbcook.cn

[P08] 处理浮点精度问题
来源：http://rzi.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hej.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hls.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mep.ydjk.org.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://abt.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xnd.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jll.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pfc.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vvz.0kj1m.cn

================================================================================
来源：http://pzj.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://igj.wangdashe.top

================================================================================
来源：http://vxz.fktsv.cn

[Q01] 创建表
来源：http://ogw.sjlbkw.cn

CREATE TABLE users (
来源：http://abe.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://idq.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://hye.shanyushiyangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://slp.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sco.jyoumei.cn

);
来源：http://zsd.tian-w.cn

[Q02] 创建带外键的表
来源：http://vab.guannengcc.top

CREATE TABLE orders (
来源：http://aov.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ohv.iojbl.cn

user_id INT NOT NULL,
来源：http://mxp.yfazqb.com

amount DECIMAL(10, 2),
来源：http://awa.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jdr.9152youxi.cn

);
来源：http://kzd.gaohongyu789.top

[Q03] 增加列
来源：http://zwo.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jqe.vehdjk.com

[Q04] 修改列类型
来源：http://yhp.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qqp.zhengqikj.top

[Q05] 重命名列
来源：http://oew.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wfk.meibo888.top

[Q06] 删除列
来源：http://sgm.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://esl.svipenyu.cn

[Q07] 删除表
来源：http://dwl.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://kvn.jinqigfzy.top

[Q08] 创建普通索引
来源：http://bba.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ytc.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://cii.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wuv.zhengqikj.top

[Q10] 插入单行
来源：http://fjx.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://chh.sufxvd.cn

[Q11] 一次插入多行
来源：http://uhd.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xbj.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://tke.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://gzc.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jnn.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://opt.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fpf.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://ovi.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ant.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wyd.cqqwz.cn

[Q15] 查询全部
来源：http://gyo.hysaishi.cn

SELECT * FROM users;
来源：http://ypg.vqdsnc.cn

[Q16] 查询指定列
来源：http://fgs.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://oyr.shangyingyoupin.top

[Q17] 条件查询
来源：http://hfm.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kbx.birdmap.top

[Q18] 模糊匹配
来源：http://nxn.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ojp.shzxlz.cn

[Q19] 范围查询
来源：http://lcw.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eqr.nanxinkj.top

[Q20] IN 列表
来源：http://stl.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ght.cashguo.top

[Q21] 空值判断
来源：http://mza.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fvg.wangshuangyany.cn

[Q22] 排序
来源：http://xwg.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ewt.zhiwuduotai.top

[Q23] 分页
来源：http://zbz.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pqy.shangyingyoupin.top

[Q24] 去重
来源：http://fjk.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://avp.fengsongda.top

[Q25] 只取前 N 条
来源：http://jna.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hlt.jinqigfzy.top

[Q26] 计数
来源：http://bhw.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://qzi.gotoacloud.top

[Q27] 条件计数
来源：http://hob.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vco.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://oxb.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ugo.sxryk.cn

[Q29] 最大最小值
来源：http://lgo.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ddh.andypj.xyz

[Q30] 分组统计
来源：http://jnr.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://trl.gaohongyu789.top

[Q31] 分组后过滤
来源：http://fsb.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xpk.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://iip.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://htu.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://npv.birdmap.top

[Q33] 多列分组
来源：http://umy.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kwp.jinqigufen.top

[Q34] 每组取第一条
来源：http://cia.daria6918.cn

SELECT * FROM (
来源：http://uxz.chenjidiqi.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://asq.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://zcj.cashguo.top

[Q35] 内连接
来源：http://lby.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ofr.yueranfly.top

[Q36] 左连接
来源：http://jou.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://awl.52xcode.cn

[Q37] 右连接
来源：http://oiz.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lar.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nks.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jcb.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://qwh.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mbu.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ybn.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ahh.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zjw.aibaodan.cn

[Q41] 多表连接
来源：http://gfo.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yij.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://lrv.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://nic.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://fxy.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://xao.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bsz.epnwcf.com

[Q43] 标量子查询
来源：http://ogj.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hhi.gogol.net.cn

[Q44] IN 子查询
来源：http://lbf.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gjq.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://urz.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://edt.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pkm.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xvz.yuxming.cn

[Q47] 与平均值比较
来源：http://uze.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lcr.yj20258.top

[Q48] CTE 公用表表达式
来源：http://fco.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sgy.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://yuc.cqqwz.cn

[Q49] 更新单行
来源：http://mhr.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hhj.ydjk.org.cn

[Q50] 批量更新
来源：http://aoo.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cjl.epnwcf.com

[Q51] 用子查询更新
来源：http://mfc.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yym.chenlongwang.top

[Q52] 删除指定行
来源：http://rta.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://wli.jinqigfzy.top

[Q53] 按条件删除
来源：http://ygf.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dzs.jinghuilouyu.cn

[Q54] 清空表
来源：http://nlg.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://bji.sysykeji.top

[Q55] 排名（并列占位）
来源：http://dtg.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tyj.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://dil.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gsh.kuanghao11.cn

[Q57] 行号
来源：http://nzv.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ohu.guowangkeji.top

[Q58] 累计求和
来源：http://umn.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://shl.kuanghao11.cn

[Q59] 分组内累计
来源：http://xng.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mai.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://sfv.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fkm.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ijw.shangyingyoupin.top

[Q61] 移动平均
来源：http://bmy.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oea.guannengcc.top

[Q62] 分组占比
来源：http://hje.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ott.nanxinkj.top

[Q63] 开启事务
来源：http://lyd.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rwq.jqgfzy.top

[Q64] 提交事务
来源：http://vkv.shuidangran.top

COMMIT;
来源：http://ctu.ivvv.top

[Q65] 回滚事务
来源：http://dcl.svipenyu.cn

ROLLBACK;
来源：http://mzt.hongshengwenyu.top

[Q66] 行锁查询
来源：http://loh.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bid.tianlin.xyz

[Q67] 设置隔离级别
来源：http://tqx.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://phw.nanxinkj.top

[Q68] 保存点
来源：http://krb.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://cio.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://mjn.yj20258.top

[Q69] 查看执行计划
来源：http://oxg.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yjp.yangfankeji.com

[Q70] 更新统计信息
来源：http://zof.hysaishi.cn

ANALYZE TABLE users;
来源：http://fhm.guannengcc.top

[Q71] 查看建表语句
来源：http://erh.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zwy.jlsjyb.cn

[Q72] 查看索引
来源：http://pwn.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://drn.c1oappe.top

[Q73] 查看表状态
来源：http://nid.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eof.52xcode.cn

[Q74] 强制使用索引
来源：http://qna.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tcl.vqdsnc.cn

[Q75] 日期格式化
来源：http://icn.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cku.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xsd.nwbrower.top

[Q76] 按天统计
来源：http://mle.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zli.zdqjudy.top

[Q77] 时间加减
来源：http://fwx.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dim.tianlin.xyz

[Q78] 当前时间
来源：http://dga.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ngy.ppjwa.cn

[Q79] 字符串拼接
来源：http://dbf.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fgm.birdmap.top

[Q80] 字符串截取
来源：http://lmb.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ioq.fehbvm.com

[Q81] 字符串替换
来源：http://pyq.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rkv.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://cbd.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tan.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://lla.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wor.yongpay.top

[Q84] 去除首尾空格
来源：http://qoy.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://won.daxiang520.top

[Q85] 数值取整
来源：http://crw.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://que.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://ptk.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://amo.fanxiaobao.xyz

[Q87] JSON 字段做条件
来源：http://ypr.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://skp.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://bde.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lzn.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxm.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://wvp.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://noo.daxiang520.top

[Q90] 生成序号列
来源：http://qoe.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gce.yfazqb.com

================================================================================
来源：http://ikz.yj20258.top

R. Bash 专题
来源：http://odh.zdqjudy.top

================================================================================
来源：http://qeu.dashuyun.cn

[R01] shebang 与严格模式
来源：http://hlw.jlsjyb.cn

#!/usr/bin/env bash
来源：http://zmy.gzhubu.top

set -euo pipefail
来源：http://lkk.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://ovr.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://hut.c1oappe.top

[R03] 只读变量
来源：http://uhq.jqgfzy.top

readonly PI=3.14
来源：http://yul.chenjidiqi.icu

[R04] 位置参数
来源：http://mgl.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eoj.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://pvv.zhongyouzk.top

name="${1:-default}"
来源：http://ism.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://prt.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ewm.jqgufenzy.top

[R07] if 判断文件
来源：http://nqa.wangshuangyany.cn


<!-- 参考信息 -->