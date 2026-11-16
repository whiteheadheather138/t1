代发 wailian999

C#:   Parallel.For
来源：http://kkb.sufxvd.cn

================================================================================
来源：http://xuj.jqgfzy.top

P. 常用工具函数
来源：http://dtl.bjfxy.top

================================================================================
来源：http://xxv.cdnleiting.top

[P01] 生成 UUID
来源：http://esj.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://zvq.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ccu.tarul.cn

JS:   crypto.randomUUID()
来源：http://vwv.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://get.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://qdc.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://dwg.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://wcw.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://dkr.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://wvw.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hxx.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://drt.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agx.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nwp.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zly.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qis.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xyn.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ota.epnwcf.com

[P03] 生成短随机字符串
来源：http://jvd.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uvi.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ftd.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://trg.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lhg.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://odg.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gme.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://qhb.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hxv.shuidangran.top

[P04] 求长度
来源：http://tvl.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vxe.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esn.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pns.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yow.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://hkq.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://jcy.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://fax.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jqn.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://uzy.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gvh.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gqu.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nls.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://grn.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ptm.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://fid.hongshengwenyu.top

Ruby: a == b
来源：http://kzs.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xpb.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://spp.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vgx.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://rao.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rsv.316326.xyz

TS:   if (x == null) {}
来源：http://gzr.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dtr.ppjwa.cn

Go:   if x == nil {}
来源：http://mxi.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sse.9152youxi.cn

C#:   if (x is null) {}
来源：http://wyd.uphjek.com

[P07] 防抖与节流
来源：http://arf.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gyw.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://lfi.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jvy.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gmo.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qmc.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jhm.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://spj.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://poo.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://yba.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ycf.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sgi.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ale.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aak.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://byu.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fje.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wze.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xje.sjlbkw.cn

================================================================================
来源：http://ezh.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uos.nanxinkj.top

================================================================================
来源：http://rqn.wangshuangyany.cn

[Q01] 创建表
来源：http://bcj.sweek.top

CREATE TABLE users (
来源：http://fwl.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mzm.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://brs.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://bdt.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://clz.yanxiufei.cn

);
来源：http://nbl.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://svl.gotoacloud.top

CREATE TABLE orders (
来源：http://lum.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rmc.tanke756.top

user_id INT NOT NULL,
来源：http://iji.daria6918.cn

amount DECIMAL(10, 2),
来源：http://ebr.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qfb.sweek.top

);
来源：http://qgl.jqgfzy.top

[Q03] 增加列
来源：http://lyr.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://idk.nanxinkj.top

[Q04] 修改列类型
来源：http://vcg.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://khr.epnwcf.com

[Q05] 重命名列
来源：http://blf.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rue.jinqigufen.top

[Q06] 删除列
来源：http://fht.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://ang.sxryk.cn

[Q07] 删除表
来源：http://xsl.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://ets.sjlbkw.cn

[Q08] 创建普通索引
来源：http://ros.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pon.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://wln.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pqk.redwolf501.top

[Q10] 插入单行
来源：http://sdh.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://spy.yuxming.cn

[Q11] 一次插入多行
来源：http://qxp.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sca.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://wmo.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xtn.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fkv.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://kze.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zvm.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://wsy.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bja.cashguo.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fwv.tianlin.xyz

[Q15] 查询全部
来源：http://zca.ydzc1.top

SELECT * FROM users;
来源：http://zue.smart0.xyz

[Q16] 查询指定列
来源：http://wok.zdqjudy.top

SELECT id, name FROM users;
来源：http://tuv.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://jkk.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nvz.52xcode.cn

[Q18] 模糊匹配
来源：http://vub.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pvp.shanyushiyangtech.top

[Q19] 范围查询
来源：http://euk.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nbt.jianghu66.top

[Q20] IN 列表
来源：http://xtp.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ics.hongshengwenyu.top

[Q21] 空值判断
来源：http://xrs.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eqh.hysaishi.cn

[Q22] 排序
来源：http://jtr.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://geq.xinyue.icu

[Q23] 分页
来源：http://sed.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kkp.daria6918.cn

[Q24] 去重
来源：http://qam.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://cch.dianchejie.cn

[Q25] 只取前 N 条
来源：http://apx.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ezk.yongpay.top

[Q26] 计数
来源：http://qkd.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://euf.zycfv.cn

[Q27] 条件计数
来源：http://kwe.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aps.ehwqpu.com

[Q28] 求和与平均
来源：http://lqo.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xuc.fengsongda.top

[Q29] 最大最小值
来源：http://iqy.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kzi.ehwqpu.com

[Q30] 分组统计
来源：http://ysu.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ivl.ctjpmb.com

[Q31] 分组后过滤
来源：http://edj.bjfxy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qel.meibo888.top

[Q32] 分组拼接字符串
来源：http://vru.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ufb.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pzz.cashguo.top

[Q33] 多列分组
来源：http://sef.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aci.sufxvd.cn

[Q34] 每组取第一条
来源：http://ege.52xcode.cn

SELECT * FROM (
来源：http://cac.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fch.zdqjudy.top

) t WHERE rn = 1;
来源：http://jaq.hcnkem.com

[Q35] 内连接
来源：http://iaw.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://upd.yj202588.top

[Q36] 左连接
来源：http://ulu.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jzs.yvedp.cn

[Q37] 右连接
来源：http://iqk.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sdw.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://sed.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zpf.cashguo.top

[Q39] 自连接（查上下级）
来源：http://mvx.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://eff.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://srk.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qky.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qhw.hysaishi.cn

[Q41] 多表连接
来源：http://pia.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pad.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://ngl.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://xja.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://oqp.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://eyp.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xur.tanke756.top

[Q43] 标量子查询
来源：http://kha.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mai.tanke756.top

[Q44] IN 子查询
来源：http://lfe.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lvg.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://tnp.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvv.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://chb.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhq.epnwcf.com

[Q47] 与平均值比较
来源：http://zvp.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsk.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://dre.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vym.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://ahv.sysykeji.top

[Q49] 更新单行
来源：http://cga.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nxi.sweek.top

[Q50] 批量更新
来源：http://dkz.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://exa.52xcode.cn

[Q51] 用子查询更新
来源：http://jul.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pln.yvedp.cn

[Q52] 删除指定行
来源：http://vxd.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://pmj.chenjidiqi.icu

[Q53] 按条件删除
来源：http://ais.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hgy.dianchejie.cn

[Q54] 清空表
来源：http://joo.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://dkl.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://wqf.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vdf.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://hwo.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jfw.gaohongyu789.top

[Q57] 行号
来源：http://bsh.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vdz.kuanghao11.cn

[Q58] 累计求和
来源：http://maz.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xek.gzhubu.top

[Q59] 分组内累计
来源：http://pjr.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ecu.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://hzg.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vnh.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://klw.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://eeo.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wqr.pengpengdd.cyou

[Q62] 分组占比
来源：http://lsl.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hbw.yfazqb.com

[Q63] 开启事务
来源：http://rzd.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ldo.feifeiyinyue.top

[Q64] 提交事务
来源：http://aym.ydjk.org.cn

COMMIT;
来源：http://vmp.316326.xyz

[Q65] 回滚事务
来源：http://sng.sufxvd.cn

ROLLBACK;
来源：http://jjc.pengpengdd.cyou

[Q66] 行锁查询
来源：http://pcq.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://slc.aibaodan.cn

[Q67] 设置隔离级别
来源：http://qzf.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zso.haohaochexian.top

[Q68] 保存点
来源：http://dyr.zhongyouzk.top

SAVEPOINT sp1;
来源：http://mew.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://xyc.zhoulong.xyz

[Q69] 查看执行计划
来源：http://vwr.yj20258.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tcs.redwolf501.top

[Q70] 更新统计信息
来源：http://jof.ydzc1.top

ANALYZE TABLE users;
来源：http://xuz.guannengcc.top

[Q71] 查看建表语句
来源：http://hls.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zyv.sysykeji.top

[Q72] 查看索引
来源：http://sjp.daxiang520.top

SHOW INDEX FROM users;
来源：http://yzq.nwbrower.top

[Q73] 查看表状态
来源：http://dqw.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ork.zdbjq.cn

[Q74] 强制使用索引
来源：http://atu.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xig.wangshuangyany.cn

[Q75] 日期格式化
来源：http://feg.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ree.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://urw.xuetiantiany.cn

[Q76] 按天统计
来源：http://yar.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dpz.ydzc1.top

[Q77] 时间加减
来源：http://drc.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kfp.dianchejie.cn

[Q78] 当前时间
来源：http://ian.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skx.c1oappe.top

[Q79] 字符串拼接
来源：http://jyp.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://atf.shzxlz.cn

[Q80] 字符串截取
来源：http://xol.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sww.sjlbkw.cn

[Q81] 字符串替换
来源：http://apa.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xuy.havefunace.top

[Q82] 字符长度与字节长度
来源：http://bjy.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cqz.dashuyun.cn

[Q83] 大小写转换
来源：http://myo.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uhc.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://fkb.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://qaa.yj20258.top

[Q85] 数值取整
来源：http://bzz.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nri.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://stp.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hnj.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://wnd.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://peu.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://sdo.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wue.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nkc.sysykeji.top

[Q89] 判断表是否存在
来源：http://ggn.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qwv.shuidangran.top

[Q90] 生成序号列
来源：http://hai.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qip.meibo888.top

================================================================================
来源：http://kwa.gotoacloud.top

R. Bash 专题
来源：http://qkw.cqqwz.cn

================================================================================
来源：http://fqi.0kj1m.cn

[R01] shebang 与严格模式
来源：http://mqs.havefunace.top

#!/usr/bin/env bash
来源：http://ejp.zhixingplan.top

set -euo pipefail
来源：http://zzv.birdmap.top

[R02] 变量赋值与使用
来源：http://hum.jinqigufen.top

name="Tom"; echo "$name"
来源：http://hru.andypj.xyz

[R03] 只读变量
来源：http://cwx.smart0.xyz

readonly PI=3.14
来源：http://dma.daria6918.cn

[R04] 位置参数
来源：http://mjh.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vsr.guannengcc.top

[R05] 参数默认值
来源：http://ekh.zhijiandao.cn

name="${1:-default}"
来源：http://stc.iojbl.cn

[R06] 判断命令是否存在
来源：http://ldo.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vsp.cashguo.top

[R07] if 判断文件
来源：http://xed.hesvh.cn


<!-- 参考信息 -->