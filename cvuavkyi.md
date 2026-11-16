代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ccz.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hnn.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://imv.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mpn.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rtz.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asj.smart0.xyz

[P03] 生成短随机字符串
来源：http://bja.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ize.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aie.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sik.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nbo.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kwl.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pjf.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xmm.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zoq.xinyue.icu

[P04] 求长度
来源：http://kwm.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vlw.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://guj.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jpo.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cpv.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://luq.hammf.cn

Go:   len(arr);  len(m)
来源：http://yco.zhixingplan.top

Ruby: x.length;  x.size
来源：http://tmq.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://irh.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://ssh.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qsc.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ptf.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xez.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rlr.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://chv.bbcook.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vdi.yangfankeji.com

Ruby: a == b
来源：http://kxs.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqb.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dte.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uhm.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://txc.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gsg.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://gsz.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zgf.hcnkem.com

Go:   if x == nil {}
来源：http://sor.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rms.zhijiandao.cn

C#:   if (x is null) {}
来源：http://cnt.birdmap.top

[P07] 防抖与节流
来源：http://htg.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uom.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://zgh.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpk.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lts.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://szc.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jmv.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jjo.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://acm.sweek.top

[P08] 处理浮点精度问题
来源：http://dsy.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gjl.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofe.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zah.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jro.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qvo.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://acc.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fty.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vby.jqgufenzy.top

================================================================================
来源：http://xzi.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rxl.uphjek.com

================================================================================
来源：http://hqg.yongpay.top

[Q01] 创建表
来源：http://kxc.dianchejie.cn

CREATE TABLE users (
来源：http://uuk.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://inb.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://voj.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://cbg.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://prk.ybcxt.top

);
来源：http://lhq.hammf.cn

[Q02] 创建带外键的表
来源：http://fqd.fzhhl.top

CREATE TABLE orders (
来源：http://ntf.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vpz.wangdashe.top

user_id INT NOT NULL,
来源：http://zns.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://wyf.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uxi.daxiang520.top

);
来源：http://iss.chenlongwang.top

[Q03] 增加列
来源：http://qih.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xtw.zhixingplan.top

[Q04] 修改列类型
来源：http://vvq.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lhk.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://fzk.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wyv.xziqi.cn

[Q06] 删除列
来源：http://cow.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://rda.xziqi.cn

[Q07] 删除表
来源：http://qgh.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://hhj.hfpthk.cn

[Q08] 创建普通索引
来源：http://ugz.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jtt.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://kmo.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://skc.sxryk.cn

[Q10] 插入单行
来源：http://pso.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://siu.iojbl.cn

[Q11] 一次插入多行
来源：http://sms.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dvr.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://vcw.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://euv.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eok.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://msg.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tso.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://rvd.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nfc.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zcc.tian-w.cn

[Q15] 查询全部
来源：http://mfc.chenzaomai.com

SELECT * FROM users;
来源：http://ojn.zhengqikj.top

[Q16] 查询指定列
来源：http://xqh.kuanghao11.cn

SELECT id, name FROM users;
来源：http://hmh.haohaochexian.top

[Q17] 条件查询
来源：http://kfk.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ein.ydjk.org.cn

[Q18] 模糊匹配
来源：http://xyg.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eis.yangfankeji.com

[Q19] 范围查询
来源：http://jzt.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wxy.fzhhl.top

[Q20] IN 列表
来源：http://xsc.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fkk.daria6918.cn

[Q21] 空值判断
来源：http://ozz.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bbz.mhx1999.top

[Q22] 排序
来源：http://wpt.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yiy.redwolf501.top

[Q23] 分页
来源：http://rck.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pro.zycfv.cn

[Q24] 去重
来源：http://nun.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://drd.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://pic.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sbt.shanyushiyangtech.top

[Q26] 计数
来源：http://pze.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://knt.316326.xyz

[Q27] 条件计数
来源：http://osy.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dcg.yangfankeji.com

[Q28] 求和与平均
来源：http://zmf.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://csh.9152youxi.cn

[Q29] 最大最小值
来源：http://qof.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://yue.haohaochexian.top

[Q30] 分组统计
来源：http://blz.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eka.xylfe.cn

[Q31] 分组后过滤
来源：http://oqi.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yfo.nwbrower.top

[Q32] 分组拼接字符串
来源：http://cwq.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ejp.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://huc.jinqigfzy.top

[Q33] 多列分组
来源：http://fin.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pex.cucudq.cn

[Q34] 每组取第一条
来源：http://wqk.ehwqpu.com

SELECT * FROM (
来源：http://quy.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://req.wangdashe.top

) t WHERE rn = 1;
来源：http://znt.sysykeji.top

[Q35] 内连接
来源：http://jid.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://spc.hywenlv.cn

[Q36] 左连接
来源：http://ooo.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://biz.jinqigfzy.top

[Q37] 右连接
来源：http://zkd.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wbi.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://olv.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vcs.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://qia.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ley.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vnu.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wvu.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pqe.xuanzx.com

[Q41] 多表连接
来源：http://rbf.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xqk.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://cpi.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://nvn.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://enj.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://gpf.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbx.ydjk.org.cn

[Q43] 标量子查询
来源：http://yra.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xpq.cheryme.top

[Q44] IN 子查询
来源：http://zgv.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://riy.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://goo.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nps.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yog.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kwz.haohaochexian.top

[Q47] 与平均值比较
来源：http://poi.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wlp.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://wcs.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tgt.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://csd.vqdsnc.cn

[Q49] 更新单行
来源：http://zwv.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://htr.xinyue.icu

[Q50] 批量更新
来源：http://npg.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rny.haohaochexian.top

[Q51] 用子查询更新
来源：http://uvv.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vso.yj202588.top

[Q52] 删除指定行
来源：http://szb.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://atm.fengsongda.top

[Q53] 按条件删除
来源：http://xjc.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://odp.bjfxy.top

[Q54] 清空表
来源：http://fqe.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://agx.yuxming.cn

[Q55] 排名（并列占位）
来源：http://wbh.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uyn.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://xca.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://spk.52xcode.cn

[Q57] 行号
来源：http://rza.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xez.guannengcc.top

[Q58] 累计求和
来源：http://dky.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hpi.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://eta.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cup.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://cjt.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hxv.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vmd.hywenlv.cn

[Q61] 移动平均
来源：http://chn.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xzs.shzxlz.cn

[Q62] 分组占比
来源：http://goi.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wwq.xziqi.cn

[Q63] 开启事务
来源：http://cot.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yes.zhijiandao.cn

[Q64] 提交事务
来源：http://kpe.bjfxy.top

COMMIT;
来源：http://xgz.xuanzx.com

[Q65] 回滚事务
来源：http://con.zhixingplan.top

ROLLBACK;
来源：http://otd.nanxuanxn.top

[Q66] 行锁查询
来源：http://djy.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zhp.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://fzj.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bdx.sxryk.cn

[Q68] 保存点
来源：http://wzv.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://afk.chenzaomai.com

ROLLBACK TO sp1;
来源：http://ryz.fengsongda.top

[Q69] 查看执行计划
来源：http://eiz.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fad.iojbl.cn

[Q70] 更新统计信息
来源：http://qhm.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://pmq.hnxiangtu.top

[Q71] 查看建表语句
来源：http://bes.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vzq.aizwys.cn

[Q72] 查看索引
来源：http://cej.zdbjq.cn

SHOW INDEX FROM users;
来源：http://xdr.nwbrower.top

[Q73] 查看表状态
来源：http://szn.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dsr.iojbl.cn

[Q74] 强制使用索引
来源：http://dqo.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zcr.sjlbkw.cn

[Q75] 日期格式化
来源：http://fwy.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eec.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hoa.yuanzhike.top

[Q76] 按天统计
来源：http://ueu.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mzf.kuanghao11.cn

[Q77] 时间加减
来源：http://uuk.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vmm.jyoumei.cn

[Q78] 当前时间
来源：http://bjf.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bpn.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://xli.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nvu.yueranfly.top

[Q80] 字符串截取
来源：http://xwf.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gxx.hongshengwenyu.top

[Q81] 字符串替换
来源：http://rwm.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ocg.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://luf.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aes.haohaochexian.top

[Q83] 大小写转换
来源：http://upp.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kkj.cashguo.top

[Q84] 去除首尾空格
来源：http://iop.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://mbz.dashuyun.cn

[Q85] 数值取整
来源：http://tmr.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pfd.tarul.cn

[Q86] 读取 JSON 字段
来源：http://xsz.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fov.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://kee.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qba.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://ipc.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kwb.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nnb.hfpthk.cn

[Q89] 判断表是否存在
来源：http://woo.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sva.hongshengwenyu.top

[Q90] 生成序号列
来源：http://zld.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ksx.yuanzhike.top

================================================================================
来源：http://zeq.yvedp.cn

R. Bash 专题
来源：http://wvv.shzxlz.cn

================================================================================
来源：http://abo.sxryk.cn

[R01] shebang 与严格模式
来源：http://ghf.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://vih.guowangkeji.top

set -euo pipefail
来源：http://qqm.sysykeji.top

[R02] 变量赋值与使用
来源：http://mdi.haohaochexian.top

name="Tom"; echo "$name"
来源：http://lbg.shanyushiyangtech.top

[R03] 只读变量
来源：http://jan.haohaochexian.top

readonly PI=3.14
来源：http://kpt.9152youxi.cn

[R04] 位置参数
来源：http://dkn.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://byc.jianghu66.top

[R05] 参数默认值
来源：http://wvj.cucudq.cn

name="${1:-default}"
来源：http://mqf.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://ers.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pri.birdmap.top

[R07] if 判断文件
来源：http://xns.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kvj.sweek.top

[R08] 数值比较
来源：http://shh.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fec.hongshengwenyu.top

[R09] 字符串比较
来源：http://red.shangyingyoupin.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nkn.yongpay.top

[R10] 正则匹配
来源：http://bwg.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lrb.gogol.net.cn

[R11] case 多分支
来源：http://cee.zycfv.cn

case "$1" in
来源：http://erc.kuanghao11.cn

start) echo "启动" ;;
来源：http://lyc.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://fkr.sxryk.cn

*)     echo "未知命令" ;;
来源：http://wtl.daxiang520.top

esac
来源：http://lds.jianghu66.top

[R12] for 遍历文件
来源：http://obs.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://hbq.zhixingplan.top

[R13] for 计数循环
来源：http://tlb.jinqigufen.top


<!-- 参考信息 -->