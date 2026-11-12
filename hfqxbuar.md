代发 wailian999

[P01] 生成 UUID
来源：http://bso.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://stb.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qsp.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://zxi.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://cya.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://jlb.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://gtx.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://nqx.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://xas.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://rma.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xmy.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://geh.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zqw.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mee.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qbc.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mur.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fth.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uvp.aizwys.cn

[P03] 生成短随机字符串
来源：http://ylv.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ang.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mcd.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xiv.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://euw.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gdt.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ynp.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://alt.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sbc.jianghu66.top

[P04] 求长度
来源：http://dvl.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://put.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dcn.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zjd.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eof.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://uzu.sweek.top

Go:   len(arr);  len(m)
来源：http://auf.zycfv.cn

Ruby: x.length;  x.size
来源：http://nne.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dge.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://lnh.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oyj.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jub.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gho.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kxk.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vdd.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://clp.yvedp.cn

Ruby: a == b
来源：http://kgy.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vwa.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zkb.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xzf.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://wld.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nud.cucudq.cn

TS:   if (x == null) {}
来源：http://omy.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mpo.sufxvd.cn

Go:   if x == nil {}
来源：http://dfw.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zzb.tarul.cn

C#:   if (x is null) {}
来源：http://upb.ehwqpu.com

[P07] 防抖与节流
来源：http://nzr.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ebb.uphjek.com

PHP:  // 手写时间戳比较
来源：http://njq.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snr.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uwc.316326.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oet.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wby.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nhb.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yad.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://slv.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ocx.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://krp.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vrk.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ceu.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pnt.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://quo.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://exu.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wbk.xylfe.cn

================================================================================
来源：http://chc.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nyy.daria6918.cn

================================================================================
来源：http://hlj.hnqzz.top

[Q01] 创建表
来源：http://met.zhengqikj.top

CREATE TABLE users (
来源：http://szu.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbv.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://wcf.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://zgv.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qgf.mhx1999.top

);
来源：http://dbc.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://lfh.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://hhp.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfe.9152youxi.cn

user_id INT NOT NULL,
来源：http://uvf.sysykeji.top

amount DECIMAL(10, 2),
来源：http://mho.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://emz.yongpay.top

);
来源：http://uxo.guowangkeji.top

[Q03] 增加列
来源：http://zoy.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://veg.xziqi.cn

[Q04] 修改列类型
来源：http://vzf.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lhu.yuanzhike.top

[Q05] 重命名列
来源：http://kns.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yab.ydjk.org.cn

[Q06] 删除列
来源：http://gwn.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mty.wangdashe.top

[Q07] 删除表
来源：http://jjq.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://vdn.chenlongwang.top

[Q08] 创建普通索引
来源：http://qah.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nql.tianlin.xyz

[Q09] 创建唯一索引
来源：http://mlj.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nbo.316326.xyz

[Q10] 插入单行
来源：http://ley.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwv.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://erz.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kdn.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://ihj.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://ntj.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jco.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://emk.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uxh.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://gfq.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgs.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rzq.jinqigfzy.top

[Q15] 查询全部
来源：http://csi.yongpay.top

SELECT * FROM users;
来源：http://qia.aizwys.cn

[Q16] 查询指定列
来源：http://sxn.bbcook.cn

SELECT id, name FROM users;
来源：http://gmz.vehdjk.com

[Q17] 条件查询
来源：http://rsy.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fke.xuanzx.com

[Q18] 模糊匹配
来源：http://jvb.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qgv.ehwqpu.com

[Q19] 范围查询
来源：http://nox.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bwx.xuetiantiany.cn

[Q20] IN 列表
来源：http://khy.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lhp.fanxiaobao.xyz

[Q21] 空值判断
来源：http://kby.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ovr.316326.xyz

[Q22] 排序
来源：http://uke.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jxq.9152youxi.cn

[Q23] 分页
来源：http://knb.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://emu.wangshuangyany.cn

[Q24] 去重
来源：http://efm.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://rta.yuanzhike.top

[Q25] 只取前 N 条
来源：http://isi.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dtg.meibo888.top

[Q26] 计数
来源：http://caj.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://wyz.jinqigfzy.top

[Q27] 条件计数
来源：http://naf.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://agp.yanxiufei.cn

[Q28] 求和与平均
来源：http://syd.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wfc.fengsongda.top

[Q29] 最大最小值
来源：http://ggv.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zaw.hywenlv.cn

[Q30] 分组统计
来源：http://kgy.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dki.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://soj.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jav.daria6918.cn

[Q32] 分组拼接字符串
来源：http://jge.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://prv.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltr.bjfxy.top

[Q33] 多列分组
来源：http://pth.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mwn.snrcjt.cn

[Q34] 每组取第一条
来源：http://nrx.sweek.top

SELECT * FROM (
来源：http://zqq.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://caq.nwbrower.top

) t WHERE rn = 1;
来源：http://vka.jinqigfzy.top

[Q35] 内连接
来源：http://tjo.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://izs.yanxiufei.cn

[Q36] 左连接
来源：http://wdr.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ltt.ehwqpu.com

[Q37] 右连接
来源：http://yrf.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ags.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://jqm.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aew.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://oyw.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jws.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xyt.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vka.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bmj.fzhhl.top

[Q41] 多表连接
来源：http://zid.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fil.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://ldm.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://lhi.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://tsx.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://djx.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pgg.0kj1m.cn

[Q43] 标量子查询
来源：http://qdk.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lkj.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://dqd.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bql.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://cvr.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yof.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://hiu.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dhv.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://ltx.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vbt.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://qjg.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pbx.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://xjo.jyoumei.cn

[Q49] 更新单行
来源：http://kjp.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fyf.jianghu66.top

[Q50] 批量更新
来源：http://liy.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://shk.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://cft.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vqd.hysaishi.cn

[Q52] 删除指定行
来源：http://fmx.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://cjh.haohaochexian.top

[Q53] 按条件删除
来源：http://uhx.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wya.yuxming.cn

[Q54] 清空表
来源：http://bca.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://vjo.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://frs.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yer.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://rce.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oze.svipenyu.cn

[Q57] 行号
来源：http://haz.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://spe.hnqzz.top

[Q58] 累计求和
来源：http://anq.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://flt.hammf.cn

[Q59] 分组内累计
来源：http://dtp.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vqk.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://sly.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ahb.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ibr.smart0.xyz

[Q61] 移动平均
来源：http://hsk.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nre.tanke756.top

[Q62] 分组占比
来源：http://mwy.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vna.yonumen.top

[Q63] 开启事务
来源：http://cig.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nso.bjfxy.top

[Q64] 提交事务
来源：http://jur.ctjpmb.com

COMMIT;
来源：http://xqu.nanxuanxn.top

[Q65] 回滚事务
来源：http://fdz.birdmap.top

ROLLBACK;
来源：http://yqo.epnwcf.com

[Q66] 行锁查询
来源：http://sen.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gar.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://bfq.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://brt.ybcxt.top

[Q68] 保存点
来源：http://mqa.birdmap.top

SAVEPOINT sp1;
来源：http://kvq.shuidangran.top

ROLLBACK TO sp1;
来源：http://pwi.sysykeji.top

[Q69] 查看执行计划
来源：http://zdl.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://suy.snrcjt.cn

[Q70] 更新统计信息
来源：http://qnb.nanxinkj.top

ANALYZE TABLE users;
来源：http://fhn.hywenlv.cn

[Q71] 查看建表语句
来源：http://fvi.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gva.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://uik.birdmap.top

SHOW INDEX FROM users;
来源：http://cld.sxryk.cn

[Q73] 查看表状态
来源：http://ocd.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ibh.meibo888.top

[Q74] 强制使用索引
来源：http://keo.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tyr.ydzc1.top

[Q75] 日期格式化
来源：http://qwq.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qok.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://izd.xuetiantiany.cn

[Q76] 按天统计
来源：http://qch.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dzr.shzxlz.cn

[Q77] 时间加减
来源：http://uso.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wnm.jyoumei.cn

[Q78] 当前时间
来源：http://tfh.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yxc.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://zmy.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gwu.kuanghao11.cn

[Q80] 字符串截取
来源：http://jcc.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yea.hcnkem.com

[Q81] 字符串替换
来源：http://kkz.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dls.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://oem.jinyuanbaomall.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uvj.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://lmc.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lst.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://tih.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://kkq.hfpthk.cn

[Q85] 数值取整
来源：http://awh.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sbl.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://nul.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lvn.xinyue.icu

[Q87] JSON 字段做条件
来源：http://djm.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mrn.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://nqk.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://duj.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wwa.gzhubu.top

[Q89] 判断表是否存在
来源：http://muy.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xor.redwolf501.top

[Q90] 生成序号列
来源：http://has.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xpa.wangdashe.top

================================================================================
来源：http://gyu.ydzc1.top

R. Bash 专题
来源：http://evy.yfazqb.com

================================================================================
来源：http://hjy.yj202588.top

[R01] shebang 与严格模式
来源：http://ccx.birdmap.top

#!/usr/bin/env bash
来源：http://frq.xziqi.cn

set -euo pipefail
来源：http://piz.gotoacloud.top

[R02] 变量赋值与使用
来源：http://zry.aizwys.cn

name="Tom"; echo "$name"
来源：http://ixs.fanxiaobao.xyz

[R03] 只读变量
来源：http://ual.chenzaomai.com

readonly PI=3.14
来源：http://hdn.andypj.xyz

[R04] 位置参数
来源：http://uea.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cld.redwolf501.top

[R05] 参数默认值
来源：http://ryx.yj20258888.top

name="${1:-default}"
来源：http://qur.tianlin.xyz

[R06] 判断命令是否存在
来源：http://lxi.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jji.zhixingplan.top

[R07] if 判断文件
来源：http://phy.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qfp.tanke756.top

[R08] 数值比较
来源：http://rjf.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gfy.sufxvd.cn

[R09] 字符串比较
来源：http://meg.cucudq.cn


<!-- 参考信息 -->