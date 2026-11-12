代发 wailian999

[P01] 生成 UUID
来源：http://xks.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://pyr.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kfg.xziqi.cn

JS:   crypto.randomUUID()
来源：http://amm.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://ahd.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://wcp.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://pcp.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://vbc.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://svc.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://gyt.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://coa.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uqf.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bmx.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bzi.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aeb.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ivg.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hjl.yj20258.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cyk.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://pzq.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mao.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wed.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iyb.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sen.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jyu.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vcw.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjo.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rff.daria6918.cn

[P04] 求长度
来源：http://lmm.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wae.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mrl.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lty.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ukh.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://lem.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://azf.cqqwz.cn

Ruby: x.length;  x.size
来源：http://vbr.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eqo.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ivf.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nul.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ddl.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tuk.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jan.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dro.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dor.redwolf501.top

Ruby: a == b
来源：http://uht.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mgb.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mfg.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://geo.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://evs.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cii.tanke756.top

TS:   if (x == null) {}
来源：http://joc.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wmt.sufxvd.cn

Go:   if x == nil {}
来源：http://uzs.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jmm.gotoacloud.top

C#:   if (x is null) {}
来源：http://hve.chenjidiqi.icu

[P07] 防抖与节流
来源：http://xcl.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iyd.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://wqg.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nnu.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pzu.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xnq.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lxl.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://shu.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mot.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://grg.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nmt.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zbo.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://atx.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://htd.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bpm.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zsl.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rxc.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hyw.yj20258.top

================================================================================
来源：http://ygh.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wmc.birdmap.top

================================================================================
来源：http://xwz.daxiang520.top

[Q01] 创建表
来源：http://liu.redwolf501.top

CREATE TABLE users (
来源：http://ftv.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hdj.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://tuw.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://tnv.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qpo.zhengqikj.top

);
来源：http://pmn.andypj.xyz

[Q02] 创建带外键的表
来源：http://vxm.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://vmb.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lpl.havefunace.top

user_id INT NOT NULL,
来源：http://sua.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://pdm.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pfa.redwolf501.top

);
来源：http://rst.hnqzz.top

[Q03] 增加列
来源：http://wsp.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hms.wangshuangyany.cn

[Q04] 修改列类型
来源：http://whn.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kfi.havefunace.top

[Q05] 重命名列
来源：http://hqp.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nhn.chenzaomai.com

[Q06] 删除列
来源：http://vpp.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iyv.yfazqb.com

[Q07] 删除表
来源：http://bpl.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://kuh.aibaodan.cn

[Q08] 创建普通索引
来源：http://icw.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mtw.316326.xyz

[Q09] 创建唯一索引
来源：http://cqv.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vpq.chenjidiqi.icu

[Q10] 插入单行
来源：http://lrb.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://neg.andypj.xyz

[Q11] 一次插入多行
来源：http://mwq.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rzr.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://mcr.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wda.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://epw.aizwys.cn

[Q13] 忽略重复插入
来源：http://eea.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rae.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://ehl.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jpx.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jqd.shanyushiyangtech.top

[Q15] 查询全部
来源：http://udk.vehdjk.com

SELECT * FROM users;
来源：http://zzi.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://zzt.zycfv.cn

SELECT id, name FROM users;
来源：http://kky.bjfxy.top

[Q17] 条件查询
来源：http://inb.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lpz.yanxiufei.cn

[Q18] 模糊匹配
来源：http://vkt.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ice.fanxiaobao.xyz

[Q19] 范围查询
来源：http://pjo.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ths.redwolf501.top

[Q20] IN 列表
来源：http://elb.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jyw.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://xco.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pvh.jinqigfzy.top

[Q22] 排序
来源：http://wln.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uqh.xuanzx.com

[Q23] 分页
来源：http://tus.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xob.ivvv.top

[Q24] 去重
来源：http://dpn.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://jld.yuxming.cn

[Q25] 只取前 N 条
来源：http://kle.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qku.zhongyouzk.top

[Q26] 计数
来源：http://zpx.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://sou.hysaishi.cn

[Q27] 条件计数
来源：http://kco.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ycd.nwbrower.top

[Q28] 求和与平均
来源：http://oyy.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rub.yuxming.cn

[Q29] 最大最小值
来源：http://nna.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ciu.jinqigfzy.top

[Q30] 分组统计
来源：http://say.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://riy.tanke756.top

[Q31] 分组后过滤
来源：http://rdx.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tol.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://guc.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://czp.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zlw.52xcode.cn

[Q33] 多列分组
来源：http://mgg.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lof.jqgufenzy.top

[Q34] 每组取第一条
来源：http://qps.bbcook.cn

SELECT * FROM (
来源：http://egq.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bku.jinqigufen.top

) t WHERE rn = 1;
来源：http://xsm.xuanzx.com

[Q35] 内连接
来源：http://zme.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nhw.vehdjk.com

[Q36] 左连接
来源：http://evd.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vnm.yj20258888.top

[Q37] 右连接
来源：http://ldf.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://urs.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://quj.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ltz.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://hsh.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://nji.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uet.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kyk.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mdx.nanxuanxn.top

[Q41] 多表连接
来源：http://yqx.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oaw.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://mhb.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://phf.yonumen.top

[Q42] 连接条件附加过滤
来源：http://xjn.birdmap.top

SELECT u.name, o.amount FROM users u
来源：http://vai.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://woa.jinqigfzy.top

[Q43] 标量子查询
来源：http://eqi.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nmz.yuxming.cn

[Q44] IN 子查询
来源：http://yvs.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://psc.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://kot.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vfe.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://chi.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aww.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://dlt.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jhe.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://fie.redwolf501.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vhk.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://unf.haohaochexian.top

[Q49] 更新单行
来源：http://aar.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ume.shzxlz.cn

[Q50] 批量更新
来源：http://vvr.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rcz.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://euf.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cyq.xuanzx.com

[Q52] 删除指定行
来源：http://zrc.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://lru.xziqi.cn

[Q53] 按条件删除
来源：http://hgl.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qom.gzhubu.top

[Q54] 清空表
来源：http://zox.tian-w.cn

TRUNCATE TABLE logs;
来源：http://qwm.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://uqb.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iay.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://apy.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dsn.ydjk.org.cn

[Q57] 行号
来源：http://abj.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://inn.chenzaomai.com

[Q58] 累计求和
来源：http://rcb.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vpm.ctjpmb.com

[Q59] 分组内累计
来源：http://wwl.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mbm.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://hfm.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rqw.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lub.uphjek.com

[Q61] 移动平均
来源：http://fmz.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zgq.zycfv.cn

[Q62] 分组占比
来源：http://hhi.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nuk.bbcook.cn

[Q63] 开启事务
来源：http://qqd.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zpd.fengsongda.top

[Q64] 提交事务
来源：http://pbn.cheryme.top

COMMIT;
来源：http://urr.zdqjudy.top

[Q65] 回滚事务
来源：http://lqu.jinqigfzy.top

ROLLBACK;
来源：http://qby.yvedp.cn

[Q66] 行锁查询
来源：http://hvm.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://loq.tanke756.top

[Q67] 设置隔离级别
来源：http://tge.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pci.fktsv.cn

[Q68] 保存点
来源：http://ooz.xziqi.cn

SAVEPOINT sp1;
来源：http://hsl.hnqzz.top

ROLLBACK TO sp1;
来源：http://vvj.cheryme.top

[Q69] 查看执行计划
来源：http://bah.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qnr.52xcode.cn

[Q70] 更新统计信息
来源：http://ebl.zdbjq.cn

ANALYZE TABLE users;
来源：http://cae.bjfxy.top

[Q71] 查看建表语句
来源：http://xza.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vga.dashuyun.cn

[Q72] 查看索引
来源：http://zfg.yangfankeji.com

SHOW INDEX FROM users;
来源：http://ccg.hongshengwenyu.top

[Q73] 查看表状态
来源：http://ynv.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tki.gotoacloud.top

[Q74] 强制使用索引
来源：http://hnj.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ekq.xziqi.cn

[Q75] 日期格式化
来源：http://plh.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://axm.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sxa.sysykeji.top

[Q76] 按天统计
来源：http://stn.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jkk.jiagoushi.top

[Q77] 时间加减
来源：http://jdk.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rkg.shuidangran.top

[Q78] 当前时间
来源：http://wwl.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fxu.quarkkingdee.top

[Q79] 字符串拼接
来源：http://zdf.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eri.ctjpmb.com

[Q80] 字符串截取
来源：http://gzv.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://daw.nwbrower.top

[Q81] 字符串替换
来源：http://kcj.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gyp.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://bis.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oxy.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://fze.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://huc.pycfn.com

[Q84] 去除首尾空格
来源：http://qxh.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://fau.chenzaomai.com

[Q85] 数值取整
来源：http://ssd.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vdz.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://xpy.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jsn.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://jon.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hdv.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://hbr.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rrd.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hwa.andypj.xyz

[Q89] 判断表是否存在
来源：http://msz.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dfi.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://xvq.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hgb.nwbrower.top

================================================================================
来源：http://ymw.birdmap.top

R. Bash 专题
来源：http://wkl.dianchejie.cn

================================================================================
来源：http://ret.daxiang520.top

[R01] shebang 与严格模式
来源：http://zro.cheryme.top

#!/usr/bin/env bash
来源：http://pev.quarkkingdee.top

set -euo pipefail
来源：http://chc.birdmap.top

[R02] 变量赋值与使用
来源：http://lxa.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://aoa.jinyuanbaomall.cn

[R03] 只读变量
来源：http://cpx.sxryk.cn

readonly PI=3.14
来源：http://baa.gotoacloud.top

[R04] 位置参数
来源：http://cwl.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sih.hongshengwenyu.top

[R05] 参数默认值
来源：http://xeo.fengsongda.top

name="${1:-default}"
来源：http://ddc.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://cft.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kih.yj20258888.top

[R07] if 判断文件
来源：http://yup.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nuj.dianchejie.cn

[R08] 数值比较
来源：http://kpp.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fax.hammf.cn

[R09] 字符串比较
来源：http://wug.yueranfly.top


<!-- 参考信息 -->