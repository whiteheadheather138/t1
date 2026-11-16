代发 wailian999

TS:   // child_process / cluster 模块
来源：http://fet.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rbs.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://awy.cheryme.top

Ruby: // fork 块
来源：http://ytt.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://szc.cucudq.cn

================================================================================
来源：http://vzl.hnqzz.top

P. 常用工具函数
来源：http://cnc.gotoacloud.top

================================================================================
来源：http://tec.hnqzz.top

[P01] 生成 UUID
来源：http://yiu.sweek.top

Py:   str(uuid.uuid4())
来源：http://hsa.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ugu.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://pzh.birdmap.top

TS:   crypto.randomUUID()
来源：http://win.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://bbi.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://dpq.pycfn.com

Ruby: SecureRandom.uuid
来源：http://krg.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://szt.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://cgo.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eqj.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lfp.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oun.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mch.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://scd.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zlv.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ylq.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tng.jyoumei.cn

[P03] 生成短随机字符串
来源：http://fad.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hzx.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://omn.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpj.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vzq.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fyo.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jja.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pqx.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nrn.shzxlz.cn

[P04] 求长度
来源：http://lur.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxq.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlp.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zra.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://brh.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://qcm.sxryk.cn

Go:   len(arr);  len(m)
来源：http://uxs.guannengcc.top

Ruby: x.length;  x.size
来源：http://rto.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cpz.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://koa.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://rdg.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://asm.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xna.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kfb.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vgu.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://plv.chenlongwang.top

Ruby: a == b
来源：http://pdy.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zdz.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yqb.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ssr.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://sni.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://adx.zdbjq.cn

TS:   if (x == null) {}
来源：http://yfa.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cnm.fktsv.cn

Go:   if x == nil {}
来源：http://gxr.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://klp.jiagoushi.top

C#:   if (x is null) {}
来源：http://pxs.fzhhl.top

[P07] 防抖与节流
来源：http://rqd.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pcq.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://phx.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ser.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://alc.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jzt.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uwy.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lwh.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qej.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://kvc.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lbi.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hvj.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cjl.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lxc.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zqg.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ytn.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qxi.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sga.zhengqikj.top

================================================================================
来源：http://eft.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qgi.nwbrower.top

================================================================================
来源：http://mhf.cdnleiting.top

[Q01] 创建表
来源：http://koq.shanyushiyangtech.top

CREATE TABLE users (
来源：http://glu.nanxuanxn.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vjk.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://xxo.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://cls.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ktw.jinqigfzy.top

);
来源：http://jsk.yj202588.top

[Q02] 创建带外键的表
来源：http://lwp.xuanzx.com

CREATE TABLE orders (
来源：http://kmr.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cim.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://ogj.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://aof.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aag.birdmap.top

);
来源：http://bff.shzxlz.cn

[Q03] 增加列
来源：http://pxp.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nxz.svipenyu.cn

[Q04] 修改列类型
来源：http://rcq.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lqw.fktsv.cn

[Q05] 重命名列
来源：http://bty.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sah.meibo888.top

[Q06] 删除列
来源：http://apd.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pcj.chenlongwang.top

[Q07] 删除表
来源：http://imd.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://aua.zhoulong.xyz

[Q08] 创建普通索引
来源：http://jgm.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yvx.hnqzz.top

[Q09] 创建唯一索引
来源：http://mzt.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vrj.chenjidiqi.icu

[Q10] 插入单行
来源：http://xgj.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wez.9152youxi.cn

[Q11] 一次插入多行
来源：http://idc.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://suw.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://gxn.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://hln.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://krr.zhixingplan.top

[Q13] 忽略重复插入
来源：http://lup.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ice.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://zmj.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://amn.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ovh.hfpthk.cn

[Q15] 查询全部
来源：http://ulw.jyoumei.cn

SELECT * FROM users;
来源：http://fji.kuanghao11.cn

[Q16] 查询指定列
来源：http://luk.yanxiufei.cn

SELECT id, name FROM users;
来源：http://yve.epnwcf.com

[Q17] 条件查询
来源：http://oid.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://get.sysykeji.top

[Q18] 模糊匹配
来源：http://bbp.xziqi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uqm.ydzc1.top

[Q19] 范围查询
来源：http://oum.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://koo.zhixingplan.top

[Q20] IN 列表
来源：http://vjo.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tdb.dashuyun.cn

[Q21] 空值判断
来源：http://aeq.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yex.316326.xyz

[Q22] 排序
来源：http://zjj.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bln.shanyushiyangkeji.top

[Q23] 分页
来源：http://baa.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://evx.feifeiyinyue.top

[Q24] 去重
来源：http://frr.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://tkw.gzhubu.top

[Q25] 只取前 N 条
来源：http://ull.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zdl.snrcjt.cn

[Q26] 计数
来源：http://gcu.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://kud.xinyue.icu

[Q27] 条件计数
来源：http://uep.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jia.bjfxy.top

[Q28] 求和与平均
来源：http://sfz.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hwx.vqdsnc.cn

[Q29] 最大最小值
来源：http://qtr.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://dkd.0kj1m.cn

[Q30] 分组统计
来源：http://ftf.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ocn.nanxuanxn.top

[Q31] 分组后过滤
来源：http://psk.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dop.tarul.cn

[Q32] 分组拼接字符串
来源：http://dph.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://djl.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pvo.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://hbg.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dqg.smart0.xyz

[Q34] 每组取第一条
来源：http://cxy.uphjek.com

SELECT * FROM (
来源：http://gle.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://faj.ydjk.org.cn

) t WHERE rn = 1;
来源：http://kix.epnwcf.com

[Q35] 内连接
来源：http://fvv.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mhw.guowangkeji.top

[Q36] 左连接
来源：http://nzo.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vcq.cdnleiting.top

[Q37] 右连接
来源：http://mjy.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fir.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://svz.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://muk.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://jab.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://whi.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mzu.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kjb.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://byi.xinyue.icu

[Q41] 多表连接
来源：http://zev.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fgk.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://huh.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://ifk.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://qcb.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://jga.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gwa.sufxvd.cn

[Q43] 标量子查询
来源：http://wpq.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zon.aizwys.cn

[Q44] IN 子查询
来源：http://ohn.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pbb.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://shm.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lzf.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://ksq.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qkf.yvedp.cn

[Q47] 与平均值比较
来源：http://vxk.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lxf.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://btu.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://var.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://jhg.vehdjk.com

[Q49] 更新单行
来源：http://wvp.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xpm.mhx1999.top

[Q50] 批量更新
来源：http://qma.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://apv.zdbjq.cn

[Q51] 用子查询更新
来源：http://vcz.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tum.nanxuanxn.top

[Q52] 删除指定行
来源：http://iqp.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://spf.wangshuangyany.cn

[Q53] 按条件删除
来源：http://ndg.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://owk.fktsv.cn

[Q54] 清空表
来源：http://aop.havefunace.top

TRUNCATE TABLE logs;
来源：http://ajn.birdmap.top

[Q55] 排名（并列占位）
来源：http://jub.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zuu.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://gqq.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rly.yj20258888.top

[Q57] 行号
来源：http://wju.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xow.nanxinkj.top

[Q58] 累计求和
来源：http://wjw.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jdd.sufxvd.cn

[Q59] 分组内累计
来源：http://hmc.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zny.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://cji.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fnu.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tow.vehdjk.com

[Q61] 移动平均
来源：http://itw.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fag.svipenyu.cn

[Q62] 分组占比
来源：http://xrc.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tbh.ppjwa.cn

[Q63] 开启事务
来源：http://fxw.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iyp.chenlongwang.top

[Q64] 提交事务
来源：http://fsn.ivvv.top

COMMIT;
来源：http://kjr.yfazqb.com

[Q65] 回滚事务
来源：http://cem.fehbvm.com

ROLLBACK;
来源：http://ret.zhongyouzk.top

[Q66] 行锁查询
来源：http://hax.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vdw.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://vld.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bie.dashuyun.cn

[Q68] 保存点
来源：http://iwg.ybcxt.top

SAVEPOINT sp1;
来源：http://hge.gotoacloud.top

ROLLBACK TO sp1;
来源：http://iji.tianlin.xyz

[Q69] 查看执行计划
来源：http://ulf.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://you.jqgufenzy.top

[Q70] 更新统计信息
来源：http://wbn.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://uyb.fzhhl.top

[Q71] 查看建表语句
来源：http://gtz.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qqy.yj20258.top

[Q72] 查看索引
来源：http://yvu.cdnleiting.top

SHOW INDEX FROM users;
来源：http://vka.ydzc1.top

[Q73] 查看表状态
来源：http://mdw.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bge.tian-w.cn

[Q74] 强制使用索引
来源：http://pcw.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ezv.zhiwuduotai.top

[Q75] 日期格式化
来源：http://zhx.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://peq.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mdh.svipenyu.cn

[Q76] 按天统计
来源：http://mqc.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rkb.xylfe.cn

[Q77] 时间加减
来源：http://vnp.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rlu.cucudq.cn

[Q78] 当前时间
来源：http://iof.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ozz.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://blt.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ycb.havefunace.top

[Q80] 字符串截取
来源：http://odm.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sfa.xziqi.cn

[Q81] 字符串替换
来源：http://vtf.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wwc.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://jjv.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://atg.zdqjudy.top

[Q83] 大小写转换
来源：http://ked.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://log.dianchejie.cn

[Q84] 去除首尾空格
来源：http://iol.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://hdv.tarul.cn

[Q85] 数值取整
来源：http://lao.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tyi.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://fsw.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://swh.fzhhl.top

[Q87] JSON 字段做条件
来源：http://uhk.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ntr.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://wee.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tnp.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bog.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://tpu.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ffq.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://kqr.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hfc.yongpay.top

================================================================================
来源：http://tko.gzhubu.top

R. Bash 专题
来源：http://kzr.bjfxy.top

================================================================================
来源：http://sfy.haohaochexian.top

[R01] shebang 与严格模式
来源：http://lnw.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://php.zdqjudy.top

set -euo pipefail
来源：http://djb.vehdjk.com

[R02] 变量赋值与使用
来源：http://czl.hysaishi.cn

name="Tom"; echo "$name"
来源：http://rlg.haohaochexian.top

[R03] 只读变量
来源：http://bve.xziqi.cn

readonly PI=3.14
来源：http://nmi.daria6918.cn

[R04] 位置参数
来源：http://xob.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eii.andypj.xyz

[R05] 参数默认值
来源：http://buo.dashuyun.cn


<!-- 参考信息 -->