代发 wailian999

TS:   crypto.randomUUID()
来源：http://wzj.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://lxw.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://csj.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://msn.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://azx.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://yov.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qut.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvf.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rzf.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zqz.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pxc.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hio.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tdm.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gat.chenzaomai.com

[P03] 生成短随机字符串
来源：http://gny.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ips.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nru.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyl.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jnr.guowangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pey.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dan.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bnh.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ppw.vqdsnc.cn

[P04] 求长度
来源：http://qru.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zuw.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axe.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avd.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zeb.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://izk.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://gnm.dashuyun.cn

Ruby: x.length;  x.size
来源：http://kxn.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uic.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://eub.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://xrj.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rje.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gmh.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sbc.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qbv.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://bef.bbcook.cn

Ruby: a == b
来源：http://peo.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vbu.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ins.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mxh.yj20258.top

PHP:  if (empty($x)) {}
来源：http://afy.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cdy.jlsjyb.cn

TS:   if (x == null) {}
来源：http://inh.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://emd.yuxming.cn

Go:   if x == nil {}
来源：http://nfa.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pxw.cashguo.top

C#:   if (x is null) {}
来源：http://okn.hfpthk.cn

[P07] 防抖与节流
来源：http://kml.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vtg.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://lqc.shanyushiyangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzs.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxn.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qdr.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dkh.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fvw.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eko.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://htj.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tmy.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vnr.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nls.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wxm.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kzi.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sel.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xai.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tux.shuidangran.top

================================================================================
来源：http://ctj.zhengqikj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aug.snrcjt.cn

================================================================================
来源：http://igs.chenlongwang.top

[Q01] 创建表
来源：http://kos.jiagoushi.top

CREATE TABLE users (
来源：http://dqv.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iuq.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://mgx.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://bss.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mwg.gaohongyu789.top

);
来源：http://anc.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qzp.feifeiyinyue.top

CREATE TABLE orders (
来源：http://btu.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mhk.shzxlz.cn

user_id INT NOT NULL,
来源：http://dih.yueranfly.top

amount DECIMAL(10, 2),
来源：http://gth.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cok.hfpthk.cn

);
来源：http://irg.hfpthk.cn

[Q03] 增加列
来源：http://iaq.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ili.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://jpu.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xjf.sysykeji.top

[Q05] 重命名列
来源：http://oqy.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mol.kuanghao11.cn

[Q06] 删除列
来源：http://dak.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://cjw.kuanghao11.cn

[Q07] 删除表
来源：http://vzp.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://hkz.ybcxt.top

[Q08] 创建普通索引
来源：http://egt.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://xri.zhixingplan.top

[Q09] 创建唯一索引
来源：http://aia.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oqj.yvedp.cn

[Q10] 插入单行
来源：http://ldg.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nsv.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://pdf.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mee.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://xpq.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://xem.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oqc.mhx1999.top

[Q13] 忽略重复插入
来源：http://zqr.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qrk.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://jzx.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://enq.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nwp.xinyue.icu

[Q15] 查询全部
来源：http://peo.aibaodan.cn

SELECT * FROM users;
来源：http://giv.pycfn.com

[Q16] 查询指定列
来源：http://vhb.gotoacloud.top

SELECT id, name FROM users;
来源：http://blt.epnwcf.com

[Q17] 条件查询
来源：http://msh.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vfx.hnqzz.top

[Q18] 模糊匹配
来源：http://yaj.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cix.hnxiangtu.top

[Q19] 范围查询
来源：http://aio.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iwh.hnxiangtu.top

[Q20] IN 列表
来源：http://ndf.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ibw.xuetiantiany.cn

[Q21] 空值判断
来源：http://psc.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://hqt.pycfn.com

[Q22] 排序
来源：http://jne.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xti.vehdjk.com

[Q23] 分页
来源：http://rli.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fzz.hammf.cn

[Q24] 去重
来源：http://wae.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://lbq.yfazqb.com

[Q25] 只取前 N 条
来源：http://uxw.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qpm.fktsv.cn

[Q26] 计数
来源：http://yqf.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://pua.cdnleiting.top

[Q27] 条件计数
来源：http://vvy.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ins.jinqigfzy.top

[Q28] 求和与平均
来源：http://xhl.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cjh.andypj.xyz

[Q29] 最大最小值
来源：http://jyj.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://psu.hnqzz.top

[Q30] 分组统计
来源：http://vff.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zms.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://vdj.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lgm.andypj.xyz

[Q32] 分组拼接字符串
来源：http://gxp.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://znq.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://isb.ydjk.org.cn

[Q33] 多列分组
来源：http://ask.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ktg.hywenlv.cn

[Q34] 每组取第一条
来源：http://nsm.jqgfzy.top

SELECT * FROM (
来源：http://ezv.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://esf.yfazqb.com

) t WHERE rn = 1;
来源：http://wih.cqqwz.cn

[Q35] 内连接
来源：http://dce.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tav.zdqjudy.top

[Q36] 左连接
来源：http://jrv.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kuj.zhiwuduotai.top

[Q37] 右连接
来源：http://zsl.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wmc.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mma.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ukc.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://vav.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kuv.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bmp.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://geg.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kkx.hnqzz.top

[Q41] 多表连接
来源：http://rdt.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qcd.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://tbu.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://anz.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://mcw.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://dqy.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jdb.sysykeji.top

[Q43] 标量子查询
来源：http://myj.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wmn.xuetiantiany.cn

[Q44] IN 子查询
来源：http://uyp.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xok.tanke756.top

[Q45] EXISTS 判断存在
来源：http://fun.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wkz.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://agc.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://odo.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://jiu.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://erk.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://xem.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vjz.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://qek.bjfxy.top

[Q49] 更新单行
来源：http://xpn.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bla.jyoumei.cn

[Q50] 批量更新
来源：http://hkm.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://voy.snrcjt.cn

[Q51] 用子查询更新
来源：http://zgy.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nxg.jyoumei.cn

[Q52] 删除指定行
来源：http://lpe.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://xda.ydjk.org.cn

[Q53] 按条件删除
来源：http://mgd.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zbs.zhixingplan.top

[Q54] 清空表
来源：http://byh.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://ach.hesvh.cn

[Q55] 排名（并列占位）
来源：http://brg.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mrq.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://jcj.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fvp.vehdjk.com

[Q57] 行号
来源：http://ftv.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fws.chenlongwang.top

[Q58] 累计求和
来源：http://oun.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://znq.tarul.cn

[Q59] 分组内累计
来源：http://osb.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qya.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://bix.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qmc.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pwu.bjfxy.top

[Q61] 移动平均
来源：http://znb.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mvx.hongshengwenyu.top

[Q62] 分组占比
来源：http://gks.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://smd.0kj1m.cn

[Q63] 开启事务
来源：http://plr.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hax.pycfn.com

[Q64] 提交事务
来源：http://cqq.svipenyu.cn

COMMIT;
来源：http://kij.jiagoushi.top

[Q65] 回滚事务
来源：http://qss.dashuyun.cn

ROLLBACK;
来源：http://ejm.zhijiandao.cn

[Q66] 行锁查询
来源：http://zyl.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gkl.wangdashe.top

[Q67] 设置隔离级别
来源：http://xcl.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hek.xziqi.cn

[Q68] 保存点
来源：http://aaf.tarul.cn

SAVEPOINT sp1;
来源：http://tzv.epnwcf.com

ROLLBACK TO sp1;
来源：http://ole.guowangkeji.top

[Q69] 查看执行计划
来源：http://ojy.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dla.mhx1999.top

[Q70] 更新统计信息
来源：http://bwx.zdqjudy.top

ANALYZE TABLE users;
来源：http://rac.sweek.top

[Q71] 查看建表语句
来源：http://zut.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xhz.andypj.xyz

[Q72] 查看索引
来源：http://pab.jiagoushi.top

SHOW INDEX FROM users;
来源：http://pew.tarul.cn

[Q73] 查看表状态
来源：http://egp.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aum.hnqzz.top

[Q74] 强制使用索引
来源：http://yce.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cqq.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://xdo.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hrl.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jpn.cqqwz.cn

[Q76] 按天统计
来源：http://iqm.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ksx.yuxming.cn

[Q77] 时间加减
来源：http://qaf.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://amd.daria6918.cn

[Q78] 当前时间
来源：http://ghv.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wde.yanxiufei.cn

[Q79] 字符串拼接
来源：http://zyh.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pmt.vehdjk.com

[Q80] 字符串截取
来源：http://owg.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tsl.ydjk.org.cn

[Q81] 字符串替换
来源：http://eas.jqgufenzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://omu.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://dpp.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dxu.cdnleiting.top

[Q83] 大小写转换
来源：http://vsu.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zvb.hnqzz.top

[Q84] 去除首尾空格
来源：http://xmz.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://nmo.316326.xyz

[Q85] 数值取整
来源：http://ayg.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vqp.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://rwx.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uvm.tarul.cn

[Q87] JSON 字段做条件
来源：http://vuo.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wnc.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://xii.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://abs.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://one.hesvh.cn

[Q89] 判断表是否存在
来源：http://uhm.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ggs.ydjk.org.cn

[Q90] 生成序号列
来源：http://vbb.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uee.zdqjudy.top

================================================================================
来源：http://ntq.guannengcc.top

R. Bash 专题
来源：http://xvy.haohaochexian.top

================================================================================
来源：http://yxt.316326.xyz

[R01] shebang 与严格模式
来源：http://yzl.c1oappe.top

#!/usr/bin/env bash
来源：http://crq.0kj1m.cn

set -euo pipefail
来源：http://piz.zycfv.cn

[R02] 变量赋值与使用
来源：http://xvd.tanke756.top

name="Tom"; echo "$name"
来源：http://mnh.guannengcc.top

[R03] 只读变量
来源：http://ggp.jinqigufen.top

readonly PI=3.14
来源：http://udv.daxiang520.top

[R04] 位置参数
来源：http://wjg.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qbc.zhijiandao.cn

[R05] 参数默认值
来源：http://bum.zhixingplan.top

name="${1:-default}"
来源：http://mjg.cdnleiting.top

[R06] 判断命令是否存在
来源：http://lne.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lwd.hcnkem.com

[R07] if 判断文件
来源：http://cgr.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://suu.gogol.net.cn

[R08] 数值比较
来源：http://kzj.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dvl.yuanzhike.top

[R09] 字符串比较
来源：http://duh.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aap.9152youxi.cn

[R10] 正则匹配
来源：http://obv.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kea.jinyuanbaomall.cn

[R11] case 多分支
来源：http://qom.pengpengdd.cyou


<!-- 参考信息 -->