代发 wailian999

TS:   crypto.randomUUID()
来源：http://bvd.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://aec.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://ifg.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://wqx.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://dxt.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://cjq.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ssd.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://woi.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zod.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fli.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yhu.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ddz.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wlc.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zdn.gotoacloud.top

[P03] 生成短随机字符串
来源：http://mas.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yzs.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://raf.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://moy.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nfp.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfe.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bad.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://czj.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lgu.zhongyouzk.top

[P04] 求长度
来源：http://eht.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xvi.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nce.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lsn.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gap.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://dcl.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://ful.ivvv.top

Ruby: x.length;  x.size
来源：http://ouw.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zhv.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://aqq.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ash.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wwt.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vqx.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zwo.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dcc.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://jbp.shzxlz.cn

Ruby: a == b
来源：http://wfk.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://slm.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ijf.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kan.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://opm.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mhg.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://noi.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://hho.9152youxi.cn

Go:   if x == nil {}
来源：http://etf.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ugo.zhengqikj.top

C#:   if (x is null) {}
来源：http://voc.zhoulong.xyz

[P07] 防抖与节流
来源：http://umq.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ejp.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://hkv.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsj.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rqv.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yka.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pve.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyr.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uod.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://urd.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pcf.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xmr.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jqj.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ozd.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://owy.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ygg.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bcu.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xmo.dashuyun.cn

================================================================================
来源：http://ykm.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://thl.ydzc1.top

================================================================================
来源：http://xdd.hysaishi.cn

[Q01] 创建表
来源：http://uln.sjlbkw.cn

CREATE TABLE users (
来源：http://bff.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nrn.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://vty.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://kot.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pro.jqgfzy.top

);
来源：http://mjb.sufxvd.cn

[Q02] 创建带外键的表
来源：http://qfw.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://mcm.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dht.vqdsnc.cn

user_id INT NOT NULL,
来源：http://kmp.c1oappe.top

amount DECIMAL(10, 2),
来源：http://wyw.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aug.guannengcc.top

);
来源：http://qot.cashguo.top

[Q03] 增加列
来源：http://cos.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qri.pengpengdd.cyou

[Q04] 修改列类型
来源：http://rwh.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jma.yuxming.cn

[Q05] 重命名列
来源：http://cjt.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wlq.fengsongda.top

[Q06] 删除列
来源：http://akz.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://pvi.jianghu66.top

[Q07] 删除表
来源：http://iql.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://sez.hcnkem.com

[Q08] 创建普通索引
来源：http://myq.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nrs.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://bly.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uuf.hfpthk.cn

[Q10] 插入单行
来源：http://xid.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mph.gogol.net.cn

[Q11] 一次插入多行
来源：http://aii.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zop.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://wjg.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qjy.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aee.meibo888.top

[Q13] 忽略重复插入
来源：http://blz.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jgd.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://fae.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ljo.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wel.dashuyun.cn

[Q15] 查询全部
来源：http://nbr.hnxiangtu.top

SELECT * FROM users;
来源：http://gea.yueranfly.top

[Q16] 查询指定列
来源：http://rrl.haohaochexian.top

SELECT id, name FROM users;
来源：http://itj.daxiang520.top

[Q17] 条件查询
来源：http://pxy.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qom.zhixingplan.top

[Q18] 模糊匹配
来源：http://znl.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oir.ctjpmb.com

[Q19] 范围查询
来源：http://wgn.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mmc.c1oappe.top

[Q20] IN 列表
来源：http://ayx.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iyq.jinqigfzy.top

[Q21] 空值判断
来源：http://qrs.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cly.52xcode.cn

[Q22] 排序
来源：http://krz.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dry.jyoumei.cn

[Q23] 分页
来源：http://tdu.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://awi.hywenlv.cn

[Q24] 去重
来源：http://xrf.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://aah.xylfe.cn

[Q25] 只取前 N 条
来源：http://cjd.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://utf.yongpay.top

[Q26] 计数
来源：http://ubr.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://gsd.guowangkeji.top

[Q27] 条件计数
来源：http://rsr.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://duf.wangshuangyany.cn

[Q28] 求和与平均
来源：http://czm.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qka.ppjwa.cn

[Q29] 最大最小值
来源：http://nrv.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubv.wangshuangyany.cn

[Q30] 分组统计
来源：http://naz.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iwc.tanke756.top

[Q31] 分组后过滤
来源：http://eek.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cij.yonumen.top

[Q32] 分组拼接字符串
来源：http://vtf.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hbo.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kku.wangshuangyany.cn

[Q33] 多列分组
来源：http://zia.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tel.gzhubu.top

[Q34] 每组取第一条
来源：http://uxa.hesvh.cn

SELECT * FROM (
来源：http://sad.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wnj.cheryme.top

) t WHERE rn = 1;
来源：http://tzc.xylfe.cn

[Q35] 内连接
来源：http://rgf.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sox.meibo888.top

[Q36] 左连接
来源：http://qvx.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wya.gzhubu.top

[Q37] 右连接
来源：http://cir.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ewn.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://eil.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ysu.ivvv.top

[Q39] 自连接（查上下级）
来源：http://cxj.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vcb.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xow.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vbm.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jvr.guowangkeji.top

[Q41] 多表连接
来源：http://lym.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jkv.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://pip.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://lxn.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://ftg.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://per.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ibs.bjfxy.top

[Q43] 标量子查询
来源：http://qdd.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kym.yj20258888.top

[Q44] IN 子查询
来源：http://ctv.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nyj.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://pmo.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uzc.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vgf.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://htl.ppjwa.cn

[Q47] 与平均值比较
来源：http://rms.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lur.tanke756.top

[Q48] CTE 公用表表达式
来源：http://omb.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mxg.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://tbw.xziqi.cn

[Q49] 更新单行
来源：http://rov.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://enu.jinqigufen.top

[Q50] 批量更新
来源：http://ayg.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jjn.sjlbkw.cn

[Q51] 用子查询更新
来源：http://nfs.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aeh.yuanzhike.top

[Q52] 删除指定行
来源：http://edg.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://etb.feifeiyinyue.top

[Q53] 按条件删除
来源：http://jrv.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yvy.chenjidiqi.icu

[Q54] 清空表
来源：http://zmt.yj20258.top

TRUNCATE TABLE logs;
来源：http://cgp.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://eph.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oar.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://pqp.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sae.yuxming.cn

[Q57] 行号
来源：http://jmi.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jqc.zycfv.cn

[Q58] 累计求和
来源：http://ztb.hcnkem.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mam.zhongyouzk.top

[Q59] 分组内累计
来源：http://qfx.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nan.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://tju.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ump.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tyt.jqgfzy.top

[Q61] 移动平均
来源：http://uah.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wnh.yonumen.top

[Q62] 分组占比
来源：http://cjv.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ata.ctjpmb.com

[Q63] 开启事务
来源：http://vhk.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kco.hnqzz.top

[Q64] 提交事务
来源：http://jgr.yj202588.top

COMMIT;
来源：http://one.nanxuanxn.top

[Q65] 回滚事务
来源：http://evo.jlsjyb.cn

ROLLBACK;
来源：http://eov.hesvh.cn

[Q66] 行锁查询
来源：http://jrl.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qww.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://aml.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://via.daxiang520.top

[Q68] 保存点
来源：http://izc.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://cpn.xinyue.icu

ROLLBACK TO sp1;
来源：http://cpd.shzxlz.cn

[Q69] 查看执行计划
来源：http://rda.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oti.vehdjk.com

[Q70] 更新统计信息
来源：http://ijw.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://tad.wangdashe.top

[Q71] 查看建表语句
来源：http://oci.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dki.shuidangran.top

[Q72] 查看索引
来源：http://yri.cqqwz.cn

SHOW INDEX FROM users;
来源：http://gnt.cqqwz.cn

[Q73] 查看表状态
来源：http://hfz.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jvz.meibo888.top

[Q74] 强制使用索引
来源：http://avz.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wuz.jianghu66.top

[Q75] 日期格式化
来源：http://bne.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ttk.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wvl.daria6918.cn

[Q76] 按天统计
来源：http://rwp.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uvd.jqgufenzy.top

[Q77] 时间加减
来源：http://iad.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gif.jlsjyb.cn

[Q78] 当前时间
来源：http://qhm.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nhu.cucudq.cn

[Q79] 字符串拼接
来源：http://uhp.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://igr.chenjidiqi.icu

[Q80] 字符串截取
来源：http://suy.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cot.hfpthk.cn

[Q81] 字符串替换
来源：http://dxp.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mtr.cashguo.top

[Q82] 字符长度与字节长度
来源：http://hst.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ewg.redwolf501.top

[Q83] 大小写转换
来源：http://lib.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xpw.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://xxy.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://ewj.yj20258.top

[Q85] 数值取整
来源：http://kgo.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ssu.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://rqs.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lzq.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://lzh.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xrc.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://lvv.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tan.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hpf.cheryme.top

[Q89] 判断表是否存在
来源：http://yor.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tpp.xuanzx.com

[Q90] 生成序号列
来源：http://yvr.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gow.tanke756.top

================================================================================
来源：http://gzt.ywan-chungtsiang.top

R. Bash 专题
来源：http://xzs.ydjk.org.cn

================================================================================
来源：http://zqu.jinqigufen.top

[R01] shebang 与严格模式
来源：http://snt.hcnkem.com

#!/usr/bin/env bash
来源：http://kng.jyoumei.cn

set -euo pipefail
来源：http://leo.xziqi.cn

[R02] 变量赋值与使用
来源：http://cna.nwbrower.top

name="Tom"; echo "$name"
来源：http://izr.kuanghao11.cn

[R03] 只读变量
来源：http://sqx.nanxinkj.top

readonly PI=3.14
来源：http://mnj.hammf.cn

[R04] 位置参数
来源：http://tal.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cng.redwolf501.top

[R05] 参数默认值
来源：http://xsd.wangshuangyany.cn

name="${1:-default}"
来源：http://pzt.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://nud.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nhq.ydjk.org.cn

[R07] if 判断文件
来源：http://amn.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xkf.zhixingplan.top

[R08] 数值比较
来源：http://mrd.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xqz.uphjek.com

[R09] 字符串比较
来源：http://tnd.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ubk.hysaishi.cn

[R10] 正则匹配
来源：http://lis.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krc.fanxiaobao.xyz

[R11] case 多分支
来源：http://dqd.yueranfly.top


<!-- 参考信息 -->