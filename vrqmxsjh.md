代发 wailian999

[P01] 生成 UUID
来源：http://zct.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://koi.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://twx.wangdashe.top

JS:   crypto.randomUUID()
来源：http://kog.daria6918.cn

TS:   crypto.randomUUID()
来源：http://klz.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://ltu.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://xgm.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://wru.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://zzw.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://khk.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fsr.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pzw.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dcj.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jmi.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oam.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bha.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cqk.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cjj.cucudq.cn

[P03] 生成短随机字符串
来源：http://uvt.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zlw.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iod.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mwc.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cxb.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lqv.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xoz.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zvn.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ahe.ppjwa.cn

[P04] 求长度
来源：http://jvt.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xwd.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://upg.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oas.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ifk.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://dmy.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://njp.uphjek.com

Ruby: x.length;  x.size
来源：http://lys.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rcg.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://zhl.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://age.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oed.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xwo.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fwt.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lpb.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://fae.daria6918.cn

Ruby: a == b
来源：http://iko.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pxa.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yui.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://udo.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://nic.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nbu.shzxlz.cn

TS:   if (x == null) {}
来源：http://vtm.smart0.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://whl.hnxiangtu.top

Go:   if x == nil {}
来源：http://sns.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mnc.zdqjudy.top

C#:   if (x is null) {}
来源：http://pcv.jinqigufen.top

[P07] 防抖与节流
来源：http://hqq.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qzn.yj20258.top

PHP:  // 手写时间戳比较
来源：http://fsc.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gou.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wmv.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ull.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cqk.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://cyl.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://efb.daxiang520.top

[P08] 处理浮点精度问题
来源：http://dfz.yj20258.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qbo.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mzr.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pvk.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ktq.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qnb.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://djp.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gdn.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gqi.jianghu66.top

================================================================================
来源：http://rrj.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lgz.nanxinkj.top

================================================================================
来源：http://rsb.wangdashe.top

[Q01] 创建表
来源：http://sqy.316326.xyz

CREATE TABLE users (
来源：http://ogh.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vvq.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://jrn.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://wqn.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sbp.yueranfly.top

);
来源：http://ljs.yj20258.top

[Q02] 创建带外键的表
来源：http://txq.zdqjudy.top

CREATE TABLE orders (
来源：http://tys.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://crt.pycfn.com

user_id INT NOT NULL,
来源：http://xti.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://dbx.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eez.zdbjq.cn

);
来源：http://otn.jianghu66.top

[Q03] 增加列
来源：http://mrw.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qzu.ehwqpu.com

[Q04] 修改列类型
来源：http://oam.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baj.chenzaomai.com

[Q05] 重命名列
来源：http://riv.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zai.andypj.xyz

[Q06] 删除列
来源：http://die.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aoy.guannengcc.top

[Q07] 删除表
来源：http://wnv.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://aec.epnwcf.com

[Q08] 创建普通索引
来源：http://jpf.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ham.c1oappe.top

[Q09] 创建唯一索引
来源：http://pkt.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wcz.zhixingplan.top

[Q10] 插入单行
来源：http://cjp.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://amr.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://cva.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://myw.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://wzt.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://lpd.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wru.yuanzhike.top

[Q13] 忽略重复插入
来源：http://ila.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yua.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://xfa.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pwp.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mkl.fanxiaobao.xyz

[Q15] 查询全部
来源：http://hrc.yueranfly.top

SELECT * FROM users;
来源：http://vpw.tarul.cn

[Q16] 查询指定列
来源：http://noi.jiagoushi.top

SELECT id, name FROM users;
来源：http://cer.guowangkeji.top

[Q17] 条件查询
来源：http://khk.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://usv.daxiang520.top

[Q18] 模糊匹配
来源：http://mek.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pub.vqdsnc.cn

[Q19] 范围查询
来源：http://btp.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kxl.snrcjt.cn

[Q20] IN 列表
来源：http://get.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pav.wangdashe.top

[Q21] 空值判断
来源：http://flq.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dis.jqgufenzy.top

[Q22] 排序
来源：http://yoz.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://abm.c1oappe.top

[Q23] 分页
来源：http://gkv.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gqm.zhaomingkeji.xyz

[Q24] 去重
来源：http://ets.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://nup.cashguo.top

[Q25] 只取前 N 条
来源：http://cfz.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ltb.ywan-chungtsiang.top

[Q26] 计数
来源：http://inz.sweek.top

SELECT COUNT(*) FROM users;
来源：http://jll.wangdashe.top

[Q27] 条件计数
来源：http://prm.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eiq.zhoulong.xyz

[Q28] 求和与平均
来源：http://xgo.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ixz.zhijiandao.cn

[Q29] 最大最小值
来源：http://inn.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yoe.zdqjudy.top

[Q30] 分组统计
来源：http://tsc.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ldo.gotoacloud.top

[Q31] 分组后过滤
来源：http://hxw.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oie.ybcxt.top

[Q32] 分组拼接字符串
来源：http://chf.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qbr.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bir.sweek.top

[Q33] 多列分组
来源：http://fwp.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tha.bbcook.cn

[Q34] 每组取第一条
来源：http://sgt.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://wpt.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cpm.tian-w.cn

) t WHERE rn = 1;
来源：http://xrc.vehdjk.com

[Q35] 内连接
来源：http://hpt.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wsw.guowangkeji.top

[Q36] 左连接
来源：http://nve.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jqc.jinqigufen.top

[Q37] 右连接
来源：http://ymi.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://svn.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kcj.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zeo.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://bje.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://pwi.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ddq.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dpl.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mud.yj202588.top

[Q41] 多表连接
来源：http://jeq.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vzm.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://kxa.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://jnh.pycfn.com

[Q42] 连接条件附加过滤
来源：http://ibj.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://dzy.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://htj.yvedp.cn

[Q43] 标量子查询
来源：http://hdg.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tkj.cheryme.top

[Q44] IN 子查询
来源：http://nih.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oju.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://ovm.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pch.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vrk.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kfw.aibaodan.cn

[Q47] 与平均值比较
来源：http://oak.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fjd.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://jfp.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oqg.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://dry.jqgufenzy.top

[Q49] 更新单行
来源：http://fgh.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://faq.epnwcf.com

[Q50] 批量更新
来源：http://tov.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ynn.nwbrower.top

[Q51] 用子查询更新
来源：http://jnn.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qvy.bjfxy.top

[Q52] 删除指定行
来源：http://kmb.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://wdv.zycfv.cn

[Q53] 按条件删除
来源：http://cfk.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cka.fengsongda.top

[Q54] 清空表
来源：http://ufc.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://bdx.yj20258.top

[Q55] 排名（并列占位）
来源：http://yvm.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zvf.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://pvl.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kle.sysykeji.top

[Q57] 行号
来源：http://gpk.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rli.ydzc1.top

[Q58] 累计求和
来源：http://asd.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xwm.guowangkeji.top

[Q59] 分组内累计
来源：http://ixa.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ltg.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://tol.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pnn.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://enl.xuetiantiany.cn

[Q61] 移动平均
来源：http://azh.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://frz.hnqzz.top

[Q62] 分组占比
来源：http://lir.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zxt.zhiwuduotai.top

[Q63] 开启事务
来源：http://kbq.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lss.hongshengwenyu.top

[Q64] 提交事务
来源：http://czm.tianlin.xyz

COMMIT;
来源：http://qdk.nanxinkj.top

[Q65] 回滚事务
来源：http://fqq.xziqi.cn

ROLLBACK;
来源：http://hmf.smart0.xyz

[Q66] 行锁查询
来源：http://wwo.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tad.redwolf501.top

[Q67] 设置隔离级别
来源：http://anv.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://phh.hammf.cn

[Q68] 保存点
来源：http://tbx.kuanghao11.cn

SAVEPOINT sp1;
来源：http://frt.gzhubu.top

ROLLBACK TO sp1;
来源：http://kba.yvedp.cn

[Q69] 查看执行计划
来源：http://pwj.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qsm.yuxming.cn

[Q70] 更新统计信息
来源：http://pbx.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://ett.daxiang520.top

[Q71] 查看建表语句
来源：http://vss.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jui.pycfn.com

[Q72] 查看索引
来源：http://baq.jinqigufen.top

SHOW INDEX FROM users;
来源：http://pyq.shangyingyoupin.top

[Q73] 查看表状态
来源：http://bbb.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://iqm.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://cba.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nlh.zdqjudy.top

[Q75] 日期格式化
来源：http://ctm.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sbz.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fwt.dashuyun.cn

[Q76] 按天统计
来源：http://eqo.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hyh.gotoacloud.top

[Q77] 时间加减
来源：http://zks.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rci.shangyingyoupin.top

[Q78] 当前时间
来源：http://kpq.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wbz.zdqjudy.top

[Q79] 字符串拼接
来源：http://szf.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vqb.aizwys.cn

[Q80] 字符串截取
来源：http://pfo.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kci.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://bkm.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://neg.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://tfu.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zgb.smart0.xyz

[Q83] 大小写转换
来源：http://cmb.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eyi.yfazqb.com

[Q84] 去除首尾空格
来源：http://esf.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://lqu.vqdsnc.cn

[Q85] 数值取整
来源：http://uhh.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vcv.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://kta.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hiu.yonumen.top

[Q87] JSON 字段做条件
来源：http://lrv.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://umw.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://ekw.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qyu.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dez.gotoacloud.top

[Q89] 判断表是否存在
来源：http://bie.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wll.redwolf501.top

[Q90] 生成序号列
来源：http://wtx.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wvo.hywenlv.cn

================================================================================
来源：http://qzq.xingfuxueyuan.xyz

R. Bash 专题
来源：http://ywz.sxryk.cn

================================================================================
来源：http://fdt.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://lvw.mhx1999.top

#!/usr/bin/env bash
来源：http://ktw.uphjek.com

set -euo pipefail
来源：http://qfw.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://iyu.hcnkem.com

name="Tom"; echo "$name"
来源：http://onu.mhx1999.top

[R03] 只读变量
来源：http://fzr.jlsjyb.cn

readonly PI=3.14
来源：http://adz.iojbl.cn

[R04] 位置参数
来源：http://aii.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oly.zhiwuduotai.top

[R05] 参数默认值
来源：http://ccp.snrcjt.cn

name="${1:-default}"
来源：http://qij.jyoumei.cn

[R06] 判断命令是否存在
来源：http://zqn.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://umj.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://wda.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://atq.tanke756.top

[R08] 数值比较
来源：http://yag.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jxs.cqqwz.cn

[R09] 字符串比较
来源：http://fov.daxiang520.top


<!-- 参考信息 -->