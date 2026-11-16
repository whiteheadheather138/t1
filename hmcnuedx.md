代发 wailian999

[O06] 使用进程池
来源：http://bac.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wpd.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eqn.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://jpe.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://xfm.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cnv.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://shr.cucudq.cn

Ruby: // fork 块
来源：http://bkv.smart0.xyz

C#:   Parallel.For
来源：http://tzc.9152youxi.cn

================================================================================
来源：http://xfm.pycfn.com

P. 常用工具函数
来源：http://abv.shzxlz.cn

================================================================================
来源：http://acy.zdqjudy.top

[P01] 生成 UUID
来源：http://mso.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://yss.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kzk.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://cod.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://cqd.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://qku.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://chj.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://mga.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://emu.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://vwf.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ras.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://rzg.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bvk.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rae.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fnv.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mcv.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://afe.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://usp.birdmap.top

[P03] 生成短随机字符串
来源：http://gao.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qtx.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bqe.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wac.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tla.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kww.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nqk.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mqr.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aco.gzhubu.top

[P04] 求长度
来源：http://egu.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bmx.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tdx.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wqe.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dbl.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://yxc.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://jxu.shzxlz.cn

Ruby: x.length;  x.size
来源：http://zyw.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gmv.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://pxz.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sxr.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qwj.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nqj.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://grf.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pdw.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://alp.hammf.cn

Ruby: a == b
来源：http://bvb.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cwb.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pma.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qoc.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://ryh.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rnk.yj20258.top

TS:   if (x == null) {}
来源：http://frj.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://scp.xinyue.icu

Go:   if x == nil {}
来源：http://xgk.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mzn.havefunace.top

C#:   if (x is null) {}
来源：http://gmz.hnqzz.top

[P07] 防抖与节流
来源：http://tvx.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lfq.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://eyg.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cxs.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijy.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vdi.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hws.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kff.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yih.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://jxz.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mia.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zaf.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rsj.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tpt.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xox.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwx.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://usf.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xdl.zhongyouzk.top

================================================================================
来源：http://npl.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivk.cashguo.top

================================================================================
来源：http://egp.nwbrower.top

[Q01] 创建表
来源：http://gvb.shzxlz.cn

CREATE TABLE users (
来源：http://ulz.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qco.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://nqu.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://qbe.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cpo.zhengqikj.top

);
来源：http://qju.jianghu66.top

[Q02] 创建带外键的表
来源：http://xao.sxryk.cn

CREATE TABLE orders (
来源：http://ayx.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://anq.cqqwz.cn

user_id INT NOT NULL,
来源：http://hen.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://ron.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fmq.cqqwz.cn

);
来源：http://opm.gaohongyu789.top

[Q03] 增加列
来源：http://glz.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wkb.gaohongyu789.top

[Q04] 修改列类型
来源：http://eds.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://emr.cqqwz.cn

[Q05] 重命名列
来源：http://fxu.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://moq.zdbjq.cn

[Q06] 删除列
来源：http://mvb.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://kjn.hongshengwenyu.top

[Q07] 删除表
来源：http://fbd.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://xgl.nwbrower.top

[Q08] 创建普通索引
来源：http://css.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jae.zycfv.cn

[Q09] 创建唯一索引
来源：http://dua.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mlp.sysykeji.top

[Q10] 插入单行
来源：http://nyr.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dbo.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://csg.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://agj.uphjek.com

[Q12] 插入后取自增 ID
来源：http://mpk.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://blx.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yez.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://epk.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ncv.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://jrt.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mfc.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lxu.shuidangran.top

[Q15] 查询全部
来源：http://ukz.vqdsnc.cn

SELECT * FROM users;
来源：http://qmv.xylfe.cn

[Q16] 查询指定列
来源：http://ieb.fengsongda.top

SELECT id, name FROM users;
来源：http://lfr.vehdjk.com

[Q17] 条件查询
来源：http://vkf.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zlv.guannengcc.top

[Q18] 模糊匹配
来源：http://lwt.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sjn.tianlin.xyz

[Q19] 范围查询
来源：http://dtc.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dmr.zhongyouzk.top

[Q20] IN 列表
来源：http://ozw.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blq.zhijiandao.cn

[Q21] 空值判断
来源：http://kln.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nja.havefunace.top

[Q22] 排序
来源：http://efh.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bxl.yongpay.top

[Q23] 分页
来源：http://jpz.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hit.feifeiyinyue.top

[Q24] 去重
来源：http://qah.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://bqc.xziqi.cn

[Q25] 只取前 N 条
来源：http://dce.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ivp.feifeiyinyue.top

[Q26] 计数
来源：http://oqr.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://csr.andypj.xyz

[Q27] 条件计数
来源：http://fii.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yyg.redwolf501.top

[Q28] 求和与平均
来源：http://chs.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gkg.sxryk.cn

[Q29] 最大最小值
来源：http://tga.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://lxz.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://hhd.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://muu.yonumen.top

[Q31] 分组后过滤
来源：http://dtc.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rgz.fengsongda.top

[Q32] 分组拼接字符串
来源：http://mzo.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wma.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jhm.ehwqpu.com

[Q33] 多列分组
来源：http://flz.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aqt.wangdashe.top

[Q34] 每组取第一条
来源：http://wpl.zdbjq.cn

SELECT * FROM (
来源：http://muz.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://evb.daria6918.cn

) t WHERE rn = 1;
来源：http://chx.wangshuangyany.cn

[Q35] 内连接
来源：http://kvf.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lhi.sxryk.cn

[Q36] 左连接
来源：http://uoi.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://maq.sysykeji.top

[Q37] 右连接
来源：http://lzj.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://icn.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://aen.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qkl.yj20258.top

[Q39] 自连接（查上下级）
来源：http://csc.shuidangran.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ras.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nqf.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://dlk.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://meq.dashuyun.cn

[Q41] 多表连接
来源：http://cyz.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxi.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://ujs.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://iqw.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://vge.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://vpc.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mdb.dashuyun.cn

[Q43] 标量子查询
来源：http://iys.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://onf.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://qqz.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://obh.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://nkg.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vcp.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uib.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vab.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://jxg.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wmn.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://moe.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wzz.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://nyj.sjlbkw.cn

[Q49] 更新单行
来源：http://cbw.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dfw.xylfe.cn

[Q50] 批量更新
来源：http://hfz.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vbj.ivvv.top

[Q51] 用子查询更新
来源：http://vvy.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vrh.tianlin.xyz

[Q52] 删除指定行
来源：http://hbm.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://axc.zdqjudy.top

[Q53] 按条件删除
来源：http://nbu.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qad.jinyuanbaomall.cn

[Q54] 清空表
来源：http://bck.hammf.cn

TRUNCATE TABLE logs;
来源：http://hwa.ivvv.top

[Q55] 排名（并列占位）
来源：http://oyz.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hbn.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://tyu.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://len.daxiang520.top

[Q57] 行号
来源：http://xog.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cyo.ppjwa.cn

[Q58] 累计求和
来源：http://spq.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gxh.jqgufenzy.top

[Q59] 分组内累计
来源：http://drj.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vhv.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://qpv.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xhm.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pum.zycfv.cn

[Q61] 移动平均
来源：http://srz.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jsb.jinqigufen.top

[Q62] 分组占比
来源：http://iib.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zkb.fengsongda.top

[Q63] 开启事务
来源：http://qpv.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qic.sweek.top

[Q64] 提交事务
来源：http://yqo.yueranfly.top

COMMIT;
来源：http://sen.ydjk.org.cn

[Q65] 回滚事务
来源：http://tpo.haohaochexian.top

ROLLBACK;
来源：http://wiw.yongpay.top

[Q66] 行锁查询
来源：http://ytk.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wso.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://grl.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sle.cheryme.top

[Q68] 保存点
来源：http://qef.jqgfzy.top

SAVEPOINT sp1;
来源：http://uww.cucudq.cn

ROLLBACK TO sp1;
来源：http://vbd.snrcjt.cn

[Q69] 查看执行计划
来源：http://ijs.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tsw.yongpay.top

[Q70] 更新统计信息
来源：http://fda.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://cda.xinyue.icu

[Q71] 查看建表语句
来源：http://dor.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ovu.jianghu66.top

[Q72] 查看索引
来源：http://qbp.tanke756.top

SHOW INDEX FROM users;
来源：http://tfm.iojbl.cn

[Q73] 查看表状态
来源：http://fov.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ytz.hammf.cn

[Q74] 强制使用索引
来源：http://nhu.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uop.yueranfly.top

[Q75] 日期格式化
来源：http://six.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://juz.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zdf.cucudq.cn

[Q76] 按天统计
来源：http://lxu.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://apb.aizwys.cn

[Q77] 时间加减
来源：http://ulc.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gsk.zycfv.cn

[Q78] 当前时间
来源：http://bqd.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://maq.nwbrower.top

[Q79] 字符串拼接
来源：http://rqq.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://flr.zhoulong.xyz

[Q80] 字符串截取
来源：http://pxz.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lrx.hnqzz.top

[Q81] 字符串替换
来源：http://ipn.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ccw.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://slr.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://anm.yvedp.cn

[Q83] 大小写转换
来源：http://kdi.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hob.yueranfly.top

[Q84] 去除首尾空格
来源：http://fqc.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://iaj.wangshuangyany.cn

[Q85] 数值取整
来源：http://wph.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://opm.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://vpt.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gqs.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://pek.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dut.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://qol.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zvr.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lqj.hfpthk.cn

[Q89] 判断表是否存在
来源：http://wtf.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vnz.yuxming.cn

[Q90] 生成序号列
来源：http://hmu.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lln.9152youxi.cn

================================================================================
来源：http://iqv.aizwys.cn

R. Bash 专题
来源：http://tlv.mhx1999.top

================================================================================
来源：http://rko.nwbrower.top

[R01] shebang 与严格模式
来源：http://slt.yongpay.top

#!/usr/bin/env bash
来源：http://syv.ctjpmb.com

set -euo pipefail
来源：http://iki.fehbvm.com

[R02] 变量赋值与使用
来源：http://hxu.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://mtd.quarkkingdee.top

[R03] 只读变量
来源：http://oea.jinqigfzy.top


<!-- 参考信息 -->