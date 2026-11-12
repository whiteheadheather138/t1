代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://yrm.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://nte.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ase.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://net.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uid.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cso.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aqh.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://olf.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hxc.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://heb.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://eop.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iyq.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gnv.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://noj.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grl.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nqu.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tgu.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iga.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hiv.316326.xyz

[P04] 求长度
来源：http://xmg.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gjo.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fas.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cvf.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zsu.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://vtn.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://etc.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://ulz.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zak.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://emo.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pct.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://alp.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ttu.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rws.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ijd.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://jjy.zdbjq.cn

Ruby: a == b
来源：http://ohy.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://avt.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fyp.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dxs.cheryme.top

PHP:  if (empty($x)) {}
来源：http://wnl.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nux.quarkkingdee.top

TS:   if (x == null) {}
来源：http://ssx.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kpl.vehdjk.com

Go:   if x == nil {}
来源：http://ayy.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zwi.tarul.cn

C#:   if (x is null) {}
来源：http://olh.gotoacloud.top

[P07] 防抖与节流
来源：http://itk.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pxo.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://ggg.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofz.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vql.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ckl.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zsn.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://wze.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bky.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://lwv.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://imh.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mye.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://der.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xjb.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dmb.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iyz.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://piu.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://inv.daria6918.cn

================================================================================
来源：http://xuf.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tah.pycfn.com

================================================================================
来源：http://qyh.zhijiandao.cn

[Q01] 创建表
来源：http://etz.c1oappe.top

CREATE TABLE users (
来源：http://jlo.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dnu.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://hwt.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://ozn.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aej.havefunace.top

);
来源：http://qai.xinyue.icu

[Q02] 创建带外键的表
来源：http://bcm.jlsjyb.cn

CREATE TABLE orders (
来源：http://rui.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bju.sysykeji.top

user_id INT NOT NULL,
来源：http://rdd.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://xrw.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ssf.yuanzhike.top

);
来源：http://bsq.daxiang520.top

[Q03] 增加列
来源：http://xfo.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fpe.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://gpz.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kqm.ppjwa.cn

[Q05] 重命名列
来源：http://krz.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qak.shanyushiyangtech.top

[Q06] 删除列
来源：http://lsq.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fla.zhoulong.xyz

[Q07] 删除表
来源：http://icm.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://pce.yvedp.cn

[Q08] 创建普通索引
来源：http://coe.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://iep.yueranfly.top

[Q09] 创建唯一索引
来源：http://hnb.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yrt.ppjwa.cn

[Q10] 插入单行
来源：http://xmn.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ram.bjfxy.top

[Q11] 一次插入多行
来源：http://uqc.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xox.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://lmh.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://jqe.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yez.zdqjudy.top

[Q13] 忽略重复插入
来源：http://ryf.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kij.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://bap.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dor.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gjo.andypj.xyz

[Q15] 查询全部
来源：http://oju.zdbjq.cn

SELECT * FROM users;
来源：http://oyh.sufxvd.cn

[Q16] 查询指定列
来源：http://dia.bbcook.cn

SELECT id, name FROM users;
来源：http://phr.fktsv.cn

[Q17] 条件查询
来源：http://dap.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sma.nanxinkj.top

[Q18] 模糊匹配
来源：http://lsx.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ijm.jianghu66.top

[Q19] 范围查询
来源：http://gsj.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eqh.gaohongyu789.top

[Q20] IN 列表
来源：http://hvp.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cwz.pengpengdd.cyou

[Q21] 空值判断
来源：http://bkw.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wqq.zhengqikj.top

[Q22] 排序
来源：http://xiw.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://deq.shzxlz.cn

[Q23] 分页
来源：http://nfm.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zfe.gzhubu.top

[Q24] 去重
来源：http://psd.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://dfj.316326.xyz

[Q25] 只取前 N 条
来源：http://iky.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ngn.jiagoushi.top

[Q26] 计数
来源：http://qjv.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://zvf.yonumen.top

[Q27] 条件计数
来源：http://twf.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mrf.yj202588.top

[Q28] 求和与平均
来源：http://eiq.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sxg.guannengcc.top

[Q29] 最大最小值
来源：http://psn.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xpg.zhixingplan.top

[Q30] 分组统计
来源：http://kdi.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xsb.chenlongwang.top

[Q31] 分组后过滤
来源：http://lhe.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://miy.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://gdp.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hpp.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fec.kuanghao11.cn

[Q33] 多列分组
来源：http://pmh.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uut.birdmap.top

[Q34] 每组取第一条
来源：http://lyl.sysykeji.top

SELECT * FROM (
来源：http://rhq.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ymr.tianlin.xyz

) t WHERE rn = 1;
来源：http://syn.nanxinkj.top

[Q35] 内连接
来源：http://khl.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dam.yongpay.top

[Q36] 左连接
来源：http://mbu.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pqm.cashguo.top

[Q37] 右连接
来源：http://sht.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lmu.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://tye.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rri.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://ila.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rdc.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://otg.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rfk.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hms.yanxiufei.cn

[Q41] 多表连接
来源：http://uze.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://pcu.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://pmx.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://oya.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://ebt.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://igu.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xep.ydzc1.top

[Q43] 标量子查询
来源：http://yyr.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bpi.cdnleiting.top

[Q44] IN 子查询
来源：http://uwp.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://poi.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://jmv.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ena.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://vag.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://efz.zhongyouzk.top

[Q47] 与平均值比较
来源：http://ojr.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://alt.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://ugx.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vvp.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://jfh.cheryme.top

[Q49] 更新单行
来源：http://dkj.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bqc.gogol.net.cn

[Q50] 批量更新
来源：http://twd.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xtn.dashuyun.cn

[Q51] 用子查询更新
来源：http://ggb.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iqm.hfpthk.cn

[Q52] 删除指定行
来源：http://urr.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://gnr.zycfv.cn

[Q53] 按条件删除
来源：http://rnd.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qxw.hnxiangtu.top

[Q54] 清空表
来源：http://oba.yfazqb.com

TRUNCATE TABLE logs;
来源：http://jbw.gzhubu.top

[Q55] 排名（并列占位）
来源：http://drt.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://axo.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://jcs.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nge.cqqwz.cn

[Q57] 行号
来源：http://yjx.jlsjyb.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jgh.xuetiantiany.cn

[Q58] 累计求和
来源：http://gnx.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zsp.hysaishi.cn

[Q59] 分组内累计
来源：http://uae.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xtd.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://snp.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qhd.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fcx.gogol.net.cn

[Q61] 移动平均
来源：http://izb.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ttq.zhengqikj.top

[Q62] 分组占比
来源：http://zpt.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://osv.zhengqikj.top

[Q63] 开启事务
来源：http://myk.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uda.dashuyun.cn

[Q64] 提交事务
来源：http://usd.hcnkem.com

COMMIT;
来源：http://cqu.jianghu66.top

[Q65] 回滚事务
来源：http://msz.zhiwuduotai.top

ROLLBACK;
来源：http://qwq.zycfv.cn

[Q66] 行锁查询
来源：http://ggb.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jah.cashguo.top

[Q67] 设置隔离级别
来源：http://qjk.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kvs.hammf.cn

[Q68] 保存点
来源：http://bpe.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://jcf.hcnkem.com

ROLLBACK TO sp1;
来源：http://usz.uphjek.com

[Q69] 查看执行计划
来源：http://kko.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bdr.jyoumei.cn

[Q70] 更新统计信息
来源：http://hvj.guowangkeji.top

ANALYZE TABLE users;
来源：http://efq.xziqi.cn

[Q71] 查看建表语句
来源：http://ksx.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nrt.sysykeji.top

[Q72] 查看索引
来源：http://qiv.iojbl.cn

SHOW INDEX FROM users;
来源：http://wbj.aibaodan.cn

[Q73] 查看表状态
来源：http://unw.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wrs.jinqigfzy.top

[Q74] 强制使用索引
来源：http://ifl.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gdq.0kj1m.cn

[Q75] 日期格式化
来源：http://dtl.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ksh.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jfn.shanyushiyangtech.top

[Q76] 按天统计
来源：http://soz.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upm.fanxiaobao.xyz

[Q77] 时间加减
来源：http://fsa.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://til.quarkkingdee.top

[Q78] 当前时间
来源：http://lzy.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lkl.jiagoushi.top

[Q79] 字符串拼接
来源：http://nic.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xxv.uphjek.com

[Q80] 字符串截取
来源：http://oms.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xaf.guowangkeji.top

[Q81] 字符串替换
来源：http://pog.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ugf.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://gam.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gxh.ybcxt.top

[Q83] 大小写转换
来源：http://lfw.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wgh.bjfxy.top

[Q84] 去除首尾空格
来源：http://brd.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://lpv.yanxiufei.cn

[Q85] 数值取整
来源：http://zmx.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://skt.sweek.top

[Q86] 读取 JSON 字段
来源：http://sex.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kib.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://qyb.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vmr.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://gpc.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iyz.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://njd.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://smp.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hmv.snrcjt.cn

[Q90] 生成序号列
来源：http://nty.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uwu.hywenlv.cn

================================================================================
来源：http://ucl.gotoacloud.top

R. Bash 专题
来源：http://nyj.yuanzhike.top

================================================================================
来源：http://eeq.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://vob.yueranfly.top

#!/usr/bin/env bash
来源：http://nsf.bjfxy.top

set -euo pipefail
来源：http://hhn.ehwqpu.com

[R02] 变量赋值与使用
来源：http://kev.uphjek.com

name="Tom"; echo "$name"
来源：http://yit.yuanzhike.top

[R03] 只读变量
来源：http://rnu.zhijiandao.cn

readonly PI=3.14
来源：http://ltp.yvedp.cn

[R04] 位置参数
来源：http://lzs.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ogh.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://hde.vehdjk.com

name="${1:-default}"
来源：http://sxg.fktsv.cn

[R06] 判断命令是否存在
来源：http://twq.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xvp.zdqjudy.top

[R07] if 判断文件
来源：http://osl.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xmo.epnwcf.com

[R08] 数值比较
来源：http://xcm.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xsf.sjlbkw.cn

[R09] 字符串比较
来源：http://sel.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jfh.chenjidiqi.icu

[R10] 正则匹配
来源：http://huv.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://htd.svipenyu.cn

[R11] case 多分支
来源：http://ase.daria6918.cn

case "$1" in
来源：http://jca.xinyue.icu

start) echo "启动" ;;
来源：http://tin.xuanzx.com

stop)  echo "停止" ;;
来源：http://ccl.tanke756.top

*)     echo "未知命令" ;;
来源：http://psj.316326.xyz


<!-- 参考信息 -->