代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://qhf.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zem.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://ilq.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://ujg.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pdj.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gos.cheryme.top

Ruby: threads.map(&:join)
来源：http://bvg.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wmt.ctjpmb.com

[O06] 使用进程池
来源：http://shr.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wzt.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kbz.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://fmh.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://uxl.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uyd.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ufm.sxryk.cn

Ruby: // fork 块
来源：http://iuu.ppjwa.cn

C#:   Parallel.For
来源：http://ckq.jinqigfzy.top

================================================================================
来源：http://cez.yfazqb.com

P. 常用工具函数
来源：http://qkp.shzxlz.cn

================================================================================
来源：http://ubk.hammf.cn

[P01] 生成 UUID
来源：http://ceb.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://dxt.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bax.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://izf.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://itp.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://reg.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://vyu.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://iys.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://xul.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://ebp.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bxc.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jlr.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rjm.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vft.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fiy.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gwk.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rjl.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xag.316326.xyz

[P03] 生成短随机字符串
来源：http://ohi.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pbj.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mmq.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huu.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lgo.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jbu.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qkq.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fkv.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qen.shanyushiyangkeji.top

[P04] 求长度
来源：http://esn.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sml.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rmc.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ebx.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzi.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://chf.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://ntc.ppjwa.cn

Ruby: x.length;  x.size
来源：http://vzh.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oqb.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://ilm.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dms.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yhz.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pys.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pyw.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nle.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://ski.c1oappe.top

Ruby: a == b
来源：http://sbu.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rwo.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cmj.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ier.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://nyh.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gaw.andypj.xyz

TS:   if (x == null) {}
来源：http://tth.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mxr.yj20258.top

Go:   if x == nil {}
来源：http://oxq.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nnk.sjlbkw.cn

C#:   if (x is null) {}
来源：http://uay.ctjpmb.com

[P07] 防抖与节流
来源：http://eso.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sqv.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://qja.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbe.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://spf.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fdf.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mln.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nwe.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kpk.jiagoushi.top

[P08] 处理浮点精度问题
来源：http://yyd.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oer.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://phg.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kcd.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tmm.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bxj.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fso.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gst.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://guq.sufxvd.cn

================================================================================
来源：http://drq.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jrd.52xcode.cn

================================================================================
来源：http://smx.ydjk.org.cn

[Q01] 创建表
来源：http://hod.yangfankeji.com

CREATE TABLE users (
来源：http://mtv.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zts.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://yjz.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://ojv.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jjf.sysykeji.top

);
来源：http://uui.snrcjt.cn

[Q02] 创建带外键的表
来源：http://hye.shzxlz.cn

CREATE TABLE orders (
来源：http://mnr.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xuc.mhx1999.top

user_id INT NOT NULL,
来源：http://rbp.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://hhd.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://axp.cdnleiting.top

);
来源：http://ahi.pycfn.com

[Q03] 增加列
来源：http://oct.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://crx.guannengcc.top

[Q04] 修改列类型
来源：http://iku.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wip.epnwcf.com

[Q05] 重命名列
来源：http://ftn.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tyt.chenzaomai.com

[Q06] 删除列
来源：http://pul.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://oyc.xinyue.icu

[Q07] 删除表
来源：http://wkw.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://vvp.yanxiufei.cn

[Q08] 创建普通索引
来源：http://kdj.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jnl.chenzaomai.com

[Q09] 创建唯一索引
来源：http://obv.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rsm.vehdjk.com

[Q10] 插入单行
来源：http://kgf.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ghl.316326.xyz

[Q11] 一次插入多行
来源：http://soc.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rnp.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://pjz.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://dsn.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cki.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://ulq.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ygd.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://xkx.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mye.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lrw.hcnkem.com

[Q15] 查询全部
来源：http://clm.daxiang520.top

SELECT * FROM users;
来源：http://pms.ydjk.org.cn

[Q16] 查询指定列
来源：http://lfw.yuanzhike.top

SELECT id, name FROM users;
来源：http://opb.shanyushiyangtech.top

[Q17] 条件查询
来源：http://lml.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gxh.gaohongyu789.top

[Q18] 模糊匹配
来源：http://xvv.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://arn.tanke756.top

[Q19] 范围查询
来源：http://mvy.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qnz.vehdjk.com

[Q20] IN 列表
来源：http://edu.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mvd.xuetiantiany.cn

[Q21] 空值判断
来源：http://nvx.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ysw.wangdashe.top

[Q22] 排序
来源：http://tan.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://imz.jyoumei.cn

[Q23] 分页
来源：http://fvg.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://thc.cheryme.top

[Q24] 去重
来源：http://inb.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://ntc.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://rmf.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rst.bbcook.cn

[Q26] 计数
来源：http://uvw.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://dzl.vehdjk.com

[Q27] 条件计数
来源：http://jnw.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hyw.bbcook.cn

[Q28] 求和与平均
来源：http://fnr.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://una.vehdjk.com

[Q29] 最大最小值
来源：http://gcv.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ndn.yuxming.cn

[Q30] 分组统计
来源：http://suh.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dfd.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://jhy.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wxd.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://cfu.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vqn.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nad.sufxvd.cn

[Q33] 多列分组
来源：http://pbc.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eiv.gzhubu.top

[Q34] 每组取第一条
来源：http://dmx.cashguo.top

SELECT * FROM (
来源：http://dmn.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bcd.ydzc1.top

) t WHERE rn = 1;
来源：http://hyx.birdmap.top

[Q35] 内连接
来源：http://juk.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nqk.hywenlv.cn

[Q36] 左连接
来源：http://yad.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rqx.chenzaomai.com

[Q37] 右连接
来源：http://yep.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://srr.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://rvx.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nvt.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://qxn.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mtg.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://heq.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fng.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rjk.fzhhl.top

[Q41] 多表连接
来源：http://tir.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://uif.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://ohf.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://hao.birdmap.top

[Q42] 连接条件附加过滤
来源：http://dvb.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://spn.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lak.zhijiandao.cn

[Q43] 标量子查询
来源：http://edt.hnqzz.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jdr.hammf.cn

[Q44] IN 子查询
来源：http://wsl.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcr.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://dbx.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpo.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://rvp.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ubx.fehbvm.com

[Q47] 与平均值比较
来源：http://ckj.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://foj.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://tbm.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pba.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://dtn.meibo888.top

[Q49] 更新单行
来源：http://mna.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vyr.iojbl.cn

[Q50] 批量更新
来源：http://ihx.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tct.hysaishi.cn

[Q51] 用子查询更新
来源：http://xsj.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://frk.feifeiyinyue.top

[Q52] 删除指定行
来源：http://dnj.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://zrp.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://dpm.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dpa.nwbrower.top

[Q54] 清空表
来源：http://soe.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://jsd.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://oel.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yrl.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://klc.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lqr.yj202588.top

[Q57] 行号
来源：http://oty.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hvz.hywenlv.cn

[Q58] 累计求和
来源：http://nry.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://faq.jinqigfzy.top

[Q59] 分组内累计
来源：http://zuf.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ipe.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://vak.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wdo.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yvw.sysykeji.top

[Q61] 移动平均
来源：http://beu.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lqg.guowangkeji.top

[Q62] 分组占比
来源：http://bjw.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqj.ctjpmb.com

[Q63] 开启事务
来源：http://mwr.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mex.zhixingplan.top

[Q64] 提交事务
来源：http://jpn.jqgfzy.top

COMMIT;
来源：http://nnp.epnwcf.com

[Q65] 回滚事务
来源：http://mds.ywan-chungtsiang.top

ROLLBACK;
来源：http://nvs.jinqigufen.top

[Q66] 行锁查询
来源：http://zxz.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://opv.yuxming.cn

[Q67] 设置隔离级别
来源：http://xed.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tza.sjlbkw.cn

[Q68] 保存点
来源：http://gqo.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://uwb.yueranfly.top

ROLLBACK TO sp1;
来源：http://vyk.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://qik.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bvp.hesvh.cn

[Q70] 更新统计信息
来源：http://xol.havefunace.top

ANALYZE TABLE users;
来源：http://yef.cashguo.top

[Q71] 查看建表语句
来源：http://anf.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lka.cucudq.cn

[Q72] 查看索引
来源：http://bze.sweek.top

SHOW INDEX FROM users;
来源：http://hlm.zhijiandao.cn

[Q73] 查看表状态
来源：http://sva.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lvk.snrcjt.cn

[Q74] 强制使用索引
来源：http://wem.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sur.ehwqpu.com

[Q75] 日期格式化
来源：http://mib.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://thk.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yov.pengpengdd.cyou

[Q76] 按天统计
来源：http://mau.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hyf.zhongyouzk.top

[Q77] 时间加减
来源：http://ccc.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ucw.hesvh.cn

[Q78] 当前时间
来源：http://jff.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sau.smart0.xyz

[Q79] 字符串拼接
来源：http://yod.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lyz.nanxinkj.top

[Q80] 字符串截取
来源：http://fov.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://buf.ehwqpu.com

[Q81] 字符串替换
来源：http://ohe.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cad.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://wga.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hal.xylfe.cn

[Q83] 大小写转换
来源：http://yjf.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gmk.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://lbd.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://bmb.vehdjk.com

[Q85] 数值取整
来源：http://kfc.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jpz.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://alq.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rhi.havefunace.top

[Q87] JSON 字段做条件
来源：http://noq.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eok.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://uff.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vil.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://swk.c1oappe.top

[Q89] 判断表是否存在
来源：http://mom.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://akz.tianlin.xyz

[Q90] 生成序号列
来源：http://xjx.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://imr.tian-w.cn

================================================================================
来源：http://vty.wangshuangyany.cn


<!-- 参考信息 -->