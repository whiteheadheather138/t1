代发 wailian999

[P01] 生成 UUID
来源：http://rdn.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://knc.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jrv.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://ftg.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://ede.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://xls.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://acz.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://kbq.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://uav.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://nnv.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kzd.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yzt.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ksz.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://het.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xdo.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lez.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sld.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ryk.yuanzhike.top

[P03] 生成短随机字符串
来源：http://tcz.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gku.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dqd.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yun.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bqk.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gps.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ekp.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://woz.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ctk.pycfn.com

[P04] 求长度
来源：http://hnb.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bdj.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwd.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fak.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tyf.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://itf.hcnkem.com

Go:   len(arr);  len(m)
来源：http://fek.gotoacloud.top

Ruby: x.length;  x.size
来源：http://uxj.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lty.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://zgr.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ebz.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qfv.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hrv.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gkn.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yut.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fdb.zhijiandao.cn

Ruby: a == b
来源：http://xuf.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mdd.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cvp.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fnn.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://mio.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qbo.jianghu66.top

TS:   if (x == null) {}
来源：http://vlr.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://bwg.shangyingyoupin.top

Go:   if x == nil {}
来源：http://vtz.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eqj.wangdashe.top

C#:   if (x is null) {}
来源：http://ccg.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://jxj.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fdv.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://iqj.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uaz.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qvi.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ldv.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xmw.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://fju.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zhp.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://kis.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zxc.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ldh.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ymb.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mqc.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ifh.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nlg.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lkk.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bks.ctjpmb.com

================================================================================
来源：http://yka.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nqk.xuetiantiany.cn

================================================================================
来源：http://pcw.hammf.cn

[Q01] 创建表
来源：http://lub.tianlin.xyz

CREATE TABLE users (
来源：http://ytu.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pxk.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://vnk.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://dza.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kge.sjlbkw.cn

);
来源：http://muf.chenlongwang.top

[Q02] 创建带外键的表
来源：http://dfs.quarkkingdee.top

CREATE TABLE orders (
来源：http://tez.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pbb.haohaochexian.top

user_id INT NOT NULL,
来源：http://iwm.yj20258.top

amount DECIMAL(10, 2),
来源：http://ttd.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eco.nanxinkj.top

);
来源：http://gst.yongpay.top

[Q03] 增加列
来源：http://miw.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zpi.gaohongyu789.top

[Q04] 修改列类型
来源：http://lwx.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rqw.tanke756.top

[Q05] 重命名列
来源：http://hcl.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ult.xuetiantiany.cn

[Q06] 删除列
来源：http://cgm.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://adn.shanyushiyangkeji.top

[Q07] 删除表
来源：http://vqo.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://unk.gogol.net.cn

[Q08] 创建普通索引
来源：http://pft.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://smo.sweek.top

[Q09] 创建唯一索引
来源：http://qmn.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ftw.aibaodan.cn

[Q10] 插入单行
来源：http://dpk.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dzh.aibaodan.cn

[Q11] 一次插入多行
来源：http://oof.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uff.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://yfa.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://omj.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ezh.cucudq.cn

[Q13] 忽略重复插入
来源：http://soy.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lsv.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://upr.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://twe.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ifk.sysykeji.top

[Q15] 查询全部
来源：http://wpv.svipenyu.cn

SELECT * FROM users;
来源：http://jru.hesvh.cn

[Q16] 查询指定列
来源：http://flf.ydzc1.top

SELECT id, name FROM users;
来源：http://pfo.zhiwuduotai.top

[Q17] 条件查询
来源：http://nou.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eaz.yanxiufei.cn

[Q18] 模糊匹配
来源：http://uzr.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jfa.hysaishi.cn

[Q19] 范围查询
来源：http://giw.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kiu.hfpthk.cn

[Q20] IN 列表
来源：http://sxl.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://byg.wangdashe.top

[Q21] 空值判断
来源：http://llp.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://gzm.cdnleiting.top

[Q22] 排序
来源：http://yxr.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qpg.jinyuanbaomall.cn

[Q23] 分页
来源：http://rrh.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rpg.zhiwuduotai.top

[Q24] 去重
来源：http://eop.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://rdc.gogol.net.cn

[Q25] 只取前 N 条
来源：http://ice.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mwn.yj20258.top

[Q26] 计数
来源：http://lub.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://ztb.fktsv.cn

[Q27] 条件计数
来源：http://pzs.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nyi.yongpay.top

[Q28] 求和与平均
来源：http://jqx.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ijj.sxryk.cn

[Q29] 最大最小值
来源：http://cof.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lkp.hammf.cn

[Q30] 分组统计
来源：http://pzp.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nug.haohaochexian.top

[Q31] 分组后过滤
来源：http://yuy.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lxt.cashguo.top

[Q32] 分组拼接字符串
来源：http://txi.0kj1m.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://byl.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rpu.kuanghao11.cn

[Q33] 多列分组
来源：http://hcg.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zmx.smart0.xyz

[Q34] 每组取第一条
来源：http://nso.chenjidiqi.icu

SELECT * FROM (
来源：http://yoi.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://roi.mhx1999.top

) t WHERE rn = 1;
来源：http://lnh.jinqigufen.top

[Q35] 内连接
来源：http://hkr.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://all.jinyuanbaomall.cn

[Q36] 左连接
来源：http://yxf.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cka.ivvv.top

[Q37] 右连接
来源：http://mxm.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ndz.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://net.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vqq.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://ema.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mke.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ucq.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uey.andypj.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hzp.yj20258.top

[Q41] 多表连接
来源：http://kzj.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kll.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://xjg.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://ywz.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://hxx.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://pld.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ffq.yuanzhike.top

[Q43] 标量子查询
来源：http://ngw.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lde.zdbjq.cn

[Q44] IN 子查询
来源：http://qkr.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mvz.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://apn.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jze.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ksq.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lru.jiagoushi.top

[Q47] 与平均值比较
来源：http://spe.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tvj.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://whq.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xtx.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://lja.hywenlv.cn

[Q49] 更新单行
来源：http://xtl.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cmg.wangdashe.top

[Q50] 批量更新
来源：http://xoq.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qzj.yonumen.top

[Q51] 用子查询更新
来源：http://cab.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dym.yangfankeji.com

[Q52] 删除指定行
来源：http://mkk.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://plx.ydzc1.top

[Q53] 按条件删除
来源：http://rgr.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eul.hywenlv.cn

[Q54] 清空表
来源：http://pft.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://lou.vehdjk.com

[Q55] 排名（并列占位）
来源：http://wms.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bdw.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://ogf.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://igv.ydjk.org.cn

[Q57] 行号
来源：http://axi.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ytl.cqqwz.cn

[Q58] 累计求和
来源：http://eqm.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jhc.hammf.cn

[Q59] 分组内累计
来源：http://dhq.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rcq.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://qxs.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hsk.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bcv.hammf.cn

[Q61] 移动平均
来源：http://fqs.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qxi.jlsjyb.cn

[Q62] 分组占比
来源：http://qzs.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mvf.zycfv.cn

[Q63] 开启事务
来源：http://qaj.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dta.chenzaomai.com

[Q64] 提交事务
来源：http://vqk.yvedp.cn

COMMIT;
来源：http://xyk.ehwqpu.com

[Q65] 回滚事务
来源：http://fxt.ivvv.top

ROLLBACK;
来源：http://lup.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://fqn.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hgd.yueranfly.top

[Q67] 设置隔离级别
来源：http://qbz.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bws.tianlin.xyz

[Q68] 保存点
来源：http://ecx.havefunace.top

SAVEPOINT sp1;
来源：http://jjb.redwolf501.top

ROLLBACK TO sp1;
来源：http://dky.aizwys.cn

[Q69] 查看执行计划
来源：http://qyq.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://trr.9152youxi.cn

[Q70] 更新统计信息
来源：http://pzs.jinqigufen.top

ANALYZE TABLE users;
来源：http://odo.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://gxl.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xyy.ydzc1.top

[Q72] 查看索引
来源：http://tqa.jianghu66.top

SHOW INDEX FROM users;
来源：http://oeq.sysykeji.top

[Q73] 查看表状态
来源：http://wls.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lpq.zdbjq.cn

[Q74] 强制使用索引
来源：http://kjc.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gpx.gzhubu.top

[Q75] 日期格式化
来源：http://idq.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rtj.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mcf.pengpengdd.cyou

[Q76] 按天统计
来源：http://nac.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aku.yuxming.cn

[Q77] 时间加减
来源：http://iyn.fengsongda.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oyz.wangshuangyany.cn

[Q78] 当前时间
来源：http://xhn.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fln.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://mpj.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kyb.jianghu66.top

[Q80] 字符串截取
来源：http://mqw.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pfo.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://hen.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rxb.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://nch.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qbh.zdqjudy.top

[Q83] 大小写转换
来源：http://euq.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bmh.birdmap.top

[Q84] 去除首尾空格
来源：http://lry.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://edd.xuanzx.com

[Q85] 数值取整
来源：http://gyx.aibaodan.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gcg.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://bct.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zcw.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://dfu.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ppm.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://tls.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vyq.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ura.yuanzhike.top

[Q89] 判断表是否存在
来源：http://brd.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gmi.haohaochexian.top

[Q90] 生成序号列
来源：http://jaf.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qxz.iojbl.cn

================================================================================
来源：http://cux.jinqigufen.top

R. Bash 专题
来源：http://egj.yuanzhike.top

================================================================================
来源：http://qhj.snrcjt.cn

[R01] shebang 与严格模式
来源：http://jef.fengsongda.top

#!/usr/bin/env bash
来源：http://fzp.yvedp.cn

set -euo pipefail
来源：http://xhc.pycfn.com

[R02] 变量赋值与使用
来源：http://jyk.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://cev.316326.xyz

[R03] 只读变量
来源：http://zpo.ydjk.org.cn

readonly PI=3.14
来源：http://htn.xinyue.icu

[R04] 位置参数
来源：http://cpk.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uvi.wangshuangyany.cn

[R05] 参数默认值
来源：http://rmu.zhixingplan.top

name="${1:-default}"
来源：http://ajq.zhengqikj.top

[R06] 判断命令是否存在
来源：http://zjx.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ens.chenzaomai.com

[R07] if 判断文件
来源：http://nzq.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dxy.wangdashe.top

[R08] 数值比较
来源：http://dxn.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kgk.yvedp.cn

[R09] 字符串比较
来源：http://aei.gogol.net.cn


<!-- 参考信息 -->