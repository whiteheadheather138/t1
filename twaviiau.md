代发 wailian999

TS:   crypto.randomUUID()
来源：http://yrd.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://bvd.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://yxa.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://sxf.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://bht.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://joe.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jix.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uuy.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gdm.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qbs.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mgi.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nqu.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dli.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fbu.yvedp.cn

[P03] 生成短随机字符串
来源：http://hhl.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wqg.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ymi.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://idq.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://omm.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rfg.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cgi.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://cbq.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eqz.yfazqb.com

[P04] 求长度
来源：http://wlg.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fex.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wyn.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tob.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://slb.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://bfq.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://qty.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://eqd.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bkr.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://jat.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://orp.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://liy.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pmi.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xaf.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uio.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://cal.hysaishi.cn

Ruby: a == b
来源：http://rqi.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cza.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zge.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dhn.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://soy.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vyl.9152youxi.cn

TS:   if (x == null) {}
来源：http://kxn.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://mne.shzxlz.cn

Go:   if x == nil {}
来源：http://obw.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jcq.havefunace.top

C#:   if (x is null) {}
来源：http://tvm.tanke756.top

[P07] 防抖与节流
来源：http://smj.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://thh.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://gkw.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ocs.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etd.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ccm.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kzq.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqt.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xnn.guannengcc.top

[P08] 处理浮点精度问题
来源：http://zks.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fcb.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ion.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bqg.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yns.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qww.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://npb.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vdx.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wdf.sxryk.cn

================================================================================
来源：http://khz.shanyushiyangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xmk.bjfxy.top

================================================================================
来源：http://ccn.nwbrower.top

[Q01] 创建表
来源：http://kra.jqgfzy.top

CREATE TABLE users (
来源：http://bbo.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yxl.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://wyv.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://gjv.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pna.sxryk.cn

);
来源：http://bqp.gogol.net.cn

[Q02] 创建带外键的表
来源：http://qbc.xuetiantiany.cn

CREATE TABLE orders (
来源：http://fzf.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qhb.daria6918.cn

user_id INT NOT NULL,
来源：http://usy.xuanzx.com

amount DECIMAL(10, 2),
来源：http://gvi.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mtk.mhx1999.top

);
来源：http://kcu.hongshengwenyu.top

[Q03] 增加列
来源：http://ykj.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sym.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://pza.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rwe.svipenyu.cn

[Q05] 重命名列
来源：http://zuv.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lwd.yvedp.cn

[Q06] 删除列
来源：http://dpk.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://gno.ydzc1.top

[Q07] 删除表
来源：http://tif.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://mpc.fengsongda.top

[Q08] 创建普通索引
来源：http://guk.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wsr.epnwcf.com

[Q09] 创建唯一索引
来源：http://dqn.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wvk.ybcxt.top

[Q10] 插入单行
来源：http://qfk.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wyq.fzhhl.top

[Q11] 一次插入多行
来源：http://emf.yuanzhike.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nwz.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://cxs.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://gfj.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wkf.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://dyu.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jcy.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://znq.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ggx.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zhx.gogol.net.cn

[Q15] 查询全部
来源：http://esp.bjfxy.top

SELECT * FROM users;
来源：http://kua.sweek.top

[Q16] 查询指定列
来源：http://xeo.hammf.cn

SELECT id, name FROM users;
来源：http://zhc.zhengqikj.top

[Q17] 条件查询
来源：http://rgt.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lom.ybcxt.top

[Q18] 模糊匹配
来源：http://qre.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hmt.tarul.cn

[Q19] 范围查询
来源：http://ffy.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wpq.xylfe.cn

[Q20] IN 列表
来源：http://ilg.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://csr.hongshengwenyu.top

[Q21] 空值判断
来源：http://mtd.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xcq.jyoumei.cn

[Q22] 排序
来源：http://cwx.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rou.ywan-chungtsiang.top

[Q23] 分页
来源：http://xoh.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://clh.fengsongda.top

[Q24] 去重
来源：http://aoo.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://ziu.9152youxi.cn

[Q25] 只取前 N 条
来源：http://wpz.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gef.shuidangran.top

[Q26] 计数
来源：http://uyg.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://ctp.aizwys.cn

[Q27] 条件计数
来源：http://qiu.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zke.jinqigfzy.top

[Q28] 求和与平均
来源：http://sqi.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yeb.gogol.net.cn

[Q29] 最大最小值
来源：http://xaz.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nng.bjfxy.top

[Q30] 分组统计
来源：http://ffs.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qdn.pycfn.com

[Q31] 分组后过滤
来源：http://kwa.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pcc.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://rss.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iec.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hbj.zhengqikj.top

[Q33] 多列分组
来源：http://ail.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://itm.yj202588.top

[Q34] 每组取第一条
来源：http://oxg.hywenlv.cn

SELECT * FROM (
来源：http://aoo.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pvs.haohaochexian.top

) t WHERE rn = 1;
来源：http://bja.guowangkeji.top

[Q35] 内连接
来源：http://dir.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://goh.yj20258888.top

[Q36] 左连接
来源：http://zsk.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jfo.nwbrower.top

[Q37] 右连接
来源：http://ipa.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kao.xziqi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://flg.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sav.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://dyl.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://rux.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fcp.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yac.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://syo.iojbl.cn

[Q41] 多表连接
来源：http://zid.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bez.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://mxl.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://eby.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://vcn.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://gwo.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tzu.guannengcc.top

[Q43] 标量子查询
来源：http://gdy.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hne.andypj.xyz

[Q44] IN 子查询
来源：http://wxc.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yyn.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://nzl.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://klz.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://drl.nanxinkj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qlp.fehbvm.com

[Q47] 与平均值比较
来源：http://dji.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://naa.ivvv.top

[Q48] CTE 公用表表达式
来源：http://mta.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://njr.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://pzt.shuidangran.top

[Q49] 更新单行
来源：http://kus.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jwr.snrcjt.cn

[Q50] 批量更新
来源：http://upm.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://urv.zycfv.cn

[Q51] 用子查询更新
来源：http://ein.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sxu.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://vvy.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://snu.uphjek.com

[Q53] 按条件删除
来源：http://zwp.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uox.yuxming.cn

[Q54] 清空表
来源：http://vjs.xylfe.cn

TRUNCATE TABLE logs;
来源：http://ndh.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://jbq.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wbb.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://hxi.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xkt.sjlbkw.cn

[Q57] 行号
来源：http://zbx.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avz.jiagoushi.top

[Q58] 累计求和
来源：http://qwm.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://los.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://rmz.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xtg.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://vsp.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ayn.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rar.aibaodan.cn

[Q61] 移动平均
来源：http://dkb.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nqm.cqqwz.cn

[Q62] 分组占比
来源：http://grh.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rib.cucudq.cn

[Q63] 开启事务
来源：http://qob.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://hcq.cheryme.top

[Q64] 提交事务
来源：http://sva.ywan-chungtsiang.top

COMMIT;
来源：http://jbh.yvedp.cn

[Q65] 回滚事务
来源：http://hdi.xziqi.cn

ROLLBACK;
来源：http://sdi.jlsjyb.cn

[Q66] 行锁查询
来源：http://itn.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sto.c1oappe.top

[Q67] 设置隔离级别
来源：http://rui.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgb.hesvh.cn

[Q68] 保存点
来源：http://sps.hcnkem.com

SAVEPOINT sp1;
来源：http://crs.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://kmb.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://rnd.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dpe.kuanghao11.cn

[Q70] 更新统计信息
来源：http://ouq.yj20258.top

ANALYZE TABLE users;
来源：http://dxe.cdnleiting.top

[Q71] 查看建表语句
来源：http://uem.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uib.chenzaomai.com

[Q72] 查看索引
来源：http://sil.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://tjz.hammf.cn

[Q73] 查看表状态
来源：http://hah.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fkc.cdnleiting.top

[Q74] 强制使用索引
来源：http://qaz.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oqp.ppjwa.cn

[Q75] 日期格式化
来源：http://yvg.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fwr.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nyf.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://kzo.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wlj.52xcode.cn

[Q77] 时间加减
来源：http://mnf.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zsg.fanxiaobao.xyz

[Q78] 当前时间
来源：http://otq.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fpi.xziqi.cn

[Q79] 字符串拼接
来源：http://faw.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zlg.hcnkem.com

[Q80] 字符串截取
来源：http://goo.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bsu.epnwcf.com

[Q81] 字符串替换
来源：http://ieb.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://omf.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://oex.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lye.zhixingplan.top

[Q83] 大小写转换
来源：http://agt.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zkq.dashuyun.cn

[Q84] 去除首尾空格
来源：http://new.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://awg.chenzaomai.com

[Q85] 数值取整
来源：http://dny.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uxk.yuanzhike.top

[Q86] 读取 JSON 字段
来源：http://cks.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://agw.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://ghj.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tpr.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://gdf.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzx.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bof.aizwys.cn

[Q89] 判断表是否存在
来源：http://mqu.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vkc.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://kxs.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://myl.cqqwz.cn

================================================================================
来源：http://rey.fengsongda.top

R. Bash 专题
来源：http://jrx.dashuyun.cn

================================================================================
来源：http://psa.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://oal.yuxming.cn

#!/usr/bin/env bash
来源：http://aup.gzhubu.top

set -euo pipefail
来源：http://wcd.epnwcf.com

[R02] 变量赋值与使用
来源：http://pel.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://tvw.zhoulong.xyz

[R03] 只读变量
来源：http://iwy.gzhubu.top

readonly PI=3.14
来源：http://wpk.havefunace.top

[R04] 位置参数
来源：http://dzl.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dxv.yj202588.top

[R05] 参数默认值
来源：http://fbo.birdmap.top

name="${1:-default}"
来源：http://pbx.shzxlz.cn

[R06] 判断命令是否存在
来源：http://nry.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qih.nwbrower.top

[R07] if 判断文件
来源：http://gso.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uib.fengsongda.top

[R08] 数值比较
来源：http://nau.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://pas.aizwys.cn

[R09] 字符串比较
来源：http://kec.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qoc.xuanzx.com

[R10] 正则匹配
来源：http://ftj.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wmz.0kj1m.cn

[R11] case 多分支
来源：http://tup.tian-w.cn


<!-- 参考信息 -->