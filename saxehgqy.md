代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://knr.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ysm.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fbr.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iez.snrcjt.cn

================================================================================
来源：http://iqw.havefunace.top

O. 并发与异步
来源：http://dlu.yonumen.top

================================================================================
来源：http://xev.daxiang520.top

[O01] 启动一个线程
来源：http://itz.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://btj.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lnd.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tab.hysaishi.cn

TS:   // 同 JS
来源：http://uuo.iojbl.cn

Java: new Thread(() -> f()).start()
来源：http://bqk.jinqigufen.top

Go:   go f()
来源：http://qiw.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://afa.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://aln.fengsongda.top

[O02] 使用线程池
来源：http://glu.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rmi.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uae.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://ecj.sxryk.cn

TS:   // worker_threads 线程池
来源：http://syx.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xzj.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blo.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wnw.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://loh.gzhubu.top

[O03] 加锁保护共享数据
来源：http://jkl.jinqigufen.top

Py:   with lock: shared += 1
来源：http://mgg.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://boo.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ikz.zhixingplan.top

TS:   // 同 JS
来源：http://tat.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://slq.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://myl.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vni.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://hpx.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://ivl.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://qae.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ytv.hnqzz.top

JS:   async function f() { await g(); }
来源：http://rkk.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pkq.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dyg.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xlh.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://src.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://jgq.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://jje.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://aui.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://izj.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://yzn.tarul.cn

TS:   await Promise.all(tasks)
来源：http://nfr.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://haa.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wjz.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://mpj.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://crz.fanxiaobao.xyz

[O06] 使用进程池
来源：http://dze.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vky.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://npi.meibo888.top

JS:   // child_process / cluster 模块
来源：http://rng.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://sma.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rtt.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cdf.zdqjudy.top

Ruby: // fork 块
来源：http://kla.xuanzx.com

C#:   Parallel.For
来源：http://bfq.yuanzhike.top

================================================================================
来源：http://wsn.sjlbkw.cn

P. 常用工具函数
来源：http://ywz.fktsv.cn

================================================================================
来源：http://hkt.c1oappe.top

[P01] 生成 UUID
来源：http://sno.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://wbz.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://foi.yongpay.top

JS:   crypto.randomUUID()
来源：http://nww.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://wkg.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://yqn.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://gzx.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://ahk.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://cmn.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://gkk.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xaw.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xzb.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://viu.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tek.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xbw.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://znk.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qot.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oto.xylfe.cn

[P03] 生成短随机字符串
来源：http://ekf.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fhd.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://itt.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vjt.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qbr.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://idf.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ruc.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dne.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iil.xylfe.cn

[P04] 求长度
来源：http://efh.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rlb.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://akw.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rad.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hng.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://tku.nwbrower.top

Go:   len(arr);  len(m)
来源：http://vwt.yvedp.cn

Ruby: x.length;  x.size
来源：http://zmn.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://shw.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://jqs.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wtx.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uwq.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ile.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aum.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bde.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tiy.hongshengwenyu.top

Ruby: a == b
来源：http://rvl.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hrr.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lsp.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vnb.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://qzu.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://doo.tianlin.xyz

TS:   if (x == null) {}
来源：http://uyt.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://jbt.chenjidiqi.icu

Go:   if x == nil {}
来源：http://can.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bbr.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://ebo.wangdashe.top

[P07] 防抖与节流
来源：http://ojw.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://doj.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://caw.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjl.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhp.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://htu.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gbi.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ybg.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mzu.hnqzz.top

[P08] 处理浮点精度问题
来源：http://eqi.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://feh.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kwt.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bus.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pcc.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://inf.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ncx.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mje.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ekn.pycfn.com

================================================================================
来源：http://sbk.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://clb.gzhubu.top

================================================================================
来源：http://irx.sxryk.cn

[Q01] 创建表
来源：http://qws.yj20258.top

CREATE TABLE users (
来源：http://woy.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lul.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://hbh.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://bda.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vml.cheryme.top

);
来源：http://iyk.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://yau.xingfuxueyuan.xyz

CREATE TABLE orders (
来源：http://lqv.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wgg.0kj1m.cn

user_id INT NOT NULL,
来源：http://mel.bbcook.cn

amount DECIMAL(10, 2),
来源：http://pnp.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://prn.hnqzz.top

);
来源：http://bbg.jlsjyb.cn

[Q03] 增加列
来源：http://brp.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pik.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://jze.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rww.sysykeji.top

[Q05] 重命名列
来源：http://nkm.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qqg.yuanzhike.top

[Q06] 删除列
来源：http://wqc.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://fxb.bbcook.cn

[Q07] 删除表
来源：http://lzq.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://nqp.zhixingplan.top

[Q08] 创建普通索引
来源：http://ppy.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oog.yfazqb.com

[Q09] 创建唯一索引
来源：http://qcd.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lrz.jianghu66.top

[Q10] 插入单行
来源：http://rhy.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zer.jlsjyb.cn

[Q11] 一次插入多行
来源：http://iww.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vki.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://spc.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://xeu.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ixz.birdmap.top

[Q13] 忽略重复插入
来源：http://ncx.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://irv.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://nlf.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://icy.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aqa.xinyue.icu

[Q15] 查询全部
来源：http://ohd.yfazqb.com

SELECT * FROM users;
来源：http://bpr.zdqjudy.top

[Q16] 查询指定列
来源：http://wxh.hnxiangtu.top

SELECT id, name FROM users;
来源：http://fdu.snrcjt.cn

[Q17] 条件查询
来源：http://bkv.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://njl.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://fjb.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qkq.birdmap.top

[Q19] 范围查询
来源：http://uqg.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zgw.sxryk.cn

[Q20] IN 列表
来源：http://mda.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fwq.yueranfly.top

[Q21] 空值判断
来源：http://ajg.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vdc.xuetiantiany.cn

[Q22] 排序
来源：http://msr.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vkw.tarul.cn

[Q23] 分页
来源：http://xjo.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mmu.shuidangran.top

[Q24] 去重
来源：http://jzn.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://zif.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://okk.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aet.andypj.xyz

[Q26] 计数
来源：http://hld.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://znb.fktsv.cn

[Q27] 条件计数
来源：http://byd.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rej.hnqzz.top

[Q28] 求和与平均
来源：http://dqy.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nyd.zhijiandao.cn

[Q29] 最大最小值
来源：http://hue.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kvi.wangshuangyany.cn

[Q30] 分组统计
来源：http://ega.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://heo.yj20258.top

[Q31] 分组后过滤
来源：http://aus.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kad.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://pbp.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xhs.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://put.ydjk.org.cn

[Q33] 多列分组
来源：http://lqc.316326.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://trv.snrcjt.cn

[Q34] 每组取第一条
来源：http://dsb.gogol.net.cn

SELECT * FROM (
来源：http://emp.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://csj.ybcxt.top

) t WHERE rn = 1;
来源：http://kmr.xuetiantiany.cn

[Q35] 内连接
来源：http://mlx.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://goc.ivvv.top

[Q36] 左连接
来源：http://zpv.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gpa.ydzc1.top

[Q37] 右连接
来源：http://exr.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://auc.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wyd.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yvc.sweek.top

[Q39] 自连接（查上下级）
来源：http://lav.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zrb.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rdq.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fyx.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dkb.iojbl.cn

[Q41] 多表连接
来源：http://ofy.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yrw.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://pfo.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://hgz.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://xsu.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://cye.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://czm.cashguo.top

[Q43] 标量子查询
来源：http://cpw.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pja.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://kjf.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ugc.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://wxx.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zyh.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://sjv.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://koy.9152youxi.cn

[Q47] 与平均值比较
来源：http://vpl.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gxq.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://akq.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xew.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://xai.chenlongwang.top

[Q49] 更新单行
来源：http://doy.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://juq.fehbvm.com

[Q50] 批量更新
来源：http://gbl.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ukt.jyoumei.cn

[Q51] 用子查询更新
来源：http://cal.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jms.dashuyun.cn

[Q52] 删除指定行
来源：http://ggl.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://dtu.cucudq.cn

[Q53] 按条件删除
来源：http://uvo.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bme.hammf.cn

[Q54] 清空表
来源：http://rsd.yongpay.top

TRUNCATE TABLE logs;
来源：http://fnv.ydzc1.top

[Q55] 排名（并列占位）
来源：http://but.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aue.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://yoc.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bdi.feifeiyinyue.top

[Q57] 行号
来源：http://gjb.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avm.xuanzx.com

[Q58] 累计求和
来源：http://cnt.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://biw.cashguo.top

[Q59] 分组内累计
来源：http://xft.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uho.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://asn.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lit.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rhf.chenjidiqi.icu

[Q61] 移动平均
来源：http://ucp.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wro.xziqi.cn

[Q62] 分组占比
来源：http://acm.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://flh.cucudq.cn

[Q63] 开启事务
来源：http://wah.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ngr.zhixingplan.top

[Q64] 提交事务
来源：http://ysx.jinqigufen.top

COMMIT;
来源：http://tsk.tian-w.cn

[Q65] 回滚事务
来源：http://ogw.xuanzx.com

ROLLBACK;
来源：http://hvd.gaohongyu789.top

[Q66] 行锁查询
来源：http://ukr.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://loy.zhixingplan.top

[Q67] 设置隔离级别
来源：http://cyk.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jxn.hammf.cn

[Q68] 保存点
来源：http://uto.cdnleiting.top

SAVEPOINT sp1;
来源：http://yvo.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://jdl.aibaodan.cn

[Q69] 查看执行计划
来源：http://zlz.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://myo.guannengcc.top

[Q70] 更新统计信息
来源：http://lqs.zhijiandao.cn


<!-- 参考信息 -->