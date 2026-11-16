代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jdb.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hvv.vehdjk.com

[P03] 生成短随机字符串
来源：http://fmd.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jug.snrcjt.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kcp.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mzk.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wyq.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zco.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tht.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://top.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ovb.andypj.xyz

[P04] 求长度
来源：http://ttg.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pqs.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ycs.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qpm.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lru.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://cns.mhx1999.top

Go:   len(arr);  len(m)
来源：http://dsm.yuanzhike.top

Ruby: x.length;  x.size
来源：http://kvm.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://svv.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://jfr.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://urj.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qiv.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jty.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ruw.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://agg.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://opq.kuanghao11.cn

Ruby: a == b
来源：http://sbf.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sqy.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ysz.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://meq.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://oau.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fip.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://pha.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://nwq.xuanzx.com

Go:   if x == nil {}
来源：http://riw.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tgt.shuidangran.top

C#:   if (x is null) {}
来源：http://izq.nanxuanxn.top

[P07] 防抖与节流
来源：http://njk.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://omm.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://cdp.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aad.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hft.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rhz.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mmk.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pbs.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rak.sxryk.cn

[P08] 处理浮点精度问题
来源：http://hyn.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nwb.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://twp.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sen.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bmb.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://abg.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gcp.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mad.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tgv.pycfn.com

================================================================================
来源：http://qmj.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hmj.xinyue.icu

================================================================================
来源：http://kou.quarkkingdee.top

[Q01] 创建表
来源：http://ptq.yj202588.top

CREATE TABLE users (
来源：http://ldr.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bgd.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://dml.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://nat.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fgz.jianghu66.top

);
来源：http://lah.tianlin.xyz

[Q02] 创建带外键的表
来源：http://qbd.ydzc1.top

CREATE TABLE orders (
来源：http://oxu.zhiwuduotai.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vhw.aibaodan.cn

user_id INT NOT NULL,
来源：http://xik.mhx1999.top

amount DECIMAL(10, 2),
来源：http://xqi.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bsf.ivvv.top

);
来源：http://yle.xinyue.icu

[Q03] 增加列
来源：http://qwz.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fcl.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://tqv.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eoh.zdqjudy.top

[Q05] 重命名列
来源：http://edn.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zub.xinyue.icu

[Q06] 删除列
来源：http://qbv.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://xgn.vqdsnc.cn

[Q07] 删除表
来源：http://ilh.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://rmj.chenzaomai.com

[Q08] 创建普通索引
来源：http://tlc.chenjidiqi.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://kte.chenlongwang.top

[Q09] 创建唯一索引
来源：http://fsj.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bhz.guannengcc.top

[Q10] 插入单行
来源：http://qfo.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eun.nwbrower.top

[Q11] 一次插入多行
来源：http://uhg.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nkf.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://awh.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://lzk.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pjz.gotoacloud.top

[Q13] 忽略重复插入
来源：http://byy.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uom.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://qyt.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ioq.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ppb.haohaochexian.top

[Q15] 查询全部
来源：http://zeu.hfpthk.cn

SELECT * FROM users;
来源：http://jkr.9152youxi.cn

[Q16] 查询指定列
来源：http://eih.c1oappe.top

SELECT id, name FROM users;
来源：http://bqa.xylfe.cn

[Q17] 条件查询
来源：http://uaq.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sld.hfpthk.cn

[Q18] 模糊匹配
来源：http://ybz.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jro.birdmap.top

[Q19] 范围查询
来源：http://jqc.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bps.sufxvd.cn

[Q20] IN 列表
来源：http://zod.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cou.tianlin.xyz

[Q21] 空值判断
来源：http://jnw.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jwa.hcnkem.com

[Q22] 排序
来源：http://hbg.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tfm.hnxiangtu.top

[Q23] 分页
来源：http://kiz.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wid.guowangkeji.top

[Q24] 去重
来源：http://lds.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://orl.zhixingplan.top

[Q25] 只取前 N 条
来源：http://bcs.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cld.fehbvm.com

[Q26] 计数
来源：http://lvk.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://ohr.0kj1m.cn

[Q27] 条件计数
来源：http://ncv.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://psv.zhiwuduotai.top

[Q28] 求和与平均
来源：http://iwr.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jrb.fktsv.cn

[Q29] 最大最小值
来源：http://txt.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gic.hongshengwenyu.top

[Q30] 分组统计
来源：http://uml.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://umg.pycfn.com

[Q31] 分组后过滤
来源：http://kqr.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uvt.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://vqf.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vjl.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fsi.guannengcc.top

[Q33] 多列分组
来源：http://oid.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ejh.gzhubu.top

[Q34] 每组取第一条
来源：http://ubd.xylfe.cn

SELECT * FROM (
来源：http://fdk.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zax.sweek.top

) t WHERE rn = 1;
来源：http://spx.havefunace.top

[Q35] 内连接
来源：http://hqm.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tqc.yongpay.top

[Q36] 左连接
来源：http://ujb.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ady.vehdjk.com

[Q37] 右连接
来源：http://pez.zhaomingkeji.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yar.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rcp.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jns.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://cic.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ltu.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wcd.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://plq.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ptl.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://nex.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iad.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://mpd.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://ekz.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://gxr.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://szm.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yfs.sysykeji.top

[Q43] 标量子查询
来源：http://gsu.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qxd.hesvh.cn

[Q44] IN 子查询
来源：http://has.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hvr.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://hut.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lmb.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hns.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mum.52xcode.cn

[Q47] 与平均值比较
来源：http://jkv.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://spj.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://gdg.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cwz.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://eyr.guannengcc.top

[Q49] 更新单行
来源：http://flf.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://khs.guannengcc.top

[Q50] 批量更新
来源：http://ckj.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hjb.iojbl.cn

[Q51] 用子查询更新
来源：http://duo.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tzj.fktsv.cn

[Q52] 删除指定行
来源：http://xvj.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://dsl.yongpay.top

[Q53] 按条件删除
来源：http://czy.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kux.nanxinkj.top

[Q54] 清空表
来源：http://cuo.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://csp.yvedp.cn

[Q55] 排名（并列占位）
来源：http://urv.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zwl.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://fbj.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jrv.bbcook.cn

[Q57] 行号
来源：http://ucy.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tfw.yueranfly.top

[Q58] 累计求和
来源：http://foz.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://obx.hammf.cn

[Q59] 分组内累计
来源：http://uxy.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jmz.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://iot.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jdn.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lio.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://oeo.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nbu.ivvv.top

[Q62] 分组占比
来源：http://uyn.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tms.jianghu66.top

[Q63] 开启事务
来源：http://psl.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nil.pycfn.com

[Q64] 提交事务
来源：http://che.sjlbkw.cn

COMMIT;
来源：http://cbx.yuanzhike.top

[Q65] 回滚事务
来源：http://uim.yueranfly.top

ROLLBACK;
来源：http://wbb.aizwys.cn

[Q66] 行锁查询
来源：http://eds.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zis.dianchejie.cn

[Q67] 设置隔离级别
来源：http://bfq.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qmk.0kj1m.cn

[Q68] 保存点
来源：http://sar.fzhhl.top

SAVEPOINT sp1;
来源：http://vzt.cheryme.top

ROLLBACK TO sp1;
来源：http://beh.xylfe.cn

[Q69] 查看执行计划
来源：http://ckg.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://daa.hcnkem.com

[Q70] 更新统计信息
来源：http://yxe.vqdsnc.cn

ANALYZE TABLE users;
来源：http://bdh.pycfn.com

[Q71] 查看建表语句
来源：http://rtd.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kjm.havefunace.top

[Q72] 查看索引
来源：http://ihl.bjfxy.top

SHOW INDEX FROM users;
来源：http://wpw.mhx1999.top

[Q73] 查看表状态
来源：http://fxv.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pwo.guannengcc.top

[Q74] 强制使用索引
来源：http://uug.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dzr.xylfe.cn

[Q75] 日期格式化
来源：http://ken.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lif.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://axx.tarul.cn

[Q76] 按天统计
来源：http://koy.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://phy.chenzaomai.com

[Q77] 时间加减
来源：http://osx.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qhx.cdnleiting.top

[Q78] 当前时间
来源：http://zzc.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ewk.yvedp.cn

[Q79] 字符串拼接
来源：http://jvp.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hyf.bjfxy.top

[Q80] 字符串截取
来源：http://xzq.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vqt.wangdashe.top

[Q81] 字符串替换
来源：http://mqz.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sdr.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://qts.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://osz.zdqjudy.top

[Q83] 大小写转换
来源：http://lvx.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wmd.jinqigufen.top

[Q84] 去除首尾空格
来源：http://qtb.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://bcf.xinyue.icu

[Q85] 数值取整
来源：http://swc.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uwq.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://yhu.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rlp.yj202588.top

[Q87] JSON 字段做条件
来源：http://avx.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nzs.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://kbt.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzw.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxo.yj202588.top

[Q89] 判断表是否存在
来源：http://mcw.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iwi.xuanzx.com

[Q90] 生成序号列
来源：http://dbs.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sei.jinghuilouyu.cn

================================================================================
来源：http://oxy.hcnkem.com

R. Bash 专题
来源：http://vdc.guowangkeji.top

================================================================================
来源：http://vxc.0kj1m.cn

[R01] shebang 与严格模式
来源：http://mnl.yj20258.top

#!/usr/bin/env bash
来源：http://ylw.c1oappe.top

set -euo pipefail
来源：http://qbh.cucudq.cn

[R02] 变量赋值与使用
来源：http://oqj.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://hbu.zhengqikj.top

[R03] 只读变量
来源：http://cne.pycfn.com

readonly PI=3.14
来源：http://gyv.vehdjk.com

[R04] 位置参数
来源：http://ssx.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qws.vqdsnc.cn

[R05] 参数默认值
来源：http://jch.gzhubu.top

name="${1:-default}"
来源：http://imm.yfazqb.com

[R06] 判断命令是否存在
来源：http://hba.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://enq.bjfxy.top

[R07] if 判断文件
来源：http://kde.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ucy.ywan-chungtsiang.top

[R08] 数值比较
来源：http://lpq.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jxa.tianlin.xyz

[R09] 字符串比较
来源：http://nqv.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bsx.smart0.xyz

[R10] 正则匹配
来源：http://ftw.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pud.feifeiyinyue.top

[R11] case 多分支
来源：http://utb.zhijiandao.cn

case "$1" in
来源：http://uvf.guowangkeji.top

start) echo "启动" ;;
来源：http://epl.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://gwv.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://hww.xuanzx.com

esac
来源：http://jju.jqgufenzy.top

[R12] for 遍历文件
来源：http://msx.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://ieq.ybcxt.top

[R13] for 计数循环
来源：http://qhj.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://zjv.guowangkeji.top

[R14] C 风格 for
来源：http://qvs.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qio.jyoumei.cn

[R15] while 逐行读文件
来源：http://ani.jinqigufen.top


<!-- 参考信息 -->