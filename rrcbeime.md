代发 wailian999

[O06] 使用进程池
来源：http://wry.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sjo.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://fmr.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://tpe.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://ovb.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uhs.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wfv.nanxuanxn.top

Ruby: // fork 块
来源：http://jml.vehdjk.com

C#:   Parallel.For
来源：http://bmx.fzhhl.top

================================================================================
来源：http://bpg.hongshengwenyu.top

P. 常用工具函数
来源：http://jfu.fzhhl.top

================================================================================
来源：http://dyt.sysykeji.top

[P01] 生成 UUID
来源：http://shp.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://ccl.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xus.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://izi.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://rnr.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://pcc.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://ewh.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://cjw.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://myr.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://iae.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ysb.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://puz.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ozi.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uwc.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hed.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dim.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vnj.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pwn.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://qzs.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://umz.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://acj.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxx.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tsr.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yym.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qzv.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://daj.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ufg.daxiang520.top

[P04] 求长度
来源：http://dsr.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://err.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nqo.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjf.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qld.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://wmc.tanke756.top

Go:   len(arr);  len(m)
来源：http://anx.aizwys.cn

Ruby: x.length;  x.size
来源：http://mux.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ipn.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://hsy.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://snc.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://npu.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ihf.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://afz.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uds.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sqc.birdmap.top

Ruby: a == b
来源：http://zps.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gfl.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vba.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hgs.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://bcm.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://scu.smart0.xyz

TS:   if (x == null) {}
来源：http://hua.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nkv.smart0.xyz

Go:   if x == nil {}
来源：http://xsj.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mdm.yfazqb.com

C#:   if (x is null) {}
来源：http://ooj.vehdjk.com

[P07] 防抖与节流
来源：http://uum.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://odf.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://ibu.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggh.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eao.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pui.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pke.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qnm.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://owa.meibo888.top

[P08] 处理浮点精度问题
来源：http://kkh.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://igb.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gfa.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xbl.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cnd.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bae.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sni.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lbs.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bip.ehwqpu.com

================================================================================
来源：http://vyn.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ypl.hcnkem.com

================================================================================
来源：http://ifj.aizwys.cn

[Q01] 创建表
来源：http://zkb.guowangkeji.top

CREATE TABLE users (
来源：http://umm.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nvc.ydjk.org.cn

name VARCHAR(50) NOT NULL,
来源：http://xwx.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://xuz.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://knu.snrcjt.cn

);
来源：http://ynv.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://fkh.ivvv.top

CREATE TABLE orders (
来源：http://sow.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iyo.yj20258.top

user_id INT NOT NULL,
来源：http://yiy.shuidangran.top

amount DECIMAL(10, 2),
来源：http://azo.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fei.iojbl.cn

);
来源：http://jlk.cashguo.top

[Q03] 增加列
来源：http://yfg.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zbb.zhoulong.xyz

[Q04] 修改列类型
来源：http://ieq.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sqe.zdbjq.cn

[Q05] 重命名列
来源：http://xzs.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kdf.shuidangran.top

[Q06] 删除列
来源：http://xxf.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pvj.xuanzx.com

[Q07] 删除表
来源：http://iwd.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://rlr.zhoulong.xyz

[Q08] 创建普通索引
来源：http://opj.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ktw.cheryme.top

[Q09] 创建唯一索引
来源：http://yar.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bmz.redwolf501.top

[Q10] 插入单行
来源：http://wqx.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dui.cqqwz.cn

[Q11] 一次插入多行
来源：http://fec.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://djd.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://rvg.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://tgs.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mcv.jiagoushi.top

[Q13] 忽略重复插入
来源：http://naw.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ezn.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://hjn.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://myt.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dvv.yanxiufei.cn

[Q15] 查询全部
来源：http://mzc.nwbrower.top

SELECT * FROM users;
来源：http://ovp.quarkkingdee.top

[Q16] 查询指定列
来源：http://tdo.yuanzhike.top

SELECT id, name FROM users;
来源：http://gzc.yj202588.top

[Q17] 条件查询
来源：http://dtq.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lmo.zhongyouzk.top

[Q18] 模糊匹配
来源：http://pfk.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jqe.52xcode.cn

[Q19] 范围查询
来源：http://jdo.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dim.chenzaomai.com

[Q20] IN 列表
来源：http://mfx.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uou.fktsv.cn

[Q21] 空值判断
来源：http://nsc.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wdo.daxiang520.top

[Q22] 排序
来源：http://pzt.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hid.jinghuilouyu.cn

[Q23] 分页
来源：http://mxp.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://elx.yvedp.cn

[Q24] 去重
来源：http://pax.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://wap.yuxming.cn

[Q25] 只取前 N 条
来源：http://psk.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wsb.havefunace.top

[Q26] 计数
来源：http://aim.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://smx.tianlin.xyz

[Q27] 条件计数
来源：http://gop.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ttr.jinqigufen.top

[Q28] 求和与平均
来源：http://mhd.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cdh.birdmap.top

[Q29] 最大最小值
来源：http://lsp.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nzu.daria6918.cn

[Q30] 分组统计
来源：http://nls.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wfz.zdqjudy.top

[Q31] 分组后过滤
来源：http://pwg.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ykz.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://ixt.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://caw.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xut.hongshengwenyu.top

[Q33] 多列分组
来源：http://yjb.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cxp.yanxiufei.cn

[Q34] 每组取第一条
来源：http://lhu.yj20258.top

SELECT * FROM (
来源：http://yqy.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dhz.sxryk.cn

) t WHERE rn = 1;
来源：http://gzl.yj20258.top

[Q35] 内连接
来源：http://jlk.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://erj.pengpengdd.cyou

[Q36] 左连接
来源：http://anh.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ivb.nanxinkj.top

[Q37] 右连接
来源：http://lln.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://izr.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://olt.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hek.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://tkx.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hci.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xmi.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xqg.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rwo.aizwys.cn

[Q41] 多表连接
来源：http://jyn.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qhp.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://fre.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wzw.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://akd.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://syb.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://abn.yfazqb.com

[Q43] 标量子查询
来源：http://egr.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aeo.xylfe.cn

[Q44] IN 子查询
来源：http://lus.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://miq.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://xwp.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aya.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tsp.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tes.daxiang520.top

[Q47] 与平均值比较
来源：http://pxu.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://teq.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://ssv.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ggh.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://hrp.hesvh.cn

[Q49] 更新单行
来源：http://pwd.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nvs.ehwqpu.com

[Q50] 批量更新
来源：http://qqs.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ilw.nwbrower.top

[Q51] 用子查询更新
来源：http://phn.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bfi.c1oappe.top

[Q52] 删除指定行
来源：http://uqw.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://xua.ivvv.top

[Q53] 按条件删除
来源：http://ctn.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yaz.iojbl.cn

[Q54] 清空表
来源：http://zud.fktsv.cn

TRUNCATE TABLE logs;
来源：http://fef.wangdashe.top

[Q55] 排名（并列占位）
来源：http://gbo.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://meu.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://ijw.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bfw.yangfankeji.com

[Q57] 行号
来源：http://kyn.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jfg.yj20258.top

[Q58] 累计求和
来源：http://wjv.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ljv.ivvv.top

[Q59] 分组内累计
来源：http://hkk.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bun.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://ola.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ijr.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zde.ehwqpu.com

[Q61] 移动平均
来源：http://ofu.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pcq.yangfankeji.com

[Q62] 分组占比
来源：http://zmw.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ydt.9152youxi.cn

[Q63] 开启事务
来源：http://qkl.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://raw.gogol.net.cn

[Q64] 提交事务
来源：http://ilg.jyoumei.cn

COMMIT;
来源：http://qnu.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://lhu.fengsongda.top

ROLLBACK;
来源：http://phf.wangdashe.top

[Q66] 行锁查询
来源：http://tgt.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://npj.yongpay.top

[Q67] 设置隔离级别
来源：http://vcf.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ric.fktsv.cn

[Q68] 保存点
来源：http://pmh.cashguo.top

SAVEPOINT sp1;
来源：http://xgm.daria6918.cn

ROLLBACK TO sp1;
来源：http://wjp.zhijiandao.cn

[Q69] 查看执行计划
来源：http://wis.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zos.kuanghao11.cn

[Q70] 更新统计信息
来源：http://llt.gogol.net.cn

ANALYZE TABLE users;
来源：http://tqj.nanxinkj.top

[Q71] 查看建表语句
来源：http://cnm.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zln.svipenyu.cn

[Q72] 查看索引
来源：http://nyw.svipenyu.cn

SHOW INDEX FROM users;
来源：http://zdi.zhengqikj.top

[Q73] 查看表状态
来源：http://efp.mhx1999.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bav.andypj.xyz

[Q74] 强制使用索引
来源：http://swb.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pwx.jlsjyb.cn

[Q75] 日期格式化
来源：http://zfg.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zmf.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nsr.shzxlz.cn

[Q76] 按天统计
来源：http://zrg.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sog.ctjpmb.com

[Q77] 时间加减
来源：http://ywy.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qrq.sysykeji.top

[Q78] 当前时间
来源：http://aiq.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://igp.sjlbkw.cn

[Q79] 字符串拼接
来源：http://psh.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://let.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://olo.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zap.jianghu66.top

[Q81] 字符串替换
来源：http://ypu.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ipa.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://res.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://stf.zdqjudy.top

[Q83] 大小写转换
来源：http://cjc.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oyr.316326.xyz

[Q84] 去除首尾空格
来源：http://bhl.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://tot.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://vjp.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eud.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://bgw.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://znb.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://wzb.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mtf.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://pvq.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qvd.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://knu.hfpthk.cn

[Q89] 判断表是否存在
来源：http://uzy.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qtg.sufxvd.cn

[Q90] 生成序号列
来源：http://vrl.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xpx.quarkkingdee.top

================================================================================
来源：http://wtb.jlsjyb.cn

R. Bash 专题
来源：http://erx.fanxiaobao.xyz

================================================================================
来源：http://qmt.sxryk.cn

[R01] shebang 与严格模式
来源：http://qwh.fehbvm.com

#!/usr/bin/env bash
来源：http://veb.mhx1999.top

set -euo pipefail
来源：http://rml.snrcjt.cn

[R02] 变量赋值与使用
来源：http://udc.yj20258.top

name="Tom"; echo "$name"
来源：http://xch.guowangkeji.top

[R03] 只读变量
来源：http://tdr.tarul.cn


<!-- 参考信息 -->