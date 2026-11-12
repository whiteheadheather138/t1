代发 wailian999

[O06] 使用进程池
来源：http://ssx.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xid.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cwx.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://gex.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://jgv.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://prc.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cbz.tian-w.cn

Ruby: // fork 块
来源：http://tfy.jinghuilouyu.cn

C#:   Parallel.For
来源：http://uah.dianchejie.cn

================================================================================
来源：http://lpi.sweek.top

P. 常用工具函数
来源：http://nbq.nwbrower.top

================================================================================
来源：http://gyx.fengsongda.top

[P01] 生成 UUID
来源：http://tra.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://lop.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bhb.iojbl.cn

JS:   crypto.randomUUID()
来源：http://knz.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://kpw.xuetiantiany.cn

Java: UUID.randomUUID().toString()
来源：http://qvh.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://cod.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://zvm.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://ekn.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://lmm.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lhr.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://kre.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qpf.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wmr.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wpf.sysykeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hrn.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gig.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dxh.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://qym.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gov.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hqv.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fbq.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fuq.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://orq.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cet.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ygq.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jaa.gotoacloud.top

[P04] 求长度
来源：http://vrd.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vua.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mog.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kaa.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sly.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://mqj.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://ktx.yvedp.cn

Ruby: x.length;  x.size
来源：http://cve.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://rio.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://cpl.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nzg.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fry.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://urs.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kic.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gev.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fau.ydzc1.top

Ruby: a == b
来源：http://hpl.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ezy.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sjc.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pmx.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://sdl.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qcl.c1oappe.top

TS:   if (x == null) {}
来源：http://nyz.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rkq.316326.xyz

Go:   if x == nil {}
来源：http://akp.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zkv.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://uvw.shangyingyoupin.top

[P07] 防抖与节流
来源：http://ouf.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://egp.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://ohf.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbn.c1oappe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://let.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ngx.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vlv.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vta.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bzm.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://dfd.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lkl.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wqu.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xup.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nyt.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vpc.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fgn.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://owl.smart0.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gfr.yfazqb.com

================================================================================
来源：http://pba.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tvj.andypj.xyz

================================================================================
来源：http://zcq.yfazqb.com

[Q01] 创建表
来源：http://zmk.guowangkeji.top

CREATE TABLE users (
来源：http://ekb.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://str.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://aej.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://leu.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dao.bjfxy.top

);
来源：http://dpl.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://yxf.havefunace.top

CREATE TABLE orders (
来源：http://fhz.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvx.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://ueg.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://zxv.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cus.zhijiandao.cn

);
来源：http://sct.guannengcc.top

[Q03] 增加列
来源：http://ozh.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tnb.snrcjt.cn

[Q04] 修改列类型
来源：http://cxw.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jrv.feifeiyinyue.top

[Q05] 重命名列
来源：http://xyt.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hnv.cdnleiting.top

[Q06] 删除列
来源：http://cfs.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tcp.sweek.top

[Q07] 删除表
来源：http://uxk.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://yax.shuidangran.top

[Q08] 创建普通索引
来源：http://twd.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://low.iojbl.cn

[Q09] 创建唯一索引
来源：http://cri.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cdj.dashuyun.cn

[Q10] 插入单行
来源：http://jnv.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hko.xziqi.cn

[Q11] 一次插入多行
来源：http://pqq.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vdu.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://bnj.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lbv.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rlr.ehwqpu.com

[Q13] 忽略重复插入
来源：http://gzd.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jwx.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://ifx.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ukh.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gwq.dianchejie.cn

[Q15] 查询全部
来源：http://spy.cucudq.cn

SELECT * FROM users;
来源：http://zyd.xinyue.icu

[Q16] 查询指定列
来源：http://ehw.jiagoushi.top

SELECT id, name FROM users;
来源：http://wln.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://opb.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gnb.iojbl.cn

[Q18] 模糊匹配
来源：http://rlg.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dag.sysykeji.top

[Q19] 范围查询
来源：http://szx.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mlx.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://nfo.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kum.aizwys.cn

[Q21] 空值判断
来源：http://vxz.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://agi.jqgufenzy.top

[Q22] 排序
来源：http://rke.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xlk.52xcode.cn

[Q23] 分页
来源：http://ctc.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://llb.birdmap.top

[Q24] 去重
来源：http://cwd.yfazqb.com

SELECT DISTINCT city FROM users;
来源：http://wsd.yongpay.top

[Q25] 只取前 N 条
来源：http://qur.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yta.nanxuanxn.top

[Q26] 计数
来源：http://jjd.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://wkx.nanxinkj.top

[Q27] 条件计数
来源：http://sub.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wvi.epnwcf.com

[Q28] 求和与平均
来源：http://dyi.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mvs.cashguo.top

[Q29] 最大最小值
来源：http://pdv.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://zox.yj20258888.top

[Q30] 分组统计
来源：http://iaw.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://drk.fzhhl.top

[Q31] 分组后过滤
来源：http://rbf.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zkj.hesvh.cn

[Q32] 分组拼接字符串
来源：http://dsg.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ayd.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vpr.sysykeji.top

[Q33] 多列分组
来源：http://rlp.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hqi.hnxiangtu.top

[Q34] 每组取第一条
来源：http://qog.quarkkingdee.top

SELECT * FROM (
来源：http://blf.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dfh.cucudq.cn

) t WHERE rn = 1;
来源：http://kci.tanke756.top

[Q35] 内连接
来源：http://aoi.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xss.yj20258.top

[Q36] 左连接
来源：http://lxn.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tfu.yfazqb.com

[Q37] 右连接
来源：http://abj.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vej.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://wlb.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uqd.yongpay.top

[Q39] 自连接（查上下级）
来源：http://etp.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yew.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pwq.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rpq.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ybn.chenlongwang.top

[Q41] 多表连接
来源：http://ndl.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ocw.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://vza.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://lrt.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://srj.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://gqt.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://glz.fzhhl.top

[Q43] 标量子查询
来源：http://qjo.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vmi.gotoacloud.top

[Q44] IN 子查询
来源：http://lbq.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nxp.yj202588.top

[Q45] EXISTS 判断存在
来源：http://jpk.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://idd.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://cjc.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iri.xylfe.cn

[Q47] 与平均值比较
来源：http://eke.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kmj.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://znf.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hih.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://vcs.hammf.cn

[Q49] 更新单行
来源：http://uzq.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yvw.chenlongwang.top

[Q50] 批量更新
来源：http://dqy.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hhn.ehwqpu.com

[Q51] 用子查询更新
来源：http://njb.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://flk.andypj.xyz

[Q52] 删除指定行
来源：http://yrh.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://hmg.fktsv.cn

[Q53] 按条件删除
来源：http://lug.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sdm.ydzc1.top

[Q54] 清空表
来源：http://ooh.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://cpx.yueranfly.top

[Q55] 排名（并列占位）
来源：http://rac.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gap.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://anb.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bxu.ivvv.top

[Q57] 行号
来源：http://vsz.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nwa.dashuyun.cn

[Q58] 累计求和
来源：http://hqw.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://txa.tanke756.top

[Q59] 分组内累计
来源：http://mbz.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aku.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://pze.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jck.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kuz.jqgufenzy.top

[Q61] 移动平均
来源：http://cqg.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://llv.hcnkem.com

[Q62] 分组占比
来源：http://lgj.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dvh.zdbjq.cn

[Q63] 开启事务
来源：http://shc.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hdb.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://gdk.52xcode.cn

COMMIT;
来源：http://znk.jiagoushi.top

[Q65] 回滚事务
来源：http://wno.jqgufenzy.top

ROLLBACK;
来源：http://adj.ppjwa.cn

[Q66] 行锁查询
来源：http://ukx.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://awi.wangdashe.top

[Q67] 设置隔离级别
来源：http://nby.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cfb.jinyuanbaomall.cn

[Q68] 保存点
来源：http://yyc.aizwys.cn

SAVEPOINT sp1;
来源：http://fxx.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://ceh.aizwys.cn

[Q69] 查看执行计划
来源：http://bsl.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qen.redwolf501.top

[Q70] 更新统计信息
来源：http://nwr.zhengqikj.top

ANALYZE TABLE users;
来源：http://etm.0kj1m.cn

[Q71] 查看建表语句
来源：http://ekq.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mqo.fanxiaobao.xyz

[Q72] 查看索引
来源：http://lba.ctjpmb.com

SHOW INDEX FROM users;
来源：http://gpu.vehdjk.com

[Q73] 查看表状态
来源：http://koi.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ile.xuanzx.com

[Q74] 强制使用索引
来源：http://lvv.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jgl.hfpthk.cn

[Q75] 日期格式化
来源：http://qhr.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yxd.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ini.yanxiufei.cn

[Q76] 按天统计
来源：http://kox.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zbh.fehbvm.com

[Q77] 时间加减
来源：http://rcm.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fef.yuxming.cn

[Q78] 当前时间
来源：http://otf.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jhb.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://afw.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gac.dianchejie.cn

[Q80] 字符串截取
来源：http://gwp.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nhp.pycfn.com

[Q81] 字符串替换
来源：http://jli.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yiw.havefunace.top

[Q82] 字符长度与字节长度
来源：http://zgg.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lax.hcnkem.com

[Q83] 大小写转换
来源：http://upt.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mgl.uphjek.com

[Q84] 去除首尾空格
来源：http://cqa.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://vfy.guannengcc.top

[Q85] 数值取整
来源：http://nuz.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bdq.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://own.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tfs.redwolf501.top

[Q87] JSON 字段做条件
来源：http://dos.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://prr.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://zlj.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oef.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ajv.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://ufy.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fjp.sysykeji.top

[Q90] 生成序号列
来源：http://hbq.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://czb.xuetiantiany.cn

================================================================================
来源：http://jer.vqdsnc.cn

R. Bash 专题
来源：http://kzt.iojbl.cn

================================================================================
来源：http://ghk.hcnkem.com

[R01] shebang 与严格模式
来源：http://wsb.ybcxt.top

#!/usr/bin/env bash
来源：http://mjw.ppjwa.cn

set -euo pipefail
来源：http://txq.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://kpc.hcnkem.com

name="Tom"; echo "$name"
来源：http://ywo.jqgfzy.top

[R03] 只读变量
来源：http://bol.shangyingyoupin.top


<!-- 参考信息 -->