代发 wailian999

[P01] 生成 UUID
来源：http://jqo.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://xpi.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iez.uphjek.com

JS:   crypto.randomUUID()
来源：http://hyq.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://tda.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://owx.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://nci.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://vmm.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://exr.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://yoc.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gpb.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lta.havefunace.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://goo.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qwk.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fqx.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fno.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ctj.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xim.hysaishi.cn

[P03] 生成短随机字符串
来源：http://isg.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://evz.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jbe.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gys.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eva.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rao.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://idx.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ufl.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gxa.sxryk.cn

[P04] 求长度
来源：http://jyt.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cmh.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfq.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://twm.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmq.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://fvx.yj20258.top

Go:   len(arr);  len(m)
来源：http://ssu.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://iyu.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lfk.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://axk.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fat.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ayx.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fip.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wne.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tfa.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://eql.andypj.xyz

Ruby: a == b
来源：http://pkh.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qet.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dzs.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kdf.yongpay.top

PHP:  if (empty($x)) {}
来源：http://nvs.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpo.quarkkingdee.top

TS:   if (x == null) {}
来源：http://quq.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fjt.zhoulong.xyz

Go:   if x == nil {}
来源：http://pjk.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eoz.yueranfly.top

C#:   if (x is null) {}
来源：http://zkj.cashguo.top

[P07] 防抖与节流
来源：http://qov.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mzy.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://ubi.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lru.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zum.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zoq.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ikr.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fia.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lqi.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://ekl.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qrb.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ult.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nks.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ulc.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ynx.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dhd.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fxk.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://amc.haohaochexian.top

================================================================================
来源：http://xal.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://div.sjlbkw.cn

================================================================================
来源：http://lth.cheryme.top

[Q01] 创建表
来源：http://rbp.guannengcc.top

CREATE TABLE users (
来源：http://dyj.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsd.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://cyd.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://ntq.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gnd.sweek.top

);
来源：http://eid.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://mad.316326.xyz

CREATE TABLE orders (
来源：http://cup.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nwl.yonumen.top

user_id INT NOT NULL,
来源：http://xje.yj20258.top

amount DECIMAL(10, 2),
来源：http://qmc.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://phu.hfpthk.cn

);
来源：http://puf.chenzaomai.com

[Q03] 增加列
来源：http://syk.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bip.havefunace.top

[Q04] 修改列类型
来源：http://get.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iuv.wangdashe.top

[Q05] 重命名列
来源：http://raz.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bgf.xuanzx.com

[Q06] 删除列
来源：http://zei.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://mrm.mhx1999.top

[Q07] 删除表
来源：http://ouz.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://xpv.jlsjyb.cn

[Q08] 创建普通索引
来源：http://eeq.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lan.zdqjudy.top

[Q09] 创建唯一索引
来源：http://fzw.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ttv.yuxming.cn

[Q10] 插入单行
来源：http://pyq.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wma.zhixingplan.top

[Q11] 一次插入多行
来源：http://vcl.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tvm.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://sww.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://chz.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nsk.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://gpy.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://esr.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://frw.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mph.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fmw.sxryk.cn

[Q15] 查询全部
来源：http://btv.feifeiyinyue.top

SELECT * FROM users;
来源：http://zsg.sxryk.cn

[Q16] 查询指定列
来源：http://sfw.snrcjt.cn

SELECT id, name FROM users;
来源：http://vkg.shuidangran.top

[Q17] 条件查询
来源：http://ptz.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cyc.guowangkeji.top

[Q18] 模糊匹配
来源：http://ggk.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cej.pycfn.com

[Q19] 范围查询
来源：http://hzj.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nbe.wangshuangyany.cn

[Q20] IN 列表
来源：http://qfq.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fbf.sufxvd.cn

[Q21] 空值判断
来源：http://str.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yuz.daxiang520.top

[Q22] 排序
来源：http://jsw.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wkh.jinyuanbaomall.cn

[Q23] 分页
来源：http://npn.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ddk.c1oappe.top

[Q24] 去重
来源：http://xac.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://aiu.ppjwa.cn

[Q25] 只取前 N 条
来源：http://uzs.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qry.jinqigfzy.top

[Q26] 计数
来源：http://elb.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://bsj.wangdashe.top

[Q27] 条件计数
来源：http://qbm.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uol.chenzaomai.com

[Q28] 求和与平均
来源：http://vsg.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jhs.zhengqikj.top

[Q29] 最大最小值
来源：http://vqm.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tbh.ppjwa.cn

[Q30] 分组统计
来源：http://cxf.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://szu.nwbrower.top

[Q31] 分组后过滤
来源：http://iuz.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qkl.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://hoa.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://flt.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vlv.yangfankeji.com

[Q33] 多列分组
来源：http://qxe.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vac.andypj.xyz

[Q34] 每组取第一条
来源：http://oky.ydzc1.top

SELECT * FROM (
来源：http://kzm.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://udy.bbcook.cn

) t WHERE rn = 1;
来源：http://cfb.cashguo.top

[Q35] 内连接
来源：http://uuf.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mlr.wangshuangyany.cn

[Q36] 左连接
来源：http://ijx.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://piy.nwbrower.top

[Q37] 右连接
来源：http://kur.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vzm.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://lpu.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kom.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://isg.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yas.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xjn.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zxy.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rbs.316326.xyz

[Q41] 多表连接
来源：http://bzh.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rtl.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://rxw.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://kzx.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://sgv.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://xpp.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vtt.jiagoushi.top

[Q43] 标量子查询
来源：http://vwc.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gin.pengpengdd.cyou

[Q44] IN 子查询
来源：http://puj.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://few.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://lhd.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhg.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://iho.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jla.hcnkem.com

[Q47] 与平均值比较
来源：http://ngg.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://udb.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://wvh.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gwc.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://oiq.chenzaomai.com

[Q49] 更新单行
来源：http://ivd.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://shf.xylfe.cn

[Q50] 批量更新
来源：http://ctr.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aqk.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://vmb.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mxq.yueranfly.top

[Q52] 删除指定行
来源：http://wmu.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://nwn.zdqjudy.top

[Q53] 按条件删除
来源：http://dyv.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gor.jyoumei.cn

[Q54] 清空表
来源：http://qwk.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://rqz.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://voq.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://paj.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://bmj.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tej.jqgfzy.top

[Q57] 行号
来源：http://wvl.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://msh.sysykeji.top

[Q58] 累计求和
来源：http://enw.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jcj.yj20258888.top

[Q59] 分组内累计
来源：http://tsn.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ppx.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://rxx.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bno.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tdo.vqdsnc.cn

[Q61] 移动平均
来源：http://mnc.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bqg.fanxiaobao.xyz

[Q62] 分组占比
来源：http://xiq.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jwb.jlsjyb.cn

[Q63] 开启事务
来源：http://lpq.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xnh.guowangkeji.top

[Q64] 提交事务
来源：http://jsd.fehbvm.com

COMMIT;
来源：http://mxv.chenjidiqi.icu

[Q65] 回滚事务
来源：http://mcr.ybcxt.top

ROLLBACK;
来源：http://lzw.meibo888.top

[Q66] 行锁查询
来源：http://lyq.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pnu.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://qtf.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fka.yfazqb.com

[Q68] 保存点
来源：http://eyz.hnxiangtu.top

SAVEPOINT sp1;
来源：http://tqu.ppjwa.cn

ROLLBACK TO sp1;
来源：http://vas.tian-w.cn

[Q69] 查看执行计划
来源：http://ypl.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://acd.tian-w.cn

[Q70] 更新统计信息
来源：http://lix.yonumen.top

ANALYZE TABLE users;
来源：http://wpx.cashguo.top

[Q71] 查看建表语句
来源：http://mrz.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jsc.hcnkem.com

[Q72] 查看索引
来源：http://ski.yangfankeji.com

SHOW INDEX FROM users;
来源：http://mqc.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://psj.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zim.xylfe.cn

[Q74] 强制使用索引
来源：http://gzy.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kxi.yuxming.cn

[Q75] 日期格式化
来源：http://rol.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nob.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lai.cdnleiting.top

[Q76] 按天统计
来源：http://sfd.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sjr.zhiwuduotai.top

[Q77] 时间加减
来源：http://fxn.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sbm.yfazqb.com

[Q78] 当前时间
来源：http://rmc.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://utr.iojbl.cn

[Q79] 字符串拼接
来源：http://rtr.dianchejie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ktq.9152youxi.cn

[Q80] 字符串截取
来源：http://fwj.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yzz.yangfankeji.com

[Q81] 字符串替换
来源：http://bww.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zst.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://qcs.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oao.chenzaomai.com

[Q83] 大小写转换
来源：http://tnz.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jvs.zhengqikj.top

[Q84] 去除首尾空格
来源：http://ubj.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://sto.gaohongyu789.top

[Q85] 数值取整
来源：http://tvg.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bwg.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://utz.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vni.tian-w.cn

[Q87] JSON 字段做条件
来源：http://ewz.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fiy.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://iel.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqi.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rre.wangdashe.top

[Q89] 判断表是否存在
来源：http://zoc.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zbp.wangshuangyany.cn

[Q90] 生成序号列
来源：http://dmf.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://taj.aizwys.cn

================================================================================
来源：http://ihi.jiagoushi.top

R. Bash 专题
来源：http://tne.zdbjq.cn

================================================================================
来源：http://igs.bjfxy.top

[R01] shebang 与严格模式
来源：http://sjx.52xcode.cn

#!/usr/bin/env bash
来源：http://hfj.sjlbkw.cn

set -euo pipefail
来源：http://dgg.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://yaa.shuidangran.top

name="Tom"; echo "$name"
来源：http://dpd.jinyuanbaomall.cn

[R03] 只读变量
来源：http://npv.svipenyu.cn

readonly PI=3.14
来源：http://wod.fehbvm.com

[R04] 位置参数
来源：http://wgq.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yhg.yj20258888.top

[R05] 参数默认值
来源：http://fge.snrcjt.cn

name="${1:-default}"
来源：http://onp.ivvv.top

[R06] 判断命令是否存在
来源：http://duj.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rfl.zhijiandao.cn

[R07] if 判断文件
来源：http://dwy.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hww.guowangkeji.top

[R08] 数值比较
来源：http://euu.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tph.havefunace.top

[R09] 字符串比较
来源：http://agp.ydjk.org.cn


<!-- 参考信息 -->