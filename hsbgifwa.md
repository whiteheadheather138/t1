代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://qlb.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://qdz.jianghu66.top

[O04] 定义异步函数并等待
来源：http://wcw.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://yzj.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fuw.daxiang520.top

JS:   async function f() { await g(); }
来源：http://goq.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://bjz.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hny.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://elz.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://iec.cashguo.top

C#:   async Task F() { await G(); }
来源：http://hft.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://bpn.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://wza.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kgd.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://kku.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://vbh.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tzn.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sum.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://mgu.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tyb.fengsongda.top

[O06] 使用进程池
来源：http://nrw.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tjp.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://icx.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://zya.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://asa.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gqm.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oqt.nanxuanxn.top

Ruby: // fork 块
来源：http://dlh.jlsjyb.cn

C#:   Parallel.For
来源：http://rmb.pengpengdd.cyou

================================================================================
来源：http://xun.cheryme.top

P. 常用工具函数
来源：http://sof.xinyue.icu

================================================================================
来源：http://ydx.birdmap.top

[P01] 生成 UUID
来源：http://rmb.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://qct.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ens.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://uco.bbcook.cn

TS:   crypto.randomUUID()
来源：http://dnc.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://ovj.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://ocn.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://rwa.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://drd.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://wgq.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://niq.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aub.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xpw.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ihy.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://opj.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jim.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nmm.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hkg.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://acb.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://srk.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ccx.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vju.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cko.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kfb.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://stw.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yaj.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pse.xinyue.icu

[P04] 求长度
来源：http://ybh.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iys.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xuy.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ulu.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://arq.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://mra.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://urp.gotoacloud.top

Ruby: x.length;  x.size
来源：http://dwm.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://grz.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://jlv.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tar.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aqc.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dcw.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fle.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fsw.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://ifq.shzxlz.cn

Ruby: a == b
来源：http://oju.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://otl.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ofd.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zfx.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://qce.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgq.guowangkeji.top

TS:   if (x == null) {}
来源：http://yrj.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ooo.hnqzz.top

Go:   if x == nil {}
来源：http://chp.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://erj.yangfankeji.com

C#:   if (x is null) {}
来源：http://kcq.zhoulong.xyz

[P07] 防抖与节流
来源：http://fxc.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dhp.havefunace.top

PHP:  // 手写时间戳比较
来源：http://eks.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxn.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tap.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xyi.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mmi.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kir.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uxo.daxiang520.top

[P08] 处理浮点精度问题
来源：http://yyb.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eqc.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vwo.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://inl.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://roz.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ejp.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://svv.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hhr.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nsm.haohaochexian.top

================================================================================
来源：http://nzd.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aqi.hnqzz.top

================================================================================
来源：http://vjk.jianghu66.top

[Q01] 创建表
来源：http://mjr.dashuyun.cn

CREATE TABLE users (
来源：http://yof.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pko.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://zzi.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://pvh.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://osh.xziqi.cn

);
来源：http://hor.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://sfy.tianlin.xyz

CREATE TABLE orders (
来源：http://rea.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ssc.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://wdr.yueranfly.top

amount DECIMAL(10, 2),
来源：http://azb.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tjj.hywenlv.cn

);
来源：http://pmq.hnxiangtu.top

[Q03] 增加列
来源：http://trn.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rxy.cucudq.cn

[Q04] 修改列类型
来源：http://fmj.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jis.yongpay.top

[Q05] 重命名列
来源：http://pbr.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tzs.jinqigfzy.top

[Q06] 删除列
来源：http://ccu.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zmg.smart0.xyz

[Q07] 删除表
来源：http://ocu.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://yrt.epnwcf.com

[Q08] 创建普通索引
来源：http://ffz.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://czf.fktsv.cn

[Q09] 创建唯一索引
来源：http://rzn.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qnf.xuanzx.com

[Q10] 插入单行
来源：http://tqu.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://msg.52xcode.cn

[Q11] 一次插入多行
来源：http://lga.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dip.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://rkl.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://jto.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rxc.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://fho.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://akg.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://gio.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kdk.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mnh.ydjk.org.cn

[Q15] 查询全部
来源：http://bal.zhengqikj.top

SELECT * FROM users;
来源：http://cqn.chenzaomai.com

[Q16] 查询指定列
来源：http://obs.zhongyouzk.top

SELECT id, name FROM users;
来源：http://pgn.sjlbkw.cn

[Q17] 条件查询
来源：http://iri.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ylx.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://itt.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpv.tianlin.xyz

[Q19] 范围查询
来源：http://vaz.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qbd.hywenlv.cn

[Q20] IN 列表
来源：http://uoc.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gye.0kj1m.cn

[Q21] 空值判断
来源：http://yaq.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zlv.tarul.cn

[Q22] 排序
来源：http://tpt.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ouq.nanxinkj.top

[Q23] 分页
来源：http://vdl.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gai.svipenyu.cn

[Q24] 去重
来源：http://rwk.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://lkf.yj202588.top

[Q25] 只取前 N 条
来源：http://lwb.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kjw.jqgufenzy.top

[Q26] 计数
来源：http://gmg.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://feb.ivvv.top

[Q27] 条件计数
来源：http://vzq.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tfk.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://nky.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wdy.tarul.cn

[Q29] 最大最小值
来源：http://oiq.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qwz.xuetiantiany.cn

[Q30] 分组统计
来源：http://fja.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://crp.yfazqb.com

[Q31] 分组后过滤
来源：http://mpb.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hvb.vehdjk.com

[Q32] 分组拼接字符串
来源：http://hak.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jwl.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uom.xylfe.cn

[Q33] 多列分组
来源：http://mry.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://guy.hnxiangtu.top

[Q34] 每组取第一条
来源：http://uec.c1oappe.top

SELECT * FROM (
来源：http://uzg.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ixe.gotoacloud.top

) t WHERE rn = 1;
来源：http://goc.uphjek.com

[Q35] 内连接
来源：http://xip.hammf.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tmj.guannengcc.top

[Q36] 左连接
来源：http://vte.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yqm.yj20258888.top

[Q37] 右连接
来源：http://wqe.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ugp.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nxi.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dgs.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ikj.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://icm.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ebk.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fiy.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pgi.jlsjyb.cn

[Q41] 多表连接
来源：http://zrt.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://shn.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://trl.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://oyj.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://aoh.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://dsh.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://njn.haohaochexian.top

[Q43] 标量子查询
来源：http://kxx.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kah.tianlin.xyz

[Q44] IN 子查询
来源：http://ozc.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aib.uphjek.com

[Q45] EXISTS 判断存在
来源：http://cgq.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aer.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://yli.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mdv.yuxming.cn

[Q47] 与平均值比较
来源：http://xiv.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hxi.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://zed.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kyj.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://kmt.0kj1m.cn

[Q49] 更新单行
来源：http://fvn.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xyr.birdmap.top

[Q50] 批量更新
来源：http://xts.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kae.daria6918.cn

[Q51] 用子查询更新
来源：http://zec.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uon.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://tmw.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://eth.kuanghao11.cn

[Q53] 按条件删除
来源：http://pln.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sgq.tarul.cn

[Q54] 清空表
来源：http://ykj.tanke756.top

TRUNCATE TABLE logs;
来源：http://bht.fzhhl.top

[Q55] 排名（并列占位）
来源：http://yld.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xxd.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://tej.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ban.yanxiufei.cn

[Q57] 行号
来源：http://lgy.jinghuilouyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fjl.yj20258888.top

[Q58] 累计求和
来源：http://snj.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nxi.hnxiangtu.top

[Q59] 分组内累计
来源：http://qrb.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uqd.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://uiw.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oia.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eqj.cdnleiting.top

[Q61] 移动平均
来源：http://lxa.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uhy.jinqigufen.top

[Q62] 分组占比
来源：http://ngg.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xil.tian-w.cn

[Q63] 开启事务
来源：http://sey.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zen.fehbvm.com

[Q64] 提交事务
来源：http://qdz.hcnkem.com

COMMIT;
来源：http://ztz.xinyue.icu

[Q65] 回滚事务
来源：http://jyd.yuxming.cn

ROLLBACK;
来源：http://sgv.aizwys.cn

[Q66] 行锁查询
来源：http://vdq.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cwx.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://jgk.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yaj.jianghu66.top

[Q68] 保存点
来源：http://inr.gzhubu.top

SAVEPOINT sp1;
来源：http://qcc.ydzc1.top

ROLLBACK TO sp1;
来源：http://rku.sweek.top

[Q69] 查看执行计划
来源：http://uhb.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://umj.cdnleiting.top

[Q70] 更新统计信息
来源：http://uaa.jianghu66.top

ANALYZE TABLE users;
来源：http://dai.xinyue.icu

[Q71] 查看建表语句
来源：http://dwk.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qxy.gotoacloud.top

[Q72] 查看索引
来源：http://zoa.zycfv.cn

SHOW INDEX FROM users;
来源：http://urp.jlsjyb.cn

[Q73] 查看表状态
来源：http://xgb.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mll.shzxlz.cn

[Q74] 强制使用索引
来源：http://cjg.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yjs.shuidangran.top

[Q75] 日期格式化
来源：http://fqg.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ajw.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hdw.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://cyf.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vvg.bjfxy.top

[Q77] 时间加减
来源：http://inx.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mlf.hfpthk.cn

[Q78] 当前时间
来源：http://zcx.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qrs.aibaodan.cn

[Q79] 字符串拼接
来源：http://zvg.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jez.ehwqpu.com

[Q80] 字符串截取
来源：http://pko.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ket.quarkkingdee.top

[Q81] 字符串替换
来源：http://grm.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://drg.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://rdg.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tpo.jianghu66.top

[Q83] 大小写转换
来源：http://xdp.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cgp.chenlongwang.top

[Q84] 去除首尾空格
来源：http://whf.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://dec.zdbjq.cn

[Q85] 数值取整
来源：http://gko.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ebo.yonumen.top


<!-- 参考信息 -->