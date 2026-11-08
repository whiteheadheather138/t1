代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://jd.zhonguo1118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://ai.zhonguo7118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://if.zhonguo4118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://fi.zhonguo3118.cn

================================================================================
来源：https://na.zhonguo1118.cn

O. 并发与异步
来源：https://qq.zhonguo5118.cn

================================================================================
来源：https://ky.zhonguo1118.cn

[O01] 启动一个线程
来源：https://li.zhonguo1118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://qz.zhonguo5118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://hn.zhonguo7118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://ny.zhonguo8118.cn

TS:   // 同 JS
来源：https://uc.zhonguo6118.cn

Java: new Thread(() -> f()).start()
来源：https://dz.zhonguo1118.cn

Go:   go f()
来源：https://md.zhonguo4118.cn

Ruby: Thread.new { f }
来源：https://ba.zhonguo7118.cn

C#:   Task.Run(() => F());
来源：https://bm.zhonguo5118.cn

[O02] 使用线程池
来源：https://jj.zhonguo4118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://so.zhonguo4118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://hc.zhonguo8118.cn

JS:   // worker_threads 线程池
来源：https://kl.zhonguo6118.cn

TS:   // worker_threads 线程池
来源：https://av.zhonguo3118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://yh.zhonguo1118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://jv.zhonguo2118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://jx.zhonguo6118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://xy.zhonguo1118.cn

[O03] 加锁保护共享数据
来源：https://pc.zhonguo4118.cn

Py:   with lock: shared += 1
来源：https://bb.zhonguo8118.cn

PHP:  // 用 flock() 做文件锁
来源：https://li.zhonguo7118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://ow.zhonguo5118.cn

TS:   // 同 JS
来源：https://pf.zhonguo1118.cn

Java: synchronized (this) { shared++; }
来源：https://yl.zhonguo8118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://qe.zhonguo3118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://nt.zhonguo7118.cn

C#:   lock (gate) { shared++; }
来源：https://gi.zhonguo2118.cn

[O04] 定义异步函数并等待
来源：https://gi.zhonguo7118.cn

Py:   async def f():⏎    await g()
来源：https://dt.zhonguo8118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://mo.zhonguo3118.cn

JS:   async function f() { await g(); }
来源：https://qc.zhonguo1118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://be.zhonguo4118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://pu.zhonguo5118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://oz.zhonguo8118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://qk.zhonguo6118.cn

C#:   async Task F() { await G(); }
来源：https://gg.zhonguo6118.cn

[O05] 并发执行并等待全部完成
来源：https://oy.zhonguo5118.cn

Py:   asyncio.gather(*tasks)
来源：https://ml.zhonguo4118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://ja.zhonguo1118.cn

JS:   await Promise.all(tasks)
来源：https://gr.zhonguo5118.cn

TS:   await Promise.all(tasks)
来源：https://vx.zhonguo1118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://iu.zhonguo8118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://ad.zhonguo5118.cn

Ruby: threads.map(&:join)
来源：https://tc.zhonguo8118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://mb.zhonguo4118.cn

[O06] 使用进程池
来源：https://bo.zhonguo7118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://vj.zhonguo1118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://jp.zhonguo1118.cn

JS:   // child_process / cluster 模块
来源：https://pn.zhonguo5118.cn

TS:   // child_process / cluster 模块
来源：https://yi.zhonguo2118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://cn.zhonguo6118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://vh.zhonguo2118.cn

Ruby: // fork 块
来源：https://wa.zhonguo1118.cn

C#:   Parallel.For
来源：https://vd.zhonguo1118.cn

================================================================================
来源：https://hx.zhonguo2118.cn

P. 常用工具函数
来源：https://kl.zhonguo2118.cn

================================================================================
来源：https://kw.zhonguo3118.cn

[P01] 生成 UUID
来源：https://si.zhonguo1118.cn

Py:   str(uuid.uuid4())
来源：https://nb.zhonguo3118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://eq.zhonguo6118.cn

JS:   crypto.randomUUID()
来源：https://wy.zhonguo1118.cn

TS:   crypto.randomUUID()
来源：https://yg.zhonguo7118.cn

Java: UUID.randomUUID().toString()
来源：https://nz.zhonguo7118.cn

Go:   // 用 github.com/google/uuid
来源：https://sa.zhonguo5118.cn

Ruby: SecureRandom.uuid
来源：https://cr.zhonguo7118.cn

C#:   Guid.NewGuid().ToString()
来源：https://pe.zhonguo8118.cn

[P02] MD5 / SHA256 摘要
来源：https://tc.zhonguo3118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://kg.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://es.zhonguo8118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://sk.zhonguo7118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://pi.zhonguo5118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://sh.zhonguo5118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://gv.zhonguo8118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://yu.zhonguo6118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://wn.zhonguo7118.cn

[P03] 生成短随机字符串
来源：https://ns.zhonguo2118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://du.zhonguo4118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://zv.zhonguo5118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://hg.zhonguo3118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://kv.zhonguo7118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://az.zhonguo1118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://sl.zhonguo1118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://zz.zhonguo2118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://jh.zhonguo3118.cn

[P04] 求长度
来源：https://qk.zhonguo1118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://ts.zhonguo7118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://qe.zhonguo1118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ua.zhonguo6118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://dh.zhonguo8118.cn

Java: list.size();  map.size();  s.length()
来源：https://cy.zhonguo6118.cn

Go:   len(arr);  len(m)
来源：https://ob.zhonguo1118.cn

Ruby: x.length;  x.size
来源：https://ou.zhonguo6118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://hg.zhonguo4118.cn

[P05] 判断两个对象内容是否相等
来源：https://ce.zhonguo2118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://ls.zhonguo8118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://yr.zhonguo6118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://ly.zhonguo4118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://la.zhonguo8118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://ur.zhonguo1118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://er.zhonguo3118.cn

Ruby: a == b
来源：https://lq.zhonguo6118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://at.zhonguo2118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://jy.zhonguo1118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://jy.zhonguo5118.cn

PHP:  if (empty($x)) {}
来源：https://aa.zhonguo1118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://nm.zhonguo1118.cn

TS:   if (x == null) {}
来源：https://ag.zhonguo7118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://fi.zhonguo8118.cn

Go:   if x == nil {}
来源：https://yq.zhonguo5118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://lg.zhonguo5118.cn

C#:   if (x is null) {}
来源：https://gs.zhonguo6118.cn

[P07] 防抖与节流
来源：https://hf.zhonguo4118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://fc.zhonguo1118.cn

PHP:  // 手写时间戳比较
来源：https://fq.zhonguo7118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://jf.zhonguo2118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://wp.zhonguo5118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://cn.zhonguo1118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://lb.zhonguo1118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://yg.zhonguo7118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://ee.zhonguo5118.cn

[P08] 处理浮点精度问题
来源：https://tp.zhonguo7118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://iy.zhonguo2118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://hh.zhonguo3118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://dj.zhonguo1118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://ni.zhonguo5118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://wp.zhonguo1118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://wg.zhonguo1118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://kd.zhonguo5118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://qq.zhonguo5118.cn

================================================================================
来源：https://ac.zhonguo4118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://eq.zhonguo2118.cn

================================================================================
来源：https://ew.zhonguo5118.cn

[Q01] 创建表
来源：https://zm.zhonguo2118.cn

CREATE TABLE users (
来源：https://rx.zhonguo2118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://cv.zhonguo6118.cn

name VARCHAR(50) NOT NULL,
来源：https://gz.zhonguo4118.cn

email VARCHAR(100) UNIQUE,
来源：https://me.zhonguo3118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://fe.zhonguo1118.cn

);
来源：https://jz.zhonguo7118.cn

[Q02] 创建带外键的表
来源：https://sc.zhonguo2118.cn

CREATE TABLE orders (
来源：https://kw.zhonguo7118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://kj.zhonguo4118.cn

user_id INT NOT NULL,
来源：https://ve.zhonguo7118.cn

amount DECIMAL(10, 2),
来源：https://sv.zhonguo3118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://av.zhonguo1118.cn

);
来源：https://fi.zhonguo1118.cn

[Q03] 增加列
来源：https://fh.zhonguo6118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://it.zhonguo6118.cn

[Q04] 修改列类型
来源：https://hr.zhonguo8118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://st.zhonguo6118.cn

[Q05] 重命名列
来源：https://gz.zhonguo4118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://ny.zhonguo4118.cn

[Q06] 删除列
来源：https://ko.zhonguo7118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://cq.zhonguo3118.cn

[Q07] 删除表
来源：https://zy.zhonguo8118.cn

DROP TABLE IF EXISTS orders;
来源：https://jr.zhonguo7118.cn

[Q08] 创建普通索引
来源：https://dy.zhonguo6118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://ue.zhonguo7118.cn

[Q09] 创建唯一索引
来源：https://ea.zhonguo8118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://oe.zhonguo7118.cn

[Q10] 插入单行
来源：https://na.zhonguo1118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://yy.zhonguo7118.cn

[Q11] 一次插入多行
来源：https://um.zhonguo4118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://mg.zhonguo7118.cn

[Q12] 插入后取自增 ID
来源：https://kw.zhonguo2118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://ip.zhonguo7118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://fl.zhonguo5118.cn

[Q13] 忽略重复插入
来源：https://jf.zhonguo4118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://fn.zhonguo6118.cn

[Q14] 存在则更新（upsert）
来源：https://ou.zhonguo8118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://uv.zhonguo5118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://ci.zhonguo3118.cn

[Q15] 查询全部
来源：https://kq.zhonguo7118.cn

SELECT * FROM users;
来源：https://jc.zhonguo4118.cn

[Q16] 查询指定列
来源：https://oe.zhonguo1118.cn

SELECT id, name FROM users;
来源：https://jl.zhonguo6118.cn

[Q17] 条件查询
来源：https://wy.zhonguo2118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://og.zhonguo6118.cn

[Q18] 模糊匹配
来源：https://vp.zhonguo3118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://xd.zhonguo8118.cn

[Q19] 范围查询
来源：https://zk.zhonguo5118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://tn.zhonguo4118.cn

[Q20] IN 列表
来源：https://qs.zhonguo6118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://sp.zhonguo4118.cn

[Q21] 空值判断
来源：https://rx.zhonguo7118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://cx.zhonguo3118.cn

[Q22] 排序
来源：https://tt.zhonguo8118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://da.zhonguo1118.cn

[Q23] 分页
来源：https://xn.zhonguo1118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://ms.zhonguo2118.cn

[Q24] 去重
来源：https://bn.zhonguo3118.cn

SELECT DISTINCT city FROM users;
来源：https://zw.zhonguo5118.cn

[Q25] 只取前 N 条
来源：https://vj.zhonguo7118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://di.zhonguo5118.cn

[Q26] 计数
来源：https://ih.zhonguo3118.cn

SELECT COUNT(*) FROM users;
来源：https://bu.zhonguo6118.cn

[Q27] 条件计数
来源：https://al.zhonguo8118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://uq.zhonguo1118.cn

[Q28] 求和与平均
来源：https://xk.zhonguo5118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://lu.zhonguo1118.cn

[Q29] 最大最小值
来源：https://zg.zhonguo5118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://at.zhonguo8118.cn

[Q30] 分组统计
来源：https://qe.zhonguo2118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://zz.zhonguo7118.cn

[Q31] 分组后过滤
来源：https://al.zhonguo2118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://cn.zhonguo1118.cn

[Q32] 分组拼接字符串
来源：https://ed.zhonguo4118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://ds.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://aq.zhonguo2118.cn

[Q33] 多列分组
来源：https://rq.zhonguo2118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://bi.zhonguo1118.cn

[Q34] 每组取第一条
来源：https://ez.zhonguo6118.cn

SELECT * FROM (
来源：https://jy.zhonguo1118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://es.zhonguo7118.cn

) t WHERE rn = 1;
来源：https://dr.zhonguo7118.cn

[Q35] 内连接
来源：https://cx.zhonguo3118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://iv.zhonguo6118.cn

[Q36] 左连接
来源：https://ol.zhonguo1118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://yj.zhonguo3118.cn

[Q37] 右连接
来源：https://sq.zhonguo3118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://ob.zhonguo8118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://bp.zhonguo1118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://wh.zhonguo2118.cn

[Q39] 自连接（查上下级）
来源：https://sv.zhonguo8118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://jn.zhonguo2118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://mn.zhonguo6118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://up.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://dy.zhonguo6118.cn

[Q41] 多表连接
来源：https://ps.zhonguo5118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://gr.zhonguo4118.cn

JOIN users u ON u.id = o.user_id
来源：https://de.zhonguo8118.cn

JOIN products p ON p.id = o.product_id;
来源：https://cl.zhonguo7118.cn

[Q42] 连接条件附加过滤
来源：https://mh.zhonguo7118.cn

SELECT u.name, o.amount FROM users u
来源：https://ax.zhonguo3118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://aq.zhonguo7118.cn

[Q43] 标量子查询
来源：https://od.zhonguo6118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://nl.zhonguo7118.cn

[Q44] IN 子查询
来源：https://ts.zhonguo8118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://hs.zhonguo3118.cn

[Q45] EXISTS 判断存在
来源：https://ui.zhonguo7118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://pc.zhonguo6118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://ll.zhonguo2118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://tm.zhonguo5118.cn

[Q47] 与平均值比较
来源：https://hu.zhonguo7118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://tf.zhonguo3118.cn

[Q48] CTE 公用表表达式
来源：https://lb.zhonguo3118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://st.zhonguo1118.cn

SELECT * FROM t WHERE c > 5;
来源：https://th.zhonguo3118.cn

[Q49] 更新单行
来源：https://na.zhonguo8118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://vs.zhonguo2118.cn

[Q50] 批量更新
来源：https://fw.zhonguo4118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://bf.zhonguo7118.cn

[Q51] 用子查询更新
来源：https://gx.zhonguo4118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://pi.zhonguo6118.cn

[Q52] 删除指定行
来源：https://ve.zhonguo6118.cn

DELETE FROM users WHERE id = 10;
来源：https://ns.zhonguo1118.cn

[Q53] 按条件删除
来源：https://xj.zhonguo1118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://gk.zhonguo6118.cn

[Q54] 清空表
来源：https://vb.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://ej.zhonguo3118.cn

[Q55] 排名（并列占位）
来源：https://ts.zhonguo6118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://vp.zhonguo7118.cn

[Q56] 密集排名（并列不占位）
来源：https://at.zhonguo2118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://qa.zhonguo1118.cn

[Q57] 行号
来源：https://fj.zhonguo6118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://uj.zhonguo5118.cn

[Q58] 累计求和
来源：https://mu.zhonguo1118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://np.zhonguo8118.cn

[Q59] 分组内累计
来源：https://av.zhonguo7118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://zb.zhonguo8118.cn

[Q60] 取上一行 / 下一行
来源：https://ez.zhonguo3118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://di.zhonguo4118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://sl.zhonguo3118.cn

[Q61] 移动平均
来源：https://bm.zhonguo2118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://em.zhonguo1118.cn

[Q62] 分组占比
来源：https://kp.zhonguo1118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://jg.zhonguo3118.cn

[Q63] 开启事务
来源：https://lu.zhonguo4118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://bt.zhonguo8118.cn

[Q64] 提交事务
来源：https://fn.zhonguo1118.cn

COMMIT;
来源：https://uh.zhonguo2118.cn

[Q65] 回滚事务
来源：https://av.zhonguo7118.cn

ROLLBACK;
来源：https://rt.zhonguo2118.cn

[Q66] 行锁查询
来源：https://jk.zhonguo7118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://hn.zhonguo6118.cn

[Q67] 设置隔离级别
来源：https://lg.zhonguo8118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://wg.zhonguo4118.cn

[Q68] 保存点
来源：https://hr.zhonguo6118.cn

SAVEPOINT sp1;
来源：https://by.zhonguo1118.cn

ROLLBACK TO sp1;
来源：https://yq.zhonguo4118.cn

[Q69] 查看执行计划
来源：https://la.zhonguo3118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://kr.zhonguo1118.cn

[Q70] 更新统计信息
来源：https://df.zhonguo8118.cn


<!-- 参考信息 -->