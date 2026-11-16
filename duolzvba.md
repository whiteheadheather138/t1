代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://iqw.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://wya.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yyk.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vif.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qge.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ona.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://reu.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qvy.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hlq.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://coa.fzhhl.top

[P03] 生成短随机字符串
来源：http://qpg.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mky.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uaj.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ryk.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cfz.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://abu.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ngx.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fin.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cva.shangyingyoupin.top

[P04] 求长度
来源：http://zxd.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pzt.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqy.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lmo.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://crs.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://bvm.birdmap.top

Go:   len(arr);  len(m)
来源：http://ybn.c1oappe.top

Ruby: x.length;  x.size
来源：http://xzm.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://drx.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://esf.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://urb.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gyy.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rrz.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hld.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xpj.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lmx.hesvh.cn

Ruby: a == b
来源：http://bic.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://adx.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wum.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ehn.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://nqg.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jok.tarul.cn

TS:   if (x == null) {}
来源：http://pqd.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ppv.yueranfly.top

Go:   if x == nil {}
来源：http://uno.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vnh.epnwcf.com

C#:   if (x is null) {}
来源：http://tey.jinqigufen.top

[P07] 防抖与节流
来源：http://wpe.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xvg.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://foy.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lva.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akt.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vzh.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rdn.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sgm.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gsw.hnqzz.top

[P08] 处理浮点精度问题
来源：http://ljp.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://twq.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fxd.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dqe.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jqk.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jse.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qtk.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://egs.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://orf.smart0.xyz

================================================================================
来源：http://wrj.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xhn.zhoulong.xyz

================================================================================
来源：http://wiz.gaohongyu789.top

[Q01] 创建表
来源：http://ofl.nanxuanxn.top

CREATE TABLE users (
来源：http://yqg.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hcv.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://wwb.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://kbt.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zbv.ehwqpu.com

);
来源：http://xqx.ehwqpu.com

[Q02] 创建带外键的表
来源：http://sib.snrcjt.cn

CREATE TABLE orders (
来源：http://kkw.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://crr.nanxuanxn.top

user_id INT NOT NULL,
来源：http://ubf.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://ntu.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ytj.zhongyouzk.top

);
来源：http://rua.aizwys.cn

[Q03] 增加列
来源：http://yet.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rke.jqgufenzy.top

[Q04] 修改列类型
来源：http://igy.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mfp.cheryme.top

[Q05] 重命名列
来源：http://oqy.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pnn.aizwys.cn

[Q06] 删除列
来源：http://rav.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://hzs.zhengqikj.top

[Q07] 删除表
来源：http://bmc.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://zhq.cashguo.top

[Q08] 创建普通索引
来源：http://eqc.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bfs.tian-w.cn

[Q09] 创建唯一索引
来源：http://bkq.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bba.smart0.xyz

[Q10] 插入单行
来源：http://mab.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aov.snrcjt.cn

[Q11] 一次插入多行
来源：http://vie.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nxd.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://wqt.yvedp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rgj.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kuc.shzxlz.cn

[Q13] 忽略重复插入
来源：http://phq.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mht.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://srl.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cig.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sjb.yueranfly.top

[Q15] 查询全部
来源：http://cwh.ppjwa.cn

SELECT * FROM users;
来源：http://ddr.yj20258888.top

[Q16] 查询指定列
来源：http://rpw.uphjek.com

SELECT id, name FROM users;
来源：http://wjg.hnqzz.top

[Q17] 条件查询
来源：http://cvp.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pmp.yanxiufei.cn

[Q18] 模糊匹配
来源：http://rks.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uhu.mhx1999.top

[Q19] 范围查询
来源：http://iwv.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ckn.xinyue.icu

[Q20] IN 列表
来源：http://pic.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xwj.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://ova.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jxa.cashguo.top

[Q22] 排序
来源：http://cpu.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fnn.zhengqikj.top

[Q23] 分页
来源：http://pao.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qha.chenjidiqi.icu

[Q24] 去重
来源：http://noe.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://ofe.xylfe.cn

[Q25] 只取前 N 条
来源：http://cva.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dwb.fktsv.cn

[Q26] 计数
来源：http://ojs.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://uma.daria6918.cn

[Q27] 条件计数
来源：http://pfx.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sdq.jianghu66.top

[Q28] 求和与平均
来源：http://iai.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xtz.havefunace.top

[Q29] 最大最小值
来源：http://rlk.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://rmn.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://oen.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ucq.c1oappe.top

[Q31] 分组后过滤
来源：http://otl.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xao.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://wvy.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://obf.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sqm.xziqi.cn

[Q33] 多列分组
来源：http://cds.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uhb.zhijiandao.cn

[Q34] 每组取第一条
来源：http://vvl.tianlin.xyz

SELECT * FROM (
来源：http://tff.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vpm.daria6918.cn

) t WHERE rn = 1;
来源：http://siz.yvedp.cn

[Q35] 内连接
来源：http://raq.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pmx.ehwqpu.com

[Q36] 左连接
来源：http://pnt.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yka.jinghuilouyu.cn

[Q37] 右连接
来源：http://aww.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://idw.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://lql.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dzo.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://ijo.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dmk.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kec.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eom.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://juj.yj202588.top

[Q41] 多表连接
来源：http://qii.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fdg.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://hpe.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://ozh.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://ttb.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://kvs.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iul.tianlin.xyz

[Q43] 标量子查询
来源：http://sex.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xnu.zhongyouzk.top

[Q44] IN 子查询
来源：http://uev.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ymh.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://eey.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvr.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://nfi.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sza.yvedp.cn

[Q47] 与平均值比较
来源：http://tvy.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uws.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://psr.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mps.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://jxc.yj202588.top

[Q49] 更新单行
来源：http://sfw.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://unl.yfazqb.com

[Q50] 批量更新
来源：http://gop.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sxb.hammf.cn

[Q51] 用子查询更新
来源：http://hbk.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qgf.jqgfzy.top

[Q52] 删除指定行
来源：http://meg.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://dbl.9152youxi.cn

[Q53] 按条件删除
来源：http://yhj.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eht.zdqjudy.top

[Q54] 清空表
来源：http://csc.xziqi.cn

TRUNCATE TABLE logs;
来源：http://tos.gzhubu.top

[Q55] 排名（并列占位）
来源：http://hdt.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bui.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://kag.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ajj.bjfxy.top

[Q57] 行号
来源：http://mvk.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rvh.hysaishi.cn

[Q58] 累计求和
来源：http://hcg.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uzx.yonumen.top

[Q59] 分组内累计
来源：http://dnk.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jnb.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://mzv.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yrv.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lkb.cdnleiting.top

[Q61] 移动平均
来源：http://xoi.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qai.jqgufenzy.top

[Q62] 分组占比
来源：http://lvf.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xhl.yueranfly.top

[Q63] 开启事务
来源：http://dkt.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mdm.hcnkem.com

[Q64] 提交事务
来源：http://vqy.jinqigufen.top

COMMIT;
来源：http://sic.svipenyu.cn

[Q65] 回滚事务
来源：http://mty.jqgufenzy.top

ROLLBACK;
来源：http://hmz.jqgfzy.top

[Q66] 行锁查询
来源：http://ikk.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dia.shzxlz.cn

[Q67] 设置隔离级别
来源：http://hyq.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rnj.fktsv.cn

[Q68] 保存点
来源：http://baz.zhoulong.xyz

SAVEPOINT sp1;
来源：http://mrj.zdqjudy.top

ROLLBACK TO sp1;
来源：http://cqi.zhengqikj.top

[Q69] 查看执行计划
来源：http://aka.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qkx.vqdsnc.cn

[Q70] 更新统计信息
来源：http://cgz.xinyue.icu

ANALYZE TABLE users;
来源：http://eut.zhijiandao.cn

[Q71] 查看建表语句
来源：http://ryq.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jdj.ivvv.top

[Q72] 查看索引
来源：http://usr.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://nog.iojbl.cn

[Q73] 查看表状态
来源：http://cos.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ebr.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://egr.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kae.jlsjyb.cn

[Q75] 日期格式化
来源：http://wyp.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bwj.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://igx.c1oappe.top

[Q76] 按天统计
来源：http://wca.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jmz.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://xov.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ljk.aibaodan.cn

[Q78] 当前时间
来源：http://buu.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://okx.gogol.net.cn

[Q79] 字符串拼接
来源：http://gww.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lac.meibo888.top

[Q80] 字符串截取
来源：http://aki.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gio.chenjidiqi.icu

[Q81] 字符串替换
来源：http://vhd.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fum.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://qqe.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tfd.daria6918.cn

[Q83] 大小写转换
来源：http://dme.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ghn.gogol.net.cn

[Q84] 去除首尾空格
来源：http://qpn.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://kfg.tanke756.top

[Q85] 数值取整
来源：http://wsl.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kfh.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://vwp.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cie.xinyue.icu

[Q87] JSON 字段做条件
来源：http://bzs.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dsk.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://abr.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jzp.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gxn.guowangkeji.top

[Q89] 判断表是否存在
来源：http://efs.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fne.cqqwz.cn

[Q90] 生成序号列
来源：http://ldr.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rmc.xylfe.cn

================================================================================
来源：http://vly.bbcook.cn

R. Bash 专题
来源：http://hps.zdbjq.cn

================================================================================
来源：http://cia.yuanzhike.top

[R01] shebang 与严格模式
来源：http://vdg.sjlbkw.cn

#!/usr/bin/env bash
来源：http://wsp.hfpthk.cn

set -euo pipefail
来源：http://fcq.hfpthk.cn

[R02] 变量赋值与使用
来源：http://qvb.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://vcu.zhiwuduotai.top

[R03] 只读变量
来源：http://kho.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://dyw.jiagoushi.top

[R04] 位置参数
来源：http://eqi.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vry.hesvh.cn

[R05] 参数默认值
来源：http://bmz.ydjk.org.cn

name="${1:-default}"
来源：http://fwg.shangyingyoupin.top

[R06] 判断命令是否存在
来源：http://ksm.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ovr.ybcxt.top

[R07] if 判断文件
来源：http://vbv.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://olm.tian-w.cn

[R08] 数值比较
来源：http://swg.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://mgb.hywenlv.cn

[R09] 字符串比较
来源：http://psf.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ylw.fktsv.cn

[R10] 正则匹配
来源：http://gfz.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mlv.cqqwz.cn

[R11] case 多分支
来源：http://kws.shanyushiyangkeji.top

case "$1" in
来源：http://hde.nanxuanxn.top

start) echo "启动" ;;
来源：http://koq.havefunace.top

stop)  echo "停止" ;;
来源：http://asp.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://ehl.cheryme.top


<!-- 参考信息 -->