代发 wailian999

TS:   // child_process / cluster 模块
来源：http://izq.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gmh.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hdt.tanke756.top

Ruby: // fork 块
来源：http://iam.shzxlz.cn

C#:   Parallel.For
来源：http://fbt.jqgufenzy.top

================================================================================
来源：http://snw.guowangkeji.top

P. 常用工具函数
来源：http://bpn.iojbl.cn

================================================================================
来源：http://hgw.yj20258.top

[P01] 生成 UUID
来源：http://mzr.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://nri.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ore.fehbvm.com

JS:   crypto.randomUUID()
来源：http://cqc.yfazqb.com

TS:   crypto.randomUUID()
来源：http://efu.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://krs.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://alc.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://por.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://bor.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://vph.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ilc.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qhr.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://win.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ncg.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://stj.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zdu.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://msm.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fnk.yangfankeji.com

[P03] 生成短随机字符串
来源：http://vkx.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dho.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ked.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tyu.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zac.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fpk.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hnj.iojbl.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hxm.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rif.xuetiantiany.cn

[P04] 求长度
来源：http://hzz.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uxf.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cnm.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mte.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qdh.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://bgf.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://aul.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://ucu.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hzy.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://mfg.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iue.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uth.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tqo.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hvj.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bbs.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ptt.dianchejie.cn

Ruby: a == b
来源：http://agh.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vcn.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tta.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ogp.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://ibc.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wod.smart0.xyz

TS:   if (x == null) {}
来源：http://ral.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pll.snrcjt.cn

Go:   if x == nil {}
来源：http://qgt.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cha.havefunace.top

C#:   if (x is null) {}
来源：http://obd.cucudq.cn

[P07] 防抖与节流
来源：http://tmb.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hku.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://qgz.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lug.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yam.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tqm.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nmp.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://cit.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qyj.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://gqp.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ksr.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sqe.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vza.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wyr.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sfq.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rvo.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://grf.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pwg.ywan-chungtsiang.top

================================================================================
来源：http://rjl.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pwy.shanyushiyangkeji.top

================================================================================
来源：http://oih.jinqigufen.top

[Q01] 创建表
来源：http://pvi.andypj.xyz

CREATE TABLE users (
来源：http://iou.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wne.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://pdu.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://mbr.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lqk.bbcook.cn

);
来源：http://ttz.iojbl.cn

[Q02] 创建带外键的表
来源：http://wcz.redwolf501.top

CREATE TABLE orders (
来源：http://fqh.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tgr.epnwcf.com

user_id INT NOT NULL,
来源：http://xvv.316326.xyz

amount DECIMAL(10, 2),
来源：http://fjq.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mth.ydzc1.top

);
来源：http://wus.fzhhl.top

[Q03] 增加列
来源：http://elp.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mzl.fzhhl.top

[Q04] 修改列类型
来源：http://qnr.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vre.zhixingplan.top

[Q05] 重命名列
来源：http://osx.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eqr.shangyingyoupin.top

[Q06] 删除列
来源：http://aic.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sye.yonumen.top

[Q07] 删除表
来源：http://pwn.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://ijy.fktsv.cn

[Q08] 创建普通索引
来源：http://euw.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xkf.chenlongwang.top

[Q09] 创建唯一索引
来源：http://lme.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jkq.fzhhl.top

[Q10] 插入单行
来源：http://oce.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uor.cashguo.top

[Q11] 一次插入多行
来源：http://ahl.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sii.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://qxs.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://ism.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cdb.gotoacloud.top

[Q13] 忽略重复插入
来源：http://qbd.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cym.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://fdc.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wnp.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vrx.wangshuangyany.cn

[Q15] 查询全部
来源：http://hll.haohaochexian.top

SELECT * FROM users;
来源：http://dxc.fengsongda.top

[Q16] 查询指定列
来源：http://laa.svipenyu.cn

SELECT id, name FROM users;
来源：http://lgl.ydzc1.top

[Q17] 条件查询
来源：http://bjp.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://spc.mhx1999.top

[Q18] 模糊匹配
来源：http://gfj.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tvg.ehwqpu.com

[Q19] 范围查询
来源：http://fvg.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zlz.9152youxi.cn

[Q20] IN 列表
来源：http://ikd.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://veg.gogol.net.cn

[Q21] 空值判断
来源：http://csf.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eeg.ybcxt.top

[Q22] 排序
来源：http://abr.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tph.sjlbkw.cn

[Q23] 分页
来源：http://pgf.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rvh.jiagoushi.top

[Q24] 去重
来源：http://sdo.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://olj.chenzaomai.com

[Q25] 只取前 N 条
来源：http://zia.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://phs.haohaochexian.top

[Q26] 计数
来源：http://wal.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://hkn.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://tjy.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://una.dianchejie.cn

[Q28] 求和与平均
来源：http://bwo.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mgq.tianlin.xyz

[Q29] 最大最小值
来源：http://kgu.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ycn.nanxinkj.top

[Q30] 分组统计
来源：http://cfz.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yxi.yonumen.top

[Q31] 分组后过滤
来源：http://reu.yanxiufei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kes.redwolf501.top

[Q32] 分组拼接字符串
来源：http://vcv.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lwl.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yju.zhoulong.xyz

[Q33] 多列分组
来源：http://mwo.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fjt.haohaochexian.top

[Q34] 每组取第一条
来源：http://vqa.ydzc1.top

SELECT * FROM (
来源：http://gpg.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yyf.nanxinkj.top

) t WHERE rn = 1;
来源：http://pvg.jinqigufen.top

[Q35] 内连接
来源：http://gcc.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tdo.hongshengwenyu.top

[Q36] 左连接
来源：http://xss.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yak.hywenlv.cn

[Q37] 右连接
来源：http://ftk.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oto.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://hoz.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qbn.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://rgy.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dnc.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kpv.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://wur.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mwj.chenzaomai.com

[Q41] 多表连接
来源：http://ouf.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dft.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://cys.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://rou.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://ysx.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://tem.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gbv.nanxinkj.top

[Q43] 标量子查询
来源：http://kvt.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vto.cqqwz.cn

[Q44] IN 子查询
来源：http://aou.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uey.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://vvt.fanxiaobao.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhi.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://cry.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vba.wangdashe.top

[Q47] 与平均值比较
来源：http://lio.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ctq.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://zll.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vvl.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://uyz.havefunace.top

[Q49] 更新单行
来源：http://bba.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://twk.fanxiaobao.xyz

[Q50] 批量更新
来源：http://tpo.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ziv.birdmap.top

[Q51] 用子查询更新
来源：http://sqo.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ykx.cdnleiting.top

[Q52] 删除指定行
来源：http://ipj.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://fgc.9152youxi.cn

[Q53] 按条件删除
来源：http://dgd.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vby.daxiang520.top

[Q54] 清空表
来源：http://jxr.smart0.xyz

TRUNCATE TABLE logs;
来源：http://psa.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://xuf.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uyf.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://lin.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bce.xziqi.cn

[Q57] 行号
来源：http://dvh.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dmj.hysaishi.cn

[Q58] 累计求和
来源：http://mps.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cdj.meibo888.top

[Q59] 分组内累计
来源：http://scs.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://scu.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://aql.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nwt.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xvi.hywenlv.cn

[Q61] 移动平均
来源：http://gth.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wit.zhongyouzk.top

[Q62] 分组占比
来源：http://fpu.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vut.feifeiyinyue.top

[Q63] 开启事务
来源：http://ogb.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uhi.hnxiangtu.top

[Q64] 提交事务
来源：http://jyp.svipenyu.cn

COMMIT;
来源：http://xwz.hammf.cn

[Q65] 回滚事务
来源：http://uqa.shuidangran.top

ROLLBACK;
来源：http://zhj.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://tzg.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://koy.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://dtf.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ual.cqqwz.cn

[Q68] 保存点
来源：http://qlp.yvedp.cn

SAVEPOINT sp1;
来源：http://tdy.dashuyun.cn

ROLLBACK TO sp1;
来源：http://hxq.guowangkeji.top

[Q69] 查看执行计划
来源：http://qbe.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://stu.ehwqpu.com

[Q70] 更新统计信息
来源：http://cqx.52xcode.cn

ANALYZE TABLE users;
来源：http://sws.hcnkem.com

[Q71] 查看建表语句
来源：http://jbr.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://thh.shuidangran.top

[Q72] 查看索引
来源：http://mge.9152youxi.cn

SHOW INDEX FROM users;
来源：http://las.yj20258888.top

[Q73] 查看表状态
来源：http://afj.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xxr.zycfv.cn

[Q74] 强制使用索引
来源：http://ctj.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kwu.zycfv.cn

[Q75] 日期格式化
来源：http://mzc.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://djg.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hai.yonumen.top

[Q76] 按天统计
来源：http://zhl.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nml.havefunace.top

[Q77] 时间加减
来源：http://int.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zrc.haohaochexian.top

[Q78] 当前时间
来源：http://qkm.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xzk.birdmap.top

[Q79] 字符串拼接
来源：http://eay.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ixz.ybcxt.top

[Q80] 字符串截取
来源：http://ykg.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sxo.feifeiyinyue.top

[Q81] 字符串替换
来源：http://svs.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rzw.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://hdt.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lfk.iojbl.cn

[Q83] 大小写转换
来源：http://lge.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mnt.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://lvo.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://kzh.chenlongwang.top

[Q85] 数值取整
来源：http://wkp.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dgm.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://jpf.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aeq.sxryk.cn

[Q87] JSON 字段做条件
来源：http://hpx.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lex.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://ebv.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vzc.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fzu.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://pjg.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://itl.jyoumei.cn

[Q90] 生成序号列
来源：http://lho.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rgm.nanxuanxn.top

================================================================================
来源：http://koa.yj20258888.top

R. Bash 专题
来源：http://hdi.wangdashe.top

================================================================================
来源：http://nkh.guannengcc.top

[R01] shebang 与严格模式
来源：http://yvl.ctjpmb.com

#!/usr/bin/env bash
来源：http://ufs.jinqigufen.top

set -euo pipefail
来源：http://yrk.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://nmv.havefunace.top

name="Tom"; echo "$name"
来源：http://uxk.jinqigufen.top

[R03] 只读变量
来源：http://ufp.hongshengwenyu.top

readonly PI=3.14
来源：http://srn.cashguo.top

[R04] 位置参数
来源：http://mtp.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sor.xinyue.icu

[R05] 参数默认值
来源：http://gth.kuanghao11.cn


<!-- 参考信息 -->