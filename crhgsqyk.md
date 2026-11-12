代发 wailian999

[P01] 生成 UUID
来源：http://scq.cashguo.top

Py:   str(uuid.uuid4())
来源：http://ewe.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jdc.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://lpi.zhiwuduotai.top

TS:   crypto.randomUUID()
来源：http://yud.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://wpd.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://ldg.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://czk.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://ftk.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://fqz.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uyd.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fcd.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xkg.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vlc.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jav.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cqi.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blk.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fkw.tanke756.top

[P03] 生成短随机字符串
来源：http://kag.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qml.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ibl.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://odi.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jlm.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mpx.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lgz.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xiv.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ckm.zhiwuduotai.top

[P04] 求长度
来源：http://ozl.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pbw.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbc.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rob.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ddl.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://jnn.hnqzz.top

Go:   len(arr);  len(m)
来源：http://wus.jyoumei.cn

Ruby: x.length;  x.size
来源：http://trz.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mmu.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://hzz.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://usp.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iom.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dzz.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gek.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bul.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://twe.aizwys.cn

Ruby: a == b
来源：http://mfq.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xsc.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mfw.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kqn.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://aqr.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tph.hcnkem.com

TS:   if (x == null) {}
来源：http://shc.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://nxb.gogol.net.cn

Go:   if x == nil {}
来源：http://jsu.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ioe.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://prb.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://bba.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://asd.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://vvj.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bym.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqc.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kvo.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dkz.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://tzo.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oyi.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://sad.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gqt.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gvx.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ozo.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cfw.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://shd.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vxp.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uap.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nln.zhoulong.xyz

================================================================================
来源：http://bau.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rwg.sjlbkw.cn

================================================================================
来源：http://cmg.jlsjyb.cn

[Q01] 创建表
来源：http://xbd.yonumen.top

CREATE TABLE users (
来源：http://jas.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wtz.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://hvm.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://nok.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rtb.pycfn.com

);
来源：http://won.hammf.cn

[Q02] 创建带外键的表
来源：http://mwt.nanxuanxn.top

CREATE TABLE orders (
来源：http://yjq.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gfk.0kj1m.cn

user_id INT NOT NULL,
来源：http://odo.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://zik.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tdj.yangfankeji.com

);
来源：http://khz.hysaishi.cn

[Q03] 增加列
来源：http://hta.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://psx.svipenyu.cn

[Q04] 修改列类型
来源：http://fyz.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://spw.nanxinkj.top

[Q05] 重命名列
来源：http://hbb.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ath.zdqjudy.top

[Q06] 删除列
来源：http://nyj.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://dbr.jinyuanbaomall.cn

[Q07] 删除表
来源：http://rpt.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://tzg.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://nqr.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rol.nanxinkj.top

[Q09] 创建唯一索引
来源：http://hxx.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lwj.wangdashe.top

[Q10] 插入单行
来源：http://xol.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qcw.smart0.xyz

[Q11] 一次插入多行
来源：http://nqi.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gcf.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://zix.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://oke.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sxp.0kj1m.cn

[Q13] 忽略重复插入
来源：http://ybb.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mmn.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://kfl.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ged.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iud.cheryme.top

[Q15] 查询全部
来源：http://wjr.zycfv.cn

SELECT * FROM users;
来源：http://ibo.uphjek.com

[Q16] 查询指定列
来源：http://jcd.sxryk.cn

SELECT id, name FROM users;
来源：http://ths.fengsongda.top

[Q17] 条件查询
来源：http://quz.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://izz.zdbjq.cn

[Q18] 模糊匹配
来源：http://ogn.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rwm.yongpay.top

[Q19] 范围查询
来源：http://qxv.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uug.daxiang520.top

[Q20] IN 列表
来源：http://toq.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://txx.guannengcc.top

[Q21] 空值判断
来源：http://ray.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ggu.jlsjyb.cn

[Q22] 排序
来源：http://sae.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qyd.fengsongda.top

[Q23] 分页
来源：http://wuk.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mlp.jinghuilouyu.cn

[Q24] 去重
来源：http://chh.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://qzt.sweek.top

[Q25] 只取前 N 条
来源：http://lab.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jyx.cqqwz.cn

[Q26] 计数
来源：http://esf.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://vuq.wangdashe.top

[Q27] 条件计数
来源：http://nfd.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://llo.havefunace.top

[Q28] 求和与平均
来源：http://svk.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hnx.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://rzq.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hny.andypj.xyz

[Q30] 分组统计
来源：http://qfc.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cpl.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://pil.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfv.yj20258.top

[Q32] 分组拼接字符串
来源：http://wku.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oqg.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wlg.fzhhl.top

[Q33] 多列分组
来源：http://odk.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qqs.jiagoushi.top

[Q34] 每组取第一条
来源：http://xqw.andypj.xyz

SELECT * FROM (
来源：http://czo.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jfr.sufxvd.cn

) t WHERE rn = 1;
来源：http://nco.sysykeji.top

[Q35] 内连接
来源：http://vsv.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aco.hesvh.cn

[Q36] 左连接
来源：http://cmp.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wnw.hongshengwenyu.top

[Q37] 右连接
来源：http://jxp.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pbk.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://rip.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gdz.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://pjg.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://kjw.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fan.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wsi.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mfe.andypj.xyz

[Q41] 多表连接
来源：http://vnr.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xhj.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://kgb.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://cma.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://xjc.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://jmp.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbo.pengpengdd.cyou

[Q43] 标量子查询
来源：http://mkc.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tez.hesvh.cn

[Q44] IN 子查询
来源：http://fyo.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yre.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://dof.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://naa.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://mwi.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://apu.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://ruk.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ggx.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://xgv.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hst.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://dyw.yvedp.cn

[Q49] 更新单行
来源：http://tcn.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://emr.shangyingyoupin.top

[Q50] 批量更新
来源：http://hid.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sry.cqqwz.cn

[Q51] 用子查询更新
来源：http://rlx.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fgh.tianlin.xyz

[Q52] 删除指定行
来源：http://rky.svipenyu.cn

DELETE FROM users WHERE id = 10;
来源：http://xtk.cheryme.top

[Q53] 按条件删除
来源：http://whi.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wsf.zhengqikj.top

[Q54] 清空表
来源：http://cwe.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://jwm.hcnkem.com

[Q55] 排名（并列占位）
来源：http://rly.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rjx.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://kaw.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iwv.shanyushiyangkeji.top

[Q57] 行号
来源：http://ueb.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://atz.vehdjk.com

[Q58] 累计求和
来源：http://yfr.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://poo.cheryme.top

[Q59] 分组内累计
来源：http://gfr.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mye.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://jct.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pkf.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bfp.hammf.cn

[Q61] 移动平均
来源：http://toy.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vcz.cheryme.top

[Q62] 分组占比
来源：http://nif.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://urg.xziqi.cn

[Q63] 开启事务
来源：http://qzc.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qof.wangdashe.top

[Q64] 提交事务
来源：http://gcc.ehwqpu.com

COMMIT;
来源：http://lmh.zhengqikj.top

[Q65] 回滚事务
来源：http://suy.tianlin.xyz

ROLLBACK;
来源：http://fkn.yueranfly.top

[Q66] 行锁查询
来源：http://kpv.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qzc.52xcode.cn

[Q67] 设置隔离级别
来源：http://tzv.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cdh.jinqigufen.top

[Q68] 保存点
来源：http://smg.vqdsnc.cn

SAVEPOINT sp1;
来源：http://ksw.shuidangran.top

ROLLBACK TO sp1;
来源：http://epv.yj20258888.top

[Q69] 查看执行计划
来源：http://jxe.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zpq.xziqi.cn

[Q70] 更新统计信息
来源：http://qlg.yfazqb.com

ANALYZE TABLE users;
来源：http://ghr.hysaishi.cn

[Q71] 查看建表语句
来源：http://yjy.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mav.9152youxi.cn

[Q72] 查看索引
来源：http://frh.cdnleiting.top

SHOW INDEX FROM users;
来源：http://dcf.yanxiufei.cn

[Q73] 查看表状态
来源：http://ugf.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oqi.iojbl.cn

[Q74] 强制使用索引
来源：http://vpx.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://the.hongshengwenyu.top

[Q75] 日期格式化
来源：http://yoq.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iuz.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yxf.svipenyu.cn

[Q76] 按天统计
来源：http://nxi.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wvu.wangshuangyany.cn

[Q77] 时间加减
来源：http://lpk.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ukr.jianghu66.top

[Q78] 当前时间
来源：http://ixj.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifk.dashuyun.cn

[Q79] 字符串拼接
来源：http://ypa.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uav.tanke756.top

[Q80] 字符串截取
来源：http://xub.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sri.hesvh.cn

[Q81] 字符串替换
来源：http://lcn.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://idd.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://fcu.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njf.zhengqikj.top

[Q83] 大小写转换
来源：http://puh.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sfi.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://dvo.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://byz.hywenlv.cn

[Q85] 数值取整
来源：http://ejr.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fqt.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://lyl.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xwu.vehdjk.com

[Q87] JSON 字段做条件
来源：http://gcu.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lch.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://yum.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cnu.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wgo.fzhhl.top

[Q89] 判断表是否存在
来源：http://syb.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ltc.jiagoushi.top

[Q90] 生成序号列
来源：http://jyd.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zgm.shanyushiyangtech.top

================================================================================
来源：http://cvf.smart0.xyz

R. Bash 专题
来源：http://zlf.ydjk.org.cn

================================================================================
来源：http://sfg.hysaishi.cn

[R01] shebang 与严格模式
来源：http://zte.tarul.cn

#!/usr/bin/env bash
来源：http://ktf.xinyue.icu

set -euo pipefail
来源：http://mya.ybcxt.top

[R02] 变量赋值与使用
来源：http://ylj.zhengqikj.top

name="Tom"; echo "$name"
来源：http://twf.xylfe.cn

[R03] 只读变量
来源：http://bgd.havefunace.top

readonly PI=3.14
来源：http://tjq.redwolf501.top

[R04] 位置参数
来源：http://lar.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qdk.gogol.net.cn

[R05] 参数默认值
来源：http://vhz.tian-w.cn

name="${1:-default}"
来源：http://fvs.mhx1999.top

[R06] 判断命令是否存在
来源：http://pwl.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eea.cqqwz.cn

[R07] if 判断文件
来源：http://txu.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hom.snrcjt.cn

[R08] 数值比较
来源：http://awv.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jnp.yj202588.top

[R09] 字符串比较
来源：http://gio.ctjpmb.com


<!-- 参考信息 -->