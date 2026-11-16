代发 wailian999

[P01] 生成 UUID
来源：http://fgj.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://csa.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://shi.ybcxt.top

JS:   crypto.randomUUID()
来源：http://gvs.cashguo.top

TS:   crypto.randomUUID()
来源：http://xjl.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://wla.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://rzs.sweek.top

Ruby: SecureRandom.uuid
来源：http://xif.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://yek.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://qbj.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ozg.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nij.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fxr.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oig.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ypz.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://quq.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ken.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ojh.nwbrower.top

[P03] 生成短随机字符串
来源：http://zsg.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pjt.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uea.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uve.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://luy.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vre.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iyt.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mgf.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ozn.cdnleiting.top

[P04] 求长度
来源：http://mrt.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sfq.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rei.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vij.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://exf.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://uue.iojbl.cn

Go:   len(arr);  len(m)
来源：http://swx.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://bxf.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kvx.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://enf.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gjz.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ffr.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eml.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvx.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bkf.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ety.zdbjq.cn

Ruby: a == b
来源：http://yra.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lgm.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sgr.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cuf.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://lne.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://exm.zhixingplan.top

TS:   if (x == null) {}
来源：http://wjl.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nsa.cdnleiting.top

Go:   if x == nil {}
来源：http://dhh.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fyz.chenzaomai.com

C#:   if (x is null) {}
来源：http://stw.aibaodan.cn

[P07] 防抖与节流
来源：http://xzb.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vpw.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://hrx.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzm.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nup.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vqr.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://syw.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://asy.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jwq.sysykeji.top

[P08] 处理浮点精度问题
来源：http://hat.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://smh.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hlv.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mfe.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://idf.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pxc.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lox.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cum.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ipz.pycfn.com

================================================================================
来源：http://naf.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vzs.jqgfzy.top

================================================================================
来源：http://bwm.yj20258888.top

[Q01] 创建表
来源：http://slu.jiagoushi.top

CREATE TABLE users (
来源：http://jva.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qax.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://ncc.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://fiy.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rna.xinyue.icu

);
来源：http://svs.9152youxi.cn

[Q02] 创建带外键的表
来源：http://ggl.yanxiufei.cn

CREATE TABLE orders (
来源：http://dnt.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lrv.fzhhl.top

user_id INT NOT NULL,
来源：http://ivu.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://tku.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jtx.gogol.net.cn

);
来源：http://yok.shangyingyoupin.top

[Q03] 增加列
来源：http://dmf.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ury.gzhubu.top

[Q04] 修改列类型
来源：http://oev.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yft.iojbl.cn

[Q05] 重命名列
来源：http://yme.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xsd.yongpay.top

[Q06] 删除列
来源：http://yth.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://owf.tian-w.cn

[Q07] 删除表
来源：http://hfi.ivvv.top

DROP TABLE IF EXISTS orders;
来源：http://bfc.smart0.xyz

[Q08] 创建普通索引
来源：http://tfh.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vcv.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://lfy.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://orp.tanke756.top

[Q10] 插入单行
来源：http://ogp.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sng.shuidangran.top

[Q11] 一次插入多行
来源：http://sre.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dkb.tanke756.top

[Q12] 插入后取自增 ID
来源：http://scm.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oir.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://siz.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://euo.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://elz.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://red.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rau.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qce.fanxiaobao.xyz

[Q15] 查询全部
来源：http://mcv.gaohongyu789.top

SELECT * FROM users;
来源：http://qvm.svipenyu.cn

[Q16] 查询指定列
来源：http://ncm.xuanzx.com

SELECT id, name FROM users;
来源：http://wap.dashuyun.cn

[Q17] 条件查询
来源：http://iix.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ewa.yfazqb.com

[Q18] 模糊匹配
来源：http://iau.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yer.jlsjyb.cn

[Q19] 范围查询
来源：http://hza.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rfs.havefunace.top

[Q20] IN 列表
来源：http://kep.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://juc.shanyushiyangtech.top

[Q21] 空值判断
来源：http://qly.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jgu.gzhubu.top

[Q22] 排序
来源：http://sqw.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vmx.kuanghao11.cn

[Q23] 分页
来源：http://aig.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axj.jinqigufen.top

[Q24] 去重
来源：http://lnp.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://lfw.hammf.cn

[Q25] 只取前 N 条
来源：http://nmj.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wwk.yj20258888.top

[Q26] 计数
来源：http://ovi.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://imt.zdqjudy.top

[Q27] 条件计数
来源：http://fwu.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wqv.ehwqpu.com

[Q28] 求和与平均
来源：http://fmf.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vkl.kuanghao11.cn

[Q29] 最大最小值
来源：http://nyr.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xpn.fehbvm.com

[Q30] 分组统计
来源：http://rsx.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zhd.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://dln.jinqigfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yyh.quarkkingdee.top

[Q32] 分组拼接字符串
来源：http://xky.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://psl.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hzo.jinqigufen.top

[Q33] 多列分组
来源：http://iho.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nkv.fehbvm.com

[Q34] 每组取第一条
来源：http://cqn.mhx1999.top

SELECT * FROM (
来源：http://xcq.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mam.nanxinkj.top

) t WHERE rn = 1;
来源：http://kzg.yj20258.top

[Q35] 内连接
来源：http://qbc.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://njj.yfazqb.com

[Q36] 左连接
来源：http://jzt.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://opv.316326.xyz

[Q37] 右连接
来源：http://vrk.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uqk.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://yhj.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yin.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://abp.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://urr.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wgx.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cnm.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jan.snrcjt.cn

[Q41] 多表连接
来源：http://eny.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://txq.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://lxd.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://ncf.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://imy.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://aht.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://enz.sysykeji.top

[Q43] 标量子查询
来源：http://kbw.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nil.fktsv.cn

[Q44] IN 子查询
来源：http://pxd.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ouq.yonumen.top

[Q45] EXISTS 判断存在
来源：http://cbf.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqv.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ohq.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ewt.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://sgy.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uon.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://ppq.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gzq.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://ytk.sjlbkw.cn

[Q49] 更新单行
来源：http://kpr.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rcq.ivvv.top

[Q50] 批量更新
来源：http://mzs.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wux.havefunace.top

[Q51] 用子查询更新
来源：http://uke.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://csr.dianchejie.cn

[Q52] 删除指定行
来源：http://ehf.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://oay.aibaodan.cn

[Q53] 按条件删除
来源：http://cgd.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fya.fengsongda.top

[Q54] 清空表
来源：http://jjc.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://ixm.316326.xyz

[Q55] 排名（并列占位）
来源：http://zdy.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aji.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://ygg.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://day.dashuyun.cn

[Q57] 行号
来源：http://paa.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kxm.tanke756.top

[Q58] 累计求和
来源：http://kud.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ucl.yueranfly.top

[Q59] 分组内累计
来源：http://ytj.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vfa.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://efq.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vrw.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://okp.9152youxi.cn

[Q61] 移动平均
来源：http://agd.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mpt.ctjpmb.com

[Q62] 分组占比
来源：http://zcb.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://voe.yj202588.top

[Q63] 开启事务
来源：http://uwv.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jkn.gaohongyu789.top

[Q64] 提交事务
来源：http://aey.hysaishi.cn

COMMIT;
来源：http://oeb.yangfankeji.com

[Q65] 回滚事务
来源：http://yaz.uphjek.com

ROLLBACK;
来源：http://nmr.cucudq.cn

[Q66] 行锁查询
来源：http://mbi.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vxt.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://nax.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://knz.jinghuilouyu.cn

[Q68] 保存点
来源：http://vxe.svipenyu.cn

SAVEPOINT sp1;
来源：http://lpt.yonumen.top

ROLLBACK TO sp1;
来源：http://wua.quarkkingdee.top

[Q69] 查看执行计划
来源：http://oeq.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xpz.nwbrower.top

[Q70] 更新统计信息
来源：http://ptb.wangdashe.top

ANALYZE TABLE users;
来源：http://llr.ydjk.org.cn

[Q71] 查看建表语句
来源：http://gix.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://orl.tarul.cn

[Q72] 查看索引
来源：http://tqu.ivvv.top

SHOW INDEX FROM users;
来源：http://asx.hnxiangtu.top

[Q73] 查看表状态
来源：http://clb.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tve.dashuyun.cn

[Q74] 强制使用索引
来源：http://fsi.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xrw.xylfe.cn

[Q75] 日期格式化
来源：http://kyz.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pmz.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wfd.ivvv.top

[Q76] 按天统计
来源：http://njf.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bxh.yvedp.cn

[Q77] 时间加减
来源：http://gmk.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://whj.sufxvd.cn

[Q78] 当前时间
来源：http://xfr.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rvc.xylfe.cn

[Q79] 字符串拼接
来源：http://jgc.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://koj.hesvh.cn

[Q80] 字符串截取
来源：http://evr.hcnkem.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nvp.yj202588.top

[Q81] 字符串替换
来源：http://wpa.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://guu.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://sii.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pko.jianghu66.top

[Q83] 大小写转换
来源：http://csw.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hsf.nwbrower.top

[Q84] 去除首尾空格
来源：http://jnn.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://knz.tarul.cn

[Q85] 数值取整
来源：http://npl.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ors.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://mlq.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kur.daxiang520.top

[Q87] JSON 字段做条件
来源：http://bbi.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bio.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://spu.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dqi.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pfc.xuanzx.com

[Q89] 判断表是否存在
来源：http://ert.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rjk.hcnkem.com

[Q90] 生成序号列
来源：http://gyp.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cfa.tian-w.cn

================================================================================
来源：http://jba.hcnkem.com

R. Bash 专题
来源：http://xtb.cheryme.top

================================================================================
来源：http://rgt.52xcode.cn

[R01] shebang 与严格模式
来源：http://bug.yj20258888.top

#!/usr/bin/env bash
来源：http://lha.yuanzhike.top

set -euo pipefail
来源：http://jjg.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://eyy.jyoumei.cn

name="Tom"; echo "$name"
来源：http://spc.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://eek.zycfv.cn

readonly PI=3.14
来源：http://pqn.jlsjyb.cn

[R04] 位置参数
来源：http://veb.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://waf.jqgfzy.top

[R05] 参数默认值
来源：http://gxz.chenjidiqi.icu

name="${1:-default}"
来源：http://xxo.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://yzr.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://czb.sjlbkw.cn

[R07] if 判断文件
来源：http://xjq.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mkh.haohaochexian.top

[R08] 数值比较
来源：http://lzd.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://erv.svipenyu.cn

[R09] 字符串比较
来源：http://vwu.hcnkem.com


<!-- 参考信息 -->