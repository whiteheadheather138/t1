代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ngc.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dhr.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kdj.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yuh.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dkt.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zuw.chenlongwang.top

[P03] 生成短随机字符串
来源：http://zqw.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hrp.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bwd.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtx.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bkl.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://par.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ecs.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hpa.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ntm.gotoacloud.top

[P04] 求长度
来源：http://spv.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uvs.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mai.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smn.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bhz.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://maj.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://uxn.bjfxy.top

Ruby: x.length;  x.size
来源：http://ery.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dpm.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://bcp.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ijm.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dqu.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ehw.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zle.hfpthk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wcz.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://qfc.sysykeji.top

Ruby: a == b
来源：http://ohh.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zdi.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fdu.guowangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://plt.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://qiv.gogol.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oct.yj20258888.top

TS:   if (x == null) {}
来源：http://jjh.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://vpf.quarkkingdee.top

Go:   if x == nil {}
来源：http://nkd.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vzl.yuanzhike.top

C#:   if (x is null) {}
来源：http://ocy.tarul.cn

[P07] 防抖与节流
来源：http://oua.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dha.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://ugl.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qpu.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldh.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vib.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bti.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpq.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wkg.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://cob.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://enm.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hxs.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dzj.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bjl.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dag.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zuc.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ypg.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jza.dashuyun.cn

================================================================================
来源：http://qzu.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xok.yuanzhike.top

================================================================================
来源：http://gcp.kuanghao11.cn

[Q01] 创建表
来源：http://mut.9152youxi.cn

CREATE TABLE users (
来源：http://jic.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sty.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://jvi.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://czw.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sog.haohaochexian.top

);
来源：http://uua.316326.xyz

[Q02] 创建带外键的表
来源：http://mjr.snrcjt.cn

CREATE TABLE orders (
来源：http://eas.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hwm.andypj.xyz

user_id INT NOT NULL,
来源：http://awc.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://aic.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gnd.uphjek.com

);
来源：http://cin.fzhhl.top

[Q03] 增加列
来源：http://dug.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kti.fzhhl.top

[Q04] 修改列类型
来源：http://qph.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://coy.shzxlz.cn

[Q05] 重命名列
来源：http://oip.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vuk.fanxiaobao.xyz

[Q06] 删除列
来源：http://tii.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://lbj.wangshuangyany.cn

[Q07] 删除表
来源：http://sxl.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://vbi.ctjpmb.com

[Q08] 创建普通索引
来源：http://fcs.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ucw.fengsongda.top

[Q09] 创建唯一索引
来源：http://rmv.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ujv.ywan-chungtsiang.top

[Q10] 插入单行
来源：http://cjl.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aem.yongpay.top

[Q11] 一次插入多行
来源：http://pys.yuanzhike.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://epk.gotoacloud.top

[Q12] 插入后取自增 ID
来源：http://enl.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://bot.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hjk.zycfv.cn

[Q13] 忽略重复插入
来源：http://uco.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://duo.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://zmx.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://egp.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://asy.shangyingyoupin.top

[Q15] 查询全部
来源：http://lct.gzhubu.top

SELECT * FROM users;
来源：http://zcu.hesvh.cn

[Q16] 查询指定列
来源：http://kzu.cdnleiting.top

SELECT id, name FROM users;
来源：http://cti.nwbrower.top

[Q17] 条件查询
来源：http://nnh.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://asy.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://myj.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oee.havefunace.top

[Q19] 范围查询
来源：http://uuj.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iki.feifeiyinyue.top

[Q20] IN 列表
来源：http://haz.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://phj.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://nkp.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ljr.tianlin.xyz

[Q22] 排序
来源：http://ceu.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uwx.yangfankeji.com

[Q23] 分页
来源：http://dgd.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fzk.mhx1999.top

[Q24] 去重
来源：http://tad.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://jio.ppjwa.cn

[Q25] 只取前 N 条
来源：http://ckg.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://umm.hywenlv.cn

[Q26] 计数
来源：http://oqe.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://odz.haohaochexian.top

[Q27] 条件计数
来源：http://rvm.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wlt.chenlongwang.top

[Q28] 求和与平均
来源：http://vyb.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vwp.bbcook.cn

[Q29] 最大最小值
来源：http://nnb.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fwn.hysaishi.cn

[Q30] 分组统计
来源：http://rbv.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rnj.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://zic.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jij.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://ldr.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://net.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ozo.nanxinkj.top

[Q33] 多列分组
来源：http://ewl.xziqi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tsj.birdmap.top

[Q34] 每组取第一条
来源：http://stb.yongpay.top

SELECT * FROM (
来源：http://qxr.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mzs.tanke756.top

) t WHERE rn = 1;
来源：http://isf.zycfv.cn

[Q35] 内连接
来源：http://kim.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://byy.cqqwz.cn

[Q36] 左连接
来源：http://fnp.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://orv.zhoulong.xyz

[Q37] 右连接
来源：http://jre.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fyw.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://itk.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ssv.pycfn.com

[Q39] 自连接（查上下级）
来源：http://pgm.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yri.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eqt.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kvu.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tbq.52xcode.cn

[Q41] 多表连接
来源：http://fck.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ljq.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://dxi.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://ifs.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://oyl.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://rwo.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dnf.ehwqpu.com

[Q43] 标量子查询
来源：http://xtm.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cea.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://oxi.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://izi.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://tzg.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dbc.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://swf.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ijk.shuidangran.top

[Q47] 与平均值比较
来源：http://cpn.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yew.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://pof.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://whw.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://osf.jinqigfzy.top

[Q49] 更新单行
来源：http://nzn.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uvc.ydjk.org.cn

[Q50] 批量更新
来源：http://aos.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aab.bbcook.cn

[Q51] 用子查询更新
来源：http://ngb.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sko.zycfv.cn

[Q52] 删除指定行
来源：http://rgo.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://wss.sufxvd.cn

[Q53] 按条件删除
来源：http://ydt.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tou.zhongyouzk.top

[Q54] 清空表
来源：http://uma.yj202588.top

TRUNCATE TABLE logs;
来源：http://syj.uphjek.com

[Q55] 排名（并列占位）
来源：http://tii.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fgu.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://gef.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gzd.quarkkingdee.top

[Q57] 行号
来源：http://cpb.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqi.yanxiufei.cn

[Q58] 累计求和
来源：http://esg.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cjx.bjfxy.top

[Q59] 分组内累计
来源：http://taj.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kuu.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://etx.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kxq.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dhv.daria6918.cn

[Q61] 移动平均
来源：http://amp.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rac.sufxvd.cn

[Q62] 分组占比
来源：http://gro.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pfr.sxryk.cn

[Q63] 开启事务
来源：http://nxb.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hmd.zhijiandao.cn

[Q64] 提交事务
来源：http://dgz.zhengqikj.top

COMMIT;
来源：http://bku.ydzc1.top

[Q65] 回滚事务
来源：http://ecp.316326.xyz

ROLLBACK;
来源：http://unu.jinqigufen.top

[Q66] 行锁查询
来源：http://iap.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dla.zdqjudy.top

[Q67] 设置隔离级别
来源：http://ivo.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sqz.sjlbkw.cn

[Q68] 保存点
来源：http://ptt.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://xdv.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://adf.yongpay.top

[Q69] 查看执行计划
来源：http://htf.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hez.svipenyu.cn

[Q70] 更新统计信息
来源：http://nik.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://onm.cucudq.cn

[Q71] 查看建表语句
来源：http://qce.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vrt.yuanzhike.top

[Q72] 查看索引
来源：http://wjk.sxryk.cn

SHOW INDEX FROM users;
来源：http://exd.zhongyouzk.top

[Q73] 查看表状态
来源：http://gha.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://xlu.aibaodan.cn

[Q74] 强制使用索引
来源：http://rzj.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oms.zhongyouzk.top

[Q75] 日期格式化
来源：http://gxx.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xem.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://neo.pycfn.com

[Q76] 按天统计
来源：http://ehx.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fnw.jqgufenzy.top

[Q77] 时间加减
来源：http://smy.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zmu.yuxming.cn

[Q78] 当前时间
来源：http://zoy.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://shb.gotoacloud.top

[Q79] 字符串拼接
来源：http://bsy.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://chr.dianchejie.cn

[Q80] 字符串截取
来源：http://ugc.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gpk.xinyue.icu

[Q81] 字符串替换
来源：http://blx.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://anw.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://vbv.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://myh.hammf.cn

[Q83] 大小写转换
来源：http://wot.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ckc.dashuyun.cn

[Q84] 去除首尾空格
来源：http://dsd.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://dum.tanke756.top

[Q85] 数值取整
来源：http://vbj.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://odr.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://jer.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://skr.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://mdz.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hfv.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://ubc.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://brc.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rqf.chenlongwang.top

[Q89] 判断表是否存在
来源：http://wxx.pycfn.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dne.yanxiufei.cn

[Q90] 生成序号列
来源：http://aeb.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://igi.yfazqb.com

================================================================================
来源：http://lvc.nanxinkj.top

R. Bash 专题
来源：http://tpk.wangdashe.top

================================================================================
来源：http://stx.nwbrower.top

[R01] shebang 与严格模式
来源：http://jgb.52xcode.cn

#!/usr/bin/env bash
来源：http://sdn.shangyingyoupin.top

set -euo pipefail
来源：http://snm.vehdjk.com

[R02] 变量赋值与使用
来源：http://cwo.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://rut.zhengqikj.top

[R03] 只读变量
来源：http://ojh.0kj1m.cn

readonly PI=3.14
来源：http://krp.hnqzz.top

[R04] 位置参数
来源：http://zht.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rtj.52xcode.cn

[R05] 参数默认值
来源：http://hai.sjlbkw.cn

name="${1:-default}"
来源：http://hpd.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://yxy.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tgj.jlsjyb.cn

[R07] if 判断文件
来源：http://mdr.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ydm.shangyingyoupin.top

[R08] 数值比较
来源：http://feh.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://zxv.dianchejie.cn

[R09] 字符串比较
来源：http://wjw.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://khx.yangfankeji.com

[R10] 正则匹配
来源：http://yck.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yzj.zhijiandao.cn

[R11] case 多分支
来源：http://bbs.xuetiantiany.cn

case "$1" in
来源：http://qgw.zdqjudy.top

start) echo "启动" ;;
来源：http://xsz.chenlongwang.top

stop)  echo "停止" ;;
来源：http://hmn.yfazqb.com

*)     echo "未知命令" ;;
来源：http://kao.zdbjq.cn

esac
来源：http://hip.andypj.xyz

[R12] for 遍历文件
来源：http://yim.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://pku.yj202588.top

[R13] for 计数循环
来源：http://dww.fengsongda.top


<!-- 参考信息 -->