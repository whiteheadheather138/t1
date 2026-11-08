代发 wailian999

TS:   // worker_threads 线程池
来源：https://si.zhonguo1118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://vm.zhonguo3118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://ip.zhonguo1118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://cw.zhonguo2118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://tq.zhonguo5118.cn

[O03] 加锁保护共享数据
来源：https://yp.zhonguo7118.cn

Py:   with lock: shared += 1
来源：https://cs.zhonguo3118.cn

PHP:  // 用 flock() 做文件锁
来源：https://nh.zhonguo8118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://nk.zhonguo2118.cn

TS:   // 同 JS
来源：https://sh.zhonguo3118.cn

Java: synchronized (this) { shared++; }
来源：https://ym.zhonguo4118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://hg.zhonguo7118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://mc.zhonguo7118.cn

C#:   lock (gate) { shared++; }
来源：https://gf.zhonguo4118.cn

[O04] 定义异步函数并等待
来源：https://cf.zhonguo4118.cn

Py:   async def f():⏎    await g()
来源：https://yl.zhonguo2118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://uy.zhonguo3118.cn

JS:   async function f() { await g(); }
来源：https://ca.zhonguo4118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://ez.zhonguo3118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://zz.zhonguo6118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://ub.zhonguo2118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://pp.zhonguo1118.cn

C#:   async Task F() { await G(); }
来源：https://lv.zhonguo5118.cn

[O05] 并发执行并等待全部完成
来源：https://kv.zhonguo2118.cn

Py:   asyncio.gather(*tasks)
来源：https://zb.zhonguo3118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://rt.zhonguo8118.cn

JS:   await Promise.all(tasks)
来源：https://rx.zhonguo2118.cn

TS:   await Promise.all(tasks)
来源：https://so.zhonguo8118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://dv.zhonguo5118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://ax.zhonguo5118.cn

Ruby: threads.map(&:join)
来源：https://tb.zhonguo4118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://zr.zhonguo3118.cn

[O06] 使用进程池
来源：https://uf.zhonguo4118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://kt.zhonguo3118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://hv.zhonguo7118.cn

JS:   // child_process / cluster 模块
来源：https://rx.zhonguo4118.cn

TS:   // child_process / cluster 模块
来源：https://oi.zhonguo5118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://no.zhonguo7118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://fe.zhonguo5118.cn

Ruby: // fork 块
来源：https://pw.zhonguo6118.cn

C#:   Parallel.For
来源：https://kb.zhonguo2118.cn

================================================================================
来源：https://in.zhonguo7118.cn

P. 常用工具函数
来源：https://uz.zhonguo8118.cn

================================================================================
来源：https://xh.zhonguo1118.cn

[P01] 生成 UUID
来源：https://zs.zhonguo4118.cn

Py:   str(uuid.uuid4())
来源：https://zg.zhonguo8118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://lo.zhonguo4118.cn

JS:   crypto.randomUUID()
来源：https://ro.zhonguo5118.cn

TS:   crypto.randomUUID()
来源：https://db.zhonguo4118.cn

Java: UUID.randomUUID().toString()
来源：https://xt.zhonguo4118.cn

Go:   // 用 github.com/google/uuid
来源：https://ui.zhonguo5118.cn

Ruby: SecureRandom.uuid
来源：https://cx.zhonguo3118.cn

C#:   Guid.NewGuid().ToString()
来源：https://ie.zhonguo4118.cn

[P02] MD5 / SHA256 摘要
来源：https://xw.zhonguo6118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://te.zhonguo4118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://vg.zhonguo4118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://wg.zhonguo4118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://zy.zhonguo4118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://uz.zhonguo4118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://bf.zhonguo3118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://dn.zhonguo6118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://zy.zhonguo3118.cn

[P03] 生成短随机字符串
来源：https://if.zhonguo6118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://gh.zhonguo4118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://is.zhonguo1118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://or.zhonguo7118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://tk.zhonguo6118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://zo.zhonguo6118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://jj.zhonguo6118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://sj.zhonguo3118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://ka.zhonguo2118.cn

[P04] 求长度
来源：https://li.zhonguo6118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://od.zhonguo4118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ke.zhonguo6118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ru.zhonguo7118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://vx.zhonguo3118.cn

Java: list.size();  map.size();  s.length()
来源：https://bs.zhonguo8118.cn

Go:   len(arr);  len(m)
来源：https://rr.zhonguo5118.cn

Ruby: x.length;  x.size
来源：https://tw.zhonguo5118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://qs.zhonguo4118.cn

[P05] 判断两个对象内容是否相等
来源：https://ha.zhonguo7118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://jm.zhonguo7118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://gj.zhonguo7118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://is.zhonguo2118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://bl.zhonguo7118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://ou.zhonguo4118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://cg.zhonguo3118.cn

Ruby: a == b
来源：https://at.zhonguo2118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://ap.zhonguo2118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://zf.zhonguo4118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://hn.zhonguo2118.cn

PHP:  if (empty($x)) {}
来源：https://dn.zhonguo3118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://wj.zhonguo1118.cn

TS:   if (x == null) {}
来源：https://fp.zhonguo5118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://fv.zhonguo2118.cn

Go:   if x == nil {}
来源：https://ev.zhonguo5118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://xf.zhonguo6118.cn

C#:   if (x is null) {}
来源：https://zh.zhonguo6118.cn

[P07] 防抖与节流
来源：https://hy.zhonguo8118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://kn.zhonguo3118.cn

PHP:  // 手写时间戳比较
来源：https://yn.zhonguo5118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://zi.zhonguo5118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://ay.zhonguo1118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://wp.zhonguo8118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://gc.zhonguo3118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://zc.zhonguo3118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://jc.zhonguo4118.cn

[P08] 处理浮点精度问题
来源：https://we.zhonguo7118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://zu.zhonguo3118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://jv.zhonguo1118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://me.zhonguo2118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://mu.zhonguo7118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://wq.zhonguo2118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://ry.zhonguo3118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://gh.zhonguo4118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://vt.zhonguo5118.cn

================================================================================
来源：https://wq.zhonguo4118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://mf.zhonguo8118.cn

================================================================================
来源：https://ek.zhonguo2118.cn

[Q01] 创建表
来源：https://qp.zhonguo2118.cn

CREATE TABLE users (
来源：https://fc.zhonguo6118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://ir.zhonguo4118.cn

name VARCHAR(50) NOT NULL,
来源：https://au.zhonguo7118.cn

email VARCHAR(100) UNIQUE,
来源：https://lr.zhonguo7118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://ka.zhonguo8118.cn

);
来源：https://rb.zhonguo5118.cn

[Q02] 创建带外键的表
来源：https://yd.zhonguo6118.cn

CREATE TABLE orders (
来源：https://zv.zhonguo5118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://rf.zhonguo1118.cn

user_id INT NOT NULL,
来源：https://ri.zhonguo8118.cn

amount DECIMAL(10, 2),
来源：https://jr.zhonguo1118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://vs.zhonguo4118.cn

);
来源：https://xa.zhonguo3118.cn

[Q03] 增加列
来源：https://mk.zhonguo8118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://kg.zhonguo7118.cn

[Q04] 修改列类型
来源：https://ic.zhonguo2118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://sy.zhonguo6118.cn

[Q05] 重命名列
来源：https://kg.zhonguo5118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://oa.zhonguo2118.cn

[Q06] 删除列
来源：https://ck.zhonguo5118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://wd.zhonguo6118.cn

[Q07] 删除表
来源：https://mh.zhonguo6118.cn

DROP TABLE IF EXISTS orders;
来源：https://wl.zhonguo7118.cn

[Q08] 创建普通索引
来源：https://vq.zhonguo3118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://wf.zhonguo3118.cn

[Q09] 创建唯一索引
来源：https://pg.zhonguo4118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://lo.zhonguo2118.cn

[Q10] 插入单行
来源：https://xf.zhonguo1118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://vv.zhonguo6118.cn

[Q11] 一次插入多行
来源：https://nb.zhonguo8118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://ob.zhonguo3118.cn

[Q12] 插入后取自增 ID
来源：https://qv.zhonguo1118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://at.zhonguo4118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://me.zhonguo6118.cn

[Q13] 忽略重复插入
来源：https://eo.zhonguo6118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://ij.zhonguo4118.cn

[Q14] 存在则更新（upsert）
来源：https://it.zhonguo6118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://tb.zhonguo2118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://us.zhonguo5118.cn

[Q15] 查询全部
来源：https://eq.zhonguo8118.cn

SELECT * FROM users;
来源：https://mb.zhonguo3118.cn

[Q16] 查询指定列
来源：https://nu.zhonguo1118.cn

SELECT id, name FROM users;
来源：https://xi.zhonguo3118.cn

[Q17] 条件查询
来源：https://hf.zhonguo7118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://vl.zhonguo7118.cn

[Q18] 模糊匹配
来源：https://vw.zhonguo4118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://gy.zhonguo3118.cn

[Q19] 范围查询
来源：https://fm.zhonguo5118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://ho.zhonguo1118.cn

[Q20] IN 列表
来源：https://li.zhonguo1118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://oq.zhonguo7118.cn

[Q21] 空值判断
来源：https://ts.zhonguo3118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://ol.zhonguo4118.cn

[Q22] 排序
来源：https://sd.zhonguo2118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://hn.zhonguo4118.cn

[Q23] 分页
来源：https://ts.zhonguo1118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://pf.zhonguo4118.cn

[Q24] 去重
来源：https://rd.zhonguo6118.cn

SELECT DISTINCT city FROM users;
来源：https://zk.zhonguo8118.cn

[Q25] 只取前 N 条
来源：https://wq.zhonguo3118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://cf.zhonguo8118.cn

[Q26] 计数
来源：https://ta.zhonguo3118.cn

SELECT COUNT(*) FROM users;
来源：https://oq.zhonguo8118.cn

[Q27] 条件计数
来源：https://xg.zhonguo6118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://im.zhonguo4118.cn

[Q28] 求和与平均
来源：https://jp.zhonguo7118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://bo.zhonguo7118.cn

[Q29] 最大最小值
来源：https://ld.zhonguo8118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://rd.zhonguo3118.cn

[Q30] 分组统计
来源：https://ye.zhonguo7118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://ax.zhonguo5118.cn

[Q31] 分组后过滤
来源：https://ra.zhonguo3118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://sg.zhonguo4118.cn

[Q32] 分组拼接字符串
来源：https://tf.zhonguo5118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://zc.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://pw.zhonguo2118.cn

[Q33] 多列分组
来源：https://vm.zhonguo3118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://ym.zhonguo6118.cn

[Q34] 每组取第一条
来源：https://hk.zhonguo4118.cn

SELECT * FROM (
来源：https://fy.zhonguo4118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://eb.zhonguo3118.cn

) t WHERE rn = 1;
来源：https://id.zhonguo5118.cn

[Q35] 内连接
来源：https://wu.zhonguo1118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://gr.zhonguo3118.cn

[Q36] 左连接
来源：https://nn.zhonguo8118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://xt.zhonguo2118.cn

[Q37] 右连接
来源：https://av.zhonguo4118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://ap.zhonguo6118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://mw.zhonguo5118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://vz.zhonguo3118.cn

[Q39] 自连接（查上下级）
来源：https://lg.zhonguo2118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://sn.zhonguo1118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://iu.zhonguo2118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://ik.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://hr.zhonguo8118.cn

[Q41] 多表连接
来源：https://ok.zhonguo4118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://ls.zhonguo4118.cn

JOIN users u ON u.id = o.user_id
来源：https://kb.zhonguo8118.cn

JOIN products p ON p.id = o.product_id;
来源：https://bh.zhonguo7118.cn

[Q42] 连接条件附加过滤
来源：https://rl.zhonguo5118.cn

SELECT u.name, o.amount FROM users u
来源：https://jx.zhonguo2118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://bk.zhonguo4118.cn

[Q43] 标量子查询
来源：https://vw.zhonguo2118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://ak.zhonguo6118.cn

[Q44] IN 子查询
来源：https://am.zhonguo3118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://gr.zhonguo5118.cn

[Q45] EXISTS 判断存在
来源：https://gc.zhonguo8118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://cq.zhonguo7118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://op.zhonguo4118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://cc.zhonguo2118.cn

[Q47] 与平均值比较
来源：https://sg.zhonguo2118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://vx.zhonguo6118.cn

[Q48] CTE 公用表表达式
来源：https://rj.zhonguo2118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://mh.zhonguo2118.cn

SELECT * FROM t WHERE c > 5;
来源：https://od.zhonguo8118.cn

[Q49] 更新单行
来源：https://vw.zhonguo3118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://us.zhonguo2118.cn

[Q50] 批量更新
来源：https://yc.zhonguo8118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://qv.zhonguo5118.cn

[Q51] 用子查询更新
来源：https://eu.zhonguo4118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://lt.zhonguo8118.cn

[Q52] 删除指定行
来源：https://cr.zhonguo8118.cn

DELETE FROM users WHERE id = 10;
来源：https://lh.zhonguo7118.cn

[Q53] 按条件删除
来源：https://fx.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://ja.zhonguo4118.cn

[Q54] 清空表
来源：https://fz.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://dq.zhonguo8118.cn

[Q55] 排名（并列占位）
来源：https://ks.zhonguo6118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://ks.zhonguo3118.cn

[Q56] 密集排名（并列不占位）
来源：https://rq.zhonguo6118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://dk.zhonguo4118.cn

[Q57] 行号
来源：https://rw.zhonguo8118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://hj.zhonguo8118.cn

[Q58] 累计求和
来源：https://ni.zhonguo8118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://qe.zhonguo2118.cn

[Q59] 分组内累计
来源：https://ob.zhonguo8118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://yv.zhonguo6118.cn

[Q60] 取上一行 / 下一行
来源：https://xw.zhonguo8118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://ll.zhonguo6118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://tn.zhonguo4118.cn

[Q61] 移动平均
来源：https://ep.zhonguo2118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://gd.zhonguo4118.cn

[Q62] 分组占比
来源：https://tn.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://rl.zhonguo4118.cn

[Q63] 开启事务
来源：https://yp.zhonguo4118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://pr.zhonguo8118.cn

[Q64] 提交事务
来源：https://me.zhonguo1118.cn

COMMIT;
来源：https://hj.zhonguo3118.cn

[Q65] 回滚事务
来源：https://ye.zhonguo3118.cn

ROLLBACK;
来源：https://gf.zhonguo4118.cn

[Q66] 行锁查询
来源：https://sg.zhonguo5118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://iy.zhonguo6118.cn

[Q67] 设置隔离级别
来源：https://ae.zhonguo7118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://ex.zhonguo5118.cn

[Q68] 保存点
来源：https://tl.zhonguo6118.cn

SAVEPOINT sp1;
来源：https://gb.zhonguo6118.cn

ROLLBACK TO sp1;
来源：https://cv.zhonguo3118.cn

[Q69] 查看执行计划
来源：https://xp.zhonguo6118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://bl.zhonguo5118.cn

[Q70] 更新统计信息
来源：https://fs.zhonguo3118.cn

ANALYZE TABLE users;
来源：https://xh.zhonguo8118.cn

[Q71] 查看建表语句
来源：https://cf.zhonguo2118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://ou.zhonguo2118.cn

[Q72] 查看索引
来源：https://rr.zhonguo6118.cn

SHOW INDEX FROM users;
来源：https://tm.zhonguo3118.cn

[Q73] 查看表状态
来源：https://iw.zhonguo4118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://hs.zhonguo7118.cn

[Q74] 强制使用索引
来源：https://sx.zhonguo1118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://cp.zhonguo3118.cn

[Q75] 日期格式化
来源：https://cp.zhonguo5118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://bb.zhonguo6118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://hs.zhonguo3118.cn

[Q76] 按天统计
来源：https://jc.zhonguo5118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://be.zhonguo5118.cn

[Q77] 时间加减
来源：https://ff.zhonguo7118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://si.zhonguo4118.cn

[Q78] 当前时间
来源：https://nr.zhonguo1118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://qf.zhonguo3118.cn

[Q79] 字符串拼接
来源：https://wm.zhonguo7118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://nu.zhonguo3118.cn


<!-- 参考信息 -->