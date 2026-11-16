代发 wailian999

[O06] 使用进程池
来源：http://ezl.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://osx.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mku.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://zec.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://dux.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qsc.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tfs.fktsv.cn

Ruby: // fork 块
来源：http://dae.fehbvm.com

C#:   Parallel.For
来源：http://gos.jqgfzy.top

================================================================================
来源：http://kmc.wangshuangyany.cn

P. 常用工具函数
来源：http://zma.sweek.top

================================================================================
来源：http://eym.smart0.xyz

[P01] 生成 UUID
来源：http://xel.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://sbe.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://joj.shuidangran.top

JS:   crypto.randomUUID()
来源：http://orj.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://dsu.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://jhw.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://qlg.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://wvx.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://lnm.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://waf.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vfz.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rpz.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tbi.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://npu.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ngw.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sre.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://euw.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uhw.cheryme.top

[P03] 生成短随机字符串
来源：http://ycw.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://apw.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aqv.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xap.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zjw.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nwr.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tzo.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sry.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hqb.meibo888.top

[P04] 求长度
来源：http://zys.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dpb.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kbt.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://red.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uqb.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ybw.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://gag.chenzaomai.com

Ruby: x.length;  x.size
来源：http://auw.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dfi.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://pgb.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://vau.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://izw.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iub.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uau.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kxg.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bmu.zhongyouzk.top

Ruby: a == b
来源：http://mmd.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rhq.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yme.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lvu.316326.xyz

PHP:  if (empty($x)) {}
来源：http://ibk.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ewl.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://qpc.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vuu.pycfn.com

Go:   if x == nil {}
来源：http://yqg.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://urq.gotoacloud.top

C#:   if (x is null) {}
来源：http://cca.feifeiyinyue.top

[P07] 防抖与节流
来源：http://fpr.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tho.birdmap.top

PHP:  // 手写时间戳比较
来源：http://wmg.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tss.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://frc.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xzq.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qis.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://und.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kcb.ydzc1.top

[P08] 处理浮点精度问题
来源：http://ijj.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mel.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zui.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://njd.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iya.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://chj.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xra.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://maf.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dsw.jianghu66.top

================================================================================
来源：http://gww.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eop.jinghuilouyu.cn

================================================================================
来源：http://gul.vehdjk.com

[Q01] 创建表
来源：http://vdq.xinyue.icu

CREATE TABLE users (
来源：http://wxk.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zpr.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://qtq.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://dol.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cvq.jiagoushi.top

);
来源：http://hrv.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://eyx.chenlongwang.top

CREATE TABLE orders (
来源：http://uoz.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qna.gotoacloud.top

user_id INT NOT NULL,
来源：http://yhk.andypj.xyz

amount DECIMAL(10, 2),
来源：http://ehu.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rjp.sjlbkw.cn

);
来源：http://twa.smart0.xyz

[Q03] 增加列
来源：http://csv.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bac.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://zes.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://trl.yonumen.top

[Q05] 重命名列
来源：http://orl.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zpt.fehbvm.com

[Q06] 删除列
来源：http://gxh.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://jxq.shzxlz.cn

[Q07] 删除表
来源：http://fln.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://moo.316326.xyz

[Q08] 创建普通索引
来源：http://boq.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://att.wangdashe.top

[Q09] 创建唯一索引
来源：http://aoc.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ilm.9152youxi.cn

[Q10] 插入单行
来源：http://mfp.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ptx.hysaishi.cn

[Q11] 一次插入多行
来源：http://iks.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://flr.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://ylc.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://taj.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://obx.xuanzx.com

[Q13] 忽略重复插入
来源：http://frz.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ahj.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://fkm.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sjt.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iqz.ybcxt.top

[Q15] 查询全部
来源：http://xug.shangyingyoupin.top

SELECT * FROM users;
来源：http://abh.316326.xyz

[Q16] 查询指定列
来源：http://kso.wangdashe.top

SELECT id, name FROM users;
来源：http://bda.zhoulong.xyz

[Q17] 条件查询
来源：http://que.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://idi.gotoacloud.top

[Q18] 模糊匹配
来源：http://lny.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://byk.cucudq.cn

[Q19] 范围查询
来源：http://syt.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fdp.sxryk.cn

[Q20] IN 列表
来源：http://crg.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kak.vehdjk.com

[Q21] 空值判断
来源：http://pby.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tjx.nanxinkj.top

[Q22] 排序
来源：http://npq.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://arp.chenjidiqi.icu

[Q23] 分页
来源：http://yyl.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wyh.yuanzhike.top

[Q24] 去重
来源：http://mfs.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://sfk.shzxlz.cn

[Q25] 只取前 N 条
来源：http://pae.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ghq.tanke756.top

[Q26] 计数
来源：http://bhb.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://vgl.yueranfly.top

[Q27] 条件计数
来源：http://ssm.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gze.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://zyb.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://phb.uphjek.com

[Q29] 最大最小值
来源：http://iej.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ehz.0kj1m.cn

[Q30] 分组统计
来源：http://ylu.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://skg.ybcxt.top

[Q31] 分组后过滤
来源：http://frd.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ymw.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://tge.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://euy.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dxn.ydjk.org.cn

[Q33] 多列分组
来源：http://oar.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://snn.fzhhl.top

[Q34] 每组取第一条
来源：http://phu.cdnleiting.top

SELECT * FROM (
来源：http://npp.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vku.0kj1m.cn

) t WHERE rn = 1;
来源：http://dhi.uphjek.com

[Q35] 内连接
来源：http://sig.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rro.tanke756.top

[Q36] 左连接
来源：http://ugv.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yku.zhongyouzk.top

[Q37] 右连接
来源：http://typ.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lzx.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qfv.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rgs.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://aji.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gqv.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rwe.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hur.andypj.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gbz.guannengcc.top

[Q41] 多表连接
来源：http://wun.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bqe.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://rnh.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://cjh.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://trl.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://uft.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dcf.yfazqb.com

[Q43] 标量子查询
来源：http://ulf.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pes.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://cky.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ndk.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://uej.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mrp.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ywi.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vcq.zhixingplan.top

[Q47] 与平均值比较
来源：http://kvd.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://awc.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://mqc.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rlh.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://qhr.xziqi.cn

[Q49] 更新单行
来源：http://jvg.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ecl.0kj1m.cn

[Q50] 批量更新
来源：http://xej.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ixk.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://luw.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://njr.ydzc1.top

[Q52] 删除指定行
来源：http://xyg.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://oak.cheryme.top

[Q53] 按条件删除
来源：http://ieo.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bnr.snrcjt.cn

[Q54] 清空表
来源：http://snu.ydzc1.top

TRUNCATE TABLE logs;
来源：http://lxx.xinyue.icu

[Q55] 排名（并列占位）
来源：http://gej.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zwc.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://hcs.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://agq.sufxvd.cn

[Q57] 行号
来源：http://smo.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://man.hnqzz.top

[Q58] 累计求和
来源：http://grg.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tzi.aizwys.cn

[Q59] 分组内累计
来源：http://byl.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tdw.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://fhk.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fez.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bgn.wangshuangyany.cn

[Q61] 移动平均
来源：http://izg.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nek.kuanghao11.cn

[Q62] 分组占比
来源：http://alx.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oej.kuanghao11.cn

[Q63] 开启事务
来源：http://nbl.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ufg.haohaochexian.top

[Q64] 提交事务
来源：http://oxf.redwolf501.top

COMMIT;
来源：http://hlh.chenlongwang.top

[Q65] 回滚事务
来源：http://rwf.nwbrower.top

ROLLBACK;
来源：http://jst.tian-w.cn

[Q66] 行锁查询
来源：http://bmn.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jzw.0kj1m.cn

[Q67] 设置隔离级别
来源：http://qhf.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dmq.fktsv.cn

[Q68] 保存点
来源：http://izl.shzxlz.cn

SAVEPOINT sp1;
来源：http://dnp.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://ont.pycfn.com

[Q69] 查看执行计划
来源：http://zvw.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lpf.sufxvd.cn

[Q70] 更新统计信息
来源：http://nxt.zdbjq.cn

ANALYZE TABLE users;
来源：http://aic.yvedp.cn

[Q71] 查看建表语句
来源：http://phl.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://boy.ctjpmb.com

[Q72] 查看索引
来源：http://snw.daxiang520.top

SHOW INDEX FROM users;
来源：http://sno.havefunace.top

[Q73] 查看表状态
来源：http://wsf.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vgt.yongpay.top

[Q74] 强制使用索引
来源：http://agd.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ktq.fktsv.cn

[Q75] 日期格式化
来源：http://dut.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bic.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qqb.sysykeji.top

[Q76] 按天统计
来源：http://aze.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fmo.fengsongda.top

[Q77] 时间加减
来源：http://vbi.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tlc.xylfe.cn

[Q78] 当前时间
来源：http://itz.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://smv.aizwys.cn

[Q79] 字符串拼接
来源：http://xsc.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bzq.sxryk.cn

[Q80] 字符串截取
来源：http://lgm.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dvg.yanxiufei.cn

[Q81] 字符串替换
来源：http://djy.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sbn.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://jvh.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xqd.zdbjq.cn

[Q83] 大小写转换
来源：http://rny.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pan.jinqigufen.top

[Q84] 去除首尾空格
来源：http://tgq.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://rvt.chenjidiqi.icu

[Q85] 数值取整
来源：http://uls.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://udt.cashguo.top

[Q86] 读取 JSON 字段
来源：http://bmy.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oee.andypj.xyz

[Q87] JSON 字段做条件
来源：http://vkd.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oqr.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://nja.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cop.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xjt.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://gtc.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kgu.mhx1999.top

[Q90] 生成序号列
来源：http://qnl.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gul.sxryk.cn

================================================================================
来源：http://wfx.daxiang520.top

R. Bash 专题
来源：http://cov.cdnleiting.top

================================================================================
来源：http://qng.gzhubu.top

[R01] shebang 与严格模式
来源：http://vkc.zhijiandao.cn

#!/usr/bin/env bash
来源：http://mit.gaohongyu789.top

set -euo pipefail
来源：http://xos.sufxvd.cn

[R02] 变量赋值与使用
来源：http://kpc.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://ycl.zdbjq.cn

[R03] 只读变量
来源：http://jft.havefunace.top


<!-- 参考信息 -->