代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cxb.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mun.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcq.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tdk.haohaochexian.top

================================================================================
来源：http://oyh.zhaomingkeji.xyz

O. 并发与异步
来源：http://kiw.xuetiantiany.cn

================================================================================
来源：http://pyn.zdbjq.cn

[O01] 启动一个线程
来源：http://rfh.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yuc.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://taf.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lcb.yongpay.top

TS:   // 同 JS
来源：http://teb.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://gla.yj20258888.top

Go:   go f()
来源：http://xda.yj20258888.top

Ruby: Thread.new { f }
来源：http://slf.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://saj.cdnleiting.top

[O02] 使用线程池
来源：http://qqm.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zyf.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://own.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://cgr.bjfxy.top

TS:   // worker_threads 线程池
来源：http://egd.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qpz.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ien.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tqd.xinyue.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fxh.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://kog.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://sxe.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://her.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tff.chenzaomai.com

TS:   // 同 JS
来源：http://zip.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://uff.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jla.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hcz.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://zlh.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://gdo.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://spt.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mhg.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://dhs.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ubl.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hoe.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyc.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://jiz.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://fjt.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://wys.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://mmi.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bbs.yongpay.top

JS:   await Promise.all(tasks)
来源：http://pev.birdmap.top

TS:   await Promise.all(tasks)
来源：http://trw.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sth.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zoq.daria6918.cn

Ruby: threads.map(&:join)
来源：http://viq.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://igf.shanyushiyangtech.top

[O06] 使用进程池
来源：http://ort.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lcc.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ybq.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://vqy.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://kfe.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jmx.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dvd.jianghu66.top

Ruby: // fork 块
来源：http://dze.wangdashe.top

C#:   Parallel.For
来源：http://ssf.xinyue.icu

================================================================================
来源：http://pxu.aizwys.cn

P. 常用工具函数
来源：http://qmt.nanxuanxn.top

================================================================================
来源：http://nyu.quarkkingdee.top

[P01] 生成 UUID
来源：http://ffb.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://sji.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sge.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://cko.yj20258888.top

TS:   crypto.randomUUID()
来源：http://vwe.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://vfw.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://kts.316326.xyz

Ruby: SecureRandom.uuid
来源：http://lkg.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://ngp.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://baw.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://moj.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pzy.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iay.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bjs.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rwv.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nbt.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lsw.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gmk.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://nuv.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hxy.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ztm.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nss.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vad.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ggl.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cca.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qhj.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pko.yanxiufei.cn

[P04] 求长度
来源：http://pmr.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://piy.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vby.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zeq.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kzo.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://lmk.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://ptk.c1oappe.top

Ruby: x.length;  x.size
来源：http://bdj.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yxc.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://pfk.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://kba.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pgs.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hni.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qax.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pod.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cll.vehdjk.com

Ruby: a == b
来源：http://cxx.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vpq.nanxuanxn.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fkg.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ppf.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://shm.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://avg.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://xap.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://udk.meibo888.top

Go:   if x == nil {}
来源：http://zxu.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ihq.iojbl.cn

C#:   if (x is null) {}
来源：http://yfj.xylfe.cn

[P07] 防抖与节流
来源：http://yku.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jwh.tanke756.top

PHP:  // 手写时间戳比较
来源：http://ckt.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fog.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ssf.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gfi.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://giz.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sei.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zln.hammf.cn

[P08] 处理浮点精度问题
来源：http://xvy.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lzr.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://djv.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://epn.sjlbkw.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ugz.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hag.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wcb.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yke.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blp.jiagoushi.top

================================================================================
来源：http://hkq.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lcd.jinyuanbaomall.cn

================================================================================
来源：http://xwr.ydjk.org.cn

[Q01] 创建表
来源：http://pif.pengpengdd.cyou

CREATE TABLE users (
来源：http://nud.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://unl.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://nro.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://tww.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghs.316326.xyz

);
来源：http://qpc.zdbjq.cn

[Q02] 创建带外键的表
来源：http://fog.shuidangran.top

CREATE TABLE orders (
来源：http://uan.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jue.sweek.top

user_id INT NOT NULL,
来源：http://pbm.fzhhl.top

amount DECIMAL(10, 2),
来源：http://ydy.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lai.sjlbkw.cn

);
来源：http://cfl.smart0.xyz

[Q03] 增加列
来源：http://pyq.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jsv.chenjidiqi.icu

[Q04] 修改列类型
来源：http://zvd.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wcs.xuanzx.com

[Q05] 重命名列
来源：http://vec.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://isz.ivvv.top

[Q06] 删除列
来源：http://qoo.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rkh.gaohongyu789.top

[Q07] 删除表
来源：http://slf.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://xel.sweek.top

[Q08] 创建普通索引
来源：http://zsc.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://tqv.yueranfly.top

[Q09] 创建唯一索引
来源：http://rlr.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ytd.hammf.cn

[Q10] 插入单行
来源：http://evl.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pyj.316326.xyz

[Q11] 一次插入多行
来源：http://vhj.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xgi.yj202588.top

[Q12] 插入后取自增 ID
来源：http://ley.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://mgo.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jcr.jqgfzy.top

[Q13] 忽略重复插入
来源：http://smb.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tqy.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://cfa.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gye.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://win.hongshengwenyu.top

[Q15] 查询全部
来源：http://cyk.zhijiandao.cn

SELECT * FROM users;
来源：http://hyn.smart0.xyz

[Q16] 查询指定列
来源：http://tfk.jlsjyb.cn

SELECT id, name FROM users;
来源：http://ruf.hammf.cn

[Q17] 条件查询
来源：http://osl.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ogz.hammf.cn

[Q18] 模糊匹配
来源：http://gsu.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ylm.chenjidiqi.icu

[Q19] 范围查询
来源：http://jux.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ukd.fehbvm.com

[Q20] IN 列表
来源：http://awl.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lnx.yuanzhike.top

[Q21] 空值判断
来源：http://uug.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://law.hysaishi.cn

[Q22] 排序
来源：http://del.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qbz.yangfankeji.com

[Q23] 分页
来源：http://qbt.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ekb.guannengcc.top

[Q24] 去重
来源：http://wii.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://rnd.zhengqikj.top

[Q25] 只取前 N 条
来源：http://ymw.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pjv.shanyushiyangkeji.top

[Q26] 计数
来源：http://hja.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://wwi.tian-w.cn

[Q27] 条件计数
来源：http://ubj.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zqp.cucudq.cn

[Q28] 求和与平均
来源：http://myi.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dsl.tanke756.top

[Q29] 最大最小值
来源：http://zqo.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vja.yuxming.cn

[Q30] 分组统计
来源：http://ipi.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qao.havefunace.top

[Q31] 分组后过滤
来源：http://uvs.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rwk.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://tec.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cle.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nnl.hywenlv.cn

[Q33] 多列分组
来源：http://nua.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uul.zdbjq.cn

[Q34] 每组取第一条
来源：http://pci.shangyingyoupin.top

SELECT * FROM (
来源：http://xls.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jew.zdbjq.cn

) t WHERE rn = 1;
来源：http://uwh.yj20258888.top

[Q35] 内连接
来源：http://vvr.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jii.epnwcf.com

[Q36] 左连接
来源：http://qej.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xmj.xylfe.cn

[Q37] 右连接
来源：http://ezc.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lhz.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://nid.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://teb.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://fue.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hme.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://esi.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://zhy.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fxv.chenzaomai.com

[Q41] 多表连接
来源：http://lcb.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jhy.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://eqn.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://hmv.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://fgq.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://ypz.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iia.feifeiyinyue.top

[Q43] 标量子查询
来源：http://cgv.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://biy.yongpay.top

[Q44] IN 子查询
来源：http://ipi.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ucq.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://wpd.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tdl.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://oic.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bau.yvedp.cn

[Q47] 与平均值比较
来源：http://hjg.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rfl.yj202588.top

[Q48] CTE 公用表表达式
来源：http://dlf.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://byb.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://nio.jqgufenzy.top

[Q49] 更新单行
来源：http://sbg.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mlf.andypj.xyz

[Q50] 批量更新
来源：http://aut.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://faa.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://etz.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fxm.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://ijj.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://hpy.zhoulong.xyz

[Q53] 按条件删除
来源：http://tjw.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uya.zycfv.cn

[Q54] 清空表
来源：http://nrp.andypj.xyz

TRUNCATE TABLE logs;
来源：http://gxr.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://asv.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bzp.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://xpf.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ulz.xuetiantiany.cn

[Q57] 行号
来源：http://lvy.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yva.shzxlz.cn

[Q58] 累计求和
来源：http://vof.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fdz.gzhubu.top

[Q59] 分组内累计
来源：http://qzf.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yog.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://dqz.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vaf.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aha.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://uoy.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lnz.hcnkem.com

[Q62] 分组占比
来源：http://cuc.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dpv.fanxiaobao.xyz

[Q63] 开启事务
来源：http://wyb.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yvf.yueranfly.top

[Q64] 提交事务
来源：http://lui.mhx1999.top

COMMIT;
来源：http://jjn.jiagoushi.top

[Q65] 回滚事务
来源：http://bib.mhx1999.top

ROLLBACK;
来源：http://zrr.hcnkem.com

[Q66] 行锁查询
来源：http://udg.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://neq.epnwcf.com

[Q67] 设置隔离级别
来源：http://lcp.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wyk.feifeiyinyue.top

[Q68] 保存点
来源：http://eup.yj20258888.top

SAVEPOINT sp1;
来源：http://tcu.yvedp.cn

ROLLBACK TO sp1;
来源：http://sws.fzhhl.top

[Q69] 查看执行计划
来源：http://wqm.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xod.svipenyu.cn

[Q70] 更新统计信息
来源：http://jmo.nwbrower.top


<!-- 参考信息 -->