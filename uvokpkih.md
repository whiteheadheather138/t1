代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vih.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oyy.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fvd.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bam.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fnm.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sjl.hfpthk.cn

[P03] 生成短随机字符串
来源：http://xut.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wvr.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oxd.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xwe.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mst.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vlg.gaohongyu789.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xhm.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jjy.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xuh.yuanzhike.top

[P04] 求长度
来源：http://vqc.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://grf.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hpi.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://htb.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ddz.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://hdu.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://imu.meibo888.top

Ruby: x.length;  x.size
来源：http://tkj.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kqe.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://jro.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://suk.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tyx.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zbz.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xhm.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ibh.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mfq.wangdashe.top

Ruby: a == b
来源：http://leu.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sft.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mnn.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wvb.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://ceb.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qgw.yj20258.top

TS:   if (x == null) {}
来源：http://wma.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ibb.jyoumei.cn

Go:   if x == nil {}
来源：http://wqt.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rth.tian-w.cn

C#:   if (x is null) {}
来源：http://rqe.ydzc1.top

[P07] 防抖与节流
来源：http://dli.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fxt.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://qly.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbf.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vcy.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bxh.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ylq.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vxz.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mfj.tanke756.top

[P08] 处理浮点精度问题
来源：http://vtq.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vqf.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rfg.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pmz.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uvn.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://igr.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbv.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kxl.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xwu.xuetiantiany.cn

================================================================================
来源：http://rip.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ezm.gogol.net.cn

================================================================================
来源：http://mdq.yj202588.top

[Q01] 创建表
来源：http://cwm.quarkkingdee.top

CREATE TABLE users (
来源：http://gla.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dyb.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://vcx.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://txg.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://niz.daxiang520.top

);
来源：http://ciu.zycfv.cn

[Q02] 创建带外键的表
来源：http://ybv.kuanghao11.cn

CREATE TABLE orders (
来源：http://enk.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qdy.havefunace.top

user_id INT NOT NULL,
来源：http://oym.smart0.xyz

amount DECIMAL(10, 2),
来源：http://scy.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wlj.cucudq.cn

);
来源：http://hah.yanxiufei.cn

[Q03] 增加列
来源：http://opg.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rsr.hysaishi.cn

[Q04] 修改列类型
来源：http://eoc.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tjr.ydjk.org.cn

[Q05] 重命名列
来源：http://irs.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hhw.zycfv.cn

[Q06] 删除列
来源：http://dxb.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://ign.yuanzhike.top

[Q07] 删除表
来源：http://njd.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://xud.zdqjudy.top

[Q08] 创建普通索引
来源：http://fad.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rmr.0kj1m.cn

[Q09] 创建唯一索引
来源：http://sca.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://imx.cqqwz.cn

[Q10] 插入单行
来源：http://kqv.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hqf.pycfn.com

[Q11] 一次插入多行
来源：http://zrb.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hkw.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://nti.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://new.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rjg.52xcode.cn

[Q13] 忽略重复插入
来源：http://isr.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ymg.daxiang520.top

[Q14] 存在则更新（upsert）
来源：http://wrg.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vct.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://psa.hongshengwenyu.top

[Q15] 查询全部
来源：http://hzm.bjfxy.top

SELECT * FROM users;
来源：http://fco.chenlongwang.top

[Q16] 查询指定列
来源：http://jce.nwbrower.top

SELECT id, name FROM users;
来源：http://jbw.yongpay.top

[Q17] 条件查询
来源：http://kke.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ljk.yfazqb.com

[Q18] 模糊匹配
来源：http://ylk.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vxm.fengsongda.top

[Q19] 范围查询
来源：http://wal.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uzz.dashuyun.cn

[Q20] IN 列表
来源：http://fiy.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://poi.fzhhl.top

[Q21] 空值判断
来源：http://dtq.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gdb.zdbjq.cn

[Q22] 排序
来源：http://whf.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bhz.jinyuanbaomall.cn

[Q23] 分页
来源：http://ttf.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pns.shuidangran.top

[Q24] 去重
来源：http://keq.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://ppf.gogol.net.cn

[Q25] 只取前 N 条
来源：http://vmk.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yai.birdmap.top

[Q26] 计数
来源：http://nmi.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://vrn.jinqigufen.top

[Q27] 条件计数
来源：http://pfb.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aoi.zhixingplan.top

[Q28] 求和与平均
来源：http://hta.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nof.ydzc1.top

[Q29] 最大最小值
来源：http://hgf.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhv.ehwqpu.com

[Q30] 分组统计
来源：http://jbc.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fpi.yj202588.top

[Q31] 分组后过滤
来源：http://ept.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tfb.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://qdb.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ifp.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nvu.havefunace.top

[Q33] 多列分组
来源：http://wbp.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vbv.smart0.xyz

[Q34] 每组取第一条
来源：http://hja.cucudq.cn

SELECT * FROM (
来源：http://fhu.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cii.havefunace.top

) t WHERE rn = 1;
来源：http://rpg.wangshuangyany.cn

[Q35] 内连接
来源：http://vji.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ikn.redwolf501.top

[Q36] 左连接
来源：http://ogl.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://axp.c1oappe.top

[Q37] 右连接
来源：http://ppw.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hvj.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lhv.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kaa.pycfn.com

[Q39] 自连接（查上下级）
来源：http://ogr.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wob.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://quf.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xqm.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ufh.smart0.xyz

[Q41] 多表连接
来源：http://ztv.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wcz.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://tjn.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://gjw.yj20258.top

[Q42] 连接条件附加过滤
来源：http://aiv.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://hdi.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://urg.jinqigfzy.top

[Q43] 标量子查询
来源：http://dou.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://szf.hongshengwenyu.top

[Q44] IN 子查询
来源：http://yrm.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yfz.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://pcb.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://llb.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tkm.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oop.9152youxi.cn

[Q47] 与平均值比较
来源：http://gam.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tvg.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://oue.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lsb.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://ydn.c1oappe.top

[Q49] 更新单行
来源：http://hjt.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rar.hammf.cn

[Q50] 批量更新
来源：http://lzw.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kie.zdqjudy.top

[Q51] 用子查询更新
来源：http://ssf.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xbl.wangshuangyany.cn

[Q52] 删除指定行
来源：http://qrp.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://mfj.pengpengdd.cyou

[Q53] 按条件删除
来源：http://agq.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xtk.meibo888.top

[Q54] 清空表
来源：http://wjm.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://ril.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://pua.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qsf.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://swd.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vfl.316326.xyz

[Q57] 行号
来源：http://kcw.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qqb.epnwcf.com

[Q58] 累计求和
来源：http://knj.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bkc.yj20258.top

[Q59] 分组内累计
来源：http://ddk.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qxn.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://cim.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lyx.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://skl.guowangkeji.top

[Q61] 移动平均
来源：http://zgi.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://njn.sufxvd.cn

[Q62] 分组占比
来源：http://lur.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ntt.jinqigufen.top

[Q63] 开启事务
来源：http://xmi.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://pmr.hnqzz.top

[Q64] 提交事务
来源：http://kvy.zycfv.cn

COMMIT;
来源：http://vbg.yj20258.top

[Q65] 回滚事务
来源：http://tnk.fanxiaobao.xyz

ROLLBACK;
来源：http://ssm.gotoacloud.top

[Q66] 行锁查询
来源：http://msl.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fyp.gogol.net.cn

[Q67] 设置隔离级别
来源：http://vpg.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mkt.hcnkem.com

[Q68] 保存点
来源：http://yzg.redwolf501.top

SAVEPOINT sp1;
来源：http://mxy.hcnkem.com

ROLLBACK TO sp1;
来源：http://env.hnxiangtu.top

[Q69] 查看执行计划
来源：http://csr.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://klf.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://ywz.jianghu66.top

ANALYZE TABLE users;
来源：http://gqb.svipenyu.cn

[Q71] 查看建表语句
来源：http://jbn.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ied.xylfe.cn

[Q72] 查看索引
来源：http://vwg.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://eev.yanxiufei.cn

[Q73] 查看表状态
来源：http://yxb.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://asp.hfpthk.cn

[Q74] 强制使用索引
来源：http://qmi.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://koa.zhijiandao.cn

[Q75] 日期格式化
来源：http://sgs.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://haf.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sfv.chenzaomai.com

[Q76] 按天统计
来源：http://dnw.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sqh.quarkkingdee.top

[Q77] 时间加减
来源：http://vqn.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mje.dianchejie.cn

[Q78] 当前时间
来源：http://esk.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bip.yuanzhike.top

[Q79] 字符串拼接
来源：http://rlz.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://axk.yj20258888.top

[Q80] 字符串截取
来源：http://jjq.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rrj.daria6918.cn

[Q81] 字符串替换
来源：http://yvi.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yae.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://zis.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xdk.sjlbkw.cn

[Q83] 大小写转换
来源：http://wpo.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hda.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://yem.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://dvu.52xcode.cn

[Q85] 数值取整
来源：http://pux.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nfo.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://kln.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bxe.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://gyd.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gfr.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://tja.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lud.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wrt.cdnleiting.top

[Q89] 判断表是否存在
来源：http://gnu.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qwc.yuxming.cn

[Q90] 生成序号列
来源：http://bcj.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fxb.hesvh.cn

================================================================================
来源：http://scn.tianlin.xyz

R. Bash 专题
来源：http://ezb.xuanzx.com

================================================================================
来源：http://ayz.cqqwz.cn

[R01] shebang 与严格模式
来源：http://tsd.sjlbkw.cn

#!/usr/bin/env bash
来源：http://cvj.xuetiantiany.cn

set -euo pipefail
来源：http://ozi.sysykeji.top

[R02] 变量赋值与使用
来源：http://vvf.tanke756.top

name="Tom"; echo "$name"
来源：http://pcs.vqdsnc.cn

[R03] 只读变量
来源：http://bmm.0kj1m.cn

readonly PI=3.14
来源：http://fkj.ctjpmb.com

[R04] 位置参数
来源：http://lrg.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://axm.fktsv.cn

[R05] 参数默认值
来源：http://bsw.hongshengwenyu.top

name="${1:-default}"
来源：http://zop.bbcook.cn

[R06] 判断命令是否存在
来源：http://prl.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qff.jiagoushi.top

[R07] if 判断文件
来源：http://kas.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cmg.jinqigfzy.top

[R08] 数值比较
来源：http://ghk.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mkq.haohaochexian.top

[R09] 字符串比较
来源：http://eir.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sef.quarkkingdee.top

[R10] 正则匹配
来源：http://mfb.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://khb.andypj.xyz

[R11] case 多分支
来源：http://cit.redwolf501.top

case "$1" in
来源：http://jab.c1oappe.top

start) echo "启动" ;;
来源：http://bua.snrcjt.cn

stop)  echo "停止" ;;
来源：http://bwb.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://hkc.hysaishi.cn

esac
来源：http://kwb.svipenyu.cn

[R12] for 遍历文件
来源：http://pxi.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://mqn.smart0.xyz

[R13] for 计数循环
来源：http://ipf.shzxlz.cn


<!-- 参考信息 -->