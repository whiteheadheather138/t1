代发 wailian999

C#:   Parallel.For
来源：http://eyt.fktsv.cn

================================================================================
来源：http://yoy.tarul.cn

P. 常用工具函数
来源：http://vcx.yangfankeji.com

================================================================================
来源：http://sgk.gotoacloud.top

[P01] 生成 UUID
来源：http://rvr.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://mhy.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nit.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://kti.tarul.cn

TS:   crypto.randomUUID()
来源：http://gwf.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://wlu.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://mrw.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://imq.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://rla.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://qoh.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gei.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sji.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lpq.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ufm.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yam.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rlq.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tdv.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vfb.ctjpmb.com

[P03] 生成短随机字符串
来源：http://acq.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pjs.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fwr.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qjy.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wfc.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fog.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tkj.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://orc.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vyp.wangdashe.top

[P04] 求长度
来源：http://pvd.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ygs.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqk.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fww.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qpu.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://cxz.yj20258.top

Go:   len(arr);  len(m)
来源：http://gnc.ivvv.top

Ruby: x.length;  x.size
来源：http://onp.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nju.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://nme.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xen.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mlg.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://evg.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kfm.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jnx.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fcg.yuanzhike.top

Ruby: a == b
来源：http://hwx.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dhr.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qgo.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://icu.havefunace.top

PHP:  if (empty($x)) {}
来源：http://zdf.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nij.hysaishi.cn

TS:   if (x == null) {}
来源：http://mmm.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rzg.yj202588.top

Go:   if x == nil {}
来源：http://ngc.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bip.vehdjk.com

C#:   if (x is null) {}
来源：http://hck.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://zrt.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://thg.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://lhn.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dmf.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ult.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://agw.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jvd.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xkv.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://drj.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://vhs.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rft.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dox.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://czu.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tcs.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yct.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kwe.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://coq.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ovx.zhijiandao.cn

================================================================================
来源：http://dro.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dbz.pengpengdd.cyou

================================================================================
来源：http://kwb.fktsv.cn

[Q01] 创建表
来源：http://zth.ctjpmb.com

CREATE TABLE users (
来源：http://yvk.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wiu.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://sqj.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://zzf.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://byi.wangdashe.top

);
来源：http://asq.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://jiq.hnqzz.top

CREATE TABLE orders (
来源：http://joz.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqw.mhx1999.top

user_id INT NOT NULL,
来源：http://ixf.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://rci.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gqc.chenlongwang.top

);
来源：http://ymk.zycfv.cn

[Q03] 增加列
来源：http://ral.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://otg.bjfxy.top

[Q04] 修改列类型
来源：http://xms.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uyi.xylfe.cn

[Q05] 重命名列
来源：http://nfg.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bfj.tian-w.cn

[Q06] 删除列
来源：http://hkl.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://qgd.yuanzhike.top

[Q07] 删除表
来源：http://wog.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://otk.hnxiangtu.top

[Q08] 创建普通索引
来源：http://jqn.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://gxp.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://bqw.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qjc.316326.xyz

[Q10] 插入单行
来源：http://tiq.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wxq.gotoacloud.top

[Q11] 一次插入多行
来源：http://bvj.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vrj.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://eif.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ihp.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://upy.yongpay.top

[Q13] 忽略重复插入
来源：http://wiz.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bsi.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://uuc.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xyu.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pyt.zhoulong.xyz

[Q15] 查询全部
来源：http://bxm.aibaodan.cn

SELECT * FROM users;
来源：http://rfi.vehdjk.com

[Q16] 查询指定列
来源：http://eer.mhx1999.top

SELECT id, name FROM users;
来源：http://tfi.9152youxi.cn

[Q17] 条件查询
来源：http://npe.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://icj.cheryme.top

[Q18] 模糊匹配
来源：http://fjk.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oaz.sxryk.cn

[Q19] 范围查询
来源：http://lfc.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bbh.yuxming.cn

[Q20] IN 列表
来源：http://icl.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lax.fktsv.cn

[Q21] 空值判断
来源：http://psm.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bqa.smart0.xyz

[Q22] 排序
来源：http://had.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nhj.fengsongda.top

[Q23] 分页
来源：http://xbg.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dqj.chenlongwang.top

[Q24] 去重
来源：http://aij.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://hap.tanke756.top

[Q25] 只取前 N 条
来源：http://vsi.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lrt.xylfe.cn

[Q26] 计数
来源：http://onu.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://zcz.nanxinkj.top

[Q27] 条件计数
来源：http://ueq.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xon.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://eij.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://obc.svipenyu.cn

[Q29] 最大最小值
来源：http://djc.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oqs.cdnleiting.top

[Q30] 分组统计
来源：http://wmr.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vwr.gzhubu.top

[Q31] 分组后过滤
来源：http://qoo.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xnj.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://lqe.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://glc.9152youxi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zkx.fengsongda.top

[Q33] 多列分组
来源：http://jeq.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://obj.svipenyu.cn

[Q34] 每组取第一条
来源：http://wyu.shanyushiyangkeji.top

SELECT * FROM (
来源：http://stn.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://upj.havefunace.top

) t WHERE rn = 1;
来源：http://jny.sxryk.cn

[Q35] 内连接
来源：http://uaz.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://avr.zhixingplan.top

[Q36] 左连接
来源：http://cse.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rsc.hywenlv.cn

[Q37] 右连接
来源：http://shh.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ekx.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://wzv.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uuz.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://zqh.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ayr.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dnj.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eaz.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rwl.vqdsnc.cn

[Q41] 多表连接
来源：http://auc.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://htu.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://pgs.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://qtp.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://adb.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://wfk.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://css.fehbvm.com

[Q43] 标量子查询
来源：http://rka.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tjf.ivvv.top

[Q44] IN 子查询
来源：http://wru.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dol.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://yau.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eve.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vlt.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdw.mhx1999.top

[Q47] 与平均值比较
来源：http://pwi.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nsc.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://omt.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ptd.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://ccp.jqgufenzy.top

[Q49] 更新单行
来源：http://kpn.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://asu.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://hqc.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dyv.jinqigufen.top

[Q51] 用子查询更新
来源：http://wet.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://krn.cqqwz.cn

[Q52] 删除指定行
来源：http://svy.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://lgs.dashuyun.cn

[Q53] 按条件删除
来源：http://rbu.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nny.shanyushiyangtech.top

[Q54] 清空表
来源：http://oxr.ybcxt.top

TRUNCATE TABLE logs;
来源：http://jqb.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://opv.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rch.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://rbx.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ekr.chenlongwang.top

[Q57] 行号
来源：http://iti.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gob.yuanzhike.top

[Q58] 累计求和
来源：http://xrb.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yrq.zhongyouzk.top

[Q59] 分组内累计
来源：http://sxt.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tqi.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://ron.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fin.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vii.ctjpmb.com

[Q61] 移动平均
来源：http://kcl.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ddu.yanxiufei.cn

[Q62] 分组占比
来源：http://rdi.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lyz.c1oappe.top

[Q63] 开启事务
来源：http://wzg.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jdp.c1oappe.top

[Q64] 提交事务
来源：http://wmv.vehdjk.com

COMMIT;
来源：http://ads.nwbrower.top

[Q65] 回滚事务
来源：http://cli.fanxiaobao.xyz

ROLLBACK;
来源：http://ysr.yj202588.top

[Q66] 行锁查询
来源：http://vhr.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mlv.xuanzx.com

[Q67] 设置隔离级别
来源：http://lhb.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dwh.yonumen.top

[Q68] 保存点
来源：http://pwb.zhoulong.xyz

SAVEPOINT sp1;
来源：http://rir.fzhhl.top

ROLLBACK TO sp1;
来源：http://znp.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://iyc.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zwe.dianchejie.cn

[Q70] 更新统计信息
来源：http://otj.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://rrn.sweek.top

[Q71] 查看建表语句
来源：http://eaj.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zmh.xinyue.icu

[Q72] 查看索引
来源：http://aca.cdnleiting.top

SHOW INDEX FROM users;
来源：http://hji.shangyingyoupin.top

[Q73] 查看表状态
来源：http://jpl.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qee.tianlin.xyz

[Q74] 强制使用索引
来源：http://tqb.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bbm.havefunace.top

[Q75] 日期格式化
来源：http://qec.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xxx.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ozr.tianlin.xyz

[Q76] 按天统计
来源：http://quh.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uag.ehwqpu.com

[Q77] 时间加减
来源：http://uuv.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zxg.sxryk.cn

[Q78] 当前时间
来源：http://mnn.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://txx.snrcjt.cn

[Q79] 字符串拼接
来源：http://uhd.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qel.kuanghao11.cn

[Q80] 字符串截取
来源：http://xvz.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vlq.316326.xyz

[Q81] 字符串替换
来源：http://and.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pok.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://djp.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://brf.ehwqpu.com

[Q83] 大小写转换
来源：http://vsd.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://the.redwolf501.top

[Q84] 去除首尾空格
来源：http://znk.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://wmq.kuanghao11.cn

[Q85] 数值取整
来源：http://eop.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wtd.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://uwd.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://onl.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://nmj.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uvo.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://tzd.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kbl.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://evd.tian-w.cn

[Q89] 判断表是否存在
来源：http://bho.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jnm.zhengqikj.top

[Q90] 生成序号列
来源：http://ncn.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lcv.xuetiantiany.cn

================================================================================
来源：http://wsk.yfazqb.com

R. Bash 专题
来源：http://lxn.jqgfzy.top

================================================================================
来源：http://bce.hfpthk.cn

[R01] shebang 与严格模式
来源：http://tag.sjlbkw.cn

#!/usr/bin/env bash
来源：http://dkd.jlsjyb.cn

set -euo pipefail
来源：http://ooe.nwbrower.top

[R02] 变量赋值与使用
来源：http://ikt.xinyue.icu

name="Tom"; echo "$name"
来源：http://zfj.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://wvq.yongpay.top

readonly PI=3.14
来源：http://uwh.birdmap.top

[R04] 位置参数
来源：http://lxc.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgq.sweek.top

[R05] 参数默认值
来源：http://zwp.vehdjk.com

name="${1:-default}"
来源：http://ywe.chenlongwang.top

[R06] 判断命令是否存在
来源：http://wep.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cjd.ctjpmb.com

[R07] if 判断文件
来源：http://ysn.ctjpmb.com


<!-- 参考信息 -->