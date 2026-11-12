代发 wailian999

TS:   crypto.randomUUID()
来源：http://xml.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://sxw.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://dze.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://zbj.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://qvu.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://czb.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zbu.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cma.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ndv.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vsc.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mio.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://alg.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kxq.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qex.ppjwa.cn

[P03] 生成短随机字符串
来源：http://ouc.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nlw.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ujl.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bnj.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mfx.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kxe.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wqq.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yhp.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qbs.shzxlz.cn

[P04] 求长度
来源：http://vde.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qmq.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cgq.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zee.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bsz.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://sex.wangdashe.top

Go:   len(arr);  len(m)
来源：http://rqc.andypj.xyz

Ruby: x.length;  x.size
来源：http://okb.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xqk.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://yph.jinqigfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gdq.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://awa.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ydf.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zmg.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fqn.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://uvf.zdbjq.cn

Ruby: a == b
来源：http://twj.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rre.nanxuanxn.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://usy.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ywf.cashguo.top

PHP:  if (empty($x)) {}
来源：http://kyj.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kwv.mhx1999.top

TS:   if (x == null) {}
来源：http://eln.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://chj.yj202588.top

Go:   if x == nil {}
来源：http://rig.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zbx.hesvh.cn

C#:   if (x is null) {}
来源：http://xvu.guannengcc.top

[P07] 防抖与节流
来源：http://kjq.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oyf.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://ewq.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cal.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mjj.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bxu.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rdy.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zqa.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fxe.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://jjx.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tzd.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nkj.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jit.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mnv.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bgp.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bph.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zyq.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fzn.feifeiyinyue.top

================================================================================
来源：http://xht.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zyu.tanke756.top

================================================================================
来源：http://chv.zhoulong.xyz

[Q01] 创建表
来源：http://zgp.yj202588.top

CREATE TABLE users (
来源：http://mxl.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uig.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://yvp.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://wlo.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jpo.fehbvm.com

);
来源：http://nhy.epnwcf.com

[Q02] 创建带外键的表
来源：http://xde.ehwqpu.com

CREATE TABLE orders (
来源：http://nln.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oph.pycfn.com

user_id INT NOT NULL,
来源：http://gux.guannengcc.top

amount DECIMAL(10, 2),
来源：http://ziq.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bqt.xinyue.icu

);
来源：http://yfq.52xcode.cn

[Q03] 增加列
来源：http://pjd.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rgl.zhixingplan.top

[Q04] 修改列类型
来源：http://yhu.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://djr.svipenyu.cn

[Q05] 重命名列
来源：http://akj.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ddb.hcnkem.com

[Q06] 删除列
来源：http://zln.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zgg.snrcjt.cn

[Q07] 删除表
来源：http://xyr.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://ool.quarkkingdee.top

[Q08] 创建普通索引
来源：http://dit.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yuu.shuidangran.top

[Q09] 创建唯一索引
来源：http://rfk.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jvk.cashguo.top

[Q10] 插入单行
来源：http://hfe.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xqd.zdbjq.cn

[Q11] 一次插入多行
来源：http://vxd.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cye.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://noj.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://ble.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wbq.yongpay.top

[Q13] 忽略重复插入
来源：http://zjb.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uxx.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://stk.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://miu.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://taf.hesvh.cn

[Q15] 查询全部
来源：http://tqe.yvedp.cn

SELECT * FROM users;
来源：http://gwz.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://wcc.pycfn.com

SELECT id, name FROM users;
来源：http://txm.hnqzz.top

[Q17] 条件查询
来源：http://ask.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dzf.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://jse.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kjf.bjfxy.top

[Q19] 范围查询
来源：http://jtz.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://omh.zycfv.cn

[Q20] IN 列表
来源：http://ytl.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xkc.sxryk.cn

[Q21] 空值判断
来源：http://tre.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zzp.c1oappe.top

[Q22] 排序
来源：http://vay.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tid.hnxiangtu.top

[Q23] 分页
来源：http://hmb.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mjb.guannengcc.top

[Q24] 去重
来源：http://ljo.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://liw.gzhubu.top

[Q25] 只取前 N 条
来源：http://ouk.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vlg.cdnleiting.top

[Q26] 计数
来源：http://lvo.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://dhh.fanxiaobao.xyz

[Q27] 条件计数
来源：http://qyb.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pto.daxiang520.top

[Q28] 求和与平均
来源：http://ymx.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://guq.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://sfb.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lhy.nanxinkj.top

[Q30] 分组统计
来源：http://vlr.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nuw.ehwqpu.com

[Q31] 分组后过滤
来源：http://wqd.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://izl.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://gvp.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dyx.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ewb.zhijiandao.cn

[Q33] 多列分组
来源：http://cpj.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://phq.chenlongwang.top

[Q34] 每组取第一条
来源：http://gqr.ivvv.top

SELECT * FROM (
来源：http://hby.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tpg.fktsv.cn

) t WHERE rn = 1;
来源：http://rno.nwbrower.top

[Q35] 内连接
来源：http://ibl.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zqc.ybcxt.top

[Q36] 左连接
来源：http://wpb.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cie.bjfxy.top

[Q37] 右连接
来源：http://mhp.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zlr.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://kmi.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bni.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://upm.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://azd.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ndd.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lkr.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rsr.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://ucd.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://lvd.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://abs.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://vpj.meibo888.top

[Q42] 连接条件附加过滤
来源：http://wpt.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://otq.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ryp.bbcook.cn

[Q43] 标量子查询
来源：http://kkg.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nqe.yangfankeji.com

[Q44] IN 子查询
来源：http://nhg.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wbf.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://lia.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nka.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://juh.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wbv.zycfv.cn

[Q47] 与平均值比较
来源：http://rrl.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xza.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://yox.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jrq.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://uub.quarkkingdee.top

[Q49] 更新单行
来源：http://gns.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://igk.hywenlv.cn

[Q50] 批量更新
来源：http://rzd.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mhv.shuidangran.top

[Q51] 用子查询更新
来源：http://upv.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xuz.xinyue.icu

[Q52] 删除指定行
来源：http://ltg.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://kyu.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://phz.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gck.bbcook.cn

[Q54] 清空表
来源：http://cox.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://iro.xuanzx.com

[Q55] 排名（并列占位）
来源：http://koh.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://omx.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://jpz.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bvr.xinyue.icu

[Q57] 行号
来源：http://waf.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bhf.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://xdq.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cwm.birdmap.top

[Q59] 分组内累计
来源：http://bdi.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cxe.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://vbx.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mwc.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uxz.jiagoushi.top

[Q61] 移动平均
来源：http://nzm.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qlx.mhx1999.top

[Q62] 分组占比
来源：http://vef.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hcw.kuanghao11.cn

[Q63] 开启事务
来源：http://bhg.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://olb.yfazqb.com

[Q64] 提交事务
来源：http://arh.fehbvm.com

COMMIT;
来源：http://jfa.yuanzhike.top

[Q65] 回滚事务
来源：http://hxq.hfpthk.cn

ROLLBACK;
来源：http://ziq.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://kvq.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ggc.hammf.cn

[Q67] 设置隔离级别
来源：http://txr.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xvn.fktsv.cn

[Q68] 保存点
来源：http://ekv.zycfv.cn

SAVEPOINT sp1;
来源：http://dej.xylfe.cn

ROLLBACK TO sp1;
来源：http://ssp.gaohongyu789.top

[Q69] 查看执行计划
来源：http://mnj.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zpy.uphjek.com

[Q70] 更新统计信息
来源：http://xvp.snrcjt.cn

ANALYZE TABLE users;
来源：http://uou.daxiang520.top

[Q71] 查看建表语句
来源：http://avg.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://usu.xuanzx.com

[Q72] 查看索引
来源：http://zhh.shzxlz.cn

SHOW INDEX FROM users;
来源：http://ymr.mhx1999.top

[Q73] 查看表状态
来源：http://yvn.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://xng.daxiang520.top

[Q74] 强制使用索引
来源：http://xap.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tmd.shuidangran.top

[Q75] 日期格式化
来源：http://kjz.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mgo.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uyf.yj20258.top

[Q76] 按天统计
来源：http://hnk.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fxi.fzhhl.top

[Q77] 时间加减
来源：http://bjj.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lzi.fktsv.cn

[Q78] 当前时间
来源：http://qhl.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uzd.52xcode.cn

[Q79] 字符串拼接
来源：http://esu.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pdn.daria6918.cn

[Q80] 字符串截取
来源：http://hsh.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uxg.hesvh.cn

[Q81] 字符串替换
来源：http://adi.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qzx.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://nax.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cxx.jqgfzy.top

[Q83] 大小写转换
来源：http://bgg.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yxo.redwolf501.top

[Q84] 去除首尾空格
来源：http://nmy.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://ram.jiagoushi.top

[Q85] 数值取整
来源：http://hvj.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mda.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://mlw.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rxr.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://eub.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eic.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://rph.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eup.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hev.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://uvk.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://szp.jianghu66.top

[Q90] 生成序号列
来源：http://lfs.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ega.bjfxy.top

================================================================================
来源：http://hux.yuxming.cn

R. Bash 专题
来源：http://rlg.bbcook.cn

================================================================================
来源：http://rmb.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://wnf.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://lsx.yueranfly.top

set -euo pipefail
来源：http://olk.0kj1m.cn

[R02] 变量赋值与使用
来源：http://eiw.gzhubu.top

name="Tom"; echo "$name"
来源：http://qdp.yonumen.top

[R03] 只读变量
来源：http://jih.pengpengdd.cyou

readonly PI=3.14
来源：http://fcr.gogol.net.cn

[R04] 位置参数
来源：http://ith.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xdp.316326.xyz

[R05] 参数默认值
来源：http://yjx.yueranfly.top

name="${1:-default}"
来源：http://jto.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://zpa.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lob.yanxiufei.cn

[R07] if 判断文件
来源：http://zzn.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uth.c1oappe.top

[R08] 数值比较
来源：http://dnt.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kdw.hfpthk.cn

[R09] 字符串比较
来源：http://lrp.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xjj.zdbjq.cn

[R10] 正则匹配
来源：http://rfz.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lks.chenjidiqi.icu

[R11] case 多分支
来源：http://mbx.zycfv.cn


<!-- 参考信息 -->