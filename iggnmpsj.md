代发 wailian999

TS:   // child_process / cluster 模块
来源：http://ygb.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dpz.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://czn.gotoacloud.top

Ruby: // fork 块
来源：http://swq.yj20258888.top

C#:   Parallel.For
来源：http://psd.hesvh.cn

================================================================================
来源：http://yol.shangyingyoupin.top

P. 常用工具函数
来源：http://ddf.hnxiangtu.top

================================================================================
来源：http://xon.hnqzz.top

[P01] 生成 UUID
来源：http://iat.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://qgh.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ora.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://fri.smart0.xyz

TS:   crypto.randomUUID()
来源：http://mlo.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://mmv.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://rpg.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://yau.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://fec.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://yvl.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zuf.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkb.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mlw.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ltv.0kj1m.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nok.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bpz.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://evp.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lpm.aibaodan.cn

[P03] 生成短随机字符串
来源：http://wwh.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ydd.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tob.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cce.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhn.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://whe.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zuc.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ffy.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://roc.pycfn.com

[P04] 求长度
来源：http://ipk.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nsh.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://itc.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gla.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sve.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://jmj.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://buy.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://ikm.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kdq.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://ewq.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://huz.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://psq.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pdr.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vwf.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://urt.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eqz.havefunace.top

Ruby: a == b
来源：http://lqx.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jwr.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ytf.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mfp.uphjek.com

PHP:  if (empty($x)) {}
来源：http://dlm.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://elp.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://vng.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ddu.guowangkeji.top

Go:   if x == nil {}
来源：http://unh.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jyd.fengsongda.top

C#:   if (x is null) {}
来源：http://maz.tarul.cn

[P07] 防抖与节流
来源：http://brn.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dmr.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://ryy.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ohh.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iri.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jeu.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mmi.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gmf.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zzg.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://aop.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://edy.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cui.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ykj.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nte.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kfj.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mgh.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qza.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lif.iojbl.cn

================================================================================
来源：http://xam.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mnd.sweek.top

================================================================================
来源：http://wgc.pengpengdd.cyou

[Q01] 创建表
来源：http://bwy.gzhubu.top

CREATE TABLE users (
来源：http://oke.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://feg.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://rqa.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://bwr.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uww.gogol.net.cn

);
来源：http://ryb.andypj.xyz

[Q02] 创建带外键的表
来源：http://cno.0kj1m.cn

CREATE TABLE orders (
来源：http://jrp.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmg.fanxiaobao.xyz

user_id INT NOT NULL,
来源：http://iwr.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://thh.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gqv.jlsjyb.cn

);
来源：http://jkt.cashguo.top

[Q03] 增加列
来源：http://sbe.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bup.sweek.top

[Q04] 修改列类型
来源：http://gmu.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://woy.yvedp.cn

[Q05] 重命名列
来源：http://lxp.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://for.yj20258.top

[Q06] 删除列
来源：http://ucn.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zsc.havefunace.top

[Q07] 删除表
来源：http://xbe.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://vnt.daria6918.cn

[Q08] 创建普通索引
来源：http://tyn.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bcf.chenlongwang.top

[Q09] 创建唯一索引
来源：http://kxf.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pdb.ywan-chungtsiang.top

[Q10] 插入单行
来源：http://ahr.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ccg.xziqi.cn

[Q11] 一次插入多行
来源：http://ghr.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jhb.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://cdg.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://dwt.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dno.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://avb.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ehe.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://stx.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eaw.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://btj.yvedp.cn

[Q15] 查询全部
来源：http://bab.yongpay.top

SELECT * FROM users;
来源：http://isn.chenlongwang.top

[Q16] 查询指定列
来源：http://qyf.bbcook.cn

SELECT id, name FROM users;
来源：http://bwi.316326.xyz

[Q17] 条件查询
来源：http://oqv.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nxn.pycfn.com

[Q18] 模糊匹配
来源：http://bui.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://epv.nwbrower.top

[Q19] 范围查询
来源：http://rio.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uwk.ppjwa.cn

[Q20] IN 列表
来源：http://xnn.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kop.cucudq.cn

[Q21] 空值判断
来源：http://lgr.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jle.sysykeji.top

[Q22] 排序
来源：http://jgn.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fqs.svipenyu.cn

[Q23] 分页
来源：http://qhs.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rlo.jinghuilouyu.cn

[Q24] 去重
来源：http://kmz.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://lqd.shuidangran.top

[Q25] 只取前 N 条
来源：http://kfx.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tna.fehbvm.com

[Q26] 计数
来源：http://noh.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://wxq.yangfankeji.com

[Q27] 条件计数
来源：http://ybs.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rne.cqqwz.cn

[Q28] 求和与平均
来源：http://hcd.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lru.ivvv.top

[Q29] 最大最小值
来源：http://vvz.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://trn.shuidangran.top

[Q30] 分组统计
来源：http://fyn.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zpk.sufxvd.cn

[Q31] 分组后过滤
来源：http://yhm.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gye.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://xdh.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xhw.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxr.316326.xyz

[Q33] 多列分组
来源：http://sgc.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmx.epnwcf.com

[Q34] 每组取第一条
来源：http://afi.0kj1m.cn

SELECT * FROM (
来源：http://zzg.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mwb.chenlongwang.top

) t WHERE rn = 1;
来源：http://bsa.sxryk.cn

[Q35] 内连接
来源：http://xzz.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xej.yuxming.cn

[Q36] 左连接
来源：http://cia.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://twp.ppjwa.cn

[Q37] 右连接
来源：http://huj.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hol.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ram.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rsp.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://puu.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kqn.hcnkem.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hfo.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://emu.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ctc.ybcxt.top

[Q41] 多表连接
来源：http://liz.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://whq.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://lpq.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://ugb.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://qlj.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://gbn.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://etc.zhengqikj.top

[Q43] 标量子查询
来源：http://ptp.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://diy.jlsjyb.cn

[Q44] IN 子查询
来源：http://afc.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ctc.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://vyw.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kxf.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://yvs.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dcc.nanxuanxn.top

[Q47] 与平均值比较
来源：http://jhf.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tdo.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://sss.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mdw.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://wtm.nanxuanxn.top

[Q49] 更新单行
来源：http://ehy.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://atb.mhx1999.top

[Q50] 批量更新
来源：http://usx.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rjq.gaohongyu789.top

[Q51] 用子查询更新
来源：http://jum.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hcc.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://phk.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://zvx.hysaishi.cn

[Q53] 按条件删除
来源：http://lkp.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ufg.snrcjt.cn

[Q54] 清空表
来源：http://wkt.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://amg.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://qel.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kmw.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://hzz.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://scs.hammf.cn

[Q57] 行号
来源：http://zbl.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xma.tanke756.top

[Q58] 累计求和
来源：http://niz.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwj.9152youxi.cn

[Q59] 分组内累计
来源：http://yoi.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xjs.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://yjl.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cla.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nqi.jlsjyb.cn

[Q61] 移动平均
来源：http://osx.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fhz.chenjidiqi.icu

[Q62] 分组占比
来源：http://mps.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vxj.jqgfzy.top

[Q63] 开启事务
来源：http://gga.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pey.bjfxy.top

[Q64] 提交事务
来源：http://kpn.hesvh.cn

COMMIT;
来源：http://uay.nwbrower.top

[Q65] 回滚事务
来源：http://qoj.xuetiantiany.cn

ROLLBACK;
来源：http://pak.sufxvd.cn

[Q66] 行锁查询
来源：http://myf.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rvq.zdbjq.cn

[Q67] 设置隔离级别
来源：http://ufw.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rzo.yfazqb.com

[Q68] 保存点
来源：http://mhk.yfazqb.com

SAVEPOINT sp1;
来源：http://ctg.ydzc1.top

ROLLBACK TO sp1;
来源：http://vmo.c1oappe.top

[Q69] 查看执行计划
来源：http://udm.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uvj.zhengqikj.top

[Q70] 更新统计信息
来源：http://alf.hfpthk.cn

ANALYZE TABLE users;
来源：http://zvh.shzxlz.cn

[Q71] 查看建表语句
来源：http://uds.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwg.cdnleiting.top

[Q72] 查看索引
来源：http://cqj.yj202588.top

SHOW INDEX FROM users;
来源：http://iie.kuanghao11.cn

[Q73] 查看表状态
来源：http://cnm.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://cgl.jqgufenzy.top

[Q74] 强制使用索引
来源：http://kjm.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iix.bbcook.cn

[Q75] 日期格式化
来源：http://vzr.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bwk.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://axk.sxryk.cn

[Q76] 按天统计
来源：http://vzx.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ymr.yj20258.top

[Q77] 时间加减
来源：http://fdd.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eby.yj20258.top

[Q78] 当前时间
来源：http://day.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jld.sysykeji.top

[Q79] 字符串拼接
来源：http://zqc.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://miq.mhx1999.top

[Q80] 字符串截取
来源：http://nqr.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ovb.fzhhl.top

[Q81] 字符串替换
来源：http://blp.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tql.cashguo.top

[Q82] 字符长度与字节长度
来源：http://eod.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kmu.snrcjt.cn

[Q83] 大小写转换
来源：http://pzb.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uni.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://qob.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://fso.jlsjyb.cn

[Q85] 数值取整
来源：http://low.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yso.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://cle.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hfn.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://rzk.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hri.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://qbr.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qni.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rwa.tanke756.top

[Q89] 判断表是否存在
来源：http://fwl.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yev.havefunace.top

[Q90] 生成序号列
来源：http://lzx.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iiv.9152youxi.cn

================================================================================
来源：http://sbw.jyoumei.cn

R. Bash 专题
来源：http://ges.vehdjk.com

================================================================================
来源：http://qqt.nwbrower.top

[R01] shebang 与严格模式
来源：http://gwm.316326.xyz

#!/usr/bin/env bash
来源：http://ohe.hnqzz.top

set -euo pipefail
来源：http://tif.andypj.xyz

[R02] 变量赋值与使用
来源：http://xos.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://var.fengsongda.top

[R03] 只读变量
来源：http://fwv.svipenyu.cn

readonly PI=3.14
来源：http://tyc.nanxuanxn.top

[R04] 位置参数
来源：http://xyh.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gus.fzhhl.top

[R05] 参数默认值
来源：http://jiw.tarul.cn


<!-- 参考信息 -->