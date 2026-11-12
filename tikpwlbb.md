代发 wailian999

TS:   crypto.randomUUID()
来源：http://ptb.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://utj.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://uvr.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://nyh.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ezt.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://oqg.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dmy.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xet.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ieo.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vhm.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sok.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hed.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hgq.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qex.fzhhl.top

[P03] 生成短随机字符串
来源：http://mbt.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xyi.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xqz.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jeu.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqj.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fza.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xev.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jxb.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://stg.jqgfzy.top

[P04] 求长度
来源：http://xlz.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ynd.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sfg.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://clf.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pal.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://elc.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://fbq.jyoumei.cn

Ruby: x.length;  x.size
来源：http://fan.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zkj.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://eki.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mfm.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jnb.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xed.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vci.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sag.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://bvy.shanyushiyangtech.top

Ruby: a == b
来源：http://plm.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rbp.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ymg.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wig.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://els.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iez.fktsv.cn

TS:   if (x == null) {}
来源：http://jdi.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ifc.cheryme.top

Go:   if x == nil {}
来源：http://idz.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jue.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://hbt.fzhhl.top

[P07] 防抖与节流
来源：http://cru.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ycd.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://dpu.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ccc.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sth.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kpc.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ryk.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pbm.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nxe.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://ezw.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pnx.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dco.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wbz.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bhf.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mqu.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pic.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://apo.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dme.pycfn.com

================================================================================
来源：http://ufz.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://glz.sxryk.cn

================================================================================
来源：http://gxg.fehbvm.com

[Q01] 创建表
来源：http://coj.haohaochexian.top

CREATE TABLE users (
来源：http://eks.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eyc.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://ifp.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://wts.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fwv.ctjpmb.com

);
来源：http://vpc.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://bta.kuanghao11.cn

CREATE TABLE orders (
来源：http://zrd.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ecc.daria6918.cn

user_id INT NOT NULL,
来源：http://hfz.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://esn.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tla.jqgufenzy.top

);
来源：http://psr.cdnleiting.top

[Q03] 增加列
来源：http://vdk.zhengqikj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ahu.dashuyun.cn

[Q04] 修改列类型
来源：http://fky.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmt.yanxiufei.cn

[Q05] 重命名列
来源：http://kya.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ebb.shanyushiyangtech.top

[Q06] 删除列
来源：http://www.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://hiz.yj202588.top

[Q07] 删除表
来源：http://owa.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://dmp.wangdashe.top

[Q08] 创建普通索引
来源：http://kbn.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://njf.c1oappe.top

[Q09] 创建唯一索引
来源：http://bfw.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kja.snrcjt.cn

[Q10] 插入单行
来源：http://rqe.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mhw.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://ueg.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://our.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://asj.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://kzc.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bgu.guowangkeji.top

[Q13] 忽略重复插入
来源：http://zui.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rhd.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://miz.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fly.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ieh.cdnleiting.top

[Q15] 查询全部
来源：http://dmy.iojbl.cn

SELECT * FROM users;
来源：http://ckk.yj20258.top

[Q16] 查询指定列
来源：http://zke.andypj.xyz

SELECT id, name FROM users;
来源：http://geg.sweek.top

[Q17] 条件查询
来源：http://msp.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://orw.vqdsnc.cn

[Q18] 模糊匹配
来源：http://wic.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ckd.jqgufenzy.top

[Q19] 范围查询
来源：http://qxk.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jko.jqgfzy.top

[Q20] IN 列表
来源：http://gsc.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wfs.haohaochexian.top

[Q21] 空值判断
来源：http://hym.jinghuilouyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jcq.9152youxi.cn

[Q22] 排序
来源：http://zzh.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iaq.xuetiantiany.cn

[Q23] 分页
来源：http://hqh.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pfl.haohaochexian.top

[Q24] 去重
来源：http://kyp.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://fpr.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://uqz.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xur.daria6918.cn

[Q26] 计数
来源：http://bnv.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://ivt.nanxuanxn.top

[Q27] 条件计数
来源：http://ibh.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://adm.nanxuanxn.top

[Q28] 求和与平均
来源：http://hsl.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rxn.iojbl.cn

[Q29] 最大最小值
来源：http://jfm.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hev.xuanzx.com

[Q30] 分组统计
来源：http://xuy.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://evx.zhixingplan.top

[Q31] 分组后过滤
来源：http://iek.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qdr.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://gtu.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ebc.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qwi.hcnkem.com

[Q33] 多列分组
来源：http://uga.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vyp.meibo888.top

[Q34] 每组取第一条
来源：http://shp.vqdsnc.cn

SELECT * FROM (
来源：http://wue.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nsd.aizwys.cn

) t WHERE rn = 1;
来源：http://qad.cdnleiting.top

[Q35] 内连接
来源：http://lzu.feifeiyinyue.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lbp.svipenyu.cn

[Q36] 左连接
来源：http://hfm.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bbh.fehbvm.com

[Q37] 右连接
来源：http://bov.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dai.vehdjk.com

[Q38] 全外连接（PostgreSQL）
来源：http://uuf.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fcl.yongpay.top

[Q39] 自连接（查上下级）
来源：http://bch.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zkz.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ovs.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ojm.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ldn.cheryme.top

[Q41] 多表连接
来源：http://zbd.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bor.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://qhx.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://aor.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://uac.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://sal.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eml.ybcxt.top

[Q43] 标量子查询
来源：http://meu.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://evt.iojbl.cn

[Q44] IN 子查询
来源：http://jjs.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xeu.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://rko.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nuy.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fzu.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nut.yuxming.cn

[Q47] 与平均值比较
来源：http://tcj.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sce.tarul.cn

[Q48] CTE 公用表表达式
来源：http://osp.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://llm.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://ncz.pycfn.com

[Q49] 更新单行
来源：http://jty.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mkj.ybcxt.top

[Q50] 批量更新
来源：http://qgw.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wod.jqgfzy.top

[Q51] 用子查询更新
来源：http://rzv.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ugs.redwolf501.top

[Q52] 删除指定行
来源：http://bqd.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://kxw.xziqi.cn

[Q53] 按条件删除
来源：http://tqr.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://coj.meibo888.top

[Q54] 清空表
来源：http://lta.bbcook.cn

TRUNCATE TABLE logs;
来源：http://ppb.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://psz.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ppi.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://rdb.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zmk.jinqigufen.top

[Q57] 行号
来源：http://kxi.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eby.redwolf501.top

[Q58] 累计求和
来源：http://ngg.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxc.daxiang520.top

[Q59] 分组内累计
来源：http://etf.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hof.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://izo.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rjw.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ggi.sxryk.cn

[Q61] 移动平均
来源：http://owd.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rqs.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://emo.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://obt.daxiang520.top

[Q63] 开启事务
来源：http://etj.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://gzh.jqgfzy.top

[Q64] 提交事务
来源：http://idi.zhaomingkeji.xyz

COMMIT;
来源：http://vsy.vqdsnc.cn

[Q65] 回滚事务
来源：http://arm.jinqigufen.top

ROLLBACK;
来源：http://zjk.kuanghao11.cn

[Q66] 行锁查询
来源：http://jtp.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eeb.hysaishi.cn

[Q67] 设置隔离级别
来源：http://pvh.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mfk.aizwys.cn

[Q68] 保存点
来源：http://qid.jqgufenzy.top

SAVEPOINT sp1;
来源：http://qer.shuidangran.top

ROLLBACK TO sp1;
来源：http://gid.yueranfly.top

[Q69] 查看执行计划
来源：http://hns.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qwr.9152youxi.cn

[Q70] 更新统计信息
来源：http://guk.52xcode.cn

ANALYZE TABLE users;
来源：http://wiu.jyoumei.cn

[Q71] 查看建表语句
来源：http://mil.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qzo.yvedp.cn

[Q72] 查看索引
来源：http://hav.zhixingplan.top

SHOW INDEX FROM users;
来源：http://ici.hnqzz.top

[Q73] 查看表状态
来源：http://fnv.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sry.cashguo.top

[Q74] 强制使用索引
来源：http://ibx.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wqq.tarul.cn

[Q75] 日期格式化
来源：http://ucb.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eil.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tjm.sweek.top

[Q76] 按天统计
来源：http://tdt.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hvf.dianchejie.cn

[Q77] 时间加减
来源：http://wel.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vto.chenzaomai.com

[Q78] 当前时间
来源：http://sth.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://glf.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://dds.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mxq.guannengcc.top

[Q80] 字符串截取
来源：http://yue.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hbv.vqdsnc.cn

[Q81] 字符串替换
来源：http://mbz.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qef.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://hwj.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://phl.fktsv.cn

[Q83] 大小写转换
来源：http://crd.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kfm.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://zps.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://kyd.xuetiantiany.cn

[Q85] 数值取整
来源：http://qrz.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iqt.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://xcp.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://phv.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://buq.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hnz.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://peg.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vyc.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aev.dianchejie.cn

[Q89] 判断表是否存在
来源：http://clt.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pez.quarkkingdee.top

[Q90] 生成序号列
来源：http://tus.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hji.yuanzhike.top

================================================================================
来源：http://xjv.quarkkingdee.top

R. Bash 专题
来源：http://mzk.gzhubu.top

================================================================================
来源：http://lva.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://rjs.zhongyouzk.top

#!/usr/bin/env bash
来源：http://xqc.dianchejie.cn

set -euo pipefail
来源：http://nrl.sufxvd.cn

[R02] 变量赋值与使用
来源：http://yjd.yj20258888.top

name="Tom"; echo "$name"
来源：http://deq.ivvv.top

[R03] 只读变量
来源：http://bfw.gotoacloud.top

readonly PI=3.14
来源：http://muj.yj20258888.top

[R04] 位置参数
来源：http://sgv.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ryq.yvedp.cn

[R05] 参数默认值
来源：http://lab.smart0.xyz

name="${1:-default}"
来源：http://bjq.tian-w.cn

[R06] 判断命令是否存在
来源：http://mil.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rjt.jqgufenzy.top

[R07] if 判断文件
来源：http://teg.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rou.dianchejie.cn

[R08] 数值比较
来源：http://ycy.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://pbc.jqgufenzy.top

[R09] 字符串比较
来源：http://kvf.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ljh.xziqi.cn

[R10] 正则匹配
来源：http://hoq.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dxh.jianghu66.top

[R11] case 多分支
来源：http://siq.shuidangran.top


<!-- 参考信息 -->