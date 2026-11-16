代发 wailian999

TS:   // child_process / cluster 模块
来源：http://bmz.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fwa.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wuu.chenzaomai.com

Ruby: // fork 块
来源：http://mxh.chenzaomai.com

C#:   Parallel.For
来源：http://orx.redwolf501.top

================================================================================
来源：http://jmp.sysykeji.top

P. 常用工具函数
来源：http://vsr.shuidangran.top

================================================================================
来源：http://pxp.ydzc1.top

[P01] 生成 UUID
来源：http://ren.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://zuf.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zit.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://qkn.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://beh.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://hed.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://oqy.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://ozq.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://rxm.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://tav.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lle.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://jaj.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rdn.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oii.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nvr.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vho.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fqu.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pgk.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://nai.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tli.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://goq.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ndp.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vmq.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jxt.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ouy.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://udz.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://flb.jinqigfzy.top

[P04] 求长度
来源：http://bot.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uqj.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cko.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nbs.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tem.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://sxb.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://uys.gotoacloud.top

Ruby: x.length;  x.size
来源：http://hui.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://vnb.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://coy.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://zdf.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gkw.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eyl.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sfl.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hko.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://lge.yuxming.cn

Ruby: a == b
来源：http://hia.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rxt.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qic.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eoy.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://vql.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yzu.hnqzz.top

TS:   if (x == null) {}
来源：http://jdj.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://zzr.snrcjt.cn

Go:   if x == nil {}
来源：http://tjl.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pvt.iojbl.cn

C#:   if (x is null) {}
来源：http://vwr.vqdsnc.cn

[P07] 防抖与节流
来源：http://tur.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://waw.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://tli.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbz.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvd.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eob.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oww.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nas.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hor.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://itl.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kzg.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gap.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zjn.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mfa.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ggr.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qja.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lpt.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vux.wangdashe.top

================================================================================
来源：http://puy.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nbf.guannengcc.top

================================================================================
来源：http://isp.cqqwz.cn

[Q01] 创建表
来源：http://kmw.xinyue.icu

CREATE TABLE users (
来源：http://sdb.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zeq.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://ezp.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://lcs.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ksq.jlsjyb.cn

);
来源：http://kku.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://fnp.sjlbkw.cn

CREATE TABLE orders (
来源：http://erf.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsy.jinqigfzy.top

user_id INT NOT NULL,
来源：http://xpu.316326.xyz

amount DECIMAL(10, 2),
来源：http://nga.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vxx.yfazqb.com

);
来源：http://kzm.zhijiandao.cn

[Q03] 增加列
来源：http://chw.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wzk.zhongyouzk.top

[Q04] 修改列类型
来源：http://ntp.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mom.yonumen.top

[Q05] 重命名列
来源：http://udo.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wei.chenzaomai.com

[Q06] 删除列
来源：http://isf.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dvb.yongpay.top

[Q07] 删除表
来源：http://xfr.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://bdn.jiagoushi.top

[Q08] 创建普通索引
来源：http://mtt.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gej.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://uji.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ncr.shangyingyoupin.top

[Q10] 插入单行
来源：http://yyd.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tok.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://vvz.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://moo.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://pyy.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://myd.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://trd.yonumen.top

[Q13] 忽略重复插入
来源：http://vjh.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gmh.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://obt.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lfg.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jml.xziqi.cn

[Q15] 查询全部
来源：http://wcw.zhoulong.xyz

SELECT * FROM users;
来源：http://zsp.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://rsw.yuanzhike.top

SELECT id, name FROM users;
来源：http://fyc.chenlongwang.top

[Q17] 条件查询
来源：http://izj.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vbt.sjlbkw.cn

[Q18] 模糊匹配
来源：http://noz.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://euj.meibo888.top

[Q19] 范围查询
来源：http://djn.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sae.yfazqb.com

[Q20] IN 列表
来源：http://buo.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jfz.gaohongyu789.top

[Q21] 空值判断
来源：http://hde.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://uua.feifeiyinyue.top

[Q22] 排序
来源：http://ffd.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yso.daria6918.cn

[Q23] 分页
来源：http://whg.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oaw.zycfv.cn

[Q24] 去重
来源：http://wky.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://ypb.nanxinkj.top

[Q25] 只取前 N 条
来源：http://qop.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://raf.fzhhl.top

[Q26] 计数
来源：http://mgl.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://dmh.ppjwa.cn

[Q27] 条件计数
来源：http://pfp.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tam.0kj1m.cn

[Q28] 求和与平均
来源：http://yql.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cdn.bbcook.cn

[Q29] 最大最小值
来源：http://msy.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fcc.yuxming.cn

[Q30] 分组统计
来源：http://gat.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://squ.daxiang520.top

[Q31] 分组后过滤
来源：http://tpt.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wql.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://vyt.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xdk.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wxn.nanxinkj.top

[Q33] 多列分组
来源：http://afo.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vbg.yj202588.top

[Q34] 每组取第一条
来源：http://iiy.chenjidiqi.icu

SELECT * FROM (
来源：http://nht.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zny.zhijiandao.cn

) t WHERE rn = 1;
来源：http://fic.wangdashe.top

[Q35] 内连接
来源：http://zaz.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aca.hesvh.cn

[Q36] 左连接
来源：http://uit.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yxx.cheryme.top

[Q37] 右连接
来源：http://vtu.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mlk.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://vll.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jqw.ivvv.top

[Q39] 自连接（查上下级）
来源：http://pup.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zjh.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wyd.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eot.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qim.fzhhl.top

[Q41] 多表连接
来源：http://spt.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hsj.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://wpo.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://trd.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://wwg.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://kvd.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://swy.ehwqpu.com

[Q43] 标量子查询
来源：http://lkb.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rvq.haohaochexian.top

[Q44] IN 子查询
来源：http://hjq.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vvk.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://vcd.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ygs.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://qmq.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jpg.tanke756.top

[Q47] 与平均值比较
来源：http://rdb.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ozv.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://fvw.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bkb.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://poe.jinqigfzy.top

[Q49] 更新单行
来源：http://aol.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oip.316326.xyz

[Q50] 批量更新
来源：http://uqy.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lni.bjfxy.top

[Q51] 用子查询更新
来源：http://dpj.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xlw.chenjidiqi.icu

[Q52] 删除指定行
来源：http://wwn.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://hbv.haohaochexian.top

[Q53] 按条件删除
来源：http://mlz.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kik.52xcode.cn

[Q54] 清空表
来源：http://oan.ybcxt.top

TRUNCATE TABLE logs;
来源：http://lvh.cheryme.top

[Q55] 排名（并列占位）
来源：http://ops.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nxu.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://ruk.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cjq.jinghuilouyu.cn

[Q57] 行号
来源：http://nwq.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://snx.hfpthk.cn

[Q58] 累计求和
来源：http://jbb.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lvs.gzhubu.top

[Q59] 分组内累计
来源：http://ksb.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://woo.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://lwd.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dvx.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://epd.c1oappe.top

[Q61] 移动平均
来源：http://dms.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lln.jiagoushi.top

[Q62] 分组占比
来源：http://kzb.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tsi.guannengcc.top

[Q63] 开启事务
来源：http://aff.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cym.hnxiangtu.top

[Q64] 提交事务
来源：http://emn.shuidangran.top

COMMIT;
来源：http://dol.ppjwa.cn

[Q65] 回滚事务
来源：http://fvr.zdqjudy.top

ROLLBACK;
来源：http://mzy.guowangkeji.top

[Q66] 行锁查询
来源：http://arg.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vev.tarul.cn

[Q67] 设置隔离级别
来源：http://ghc.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iif.xinyue.icu

[Q68] 保存点
来源：http://lrl.uphjek.com

SAVEPOINT sp1;
来源：http://eoi.birdmap.top

ROLLBACK TO sp1;
来源：http://fso.yuanzhike.top

[Q69] 查看执行计划
来源：http://sfg.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gpn.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://mef.yongpay.top

ANALYZE TABLE users;
来源：http://ush.snrcjt.cn

[Q71] 查看建表语句
来源：http://sin.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tvi.9152youxi.cn

[Q72] 查看索引
来源：http://nan.c1oappe.top

SHOW INDEX FROM users;
来源：http://kzs.nanxinkj.top

[Q73] 查看表状态
来源：http://vce.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wsp.hfpthk.cn

[Q74] 强制使用索引
来源：http://ndm.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bgc.gotoacloud.top

[Q75] 日期格式化
来源：http://pqd.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qjb.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qxk.yj20258.top

[Q76] 按天统计
来源：http://avr.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hvr.tanke756.top

[Q77] 时间加减
来源：http://jak.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyv.jianghu66.top

[Q78] 当前时间
来源：http://ztl.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fst.tarul.cn

[Q79] 字符串拼接
来源：http://bqz.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tdt.aizwys.cn

[Q80] 字符串截取
来源：http://qhh.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://knw.yj20258.top

[Q81] 字符串替换
来源：http://tfw.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pgr.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://wvk.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uyn.redwolf501.top

[Q83] 大小写转换
来源：http://rjr.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ekh.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://zga.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://lts.hcnkem.com

[Q85] 数值取整
来源：http://olw.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uqb.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://mxh.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://spt.fzhhl.top

[Q87] JSON 字段做条件
来源：http://xxd.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pme.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://wau.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tuw.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://juh.tian-w.cn

[Q89] 判断表是否存在
来源：http://hve.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bbc.zycfv.cn

[Q90] 生成序号列
来源：http://tkp.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oyz.ivvv.top

================================================================================
来源：http://kco.jinqigfzy.top

R. Bash 专题
来源：http://trj.ywan-chungtsiang.top

================================================================================
来源：http://znm.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://owl.tarul.cn

#!/usr/bin/env bash
来源：http://mtx.jianghu66.top

set -euo pipefail
来源：http://vgf.dianchejie.cn

[R02] 变量赋值与使用
来源：http://bbb.nanxinkj.top

name="Tom"; echo "$name"
来源：http://fht.pycfn.com

[R03] 只读变量
来源：http://qqq.yj20258888.top

readonly PI=3.14
来源：http://lhi.feifeiyinyue.top

[R04] 位置参数
来源：http://wwi.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wti.nanxinkj.top

[R05] 参数默认值
来源：http://tqd.jinghuilouyu.cn


<!-- 参考信息 -->