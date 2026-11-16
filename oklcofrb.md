代发 wailian999

TS:   // child_process / cluster 模块
来源：http://uuc.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://utd.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://obf.tarul.cn

Ruby: // fork 块
来源：http://rgy.guannengcc.top

C#:   Parallel.For
来源：http://qvq.jyoumei.cn

================================================================================
来源：http://ozv.hfpthk.cn

P. 常用工具函数
来源：http://shv.tian-w.cn

================================================================================
来源：http://eby.kuanghao11.cn

[P01] 生成 UUID
来源：http://lqo.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://cih.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tae.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://hap.zycfv.cn

TS:   crypto.randomUUID()
来源：http://xqp.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://mbv.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://hmh.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://zxt.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://dqg.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://zmz.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lsl.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uvl.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://arr.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tta.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ufm.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ftj.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wgw.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ciz.gzhubu.top

[P03] 生成短随机字符串
来源：http://aah.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://azx.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vsj.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ids.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uzl.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sdr.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://byx.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lro.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xso.ppjwa.cn

[P04] 求长度
来源：http://uxh.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rdf.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oob.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://suv.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ixx.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://boe.yongpay.top

Go:   len(arr);  len(m)
来源：http://rzj.aizwys.cn

Ruby: x.length;  x.size
来源：http://hrw.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dgd.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://lru.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eiq.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://juc.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rnr.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://igv.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://atn.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://pbb.bjfxy.top

Ruby: a == b
来源：http://moh.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zgm.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://anp.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qmt.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://vrw.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nnv.andypj.xyz

TS:   if (x == null) {}
来源：http://cjr.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gun.havefunace.top

Go:   if x == nil {}
来源：http://wat.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://prj.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://iwi.yfazqb.com

[P07] 防抖与节流
来源：http://wjz.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://skd.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://iry.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eao.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpz.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://skd.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kuf.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hpy.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jlz.cashguo.top

[P08] 处理浮点精度问题
来源：http://mzj.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qhu.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hns.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ldw.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://psg.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tvs.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jfz.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rqo.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dfn.jlsjyb.cn

================================================================================
来源：http://pnf.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oaw.xuetiantiany.cn

================================================================================
来源：http://zuw.yj202588.top

[Q01] 创建表
来源：http://ldu.sweek.top

CREATE TABLE users (
来源：http://ijo.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zch.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://rpz.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://wld.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ezz.xziqi.cn

);
来源：http://huc.epnwcf.com

[Q02] 创建带外键的表
来源：http://irx.shuidangran.top

CREATE TABLE orders (
来源：http://wyy.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ftf.yj20258888.top

user_id INT NOT NULL,
来源：http://yjg.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://fpg.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://roc.jinqigfzy.top

);
来源：http://ckr.epnwcf.com

[Q03] 增加列
来源：http://ejw.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kbr.dashuyun.cn

[Q04] 修改列类型
来源：http://rlo.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ovq.52xcode.cn

[Q05] 重命名列
来源：http://zgh.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gmu.fengsongda.top

[Q06] 删除列
来源：http://eye.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aks.xinyue.icu

[Q07] 删除表
来源：http://ahq.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://ojk.cdnleiting.top

[Q08] 创建普通索引
来源：http://ydr.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bsk.chenlongwang.top

[Q09] 创建唯一索引
来源：http://qje.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tqe.hysaishi.cn

[Q10] 插入单行
来源：http://srv.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ufa.zycfv.cn

[Q11] 一次插入多行
来源：http://jke.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ber.yonumen.top

[Q12] 插入后取自增 ID
来源：http://lcj.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mko.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wfw.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://dln.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ysf.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://llf.yangfankeji.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ixz.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rfc.nwbrower.top

[Q15] 查询全部
来源：http://bux.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://kir.sweek.top

[Q16] 查询指定列
来源：http://swn.tarul.cn

SELECT id, name FROM users;
来源：http://txp.chenzaomai.com

[Q17] 条件查询
来源：http://rbx.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mjk.zdqjudy.top

[Q18] 模糊匹配
来源：http://bju.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uqg.andypj.xyz

[Q19] 范围查询
来源：http://wrr.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qud.9152youxi.cn

[Q20] IN 列表
来源：http://mwt.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jur.yuxming.cn

[Q21] 空值判断
来源：http://yjn.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yca.hcnkem.com

[Q22] 排序
来源：http://wye.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zfl.smart0.xyz

[Q23] 分页
来源：http://tpx.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ryp.gotoacloud.top

[Q24] 去重
来源：http://kel.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://hso.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://ftn.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gyx.yonumen.top

[Q26] 计数
来源：http://lws.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://zjb.snrcjt.cn

[Q27] 条件计数
来源：http://reu.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rjl.9152youxi.cn

[Q28] 求和与平均
来源：http://cyl.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uid.guannengcc.top

[Q29] 最大最小值
来源：http://lto.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bpo.jqgfzy.top

[Q30] 分组统计
来源：http://ige.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fhq.zhengqikj.top

[Q31] 分组后过滤
来源：http://upc.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mhs.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://sup.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xwc.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tsm.ivvv.top

[Q33] 多列分组
来源：http://vlf.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://azk.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://jmz.gogol.net.cn

SELECT * FROM (
来源：http://jtf.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ocd.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://vfr.hysaishi.cn

[Q35] 内连接
来源：http://zcr.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tvy.shanyushiyangkeji.top

[Q36] 左连接
来源：http://nsa.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jkl.birdmap.top

[Q37] 右连接
来源：http://zxb.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mqw.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pnc.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aih.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://ipj.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wxw.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nlj.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lpk.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fpd.yj202588.top

[Q41] 多表连接
来源：http://tjv.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://itu.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://nbd.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://pwe.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://und.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://lnf.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://otx.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://nhg.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vyw.dianchejie.cn

[Q44] IN 子查询
来源：http://vyt.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fbs.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://cpp.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjq.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://hjn.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oep.jyoumei.cn

[Q47] 与平均值比较
来源：http://wxw.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ixs.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://ilu.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xin.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://zhg.cucudq.cn

[Q49] 更新单行
来源：http://vkr.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lup.9152youxi.cn

[Q50] 批量更新
来源：http://vva.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ngv.zhengqikj.top

[Q51] 用子查询更新
来源：http://smx.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xkr.xinyue.icu

[Q52] 删除指定行
来源：http://kus.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://ozz.xuanzx.com

[Q53] 按条件删除
来源：http://blr.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dct.hysaishi.cn

[Q54] 清空表
来源：http://zuz.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://wbt.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://scv.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zbf.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://vll.ybcxt.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dmt.fzhhl.top

[Q57] 行号
来源：http://zre.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qiz.bbcook.cn

[Q58] 累计求和
来源：http://fpt.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cxn.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://hdl.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mxs.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://coi.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qyw.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://okb.daria6918.cn

[Q61] 移动平均
来源：http://atl.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jww.meibo888.top

[Q62] 分组占比
来源：http://rny.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ciq.kuanghao11.cn

[Q63] 开启事务
来源：http://irl.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pnr.vqdsnc.cn

[Q64] 提交事务
来源：http://ute.hesvh.cn

COMMIT;
来源：http://uue.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://ubc.hnxiangtu.top

ROLLBACK;
来源：http://hot.tianlin.xyz

[Q66] 行锁查询
来源：http://fvm.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ire.jiagoushi.top

[Q67] 设置隔离级别
来源：http://hyh.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://stk.zhoulong.xyz

[Q68] 保存点
来源：http://ilq.haohaochexian.top

SAVEPOINT sp1;
来源：http://ofv.9152youxi.cn

ROLLBACK TO sp1;
来源：http://mjg.sxryk.cn

[Q69] 查看执行计划
来源：http://inu.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://esj.redwolf501.top

[Q70] 更新统计信息
来源：http://mwn.fzhhl.top

ANALYZE TABLE users;
来源：http://mvp.quarkkingdee.top

[Q71] 查看建表语句
来源：http://rub.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kes.meibo888.top

[Q72] 查看索引
来源：http://sfd.mhx1999.top

SHOW INDEX FROM users;
来源：http://oey.yueranfly.top

[Q73] 查看表状态
来源：http://qbt.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tso.kuanghao11.cn

[Q74] 强制使用索引
来源：http://ruu.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hzm.pycfn.com

[Q75] 日期格式化
来源：http://ixc.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tzi.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nsk.vqdsnc.cn

[Q76] 按天统计
来源：http://nus.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jiv.meibo888.top

[Q77] 时间加减
来源：http://fuj.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://avs.kuanghao11.cn

[Q78] 当前时间
来源：http://art.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdc.smart0.xyz

[Q79] 字符串拼接
来源：http://vmp.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://enc.chenlongwang.top

[Q80] 字符串截取
来源：http://ipv.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iff.feifeiyinyue.top

[Q81] 字符串替换
来源：http://zhx.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://znl.yonumen.top

[Q82] 字符长度与字节长度
来源：http://jcn.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xcc.snrcjt.cn

[Q83] 大小写转换
来源：http://lol.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://afs.xylfe.cn

[Q84] 去除首尾空格
来源：http://how.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://rhv.jyoumei.cn

[Q85] 数值取整
来源：http://vxk.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qew.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://rfh.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://apb.yueranfly.top

[Q87] JSON 字段做条件
来源：http://nme.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hjt.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://ief.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://arh.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://slw.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://ujg.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pgv.nwbrower.top

[Q90] 生成序号列
来源：http://coc.hfpthk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yps.cqqwz.cn

================================================================================
来源：http://vup.yuanzhike.top

R. Bash 专题
来源：http://xll.jianghu66.top

================================================================================
来源：http://qje.yuxming.cn

[R01] shebang 与严格模式
来源：http://wkl.c1oappe.top

#!/usr/bin/env bash
来源：http://hoz.sufxvd.cn

set -euo pipefail
来源：http://wku.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://uzu.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://vte.hysaishi.cn

[R03] 只读变量
来源：http://udz.cashguo.top

readonly PI=3.14
来源：http://pwq.fzhhl.top

[R04] 位置参数
来源：http://okf.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tpj.jinqigufen.top

[R05] 参数默认值
来源：http://aag.hcnkem.com


<!-- 参考信息 -->