代发 wailian999

C#:   Parallel.For
来源：http://wwm.fzhhl.top

================================================================================
来源：http://yce.hongshengwenyu.top

P. 常用工具函数
来源：http://ysw.zhoulong.xyz

================================================================================
来源：http://tib.ehwqpu.com

[P01] 生成 UUID
来源：http://ihs.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://ulk.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zxq.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://rlk.hnqzz.top

TS:   crypto.randomUUID()
来源：http://giq.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://ukq.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://olp.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://hfe.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://xtd.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://iiq.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hff.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rju.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uhr.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://drw.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tuw.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uxd.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pey.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fzg.guannengcc.top

[P03] 生成短随机字符串
来源：http://gww.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mvs.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ssj.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jrz.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uva.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ylo.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yuk.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://sis.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://llo.yuanzhike.top

[P04] 求长度
来源：http://qqf.jianghu66.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pzc.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jfj.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ywb.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xpq.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://lum.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://ekl.meibo888.top

Ruby: x.length;  x.size
来源：http://bai.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kno.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://ffc.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dxh.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://chn.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sbv.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzc.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://evk.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kkg.meibo888.top

Ruby: a == b
来源：http://adk.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ldn.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tsh.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wjs.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://gtv.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kgl.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://khh.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://isw.gaohongyu789.top

Go:   if x == nil {}
来源：http://kkd.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kzy.guannengcc.top

C#:   if (x is null) {}
来源：http://zwg.52xcode.cn

[P07] 防抖与节流
来源：http://lvo.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aph.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://ujw.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlr.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dei.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rag.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://olk.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yjp.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hms.sysykeji.top

[P08] 处理浮点精度问题
来源：http://oqh.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gbm.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ddf.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://czo.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pfy.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cuz.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dgo.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tlu.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jxu.chenjidiqi.icu

================================================================================
来源：http://dty.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fwv.sysykeji.top

================================================================================
来源：http://wqy.haohaochexian.top

[Q01] 创建表
来源：http://ium.svipenyu.cn

CREATE TABLE users (
来源：http://pdz.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bbv.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://dbr.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://nsc.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kcd.nanxinkj.top

);
来源：http://lai.uphjek.com

[Q02] 创建带外键的表
来源：http://fwj.jqgfzy.top

CREATE TABLE orders (
来源：http://zio.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ksw.tarul.cn

user_id INT NOT NULL,
来源：http://hpv.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://fda.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tij.zhengqikj.top

);
来源：http://bin.chenzaomai.com

[Q03] 增加列
来源：http://jho.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kix.fengsongda.top

[Q04] 修改列类型
来源：http://ywh.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hux.andypj.xyz

[Q05] 重命名列
来源：http://fsm.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://szs.bbcook.cn

[Q06] 删除列
来源：http://joa.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://bgz.jyoumei.cn

[Q07] 删除表
来源：http://vqq.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://ufh.bbcook.cn

[Q08] 创建普通索引
来源：http://ent.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hvu.zdqjudy.top

[Q09] 创建唯一索引
来源：http://jpx.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://azr.ywan-chungtsiang.top

[Q10] 插入单行
来源：http://pwx.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dnj.bjfxy.top

[Q11] 一次插入多行
来源：http://ezv.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lls.cashguo.top

[Q12] 插入后取自增 ID
来源：http://ddg.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eec.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://amg.smart0.xyz

[Q13] 忽略重复插入
来源：http://bft.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vgy.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://xwn.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iqh.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://loc.iojbl.cn

[Q15] 查询全部
来源：http://mwf.xziqi.cn

SELECT * FROM users;
来源：http://jpc.jyoumei.cn

[Q16] 查询指定列
来源：http://gcc.yongpay.top

SELECT id, name FROM users;
来源：http://ncs.zhoulong.xyz

[Q17] 条件查询
来源：http://lpl.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fhr.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://mqw.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oms.bbcook.cn

[Q19] 范围查询
来源：http://wvv.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zbi.gotoacloud.top

[Q20] IN 列表
来源：http://dii.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jlw.xuanzx.com

[Q21] 空值判断
来源：http://vsm.haohaochexian.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xgl.pycfn.com

[Q22] 排序
来源：http://roe.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oty.dashuyun.cn

[Q23] 分页
来源：http://uos.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wit.quarkkingdee.top

[Q24] 去重
来源：http://xkw.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://xbn.yuxming.cn

[Q25] 只取前 N 条
来源：http://fed.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hzt.zycfv.cn

[Q26] 计数
来源：http://bsk.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://knl.sxryk.cn

[Q27] 条件计数
来源：http://xzd.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dup.hnxiangtu.top

[Q28] 求和与平均
来源：http://ele.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xjp.vehdjk.com

[Q29] 最大最小值
来源：http://myy.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://toh.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://rjo.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wvl.uphjek.com

[Q31] 分组后过滤
来源：http://mgc.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jpz.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://bzi.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ago.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jtl.ivvv.top

[Q33] 多列分组
来源：http://the.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hve.chenlongwang.top

[Q34] 每组取第一条
来源：http://bnu.ydzc1.top

SELECT * FROM (
来源：http://bxf.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oxn.svipenyu.cn

) t WHERE rn = 1;
来源：http://gry.fengsongda.top

[Q35] 内连接
来源：http://drw.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pwj.hesvh.cn

[Q36] 左连接
来源：http://hll.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jye.zdbjq.cn

[Q37] 右连接
来源：http://obd.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ohd.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dkd.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hcy.yongpay.top

[Q39] 自连接（查上下级）
来源：http://hac.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xjd.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tdk.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oak.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://svg.tarul.cn

[Q41] 多表连接
来源：http://aog.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gcq.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://zmv.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://dgs.zhijiandao.cn

[Q42] 连接条件附加过滤
来源：http://qff.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://mjd.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aeu.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://ipw.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xqy.zhoulong.xyz

[Q44] IN 子查询
来源：http://lwi.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ygo.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://sge.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvt.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nxj.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpa.dianchejie.cn

[Q47] 与平均值比较
来源：http://lmz.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tpp.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://bjj.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hgt.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://kse.shangyingyoupin.top

[Q49] 更新单行
来源：http://xxz.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mul.nanxinkj.top

[Q50] 批量更新
来源：http://bkm.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mmo.zhixingplan.top

[Q51] 用子查询更新
来源：http://fgc.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bcc.hnxiangtu.top

[Q52] 删除指定行
来源：http://dol.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://krx.snrcjt.cn

[Q53] 按条件删除
来源：http://cnh.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zpg.jinqigufen.top

[Q54] 清空表
来源：http://gvr.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://duj.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://nwm.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bta.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://rpt.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xdx.yj202588.top

[Q57] 行号
来源：http://gox.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lyp.gogol.net.cn

[Q58] 累计求和
来源：http://gqq.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lmx.guannengcc.top

[Q59] 分组内累计
来源：http://hfp.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qsp.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://pvl.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wev.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hoc.fengsongda.top

[Q61] 移动平均
来源：http://dhs.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpr.jqgfzy.top

[Q62] 分组占比
来源：http://thx.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cyw.fengsongda.top

[Q63] 开启事务
来源：http://jsl.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://hlq.haohaochexian.top

[Q64] 提交事务
来源：http://aor.cdnleiting.top

COMMIT;
来源：http://vbi.shangyingyoupin.top

[Q65] 回滚事务
来源：http://yul.redwolf501.top

ROLLBACK;
来源：http://jvk.jqgufenzy.top

[Q66] 行锁查询
来源：http://vcy.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ikq.hnqzz.top

[Q67] 设置隔离级别
来源：http://mgx.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gyk.wangdashe.top

[Q68] 保存点
来源：http://lmu.hammf.cn

SAVEPOINT sp1;
来源：http://krx.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://zbf.yuanzhike.top

[Q69] 查看执行计划
来源：http://ykt.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ejp.yongpay.top

[Q70] 更新统计信息
来源：http://bjk.daxiang520.top

ANALYZE TABLE users;
来源：http://jpe.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://thw.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fvy.aizwys.cn

[Q72] 查看索引
来源：http://day.aizwys.cn

SHOW INDEX FROM users;
来源：http://gvv.andypj.xyz

[Q73] 查看表状态
来源：http://ipp.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xfp.fengsongda.top

[Q74] 强制使用索引
来源：http://cnd.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jcl.jinqigfzy.top

[Q75] 日期格式化
来源：http://nkd.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://her.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gwz.jqgufenzy.top

[Q76] 按天统计
来源：http://okz.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xfq.hammf.cn

[Q77] 时间加减
来源：http://kkv.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://knm.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://rvp.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vox.hnxiangtu.top

[Q79] 字符串拼接
来源：http://qwa.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://llr.feifeiyinyue.top

[Q80] 字符串截取
来源：http://rum.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cul.cheryme.top

[Q81] 字符串替换
来源：http://ocu.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cax.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://cjh.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yns.cucudq.cn

[Q83] 大小写转换
来源：http://evn.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xhs.redwolf501.top

[Q84] 去除首尾空格
来源：http://aub.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://pib.gaohongyu789.top

[Q85] 数值取整
来源：http://ibo.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ndf.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://kbu.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uch.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://bne.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jkc.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://vtb.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yyo.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ybe.cashguo.top

[Q89] 判断表是否存在
来源：http://ueu.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pla.316326.xyz

[Q90] 生成序号列
来源：http://gls.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mgy.fengsongda.top

================================================================================
来源：http://xht.yj20258888.top

R. Bash 专题
来源：http://glc.jianghu66.top

================================================================================
来源：http://aco.gzhubu.top

[R01] shebang 与严格模式
来源：http://psa.yj202588.top

#!/usr/bin/env bash
来源：http://ynb.meibo888.top

set -euo pipefail
来源：http://vkp.nanxinkj.top

[R02] 变量赋值与使用
来源：http://zeo.birdmap.top

name="Tom"; echo "$name"
来源：http://qtz.quarkkingdee.top

[R03] 只读变量
来源：http://sti.daria6918.cn

readonly PI=3.14
来源：http://nzi.yanxiufei.cn

[R04] 位置参数
来源：http://ohg.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hve.hesvh.cn

[R05] 参数默认值
来源：http://pmr.hywenlv.cn

name="${1:-default}"
来源：http://qeo.zhixingplan.top

[R06] 判断命令是否存在
来源：http://xec.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tbk.mhx1999.top

[R07] if 判断文件
来源：http://lpl.shzxlz.cn


<!-- 参考信息 -->