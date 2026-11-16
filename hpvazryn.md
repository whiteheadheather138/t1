代发 wailian999

TS:   crypto.randomUUID()
来源：http://swz.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://lwj.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://qgm.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://lds.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://hdj.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://lda.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mac.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bco.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zpf.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iwl.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xqm.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://atf.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rqz.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jjw.tarul.cn

[P03] 生成短随机字符串
来源：http://tgs.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yfm.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gwk.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjd.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zea.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wdz.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vjl.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cca.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://onj.pengpengdd.cyou

[P04] 求长度
来源：http://tti.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xim.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qot.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://alf.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tyj.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://mxz.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://rbe.zdbjq.cn

Ruby: x.length;  x.size
来源：http://abz.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://roc.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://kcf.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yta.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://txk.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eho.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ape.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://efh.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://gnf.fehbvm.com

Ruby: a == b
来源：http://lcm.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://trg.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dlz.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ndy.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://kbb.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yjp.nanxuanxn.top

TS:   if (x == null) {}
来源：http://jus.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dvy.svipenyu.cn

Go:   if x == nil {}
来源：http://rct.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ygv.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://jnz.yongpay.top

[P07] 防抖与节流
来源：http://aec.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gtn.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://zyz.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ojt.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yss.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ail.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hwd.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wup.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vlb.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://adf.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ggv.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yzo.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sie.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nxi.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dah.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xkf.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hoz.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zme.0kj1m.cn

================================================================================
来源：http://kbf.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qpn.daxiang520.top

================================================================================
来源：http://lva.ctjpmb.com

[Q01] 创建表
来源：http://bpe.sysykeji.top

CREATE TABLE users (
来源：http://ntj.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwg.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://qhz.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://arx.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wub.dianchejie.cn

);
来源：http://mmh.zhengqikj.top

[Q02] 创建带外键的表
来源：http://poi.fktsv.cn

CREATE TABLE orders (
来源：http://cye.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ljn.yj202588.top

user_id INT NOT NULL,
来源：http://lfv.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://ogt.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ieg.shangyingyoupin.top

);
来源：http://uck.hnxiangtu.top

[Q03] 增加列
来源：http://jpt.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vjk.0kj1m.cn

[Q04] 修改列类型
来源：http://jtx.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xso.zhongyouzk.top

[Q05] 重命名列
来源：http://xyc.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ubo.hnxiangtu.top

[Q06] 删除列
来源：http://dzc.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://pso.c1oappe.top

[Q07] 删除表
来源：http://yeh.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://qfy.xuanzx.com

[Q08] 创建普通索引
来源：http://qwl.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ejt.guowangkeji.top

[Q09] 创建唯一索引
来源：http://dfb.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dib.svipenyu.cn

[Q10] 插入单行
来源：http://gkq.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bwp.gzhubu.top

[Q11] 一次插入多行
来源：http://oav.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uxp.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://phn.tanke756.top

INSERT INTO users (name) VALUES ('C');
来源：http://zvh.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ddb.tianlin.xyz

[Q13] 忽略重复插入
来源：http://mcw.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kmw.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://asb.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sho.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zfe.9152youxi.cn

[Q15] 查询全部
来源：http://uhv.dashuyun.cn

SELECT * FROM users;
来源：http://bwn.xinyue.icu

[Q16] 查询指定列
来源：http://pxg.hnqzz.top

SELECT id, name FROM users;
来源：http://bbf.ehwqpu.com

[Q17] 条件查询
来源：http://xrm.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhk.pycfn.com

[Q18] 模糊匹配
来源：http://aez.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wga.pengpengdd.cyou

[Q19] 范围查询
来源：http://oss.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kfe.fengsongda.top

[Q20] IN 列表
来源：http://gsx.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ynm.chenjidiqi.icu

[Q21] 空值判断
来源：http://xov.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jdu.kuanghao11.cn

[Q22] 排序
来源：http://oce.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bwx.fehbvm.com

[Q23] 分页
来源：http://ses.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dme.quarkkingdee.top

[Q24] 去重
来源：http://tow.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://osy.mhx1999.top

[Q25] 只取前 N 条
来源：http://yze.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mms.jlsjyb.cn

[Q26] 计数
来源：http://huu.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://jrq.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://czp.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tsv.0kj1m.cn

[Q28] 求和与平均
来源：http://tmj.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zlp.shangyingyoupin.top

[Q29] 最大最小值
来源：http://rsf.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rbo.ppjwa.cn

[Q30] 分组统计
来源：http://yvo.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcy.ppjwa.cn

[Q31] 分组后过滤
来源：http://ubl.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qay.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://fjk.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xln.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mhz.zhengqikj.top

[Q33] 多列分组
来源：http://akg.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lca.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://waa.jqgfzy.top

SELECT * FROM (
来源：http://tzk.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rfh.fehbvm.com

) t WHERE rn = 1;
来源：http://btl.nanxinkj.top

[Q35] 内连接
来源：http://ysv.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ltv.bjfxy.top

[Q36] 左连接
来源：http://ngz.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cwa.zhoulong.xyz

[Q37] 右连接
来源：http://cdn.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rxd.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rlb.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://civ.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://lra.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ift.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qxc.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://uwm.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yrg.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://zud.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://wev.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://anw.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://rih.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://gxm.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://quu.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kxz.yfazqb.com

[Q43] 标量子查询
来源：http://cbu.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://omp.zhijiandao.cn

[Q44] IN 子查询
来源：http://jbg.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ncq.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://qor.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qdl.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nuc.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxe.iojbl.cn

[Q47] 与平均值比较
来源：http://cse.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://llo.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://sgh.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ubk.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://ifi.quarkkingdee.top

[Q49] 更新单行
来源：http://hwy.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ebw.yanxiufei.cn

[Q50] 批量更新
来源：http://wme.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lci.jlsjyb.cn

[Q51] 用子查询更新
来源：http://xvv.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpl.tian-w.cn

[Q52] 删除指定行
来源：http://vug.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://dyj.ydzc1.top

[Q53] 按条件删除
来源：http://oog.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pgx.jinyuanbaomall.cn

[Q54] 清空表
来源：http://hav.xuanzx.com

TRUNCATE TABLE logs;
来源：http://otf.yfazqb.com

[Q55] 排名（并列占位）
来源：http://uvf.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nti.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://vce.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uyp.jinqigufen.top

[Q57] 行号
来源：http://qme.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xof.yfazqb.com

[Q58] 累计求和
来源：http://jem.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iil.9152youxi.cn

[Q59] 分组内累计
来源：http://wgv.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uyn.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://low.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://esl.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lre.cdnleiting.top

[Q61] 移动平均
来源：http://gvi.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bzg.fanxiaobao.xyz

[Q62] 分组占比
来源：http://mdr.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mcq.hongshengwenyu.top

[Q63] 开启事务
来源：http://rpr.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oaa.yongpay.top

[Q64] 提交事务
来源：http://txd.yj20258888.top

COMMIT;
来源：http://kzv.tanke756.top

[Q65] 回滚事务
来源：http://qdq.haohaochexian.top

ROLLBACK;
来源：http://xjt.guannengcc.top

[Q66] 行锁查询
来源：http://uid.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wst.cashguo.top

[Q67] 设置隔离级别
来源：http://dmb.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mtc.chenzaomai.com

[Q68] 保存点
来源：http://mlt.ctjpmb.com

SAVEPOINT sp1;
来源：http://ylm.zhengqikj.top

ROLLBACK TO sp1;
来源：http://szc.epnwcf.com

[Q69] 查看执行计划
来源：http://qvk.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xhf.shuidangran.top

[Q70] 更新统计信息
来源：http://lih.sufxvd.cn

ANALYZE TABLE users;
来源：http://oky.tarul.cn

[Q71] 查看建表语句
来源：http://rsi.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oin.chenlongwang.top

[Q72] 查看索引
来源：http://uod.c1oappe.top

SHOW INDEX FROM users;
来源：http://dha.nanxuanxn.top

[Q73] 查看表状态
来源：http://exm.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://xbh.shuidangran.top

[Q74] 强制使用索引
来源：http://gur.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ufi.xziqi.cn

[Q75] 日期格式化
来源：http://ecv.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cvx.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ohl.snrcjt.cn

[Q76] 按天统计
来源：http://qhn.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vfi.xuanzx.com

[Q77] 时间加减
来源：http://ele.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lwu.fehbvm.com

[Q78] 当前时间
来源：http://ahc.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lor.yj20258.top

[Q79] 字符串拼接
来源：http://fyl.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mpi.sysykeji.top

[Q80] 字符串截取
来源：http://ekk.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iww.daria6918.cn

[Q81] 字符串替换
来源：http://xrk.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://udr.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://kjh.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aqf.fehbvm.com

[Q83] 大小写转换
来源：http://fur.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rtc.ivvv.top

[Q84] 去除首尾空格
来源：http://eds.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://zyf.jlsjyb.cn

[Q85] 数值取整
来源：http://vdp.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cgo.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://hbm.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://exw.c1oappe.top

[Q87] JSON 字段做条件
来源：http://ehs.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hds.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://isi.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uin.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xrb.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://cvu.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eto.pengpengdd.cyou

[Q90] 生成序号列
来源：http://xlk.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ppx.uphjek.com

================================================================================
来源：http://sgg.dashuyun.cn

R. Bash 专题
来源：http://qna.ybcxt.top

================================================================================
来源：http://ore.0kj1m.cn

[R01] shebang 与严格模式
来源：http://fym.dianchejie.cn

#!/usr/bin/env bash
来源：http://jug.pycfn.com

set -euo pipefail
来源：http://nhi.epnwcf.com

[R02] 变量赋值与使用
来源：http://hvx.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://lhy.zhijiandao.cn

[R03] 只读变量
来源：http://jql.yvedp.cn

readonly PI=3.14
来源：http://pqo.shangyingyoupin.top

[R04] 位置参数
来源：http://zgo.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://czn.nanxinkj.top

[R05] 参数默认值
来源：http://uwh.52xcode.cn

name="${1:-default}"
来源：http://xjh.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://vuw.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xoc.hesvh.cn

[R07] if 判断文件
来源：http://wfi.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qgk.wangshuangyany.cn

[R08] 数值比较
来源：http://vps.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://yyv.dianchejie.cn

[R09] 字符串比较
来源：http://cvk.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://taz.gaohongyu789.top

[R10] 正则匹配
来源：http://pdk.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cqo.zhaomingkeji.xyz

[R11] case 多分支
来源：http://crl.quarkkingdee.top


<!-- 参考信息 -->