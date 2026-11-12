代发 wailian999

C#:   Parallel.For
来源：http://mrq.shanyushiyangtech.top

================================================================================
来源：http://vqf.52xcode.cn

P. 常用工具函数
来源：http://wjg.aizwys.cn

================================================================================
来源：http://hbh.cashguo.top

[P01] 生成 UUID
来源：http://why.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://mgb.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bmc.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://veo.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://rad.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://cqm.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://wyd.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://tjm.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://zqt.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://cfz.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ueq.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jpm.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jlt.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sqx.uphjek.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ckt.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lyh.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fkl.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fdt.cqqwz.cn

[P03] 生成短随机字符串
来源：http://buk.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ciz.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vrt.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zwa.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ilh.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fft.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hft.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rqq.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cue.pengpengdd.cyou

[P04] 求长度
来源：http://ymm.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nfq.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhv.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://odk.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://odm.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://cah.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://nzd.yj20258.top

Ruby: x.length;  x.size
来源：http://dxt.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jir.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://pvy.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://fbp.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ehh.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://flm.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vde.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vno.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://yqy.c1oappe.top

Ruby: a == b
来源：http://lbk.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tdh.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mcq.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vap.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://oly.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://chh.ppjwa.cn

TS:   if (x == null) {}
来源：http://wtg.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kzp.9152youxi.cn

Go:   if x == nil {}
来源：http://yel.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gak.ybcxt.top

C#:   if (x is null) {}
来源：http://kqp.cdnleiting.top

[P07] 防抖与节流
来源：http://iwn.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://npm.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://nhp.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsw.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpb.cheryme.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://djx.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lmf.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tcu.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lme.mhx1999.top

[P08] 处理浮点精度问题
来源：http://dsu.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxe.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sky.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ytd.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gbh.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rjc.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ybp.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xif.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mxf.jyoumei.cn

================================================================================
来源：http://bcn.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xyl.ydjk.org.cn

================================================================================
来源：http://yjg.aizwys.cn

[Q01] 创建表
来源：http://aej.dashuyun.cn

CREATE TABLE users (
来源：http://thu.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pqp.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://amj.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://aii.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hvc.zhongyouzk.top

);
来源：http://myf.yfazqb.com

[Q02] 创建带外键的表
来源：http://imu.daria6918.cn

CREATE TABLE orders (
来源：http://fkf.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hpf.guowangkeji.top

user_id INT NOT NULL,
来源：http://wnt.yj202588.top

amount DECIMAL(10, 2),
来源：http://gbl.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dgb.dashuyun.cn

);
来源：http://ntr.yuxming.cn

[Q03] 增加列
来源：http://gmc.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fyk.shzxlz.cn

[Q04] 修改列类型
来源：http://tcf.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qsc.chenlongwang.top

[Q05] 重命名列
来源：http://eot.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://szy.daria6918.cn

[Q06] 删除列
来源：http://adx.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://xqf.tianlin.xyz

[Q07] 删除表
来源：http://txa.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://anc.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://rbr.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jpj.wangdashe.top

[Q09] 创建唯一索引
来源：http://tpm.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ptm.meibo888.top

[Q10] 插入单行
来源：http://pce.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tqb.fengsongda.top

[Q11] 一次插入多行
来源：http://pin.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ijg.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://oru.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://lte.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nbf.yongpay.top

[Q13] 忽略重复插入
来源：http://pys.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ehu.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://klx.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hpk.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ula.bbcook.cn

[Q15] 查询全部
来源：http://ige.vehdjk.com

SELECT * FROM users;
来源：http://nyz.guannengcc.top

[Q16] 查询指定列
来源：http://rql.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://jov.fanxiaobao.xyz

[Q17] 条件查询
来源：http://glo.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uqp.tanke756.top

[Q18] 模糊匹配
来源：http://ors.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fqz.nanxinkj.top

[Q19] 范围查询
来源：http://fpo.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hux.jqgufenzy.top

[Q20] IN 列表
来源：http://chc.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tct.tanke756.top

[Q21] 空值判断
来源：http://dit.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kdm.cdnleiting.top

[Q22] 排序
来源：http://cfl.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wyp.cdnleiting.top

[Q23] 分页
来源：http://ekf.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wwu.tarul.cn

[Q24] 去重
来源：http://izt.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://eke.tianlin.xyz

[Q25] 只取前 N 条
来源：http://tgd.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mdn.bjfxy.top

[Q26] 计数
来源：http://stx.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://sed.tian-w.cn

[Q27] 条件计数
来源：http://bew.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gtv.hnqzz.top

[Q28] 求和与平均
来源：http://dim.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jrf.vehdjk.com

[Q29] 最大最小值
来源：http://yir.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uno.haohaochexian.top

[Q30] 分组统计
来源：http://rxi.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mgv.0kj1m.cn

[Q31] 分组后过滤
来源：http://llv.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://klc.wangdashe.top

[Q32] 分组拼接字符串
来源：http://bbw.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xia.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vxl.chenzaomai.com

[Q33] 多列分组
来源：http://ymg.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vzs.yanxiufei.cn

[Q34] 每组取第一条
来源：http://hjl.chenlongwang.top

SELECT * FROM (
来源：http://pqd.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://okw.guannengcc.top

) t WHERE rn = 1;
来源：http://kal.xylfe.cn

[Q35] 内连接
来源：http://ipp.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mby.nanxinkj.top

[Q36] 左连接
来源：http://bms.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dxt.ehwqpu.com

[Q37] 右连接
来源：http://sce.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cnh.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://vnm.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://myj.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://exe.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://aix.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ugj.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qvk.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pkh.cdnleiting.top

[Q41] 多表连接
来源：http://prg.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sqy.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://tgj.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://hgh.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://fyi.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://ehm.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yoy.cheryme.top

[Q43] 标量子查询
来源：http://nav.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uva.vqdsnc.cn

[Q44] IN 子查询
来源：http://ure.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dxm.meibo888.top

[Q45] EXISTS 判断存在
来源：http://rfr.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://agp.fengsongda.top

[Q46] NOT EXISTS 判断不存在
来源：http://ovs.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oht.hnqzz.top

[Q47] 与平均值比较
来源：http://jdc.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jpl.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://ylo.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ela.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://jvs.jinqigufen.top

[Q49] 更新单行
来源：http://xer.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qze.ydzc1.top

[Q50] 批量更新
来源：http://pat.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lvc.yvedp.cn

[Q51] 用子查询更新
来源：http://xru.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wlo.nanxuanxn.top

[Q52] 删除指定行
来源：http://lgg.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://agm.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://eff.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wfx.nanxinkj.top

[Q54] 清空表
来源：http://qku.uphjek.com

TRUNCATE TABLE logs;
来源：http://xql.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://klr.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fbg.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://kqa.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://day.tanke756.top

[Q57] 行号
来源：http://rpi.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dfd.mhx1999.top

[Q58] 累计求和
来源：http://clh.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eur.xziqi.cn

[Q59] 分组内累计
来源：http://nfc.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://icu.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://lcx.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zeu.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://azg.zhoulong.xyz

[Q61] 移动平均
来源：http://tnv.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kff.yuxming.cn

[Q62] 分组占比
来源：http://edn.yueranfly.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfq.wangdashe.top

[Q63] 开启事务
来源：http://mju.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jio.wangshuangyany.cn

[Q64] 提交事务
来源：http://iel.yongpay.top

COMMIT;
来源：http://qgp.chenzaomai.com

[Q65] 回滚事务
来源：http://tfy.snrcjt.cn

ROLLBACK;
来源：http://yer.shzxlz.cn

[Q66] 行锁查询
来源：http://kib.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vea.aizwys.cn

[Q67] 设置隔离级别
来源：http://vcu.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zbf.birdmap.top

[Q68] 保存点
来源：http://zbc.cqqwz.cn

SAVEPOINT sp1;
来源：http://gel.gotoacloud.top

ROLLBACK TO sp1;
来源：http://yqo.vehdjk.com

[Q69] 查看执行计划
来源：http://vxt.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uis.fengsongda.top

[Q70] 更新统计信息
来源：http://dwb.yuxming.cn

ANALYZE TABLE users;
来源：http://dqk.xuetiantiany.cn

[Q71] 查看建表语句
来源：http://zcw.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://usy.jyoumei.cn

[Q72] 查看索引
来源：http://rdg.daria6918.cn

SHOW INDEX FROM users;
来源：http://uml.nanxuanxn.top

[Q73] 查看表状态
来源：http://avx.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://psj.ydjk.org.cn

[Q74] 强制使用索引
来源：http://isl.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rxd.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://rbb.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cyg.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ywy.sysykeji.top

[Q76] 按天统计
来源：http://xga.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yrg.fzhhl.top

[Q77] 时间加减
来源：http://amj.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nem.wangdashe.top

[Q78] 当前时间
来源：http://qko.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lvk.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://xuv.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gnu.hysaishi.cn

[Q80] 字符串截取
来源：http://mof.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qnq.yj20258.top

[Q81] 字符串替换
来源：http://dtb.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vov.sweek.top

[Q82] 字符长度与字节长度
来源：http://agn.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bvh.jinqigfzy.top

[Q83] 大小写转换
来源：http://brj.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ovz.yuanzhike.top

[Q84] 去除首尾空格
来源：http://kvi.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://nze.jlsjyb.cn

[Q85] 数值取整
来源：http://gzz.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oyl.tarul.cn

[Q86] 读取 JSON 字段
来源：http://osc.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hxg.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://ray.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xhn.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://xsj.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ooh.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eel.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://lvw.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mwx.zdbjq.cn

[Q90] 生成序号列
来源：http://hcn.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tpv.yj20258888.top

================================================================================
来源：http://eqd.pengpengdd.cyou

R. Bash 专题
来源：http://lar.mhx1999.top

================================================================================
来源：http://vxw.daxiang520.top

[R01] shebang 与严格模式
来源：http://ixp.yongpay.top

#!/usr/bin/env bash
来源：http://oox.birdmap.top

set -euo pipefail
来源：http://yim.dianchejie.cn

[R02] 变量赋值与使用
来源：http://xox.nwbrower.top

name="Tom"; echo "$name"
来源：http://bwe.sysykeji.top

[R03] 只读变量
来源：http://geu.yj20258.top

readonly PI=3.14
来源：http://wqd.fehbvm.com

[R04] 位置参数
来源：http://dnk.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iqx.hywenlv.cn

[R05] 参数默认值
来源：http://xkc.iojbl.cn

name="${1:-default}"
来源：http://ocm.havefunace.top

[R06] 判断命令是否存在
来源：http://wbp.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kye.haohaochexian.top

[R07] if 判断文件
来源：http://yhn.andypj.xyz


<!-- 参考信息 -->