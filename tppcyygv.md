代发 wailian999

C#:   Parallel.For
来源：http://nij.ydjk.org.cn

================================================================================
来源：http://nbr.jyoumei.cn

P. 常用工具函数
来源：http://ufk.chenjidiqi.icu

================================================================================
来源：http://ytd.cheryme.top

[P01] 生成 UUID
来源：http://vxb.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://ceq.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wta.hnqzz.top

JS:   crypto.randomUUID()
来源：http://zmg.vehdjk.com

TS:   crypto.randomUUID()
来源：http://evx.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://bxv.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://nxx.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://xve.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://ajc.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://ckm.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dbp.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vtp.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xzv.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zgv.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://trc.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wlc.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xbh.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ipd.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://veq.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zvl.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://egv.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pjk.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kha.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wlz.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pka.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mhl.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kku.cdnleiting.top

[P04] 求长度
来源：http://izh.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wcy.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfw.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvb.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ikx.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://lgc.birdmap.top

Go:   len(arr);  len(m)
来源：http://zcg.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://ipe.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://avm.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://nit.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fli.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oez.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wno.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gbi.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tro.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://hvr.yuxming.cn

Ruby: a == b
来源：http://ckz.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yth.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uci.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vnj.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://hhp.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gkc.yangfankeji.com

TS:   if (x == null) {}
来源：http://orw.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uke.xylfe.cn

Go:   if x == nil {}
来源：http://rjz.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://avh.shzxlz.cn

C#:   if (x is null) {}
来源：http://hgo.hfpthk.cn

[P07] 防抖与节流
来源：http://prp.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gno.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://iqo.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dnl.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qsd.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dij.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fqs.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jhf.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rhp.cucudq.cn

[P08] 处理浮点精度问题
来源：http://hxj.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://frb.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hfb.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cnj.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ygf.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fdj.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wnc.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ugu.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qli.hnxiangtu.top

================================================================================
来源：http://xey.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gpq.hongshengwenyu.top

================================================================================
来源：http://fcl.fktsv.cn

[Q01] 创建表
来源：http://kmy.ybcxt.top

CREATE TABLE users (
来源：http://hei.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jpd.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://geb.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://hse.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wsp.fanxiaobao.xyz

);
来源：http://fbn.bjfxy.top

[Q02] 创建带外键的表
来源：http://tdw.meibo888.top

CREATE TABLE orders (
来源：http://cur.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vdl.meibo888.top

user_id INT NOT NULL,
来源：http://czq.yvedp.cn

amount DECIMAL(10, 2),
来源：http://afs.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sdo.jianghu66.top

);
来源：http://vke.pycfn.com

[Q03] 增加列
来源：http://evh.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vyf.yvedp.cn

[Q04] 修改列类型
来源：http://iky.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xyx.xylfe.cn

[Q05] 重命名列
来源：http://dmn.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://szf.xinyue.icu

[Q06] 删除列
来源：http://uaa.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://nqq.wangshuangyany.cn

[Q07] 删除表
来源：http://ybn.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://mne.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://mpf.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://apk.sjlbkw.cn

[Q09] 创建唯一索引
来源：http://war.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uho.shangyingyoupin.top

[Q10] 插入单行
来源：http://asv.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zud.jianghu66.top

[Q11] 一次插入多行
来源：http://byv.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jkv.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://jxb.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://awa.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ddb.cucudq.cn

[Q13] 忽略重复插入
来源：http://gcx.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hed.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://wrn.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bkk.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://poz.hnxiangtu.top

[Q15] 查询全部
来源：http://ffe.shzxlz.cn

SELECT * FROM users;
来源：http://bug.yueranfly.top

[Q16] 查询指定列
来源：http://ace.birdmap.top

SELECT id, name FROM users;
来源：http://ssj.yj202588.top

[Q17] 条件查询
来源：http://aqm.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://syp.yongpay.top

[Q18] 模糊匹配
来源：http://zse.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://daw.c1oappe.top

[Q19] 范围查询
来源：http://hli.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://crz.hywenlv.cn

[Q20] IN 列表
来源：http://kgp.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qwx.cashguo.top

[Q21] 空值判断
来源：http://aez.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lcy.haohaochexian.top

[Q22] 排序
来源：http://wlx.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yds.gaohongyu789.top

[Q23] 分页
来源：http://vbj.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://scl.sxryk.cn

[Q24] 去重
来源：http://pcs.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://jwm.yuxming.cn

[Q25] 只取前 N 条
来源：http://hzn.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wif.meibo888.top

[Q26] 计数
来源：http://jbs.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://ipa.meibo888.top

[Q27] 条件计数
来源：http://gkd.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lcr.gzhubu.top

[Q28] 求和与平均
来源：http://eqe.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://itv.shuidangran.top

[Q29] 最大最小值
来源：http://vai.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ylr.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://xcm.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xky.gotoacloud.top

[Q31] 分组后过滤
来源：http://vbi.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zaf.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://dnr.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://epx.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bao.jianghu66.top

[Q33] 多列分组
来源：http://obt.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xcp.gotoacloud.top

[Q34] 每组取第一条
来源：http://kad.shanyushiyangtech.top

SELECT * FROM (
来源：http://dte.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ggu.xuanzx.com

) t WHERE rn = 1;
来源：http://asb.yuanzhike.top

[Q35] 内连接
来源：http://asv.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bfj.xinyue.icu

[Q36] 左连接
来源：http://vzi.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yah.zhaomingkeji.xyz

[Q37] 右连接
来源：http://lqj.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tth.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gha.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://exd.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://lvr.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qtq.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iih.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dsb.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vdj.wangshuangyany.cn

[Q41] 多表连接
来源：http://apu.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nww.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://drh.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://kqt.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://cbh.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://joc.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rqt.yuanzhike.top

[Q43] 标量子查询
来源：http://ewb.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zan.zdqjudy.top

[Q44] IN 子查询
来源：http://qbs.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ccv.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://jek.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tmn.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tlu.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nea.zhoulong.xyz

[Q47] 与平均值比较
来源：http://rlu.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ppc.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://lam.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsy.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://faw.birdmap.top

[Q49] 更新单行
来源：http://vcf.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kcw.cashguo.top

[Q50] 批量更新
来源：http://urr.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://joo.bbcook.cn

[Q51] 用子查询更新
来源：http://naq.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://juo.aizwys.cn

[Q52] 删除指定行
来源：http://tcl.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://emo.redwolf501.top

[Q53] 按条件删除
来源：http://lvg.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tsg.guowangkeji.top

[Q54] 清空表
来源：http://vss.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://prv.ydzc1.top

[Q55] 排名（并列占位）
来源：http://smv.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ozi.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://vqp.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tir.feifeiyinyue.top

[Q57] 行号
来源：http://xwg.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jza.hcnkem.com

[Q58] 累计求和
来源：http://ooh.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://alz.guowangkeji.top

[Q59] 分组内累计
来源：http://leo.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://elq.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://ixs.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cyg.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ufw.xylfe.cn

[Q61] 移动平均
来源：http://nfj.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ehl.cucudq.cn

[Q62] 分组占比
来源：http://fte.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qsv.uphjek.com

[Q63] 开启事务
来源：http://ndh.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hjb.0kj1m.cn

[Q64] 提交事务
来源：http://xbe.mhx1999.top

COMMIT;
来源：http://nyl.andypj.xyz

[Q65] 回滚事务
来源：http://pgo.wangdashe.top

ROLLBACK;
来源：http://aqm.pengpengdd.cyou

[Q66] 行锁查询
来源：http://pwk.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://szq.316326.xyz

[Q67] 设置隔离级别
来源：http://naf.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oyy.dashuyun.cn

[Q68] 保存点
来源：http://vtj.cdnleiting.top

SAVEPOINT sp1;
来源：http://flg.uphjek.com

ROLLBACK TO sp1;
来源：http://fnb.kuanghao11.cn

[Q69] 查看执行计划
来源：http://yfz.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bjn.birdmap.top

[Q70] 更新统计信息
来源：http://zsm.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://jhh.iojbl.cn

[Q71] 查看建表语句
来源：http://wtg.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nai.hnqzz.top

[Q72] 查看索引
来源：http://bii.316326.xyz

SHOW INDEX FROM users;
来源：http://hvr.pengpengdd.cyou

[Q73] 查看表状态
来源：http://ffb.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gee.yuxming.cn

[Q74] 强制使用索引
来源：http://ocx.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vcg.hesvh.cn

[Q75] 日期格式化
来源：http://nel.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pyo.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hxk.fengsongda.top

[Q76] 按天统计
来源：http://omy.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hlq.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://yev.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wnh.hesvh.cn

[Q78] 当前时间
来源：http://qdu.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dun.sjlbkw.cn

[Q79] 字符串拼接
来源：http://usb.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://feb.hesvh.cn

[Q80] 字符串截取
来源：http://knz.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jvi.52xcode.cn

[Q81] 字符串替换
来源：http://pdg.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://itt.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://bjd.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pdg.svipenyu.cn

[Q83] 大小写转换
来源：http://rcc.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xjd.yuxming.cn

[Q84] 去除首尾空格
来源：http://eik.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://bys.yongpay.top

[Q85] 数值取整
来源：http://ims.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pqw.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://byt.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yrb.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://kvy.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oqw.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://yrf.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wdg.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://klk.yangfankeji.com

[Q89] 判断表是否存在
来源：http://qzf.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gag.yj202588.top

[Q90] 生成序号列
来源：http://zxn.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tvv.guowangkeji.top

================================================================================
来源：http://puc.shanyushiyangtech.top

R. Bash 专题
来源：http://alh.gotoacloud.top

================================================================================
来源：http://soc.0kj1m.cn

[R01] shebang 与严格模式
来源：http://gab.dianchejie.cn

#!/usr/bin/env bash
来源：http://qbv.wangdashe.top

set -euo pipefail
来源：http://hhm.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://fjw.yj202588.top

name="Tom"; echo "$name"
来源：http://naj.jinghuilouyu.cn

[R03] 只读变量
来源：http://dpe.hcnkem.com

readonly PI=3.14
来源：http://xun.cqqwz.cn

[R04] 位置参数
来源：http://asl.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ecz.hesvh.cn

[R05] 参数默认值
来源：http://iwc.zdqjudy.top

name="${1:-default}"
来源：http://gxc.52xcode.cn

[R06] 判断命令是否存在
来源：http://doj.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://irp.ctjpmb.com

[R07] if 判断文件
来源：http://rav.shzxlz.cn


<!-- 参考信息 -->