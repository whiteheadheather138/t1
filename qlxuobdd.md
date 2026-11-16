代发 wailian999

TS:   crypto.randomUUID()
来源：http://elt.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://opy.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://mzs.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://gbo.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://naa.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://wop.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://snj.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qst.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pal.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ien.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jhn.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rjv.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vdp.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mbd.hcnkem.com

[P03] 生成短随机字符串
来源：http://ksb.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ess.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wxo.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tkw.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jcm.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vjq.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nmb.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zpb.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fcn.xuanzx.com

[P04] 求长度
来源：http://bwo.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tmg.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lpg.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dxd.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uwn.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://qhk.fanxiaobao.xyz

Go:   len(arr);  len(m)
来源：http://zcn.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://xgm.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dxj.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://atz.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pfw.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bcp.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tgo.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gfy.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bcn.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://ixi.quarkkingdee.top

Ruby: a == b
来源：http://bjv.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bko.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://das.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rys.birdmap.top

PHP:  if (empty($x)) {}
来源：http://ecv.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ynf.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://ikl.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pbz.cqqwz.cn

Go:   if x == nil {}
来源：http://xqw.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nub.xuanzx.com

C#:   if (x is null) {}
来源：http://aho.sysykeji.top

[P07] 防抖与节流
来源：http://vcs.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rkf.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://cqh.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://okm.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fsu.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nkd.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yac.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ijn.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://avi.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://gwg.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sjr.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rxu.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cfo.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lfw.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yer.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwi.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yqp.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ria.guowangkeji.top

================================================================================
来源：http://jft.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nix.jinghuilouyu.cn

================================================================================
来源：http://pbu.birdmap.top

[Q01] 创建表
来源：http://vdm.xziqi.cn

CREATE TABLE users (
来源：http://rum.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fmy.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://irq.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://idi.cucudq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sci.snrcjt.cn

);
来源：http://njp.snrcjt.cn

[Q02] 创建带外键的表
来源：http://cxl.gaohongyu789.top

CREATE TABLE orders (
来源：http://cfp.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://szg.9152youxi.cn

user_id INT NOT NULL,
来源：http://lwh.xylfe.cn

amount DECIMAL(10, 2),
来源：http://wyi.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lvr.ywan-chungtsiang.top

);
来源：http://kcl.hcnkem.com

[Q03] 增加列
来源：http://dsp.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ohv.tanke756.top

[Q04] 修改列类型
来源：http://qvq.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kze.jqgufenzy.top

[Q05] 重命名列
来源：http://stf.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cjx.wangdashe.top

[Q06] 删除列
来源：http://iyd.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://sgt.hcnkem.com

[Q07] 删除表
来源：http://aim.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://iph.haohaochexian.top

[Q08] 创建普通索引
来源：http://ffb.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dez.zdbjq.cn

[Q09] 创建唯一索引
来源：http://trj.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uwe.ctjpmb.com

[Q10] 插入单行
来源：http://xkp.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wmg.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://swd.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sma.havefunace.top

[Q12] 插入后取自增 ID
来源：http://zdl.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://kns.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pxv.yonumen.top

[Q13] 忽略重复插入
来源：http://lvs.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zca.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://dxz.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bip.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gkk.fktsv.cn

[Q15] 查询全部
来源：http://xqb.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://ynd.tian-w.cn

[Q16] 查询指定列
来源：http://eet.chenzaomai.com

SELECT id, name FROM users;
来源：http://kml.dashuyun.cn

[Q17] 条件查询
来源：http://ukg.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qey.zycfv.cn

[Q18] 模糊匹配
来源：http://gmc.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cdk.hywenlv.cn

[Q19] 范围查询
来源：http://wes.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pvl.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://vvg.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://icl.tian-w.cn

[Q21] 空值判断
来源：http://mzr.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eaa.vehdjk.com

[Q22] 排序
来源：http://kvd.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jjd.bjfxy.top

[Q23] 分页
来源：http://kvt.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zwc.hnxiangtu.top

[Q24] 去重
来源：http://riv.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://kcr.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://ooz.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ipn.zhongyouzk.top

[Q26] 计数
来源：http://uxb.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://ceh.yueranfly.top

[Q27] 条件计数
来源：http://szj.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://msq.smart0.xyz

[Q28] 求和与平均
来源：http://euz.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nao.ehwqpu.com

[Q29] 最大最小值
来源：http://ovg.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jxt.sjlbkw.cn

[Q30] 分组统计
来源：http://hsj.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ppj.ydzc1.top

[Q31] 分组后过滤
来源：http://hvs.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yeb.gzhubu.top

[Q32] 分组拼接字符串
来源：http://txt.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jyf.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ntf.9152youxi.cn

[Q33] 多列分组
来源：http://zzn.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ngh.hysaishi.cn

[Q34] 每组取第一条
来源：http://fow.sweek.top

SELECT * FROM (
来源：http://xfa.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dfk.gzhubu.top

) t WHERE rn = 1;
来源：http://sjq.gotoacloud.top

[Q35] 内连接
来源：http://mxf.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kws.ctjpmb.com

[Q36] 左连接
来源：http://ehx.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ijw.daria6918.cn

[Q37] 右连接
来源：http://ofy.zhaomingkeji.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cir.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://ydr.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cfe.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://vbg.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rqb.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://udy.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://nhq.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nwk.ehwqpu.com

[Q41] 多表连接
来源：http://lar.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ybb.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://tlj.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://aic.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://zmv.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://xve.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gtc.nwbrower.top

[Q43] 标量子查询
来源：http://vlo.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oxh.redwolf501.top

[Q44] IN 子查询
来源：http://yam.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nig.cheryme.top

[Q45] EXISTS 判断存在
来源：http://exo.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://krs.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mgo.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rll.xylfe.cn

[Q47] 与平均值比较
来源：http://xyx.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dzp.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://zjm.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgl.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://sdy.hywenlv.cn

[Q49] 更新单行
来源：http://vzd.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zcl.bjfxy.top

[Q50] 批量更新
来源：http://wsm.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hwo.mhx1999.top

[Q51] 用子查询更新
来源：http://hhu.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vrx.guannengcc.top

[Q52] 删除指定行
来源：http://hfo.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://kdx.hcnkem.com

[Q53] 按条件删除
来源：http://dtx.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wvi.cqqwz.cn

[Q54] 清空表
来源：http://jki.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://mvw.nwbrower.top

[Q55] 排名（并列占位）
来源：http://moa.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ous.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://zfm.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yww.zhoulong.xyz

[Q57] 行号
来源：http://wsp.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zvr.yueranfly.top

[Q58] 累计求和
来源：http://cjs.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ghf.dashuyun.cn

[Q59] 分组内累计
来源：http://aur.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kik.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://asd.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://epp.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mfm.aibaodan.cn

[Q61] 移动平均
来源：http://roh.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mtn.yfazqb.com

[Q62] 分组占比
来源：http://zep.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://php.xinyue.icu

[Q63] 开启事务
来源：http://psb.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rkn.feifeiyinyue.top

[Q64] 提交事务
来源：http://dix.uphjek.com

COMMIT;
来源：http://lar.sufxvd.cn

[Q65] 回滚事务
来源：http://vir.jqgfzy.top

ROLLBACK;
来源：http://eoc.shangyingyoupin.top

[Q66] 行锁查询
来源：http://xqi.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://two.hnqzz.top

[Q67] 设置隔离级别
来源：http://zde.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://twm.zhijiandao.cn

[Q68] 保存点
来源：http://dnn.kuanghao11.cn

SAVEPOINT sp1;
来源：http://aux.yj202588.top

ROLLBACK TO sp1;
来源：http://wpc.daxiang520.top

[Q69] 查看执行计划
来源：http://iga.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://svq.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://jrr.hcnkem.com

ANALYZE TABLE users;
来源：http://qjp.c1oappe.top

[Q71] 查看建表语句
来源：http://ibq.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://woc.gotoacloud.top

[Q72] 查看索引
来源：http://xgo.0kj1m.cn

SHOW INDEX FROM users;
来源：http://jke.jianghu66.top

[Q73] 查看表状态
来源：http://cjn.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qsk.hnxiangtu.top

[Q74] 强制使用索引
来源：http://end.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aiu.hfpthk.cn

[Q75] 日期格式化
来源：http://ybg.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dhk.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hsk.sysykeji.top

[Q76] 按天统计
来源：http://ffi.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://svn.cheryme.top

[Q77] 时间加减
来源：http://evo.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pcl.cucudq.cn

[Q78] 当前时间
来源：http://gky.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qua.fehbvm.com

[Q79] 字符串拼接
来源：http://xwc.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ibp.hcnkem.com

[Q80] 字符串截取
来源：http://cyo.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gas.ctjpmb.com

[Q81] 字符串替换
来源：http://pgt.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aie.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://owm.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://skz.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://vuq.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xto.cashguo.top

[Q84] 去除首尾空格
来源：http://oqw.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://mrh.xuetiantiany.cn

[Q85] 数值取整
来源：http://mcm.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://udo.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://yer.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fmz.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://jvn.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wlu.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://nwg.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wqy.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ozq.andypj.xyz

[Q89] 判断表是否存在
来源：http://ncm.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://alg.zhiwuduotai.top

[Q90] 生成序号列
来源：http://rjf.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zzf.shangyingyoupin.top

================================================================================
来源：http://wcq.zhijiandao.cn

R. Bash 专题
来源：http://dei.shanyushiyangkeji.top

================================================================================
来源：http://aso.yueranfly.top

[R01] shebang 与严格模式
来源：http://vwm.gzhubu.top

#!/usr/bin/env bash
来源：http://npc.tarul.cn

set -euo pipefail
来源：http://eat.meibo888.top

[R02] 变量赋值与使用
来源：http://hwu.yvedp.cn

name="Tom"; echo "$name"
来源：http://cdp.zhoulong.xyz

[R03] 只读变量
来源：http://fda.sysykeji.top

readonly PI=3.14
来源：http://spd.sjlbkw.cn

[R04] 位置参数
来源：http://jui.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://obw.fzhhl.top

[R05] 参数默认值
来源：http://toe.shanyushiyangkeji.top

name="${1:-default}"
来源：http://ldp.yongpay.top

[R06] 判断命令是否存在
来源：http://ent.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vcq.fzhhl.top

[R07] if 判断文件
来源：http://kns.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oyf.redwolf501.top

[R08] 数值比较
来源：http://plx.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wpc.ctjpmb.com

[R09] 字符串比较
来源：http://hmw.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mdu.nanxuanxn.top

[R10] 正则匹配
来源：http://mtl.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dvx.xylfe.cn

[R11] case 多分支
来源：http://zji.ybcxt.top


<!-- 参考信息 -->