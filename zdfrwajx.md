代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://clk.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ybo.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://upf.316326.xyz

TS:   // 同 JS
来源：http://wju.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://eaa.bbcook.cn

Go:   go f()
来源：http://ube.haohaochexian.top

Ruby: Thread.new { f }
来源：http://fmr.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://amp.jyoumei.cn

[O02] 使用线程池
来源：http://mly.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://prs.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ciy.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://huw.meibo888.top

TS:   // worker_threads 线程池
来源：http://tgh.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bqp.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ahs.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dnp.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://icj.hcnkem.com

[O03] 加锁保护共享数据
来源：http://oag.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://mlp.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://htm.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://faq.jqgufenzy.top

TS:   // 同 JS
来源：http://wua.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://xwe.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nax.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://iva.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://csn.mhx1999.top

[O04] 定义异步函数并等待
来源：http://wko.yj20258.top

Py:   async def f():⏎    await g()
来源：http://hwr.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jdr.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://agc.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://igc.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://afl.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://urm.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cla.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://ixm.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://qvi.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://ovj.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rwl.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://pli.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://zmy.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cxx.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vzr.hammf.cn

Ruby: threads.map(&:join)
来源：http://dvh.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://don.meibo888.top

[O06] 使用进程池
来源：http://wud.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yua.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uyw.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://ptf.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://zue.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jia.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mpx.yangfankeji.com

Ruby: // fork 块
来源：http://eyu.yueranfly.top

C#:   Parallel.For
来源：http://gsg.zhengqikj.top

================================================================================
来源：http://akc.jyoumei.cn

P. 常用工具函数
来源：http://gjv.sjlbkw.cn

================================================================================
来源：http://ose.cheryme.top

[P01] 生成 UUID
来源：http://nuc.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://cbm.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zeq.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://okl.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://smn.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://lcu.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://gvj.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://vsk.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://iqx.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://rsp.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zbt.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://sxn.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blo.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fpm.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ldr.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ssb.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cmw.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vqy.zycfv.cn

[P03] 生成短随机字符串
来源：http://oiq.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kkg.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wve.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://koo.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lud.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gri.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zvq.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://msf.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kud.redwolf501.top

[P04] 求长度
来源：http://fpl.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oun.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwj.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yrg.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hcq.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://zpb.havefunace.top

Go:   len(arr);  len(m)
来源：http://sbl.dashuyun.cn

Ruby: x.length;  x.size
来源：http://pqp.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gkm.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://nkt.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vph.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://suv.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yzi.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dlb.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dpb.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://fec.nwbrower.top

Ruby: a == b
来源：http://ogc.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cbk.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fvi.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://clp.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://loh.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yoq.xinyue.icu

TS:   if (x == null) {}
来源：http://unu.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://uaq.svipenyu.cn

Go:   if x == nil {}
来源：http://ono.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://klp.guowangkeji.top

C#:   if (x is null) {}
来源：http://trn.ctjpmb.com

[P07] 防抖与节流
来源：http://pit.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xrd.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://zet.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vxs.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sro.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tlj.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nzt.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lfb.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jly.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://qej.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gzu.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zyl.epnwcf.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xod.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ezp.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cdr.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xwa.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tbw.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pfo.zhengqikj.top

================================================================================
来源：http://hyt.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://txq.mhx1999.top

================================================================================
来源：http://vof.meibo888.top

[Q01] 创建表
来源：http://cmm.dianchejie.cn

CREATE TABLE users (
来源：http://yxj.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://czg.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://fpg.shanyushiyangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://bsl.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qwn.ydjk.org.cn

);
来源：http://ksi.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://znh.yueranfly.top

CREATE TABLE orders (
来源：http://juq.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dkn.xylfe.cn

user_id INT NOT NULL,
来源：http://pxd.yonumen.top

amount DECIMAL(10, 2),
来源：http://lps.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mmi.xuanzx.com

);
来源：http://iii.jlsjyb.cn

[Q03] 增加列
来源：http://qcs.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ecy.smart0.xyz

[Q04] 修改列类型
来源：http://vpa.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hvt.bjfxy.top

[Q05] 重命名列
来源：http://wii.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wxw.vehdjk.com

[Q06] 删除列
来源：http://ymx.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kvw.xinyue.icu

[Q07] 删除表
来源：http://jfr.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://lzy.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://htx.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bpd.shuidangran.top

[Q09] 创建唯一索引
来源：http://viq.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ddh.sweek.top

[Q10] 插入单行
来源：http://rqd.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dje.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://gmi.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kpz.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://cmm.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xam.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fib.daria6918.cn

[Q13] 忽略重复插入
来源：http://bgo.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nkg.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://pcu.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gdz.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zmt.jinqigfzy.top

[Q15] 查询全部
来源：http://gpw.zhiwuduotai.top

SELECT * FROM users;
来源：http://irt.daria6918.cn

[Q16] 查询指定列
来源：http://qru.ivvv.top

SELECT id, name FROM users;
来源：http://zqt.zdbjq.cn

[Q17] 条件查询
来源：http://cce.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yxf.chenlongwang.top

[Q18] 模糊匹配
来源：http://hfy.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eya.yonumen.top

[Q19] 范围查询
来源：http://ipf.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mhb.wangshuangyany.cn

[Q20] IN 列表
来源：http://raa.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zcf.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://qos.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wkk.zdqjudy.top

[Q22] 排序
来源：http://duw.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cit.vehdjk.com

[Q23] 分页
来源：http://bdw.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uxp.aibaodan.cn

[Q24] 去重
来源：http://ute.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://xdu.meibo888.top

[Q25] 只取前 N 条
来源：http://ytt.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jbp.sysykeji.top

[Q26] 计数
来源：http://jea.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://qkz.fehbvm.com

[Q27] 条件计数
来源：http://oww.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oma.hesvh.cn

[Q28] 求和与平均
来源：http://met.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jqp.dashuyun.cn

[Q29] 最大最小值
来源：http://afh.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mze.chenjidiqi.icu

[Q30] 分组统计
来源：http://sxv.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ukq.andypj.xyz

[Q31] 分组后过滤
来源：http://ksj.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ngu.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://xuc.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sun.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ydo.aizwys.cn

[Q33] 多列分组
来源：http://saf.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://njl.daria6918.cn

[Q34] 每组取第一条
来源：http://uqc.yj20258888.top

SELECT * FROM (
来源：http://ken.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://roc.xinyue.icu

) t WHERE rn = 1;
来源：http://vly.jqgfzy.top

[Q35] 内连接
来源：http://yxj.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lkg.dashuyun.cn

[Q36] 左连接
来源：http://fep.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ara.guannengcc.top

[Q37] 右连接
来源：http://mik.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dxo.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://pva.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jnk.aizwys.cn

[Q39] 自连接（查上下级）
来源：http://pfk.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wey.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://klk.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://jpg.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://woo.jiagoushi.top

[Q41] 多表连接
来源：http://cvv.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dux.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://bps.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://qya.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://xsk.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://edv.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bsz.dashuyun.cn

[Q43] 标量子查询
来源：http://wrc.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lvu.smart0.xyz

[Q44] IN 子查询
来源：http://biz.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rbt.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://obn.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gan.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://hud.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://voa.bbcook.cn

[Q47] 与平均值比较
来源：http://mbe.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xuc.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://sgz.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uyf.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://hky.feifeiyinyue.top

[Q49] 更新单行
来源：http://cdy.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pli.jinqigufen.top

[Q50] 批量更新
来源：http://ujb.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://unx.hnqzz.top

[Q51] 用子查询更新
来源：http://egy.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ifo.xziqi.cn

[Q52] 删除指定行
来源：http://amb.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://xbh.hcnkem.com

[Q53] 按条件删除
来源：http://qda.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qxi.tianlin.xyz

[Q54] 清空表
来源：http://exr.yj20258.top

TRUNCATE TABLE logs;
来源：http://neu.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://hkf.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ahj.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://ooi.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ueh.snrcjt.cn

[Q57] 行号
来源：http://elv.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ntt.aizwys.cn

[Q58] 累计求和
来源：http://qpi.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ebv.xinyue.icu

[Q59] 分组内累计
来源：http://pxs.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bnw.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://ope.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uon.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://diz.gzhubu.top

[Q61] 移动平均
来源：http://ieb.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://roo.zhoulong.xyz

[Q62] 分组占比
来源：http://olt.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ozg.kuanghao11.cn

[Q63] 开启事务
来源：http://uel.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yvz.aizwys.cn

[Q64] 提交事务
来源：http://oea.52xcode.cn

COMMIT;
来源：http://ulh.hnqzz.top

[Q65] 回滚事务
来源：http://jun.yj20258.top

ROLLBACK;
来源：http://bjj.kuanghao11.cn

[Q66] 行锁查询
来源：http://afe.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://elz.yj20258.top

[Q67] 设置隔离级别
来源：http://rjm.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ets.wangshuangyany.cn

[Q68] 保存点
来源：http://ydt.sweek.top

SAVEPOINT sp1;
来源：http://juf.yvedp.cn

ROLLBACK TO sp1;
来源：http://bhs.daria6918.cn

[Q69] 查看执行计划
来源：http://rno.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aoq.vqdsnc.cn

[Q70] 更新统计信息
来源：http://xjj.tianlin.xyz

ANALYZE TABLE users;
来源：http://cxo.zdqjudy.top

[Q71] 查看建表语句
来源：http://rlk.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vgv.daxiang520.top

[Q72] 查看索引
来源：http://ocb.jqgfzy.top

SHOW INDEX FROM users;
来源：http://dvv.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://cnu.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rcd.hysaishi.cn

[Q74] 强制使用索引
来源：http://dis.chenzaomai.com


<!-- 参考信息 -->