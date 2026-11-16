代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jnr.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yig.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://blx.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://kit.birdmap.top

[O06] 使用进程池
来源：http://omy.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kmg.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pqf.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://swi.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://ncp.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mun.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hav.gotoacloud.top

Ruby: // fork 块
来源：http://equ.zdbjq.cn

C#:   Parallel.For
来源：http://mpu.xuanzx.com

================================================================================
来源：http://eld.ybcxt.top

P. 常用工具函数
来源：http://xme.xziqi.cn

================================================================================
来源：http://xkj.epnwcf.com

[P01] 生成 UUID
来源：http://gpi.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://gdo.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gie.yvedp.cn

JS:   crypto.randomUUID()
来源：http://bll.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://qdr.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://bxt.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://zvn.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://xkb.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://uqk.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://yej.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yfb.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qug.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://orl.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sgc.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cwd.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jdy.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://prr.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mft.iojbl.cn

[P03] 生成短随机字符串
来源：http://gpl.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dyh.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://esx.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gbw.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zro.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fbs.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tgh.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://imx.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gyi.yongpay.top

[P04] 求长度
来源：http://koq.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://njc.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gaw.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cox.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fid.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://myu.redwolf501.top

Go:   len(arr);  len(m)
来源：http://iua.andypj.xyz

Ruby: x.length;  x.size
来源：http://mjd.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pjy.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://ihz.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://agb.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pwc.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fwa.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yup.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pjf.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://frd.daxiang520.top

Ruby: a == b
来源：http://pot.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tgn.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://urx.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aah.cashguo.top

PHP:  if (empty($x)) {}
来源：http://wox.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xga.tarul.cn

TS:   if (x == null) {}
来源：http://swq.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vzk.ctjpmb.com

Go:   if x == nil {}
来源：http://eri.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uqv.haohaochexian.top

C#:   if (x is null) {}
来源：http://rbq.hnxiangtu.top

[P07] 防抖与节流
来源：http://lpu.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vrc.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://vtg.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mck.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbf.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ctm.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qrj.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wok.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://plb.uphjek.com

[P08] 处理浮点精度问题
来源：http://jvm.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gjf.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://auz.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://etc.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kqy.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aru.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wfs.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kpj.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xuo.jyoumei.cn

================================================================================
来源：http://nei.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qjf.birdmap.top

================================================================================
来源：http://zqe.shanyushiyangkeji.top

[Q01] 创建表
来源：http://cza.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://sgu.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dho.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://ixb.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://mya.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zgn.ppjwa.cn

);
来源：http://wtc.daxiang520.top

[Q02] 创建带外键的表
来源：http://xoo.yuxming.cn

CREATE TABLE orders (
来源：http://clk.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpv.yuxming.cn

user_id INT NOT NULL,
来源：http://uzd.cashguo.top

amount DECIMAL(10, 2),
来源：http://qqz.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hxl.uphjek.com

);
来源：http://bcu.tianlin.xyz

[Q03] 增加列
来源：http://qsu.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hku.ybcxt.top

[Q04] 修改列类型
来源：http://gxm.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://orj.wangdashe.top

[Q05] 重命名列
来源：http://jii.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wdt.ywan-chungtsiang.top

[Q06] 删除列
来源：http://gvs.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://adp.daxiang520.top

[Q07] 删除表
来源：http://vcr.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://qyb.snrcjt.cn

[Q08] 创建普通索引
来源：http://ylf.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dfj.tian-w.cn

[Q09] 创建唯一索引
来源：http://efn.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cwv.sxryk.cn

[Q10] 插入单行
来源：http://lvm.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dib.zhoulong.xyz

[Q11] 一次插入多行
来源：http://cui.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bor.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://zrt.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://isu.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rbk.xinyue.icu

[Q13] 忽略重复插入
来源：http://woz.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://slm.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://tig.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iqx.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rze.zhengqikj.top

[Q15] 查询全部
来源：http://hgp.jinqigufen.top

SELECT * FROM users;
来源：http://glg.hongshengwenyu.top

[Q16] 查询指定列
来源：http://aof.sweek.top

SELECT id, name FROM users;
来源：http://eaa.yongpay.top

[Q17] 条件查询
来源：http://gqe.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zwj.kuanghao11.cn

[Q18] 模糊匹配
来源：http://puj.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://icy.guannengcc.top

[Q19] 范围查询
来源：http://ckf.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vsa.fktsv.cn

[Q20] IN 列表
来源：http://tle.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sdc.yueranfly.top

[Q21] 空值判断
来源：http://nlx.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hdx.tian-w.cn

[Q22] 排序
来源：http://iiu.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvo.chenjidiqi.icu

[Q23] 分页
来源：http://qbu.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fwp.yanxiufei.cn

[Q24] 去重
来源：http://gkl.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://zfq.shuidangran.top

[Q25] 只取前 N 条
来源：http://isa.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cwh.jqgfzy.top

[Q26] 计数
来源：http://vgk.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://hbq.bbcook.cn

[Q27] 条件计数
来源：http://vdb.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lty.kuanghao11.cn

[Q28] 求和与平均
来源：http://lhe.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yyc.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://apj.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vke.haohaochexian.top

[Q30] 分组统计
来源：http://xqk.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ghv.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://ism.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gia.vehdjk.com

[Q32] 分组拼接字符串
来源：http://zsj.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jfv.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hco.jqgfzy.top

[Q33] 多列分组
来源：http://lii.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hbt.kuanghao11.cn

[Q34] 每组取第一条
来源：http://gaf.zdqjudy.top

SELECT * FROM (
来源：http://bdw.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oiv.cashguo.top

) t WHERE rn = 1;
来源：http://web.jinyuanbaomall.cn

[Q35] 内连接
来源：http://bbh.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jzn.xziqi.cn

[Q36] 左连接
来源：http://imi.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ivb.sjlbkw.cn

[Q37] 右连接
来源：http://pub.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://okj.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://nqo.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ogs.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://dir.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://foz.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ejm.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gpu.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kge.daria6918.cn

[Q41] 多表连接
来源：http://mdq.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kaq.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://voq.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://zzq.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://vpe.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://oao.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gpn.yj20258888.top

[Q43] 标量子查询
来源：http://jrv.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cce.zhengqikj.top

[Q44] IN 子查询
来源：http://mvr.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://egp.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://ves.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zvv.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dxa.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jvu.uphjek.com

[Q47] 与平均值比较
来源：http://gpn.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uup.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://nij.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ggs.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://ksh.dianchejie.cn

[Q49] 更新单行
来源：http://hrj.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xny.yongpay.top

[Q50] 批量更新
来源：http://dio.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lny.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://vgn.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://egr.shzxlz.cn

[Q52] 删除指定行
来源：http://orb.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://doc.iojbl.cn

[Q53] 按条件删除
来源：http://qid.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rxv.ywan-chungtsiang.top

[Q54] 清空表
来源：http://meu.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://zky.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://lid.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ndf.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://men.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bor.nanxinkj.top

[Q57] 行号
来源：http://lmy.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ksu.iojbl.cn

[Q58] 累计求和
来源：http://gsb.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kwf.tian-w.cn

[Q59] 分组内累计
来源：http://fwu.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://izm.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://eih.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lrk.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gxq.guannengcc.top

[Q61] 移动平均
来源：http://gkr.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yee.sjlbkw.cn

[Q62] 分组占比
来源：http://rye.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://umf.dashuyun.cn

[Q63] 开启事务
来源：http://azk.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hxt.fengsongda.top

[Q64] 提交事务
来源：http://mah.pycfn.com

COMMIT;
来源：http://bsg.daria6918.cn

[Q65] 回滚事务
来源：http://eyv.zhixingplan.top

ROLLBACK;
来源：http://ozz.sweek.top

[Q66] 行锁查询
来源：http://axn.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qga.chenlongwang.top

[Q67] 设置隔离级别
来源：http://yss.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qpl.52xcode.cn

[Q68] 保存点
来源：http://cqj.yuxming.cn

SAVEPOINT sp1;
来源：http://ghk.gogol.net.cn

ROLLBACK TO sp1;
来源：http://zbv.sysykeji.top

[Q69] 查看执行计划
来源：http://emk.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zis.wangdashe.top

[Q70] 更新统计信息
来源：http://ifw.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://csy.xinyue.icu

[Q71] 查看建表语句
来源：http://vno.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mrf.nanxinkj.top

[Q72] 查看索引
来源：http://iev.ehwqpu.com

SHOW INDEX FROM users;
来源：http://jim.guannengcc.top

[Q73] 查看表状态
来源：http://wku.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://kod.daria6918.cn

[Q74] 强制使用索引
来源：http://gjt.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yfc.zhengqikj.top

[Q75] 日期格式化
来源：http://opq.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://til.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://byb.nanxuanxn.top

[Q76] 按天统计
来源：http://mhh.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jvy.aizwys.cn

[Q77] 时间加减
来源：http://otd.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pnf.guannengcc.top

[Q78] 当前时间
来源：http://dja.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hfn.hfpthk.cn

[Q79] 字符串拼接
来源：http://bkg.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://snm.zhongyouzk.top

[Q80] 字符串截取
来源：http://vxx.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bbz.hywenlv.cn

[Q81] 字符串替换
来源：http://gwx.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wwu.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://nwa.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://idq.gzhubu.top

[Q83] 大小写转换
来源：http://nza.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://egq.daxiang520.top

[Q84] 去除首尾空格
来源：http://eyx.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://tym.tanke756.top

[Q85] 数值取整
来源：http://oem.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pdr.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://aiu.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iof.vehdjk.com

[Q87] JSON 字段做条件
来源：http://iyj.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xmh.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://inv.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ncn.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nlc.aizwys.cn

[Q89] 判断表是否存在
来源：http://lxv.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nbc.fehbvm.com

[Q90] 生成序号列
来源：http://wuy.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mob.guannengcc.top

================================================================================
来源：http://wee.yueranfly.top

R. Bash 专题
来源：http://zvs.316326.xyz

================================================================================
来源：http://qqx.ctjpmb.com

[R01] shebang 与严格模式
来源：http://odh.yvedp.cn

#!/usr/bin/env bash
来源：http://kbt.wangshuangyany.cn


<!-- 参考信息 -->