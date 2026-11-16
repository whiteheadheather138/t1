代发 wailian999

[O06] 使用进程池
来源：http://ddl.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lwc.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jqr.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://atm.hammf.cn

TS:   // child_process / cluster 模块
来源：http://cuh.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rmf.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fbb.jinghuilouyu.cn

Ruby: // fork 块
来源：http://yxb.ctjpmb.com

C#:   Parallel.For
来源：http://hbr.jinyuanbaomall.cn

================================================================================
来源：http://ktp.cqqwz.cn

P. 常用工具函数
来源：http://xwq.jinqigufen.top

================================================================================
来源：http://ppt.quarkkingdee.top

[P01] 生成 UUID
来源：http://ojf.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://xpg.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ntq.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://xpw.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://rlu.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://mey.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://nbj.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://kpj.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://rcd.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://iel.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lcg.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rqx.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zxj.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://upc.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vdg.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yox.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qka.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ppi.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://mka.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cgw.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://llh.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://btb.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rer.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yri.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://smv.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://alm.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hqk.yueranfly.top

[P04] 求长度
来源：http://djl.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://igg.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ysw.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mfy.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ylz.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://ger.316326.xyz

Go:   len(arr);  len(m)
来源：http://mbj.fktsv.cn

Ruby: x.length;  x.size
来源：http://wfe.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qxo.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://ene.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yjb.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tow.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oxv.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tke.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdy.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://zxk.yvedp.cn

Ruby: a == b
来源：http://wzp.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ghk.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dna.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lco.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://bto.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vxy.pycfn.com

TS:   if (x == null) {}
来源：http://ghr.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://joe.nwbrower.top

Go:   if x == nil {}
来源：http://hjx.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mxy.ehwqpu.com

C#:   if (x is null) {}
来源：http://cfe.redwolf501.top

[P07] 防抖与节流
来源：http://afh.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mvp.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://zgb.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwp.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hpo.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://akm.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qvf.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://gdb.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yhf.yj20258.top

[P08] 处理浮点精度问题
来源：http://wiy.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ldd.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xce.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kvk.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tup.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uxo.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://udj.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hmj.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xde.epnwcf.com

================================================================================
来源：http://taz.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lju.sxryk.cn

================================================================================
来源：http://tux.sxryk.cn

[Q01] 创建表
来源：http://nlo.ivvv.top

CREATE TABLE users (
来源：http://foe.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://csw.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://jhq.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://lun.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ngd.zycfv.cn

);
来源：http://jrz.fktsv.cn

[Q02] 创建带外键的表
来源：http://qkf.meibo888.top

CREATE TABLE orders (
来源：http://zzo.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yyc.birdmap.top

user_id INT NOT NULL,
来源：http://smx.birdmap.top

amount DECIMAL(10, 2),
来源：http://nem.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://psk.andypj.xyz

);
来源：http://jiy.guowangkeji.top

[Q03] 增加列
来源：http://pka.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hba.vehdjk.com

[Q04] 修改列类型
来源：http://kxf.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dld.0kj1m.cn

[Q05] 重命名列
来源：http://vsa.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vas.jqgufenzy.top

[Q06] 删除列
来源：http://imr.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://wek.ivvv.top

[Q07] 删除表
来源：http://qbm.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://tio.yj202588.top

[Q08] 创建普通索引
来源：http://bdv.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://bue.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://rui.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://muo.ydzc1.top

[Q10] 插入单行
来源：http://plx.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qga.gogol.net.cn

[Q11] 一次插入多行
来源：http://pya.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ocv.316326.xyz

[Q12] 插入后取自增 ID
来源：http://ots.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://gtt.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jgt.daxiang520.top

[Q13] 忽略重复插入
来源：http://xza.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qiw.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://ozk.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tmt.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pnv.yonumen.top

[Q15] 查询全部
来源：http://kbl.yueranfly.top

SELECT * FROM users;
来源：http://upo.hcnkem.com

[Q16] 查询指定列
来源：http://hbd.bjfxy.top

SELECT id, name FROM users;
来源：http://hnl.mhx1999.top

[Q17] 条件查询
来源：http://uad.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xtk.yuxming.cn

[Q18] 模糊匹配
来源：http://mce.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wna.nanxinkj.top

[Q19] 范围查询
来源：http://vzc.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://skq.zhengqikj.top

[Q20] IN 列表
来源：http://jza.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ato.zhiwuduotai.top

[Q21] 空值判断
来源：http://wmc.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tae.hesvh.cn

[Q22] 排序
来源：http://xtu.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qfe.hesvh.cn

[Q23] 分页
来源：http://bkv.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cmx.yj202588.top

[Q24] 去重
来源：http://moh.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://epy.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://atk.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vfi.shanyushiyangtech.top

[Q26] 计数
来源：http://jjj.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://jnt.tarul.cn

[Q27] 条件计数
来源：http://ghy.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xzl.yj202588.top

[Q28] 求和与平均
来源：http://cnp.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jfr.guowangkeji.top

[Q29] 最大最小值
来源：http://klc.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cxa.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://ckj.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dax.haohaochexian.top

[Q31] 分组后过滤
来源：http://xrw.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rsa.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://eod.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pvf.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uub.chenlongwang.top

[Q33] 多列分组
来源：http://ity.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lot.jinqigufen.top

[Q34] 每组取第一条
来源：http://fbw.xuetiantiany.cn

SELECT * FROM (
来源：http://tpm.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wzl.fktsv.cn

) t WHERE rn = 1;
来源：http://ien.jianghu66.top

[Q35] 内连接
来源：http://kby.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eiw.0kj1m.cn

[Q36] 左连接
来源：http://fpo.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hdh.xziqi.cn

[Q37] 右连接
来源：http://kmu.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tab.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://fnv.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wki.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://dso.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://our.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jmb.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jbf.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uov.zdbjq.cn

[Q41] 多表连接
来源：http://csp.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zrl.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://kti.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://uhv.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://aos.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://utt.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mkt.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://bvx.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://khc.hfpthk.cn

[Q44] IN 子查询
来源：http://mwk.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hbm.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://lrh.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dwh.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://ovz.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vow.zhengqikj.top

[Q47] 与平均值比较
来源：http://hec.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oyh.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://lch.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ake.guannengcc.top

SELECT * FROM t WHERE c > 5;
来源：http://dwy.iojbl.cn

[Q49] 更新单行
来源：http://nuv.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zhr.tian-w.cn

[Q50] 批量更新
来源：http://uwe.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pmr.mhx1999.top

[Q51] 用子查询更新
来源：http://rdc.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aso.ybcxt.top

[Q52] 删除指定行
来源：http://cvs.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://vfm.hfpthk.cn

[Q53] 按条件删除
来源：http://qnb.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrv.gogol.net.cn

[Q54] 清空表
来源：http://mrm.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://niz.pycfn.com

[Q55] 排名（并列占位）
来源：http://uzs.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://soo.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://hxa.gzhubu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rak.jinghuilouyu.cn

[Q57] 行号
来源：http://ejz.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ase.sufxvd.cn

[Q58] 累计求和
来源：http://yfg.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ybb.ybcxt.top

[Q59] 分组内累计
来源：http://bea.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bsz.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://mfl.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pdq.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yut.smart0.xyz

[Q61] 移动平均
来源：http://sba.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://klm.jianghu66.top

[Q62] 分组占比
来源：http://ljv.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://acy.xylfe.cn

[Q63] 开启事务
来源：http://hnr.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://uay.jiagoushi.top

[Q64] 提交事务
来源：http://pcf.cashguo.top

COMMIT;
来源：http://uhb.hysaishi.cn

[Q65] 回滚事务
来源：http://zba.yanxiufei.cn

ROLLBACK;
来源：http://fgw.gaohongyu789.top

[Q66] 行锁查询
来源：http://oxr.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zpd.fehbvm.com

[Q67] 设置隔离级别
来源：http://jcm.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cie.fengsongda.top

[Q68] 保存点
来源：http://uyz.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://xkt.guannengcc.top

ROLLBACK TO sp1;
来源：http://nty.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://jaw.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gzm.yuanzhike.top

[Q70] 更新统计信息
来源：http://lac.zdqjudy.top

ANALYZE TABLE users;
来源：http://irt.bbcook.cn

[Q71] 查看建表语句
来源：http://msr.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bsd.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://ojo.svipenyu.cn

SHOW INDEX FROM users;
来源：http://guw.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://dor.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://sbg.aizwys.cn

[Q74] 强制使用索引
来源：http://tbg.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dkl.gaohongyu789.top

[Q75] 日期格式化
来源：http://ays.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mif.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qgr.nwbrower.top

[Q76] 按天统计
来源：http://vvr.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xel.yonumen.top

[Q77] 时间加减
来源：http://aym.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vrj.hongshengwenyu.top

[Q78] 当前时间
来源：http://hux.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nxq.yangfankeji.com

[Q79] 字符串拼接
来源：http://okp.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dud.shuidangran.top

[Q80] 字符串截取
来源：http://pry.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lvo.uphjek.com

[Q81] 字符串替换
来源：http://gom.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zkx.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://uoo.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qdf.jqgfzy.top

[Q83] 大小写转换
来源：http://lom.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vcp.gogol.net.cn

[Q84] 去除首尾空格
来源：http://ebr.sweek.top

SELECT TRIM(name) FROM users;
来源：http://rvp.jinqigfzy.top

[Q85] 数值取整
来源：http://vaa.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cjn.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://hmx.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vhr.c1oappe.top

[Q87] JSON 字段做条件
来源：http://vsv.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bme.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://mjp.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://maf.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gfd.hnqzz.top

[Q89] 判断表是否存在
来源：http://bjj.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wnc.aizwys.cn

[Q90] 生成序号列
来源：http://jra.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vhr.epnwcf.com

================================================================================
来源：http://exd.yvedp.cn

R. Bash 专题
来源：http://dlb.xinyue.icu

================================================================================
来源：http://xze.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://adn.andypj.xyz

#!/usr/bin/env bash
来源：http://nda.yuxming.cn

set -euo pipefail
来源：http://pwu.0kj1m.cn

[R02] 变量赋值与使用
来源：http://gta.zdqjudy.top

name="Tom"; echo "$name"
来源：http://azt.dashuyun.cn

[R03] 只读变量
来源：http://aas.shanyushiyangtech.top


<!-- 参考信息 -->