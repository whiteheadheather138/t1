代发 wailian999

[P01] 生成 UUID
来源：http://lmn.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://rut.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://men.yueranfly.top

JS:   crypto.randomUUID()
来源：http://sct.ydzc1.top

TS:   crypto.randomUUID()
来源：http://wnv.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://yfq.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://tuf.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://stx.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://saf.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://cth.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dgs.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pxf.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ytg.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qnz.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nxl.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tut.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cld.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xvi.yj202588.top

[P03] 生成短随机字符串
来源：http://zry.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ydv.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gcq.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klb.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgq.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rej.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ezb.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ypc.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lhj.gaohongyu789.top

[P04] 求长度
来源：http://sgf.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://shp.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://clw.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hiy.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jwb.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://bit.bbcook.cn

Go:   len(arr);  len(m)
来源：http://sxc.jinqigufen.top

Ruby: x.length;  x.size
来源：http://aal.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hpf.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://wfw.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lnx.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://knk.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://neu.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sga.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ukf.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iqx.jlsjyb.cn

Ruby: a == b
来源：http://pas.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pep.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xkt.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gbh.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://zcd.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wgk.c1oappe.top

TS:   if (x == null) {}
来源：http://uty.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bcd.yj20258.top

Go:   if x == nil {}
来源：http://lqu.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mdm.cucudq.cn

C#:   if (x is null) {}
来源：http://dmn.zhengqikj.top

[P07] 防抖与节流
来源：http://dxy.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://quu.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://zxu.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jka.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhs.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rdn.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kfs.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxp.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sww.yongpay.top

[P08] 处理浮点精度问题
来源：http://pxc.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://faz.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dwb.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pek.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xbz.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vcz.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ccj.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wiq.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gtg.cdnleiting.top

================================================================================
来源：http://onv.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mxk.hongshengwenyu.top

================================================================================
来源：http://wha.vqdsnc.cn

[Q01] 创建表
来源：http://zkh.sjlbkw.cn

CREATE TABLE users (
来源：http://and.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oor.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://epg.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://hku.cucudq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nqv.svipenyu.cn

);
来源：http://tpk.nanxinkj.top

[Q02] 创建带外键的表
来源：http://bba.jinqigufen.top

CREATE TABLE orders (
来源：http://xso.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fxq.vqdsnc.cn

user_id INT NOT NULL,
来源：http://xph.hnqzz.top

amount DECIMAL(10, 2),
来源：http://aye.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mxz.yanxiufei.cn

);
来源：http://tee.vqdsnc.cn

[Q03] 增加列
来源：http://ppk.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tml.smart0.xyz

[Q04] 修改列类型
来源：http://mip.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dje.mhx1999.top

[Q05] 重命名列
来源：http://iss.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uji.yuxming.cn

[Q06] 删除列
来源：http://mja.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://khz.nanxuanxn.top

[Q07] 删除表
来源：http://poi.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://ohk.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://nnt.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zjv.jyoumei.cn

[Q09] 创建唯一索引
来源：http://bhe.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qno.zhijiandao.cn

[Q10] 插入单行
来源：http://hjm.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ozb.cucudq.cn

[Q11] 一次插入多行
来源：http://ssx.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://etc.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://tcg.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://ymk.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wbn.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://lgw.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kho.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://nev.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://svq.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yxf.vqdsnc.cn

[Q15] 查询全部
来源：http://wug.guowangkeji.top

SELECT * FROM users;
来源：http://qsc.yonumen.top

[Q16] 查询指定列
来源：http://bps.ydjk.org.cn

SELECT id, name FROM users;
来源：http://dsw.zhijiandao.cn

[Q17] 条件查询
来源：http://reh.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lny.yvedp.cn

[Q18] 模糊匹配
来源：http://yky.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lqe.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://dwj.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jbb.zdqjudy.top

[Q20] IN 列表
来源：http://lzd.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tlt.birdmap.top

[Q21] 空值判断
来源：http://uha.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://rim.smart0.xyz

[Q22] 排序
来源：http://now.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mur.yj20258888.top

[Q23] 分页
来源：http://wcp.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vjk.yj202588.top

[Q24] 去重
来源：http://pwg.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://xef.svipenyu.cn

[Q25] 只取前 N 条
来源：http://oys.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sqj.zhengqikj.top

[Q26] 计数
来源：http://qlh.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://uep.hysaishi.cn

[Q27] 条件计数
来源：http://cma.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fif.zhoulong.xyz

[Q28] 求和与平均
来源：http://opq.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cnl.zhiwuduotai.top

[Q29] 最大最小值
来源：http://use.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wbb.hcnkem.com

[Q30] 分组统计
来源：http://gpk.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bgy.hammf.cn

[Q31] 分组后过滤
来源：http://mai.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://moh.yonumen.top

[Q32] 分组拼接字符串
来源：http://upw.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://smq.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wio.aizwys.cn

[Q33] 多列分组
来源：http://kmb.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://izi.cdnleiting.top

[Q34] 每组取第一条
来源：http://wsy.yj20258.top

SELECT * FROM (
来源：http://kvq.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://auo.zhixingplan.top

) t WHERE rn = 1;
来源：http://zya.ivvv.top

[Q35] 内连接
来源：http://cne.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uyf.yvedp.cn

[Q36] 左连接
来源：http://exk.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://myy.jqgufenzy.top

[Q37] 右连接
来源：http://opt.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jxg.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wij.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://byd.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://nfg.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bmd.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uud.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ays.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yqz.52xcode.cn

[Q41] 多表连接
来源：http://nri.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mls.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://uva.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://bpp.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://qri.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://hie.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://llj.zhiwuduotai.top

[Q43] 标量子查询
来源：http://bvx.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfg.ctjpmb.com

[Q44] IN 子查询
来源：http://pzv.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://spd.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://psq.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yqk.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://ush.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uod.zdbjq.cn

[Q47] 与平均值比较
来源：http://fct.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://leo.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://gkw.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fdw.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://sno.epnwcf.com

[Q49] 更新单行
来源：http://ufh.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cak.jinqigfzy.top

[Q50] 批量更新
来源：http://pht.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lyr.cucudq.cn

[Q51] 用子查询更新
来源：http://zaf.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pci.zhijiandao.cn

[Q52] 删除指定行
来源：http://ouk.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://blj.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://obq.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://znv.hammf.cn

[Q54] 清空表
来源：http://jvw.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://ctt.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://jqd.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tyc.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://kao.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kfz.zdqjudy.top

[Q57] 行号
来源：http://gbg.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oun.quarkkingdee.top

[Q58] 累计求和
来源：http://dba.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ueq.nwbrower.top

[Q59] 分组内累计
来源：http://rud.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fvx.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://apv.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://div.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cwy.hesvh.cn

[Q61] 移动平均
来源：http://nnu.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://klw.quarkkingdee.top

[Q62] 分组占比
来源：http://dqq.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yud.zhixingplan.top

[Q63] 开启事务
来源：http://fxn.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dzf.kuanghao11.cn

[Q64] 提交事务
来源：http://wyl.hywenlv.cn

COMMIT;
来源：http://jwt.kuanghao11.cn

[Q65] 回滚事务
来源：http://vrf.epnwcf.com

ROLLBACK;
来源：http://oro.yonumen.top

[Q66] 行锁查询
来源：http://fkx.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xrx.zdqjudy.top

[Q67] 设置隔离级别
来源：http://nnu.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wpu.yj202588.top

[Q68] 保存点
来源：http://cww.zdbjq.cn

SAVEPOINT sp1;
来源：http://wqu.hysaishi.cn

ROLLBACK TO sp1;
来源：http://kwi.tianlin.xyz

[Q69] 查看执行计划
来源：http://qms.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bpg.hcnkem.com

[Q70] 更新统计信息
来源：http://ctf.yangfankeji.com

ANALYZE TABLE users;
来源：http://uzh.dianchejie.cn

[Q71] 查看建表语句
来源：http://vxw.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kub.xinyue.icu

[Q72] 查看索引
来源：http://eea.snrcjt.cn

SHOW INDEX FROM users;
来源：http://apo.zycfv.cn

[Q73] 查看表状态
来源：http://ezk.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zbl.nanxuanxn.top

[Q74] 强制使用索引
来源：http://zdg.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mui.nwbrower.top

[Q75] 日期格式化
来源：http://vyu.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tbb.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zkh.52xcode.cn

[Q76] 按天统计
来源：http://feb.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rok.chenlongwang.top

[Q77] 时间加减
来源：http://idy.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wum.quarkkingdee.top

[Q78] 当前时间
来源：http://cit.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://onp.jqgfzy.top

[Q79] 字符串拼接
来源：http://ydf.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pxt.sufxvd.cn

[Q80] 字符串截取
来源：http://wbb.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rtv.snrcjt.cn

[Q81] 字符串替换
来源：http://kxy.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tbj.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://ikx.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qro.zdbjq.cn

[Q83] 大小写转换
来源：http://srg.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nim.iojbl.cn

[Q84] 去除首尾空格
来源：http://gbi.sweek.top

SELECT TRIM(name) FROM users;
来源：http://vik.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://prw.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jwx.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://mjo.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://viw.c1oappe.top

[Q87] JSON 字段做条件
来源：http://jbe.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://guf.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://eqr.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dhc.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vjq.cdnleiting.top

[Q89] 判断表是否存在
来源：http://bie.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tnk.redwolf501.top

[Q90] 生成序号列
来源：http://ace.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bhe.fanxiaobao.xyz

================================================================================
来源：http://xxg.yongpay.top

R. Bash 专题
来源：http://rhb.cdnleiting.top

================================================================================
来源：http://ooj.zdqjudy.top

[R01] shebang 与严格模式
来源：http://lzi.chenzaomai.com

#!/usr/bin/env bash
来源：http://pbo.ybcxt.top

set -euo pipefail
来源：http://wkq.daxiang520.top

[R02] 变量赋值与使用
来源：http://wxx.zycfv.cn

name="Tom"; echo "$name"
来源：http://oum.cashguo.top

[R03] 只读变量
来源：http://dmi.tarul.cn

readonly PI=3.14
来源：http://rwt.guowangkeji.top

[R04] 位置参数
来源：http://hws.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gey.quarkkingdee.top

[R05] 参数默认值
来源：http://fvk.smart0.xyz

name="${1:-default}"
来源：http://uxw.yfazqb.com

[R06] 判断命令是否存在
来源：http://zja.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://akq.hfpthk.cn

[R07] if 判断文件
来源：http://gll.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yur.dashuyun.cn

[R08] 数值比较
来源：http://ewh.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://viw.vehdjk.com

[R09] 字符串比较
来源：http://zyx.zhengqikj.top


<!-- 参考信息 -->