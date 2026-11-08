代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://jv.zhonguo6118.cn

[O03] 加锁保护共享数据
来源：https://us.zhonguo8118.cn

Py:   with lock: shared += 1
来源：https://fl.zhonguo3118.cn

PHP:  // 用 flock() 做文件锁
来源：https://hg.zhonguo3118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://nc.zhonguo4118.cn

TS:   // 同 JS
来源：https://my.zhonguo1118.cn

Java: synchronized (this) { shared++; }
来源：https://mg.zhonguo2118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://ue.zhonguo6118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://xa.zhonguo5118.cn

C#:   lock (gate) { shared++; }
来源：https://an.zhonguo4118.cn

[O04] 定义异步函数并等待
来源：https://xg.zhonguo5118.cn

Py:   async def f():⏎    await g()
来源：https://kv.zhonguo4118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://hm.zhonguo3118.cn

JS:   async function f() { await g(); }
来源：https://dt.zhonguo4118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://hv.zhonguo3118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://xi.zhonguo1118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://tx.zhonguo7118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://fa.zhonguo4118.cn

C#:   async Task F() { await G(); }
来源：https://ln.zhonguo4118.cn

[O05] 并发执行并等待全部完成
来源：https://sg.zhonguo2118.cn

Py:   asyncio.gather(*tasks)
来源：https://be.zhonguo8118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://ks.zhonguo2118.cn

JS:   await Promise.all(tasks)
来源：https://es.zhonguo3118.cn

TS:   await Promise.all(tasks)
来源：https://mz.zhonguo4118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://pq.zhonguo8118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://lt.zhonguo5118.cn

Ruby: threads.map(&:join)
来源：https://pk.zhonguo5118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://nl.zhonguo6118.cn

[O06] 使用进程池
来源：https://cb.zhonguo7118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://cb.zhonguo5118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://dl.zhonguo5118.cn

JS:   // child_process / cluster 模块
来源：https://ed.zhonguo5118.cn

TS:   // child_process / cluster 模块
来源：https://pb.zhonguo2118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://oc.zhonguo2118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://ve.zhonguo2118.cn

Ruby: // fork 块
来源：https://tk.zhonguo8118.cn

C#:   Parallel.For
来源：https://dl.zhonguo5118.cn

================================================================================
来源：https://ma.zhonguo6118.cn

P. 常用工具函数
来源：https://tq.zhonguo6118.cn

================================================================================
来源：https://rc.zhonguo5118.cn

[P01] 生成 UUID
来源：https://oi.zhonguo7118.cn

Py:   str(uuid.uuid4())
来源：https://qf.zhonguo4118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://ou.zhonguo7118.cn

JS:   crypto.randomUUID()
来源：https://by.zhonguo6118.cn

TS:   crypto.randomUUID()
来源：https://td.zhonguo6118.cn

Java: UUID.randomUUID().toString()
来源：https://oz.zhonguo6118.cn

Go:   // 用 github.com/google/uuid
来源：https://xm.zhonguo2118.cn

Ruby: SecureRandom.uuid
来源：https://tu.zhonguo6118.cn

C#:   Guid.NewGuid().ToString()
来源：https://zx.zhonguo7118.cn

[P02] MD5 / SHA256 摘要
来源：https://iz.zhonguo6118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://wh.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://za.zhonguo7118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://bx.zhonguo5118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://xg.zhonguo7118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://lf.zhonguo2118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://xm.zhonguo2118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://vt.zhonguo2118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://bf.zhonguo2118.cn

[P03] 生成短随机字符串
来源：https://pt.zhonguo4118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://ca.zhonguo3118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://wp.zhonguo3118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://tl.zhonguo3118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://xx.zhonguo3118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://ku.zhonguo1118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://gp.zhonguo2118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://cb.zhonguo5118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://ko.zhonguo2118.cn

[P04] 求长度
来源：https://rg.zhonguo8118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://de.zhonguo6118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://tk.zhonguo3118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://yo.zhonguo8118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://hi.zhonguo2118.cn

Java: list.size();  map.size();  s.length()
来源：https://kd.zhonguo5118.cn

Go:   len(arr);  len(m)
来源：https://mp.zhonguo7118.cn

Ruby: x.length;  x.size
来源：https://ms.zhonguo6118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://sn.zhonguo3118.cn

[P05] 判断两个对象内容是否相等
来源：https://ez.zhonguo1118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://ju.zhonguo5118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://sm.zhonguo3118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://dc.zhonguo8118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://lo.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://tb.zhonguo2118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://zz.zhonguo4118.cn

Ruby: a == b
来源：https://do.zhonguo1118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://xh.zhonguo4118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://ij.zhonguo5118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://ak.zhonguo4118.cn

PHP:  if (empty($x)) {}
来源：https://ot.zhonguo6118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://lt.zhonguo2118.cn

TS:   if (x == null) {}
来源：https://lj.zhonguo5118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://fz.zhonguo5118.cn

Go:   if x == nil {}
来源：https://sy.zhonguo6118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://te.zhonguo1118.cn

C#:   if (x is null) {}
来源：https://co.zhonguo5118.cn

[P07] 防抖与节流
来源：https://eo.zhonguo5118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://ub.zhonguo3118.cn

PHP:  // 手写时间戳比较
来源：https://wm.zhonguo4118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://sz.zhonguo6118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://nl.zhonguo4118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://vp.zhonguo1118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://jj.zhonguo4118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://xc.zhonguo8118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://fq.zhonguo5118.cn

[P08] 处理浮点精度问题
来源：https://rb.zhonguo2118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://em.zhonguo1118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://ib.zhonguo1118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://pr.zhonguo8118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://gk.zhonguo7118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://ci.zhonguo8118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://tx.zhonguo6118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://bh.zhonguo3118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://nm.zhonguo2118.cn

================================================================================
来源：https://hm.zhonguo1118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://ur.zhonguo3118.cn

================================================================================
来源：https://ls.zhonguo5118.cn

[Q01] 创建表
来源：https://td.zhonguo7118.cn

CREATE TABLE users (
来源：https://xv.zhonguo4118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://sx.zhonguo1118.cn

name VARCHAR(50) NOT NULL,
来源：https://mb.zhonguo7118.cn

email VARCHAR(100) UNIQUE,
来源：https://zu.zhonguo5118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://uj.zhonguo4118.cn

);
来源：https://lx.zhonguo8118.cn

[Q02] 创建带外键的表
来源：https://lh.zhonguo1118.cn

CREATE TABLE orders (
来源：https://wj.zhonguo4118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://mc.zhonguo2118.cn

user_id INT NOT NULL,
来源：https://cy.zhonguo1118.cn

amount DECIMAL(10, 2),
来源：https://dd.zhonguo8118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://ie.zhonguo6118.cn

);
来源：https://sl.zhonguo2118.cn

[Q03] 增加列
来源：https://xk.zhonguo6118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://ed.zhonguo8118.cn

[Q04] 修改列类型
来源：https://zk.zhonguo8118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://cn.zhonguo4118.cn

[Q05] 重命名列
来源：https://rv.zhonguo8118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://qj.zhonguo8118.cn

[Q06] 删除列
来源：https://zr.zhonguo2118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://ph.zhonguo5118.cn

[Q07] 删除表
来源：https://kd.zhonguo1118.cn

DROP TABLE IF EXISTS orders;
来源：https://je.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://dq.zhonguo7118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://ab.zhonguo7118.cn

[Q09] 创建唯一索引
来源：https://jn.zhonguo7118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://kw.zhonguo6118.cn

[Q10] 插入单行
来源：https://mw.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://aa.zhonguo3118.cn

[Q11] 一次插入多行
来源：https://og.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://wm.zhonguo1118.cn

[Q12] 插入后取自增 ID
来源：https://za.zhonguo2118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://uk.zhonguo7118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://tm.zhonguo8118.cn

[Q13] 忽略重复插入
来源：https://fd.zhonguo8118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://wp.zhonguo4118.cn

[Q14] 存在则更新（upsert）
来源：https://ho.zhonguo2118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://mq.zhonguo2118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://ur.zhonguo3118.cn

[Q15] 查询全部
来源：https://mj.zhonguo4118.cn

SELECT * FROM users;
来源：https://ec.zhonguo2118.cn

[Q16] 查询指定列
来源：https://dm.zhonguo3118.cn

SELECT id, name FROM users;
来源：https://cc.zhonguo7118.cn

[Q17] 条件查询
来源：https://bz.zhonguo3118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://kh.zhonguo7118.cn

[Q18] 模糊匹配
来源：https://gt.zhonguo1118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://dd.zhonguo1118.cn

[Q19] 范围查询
来源：https://ft.zhonguo5118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://tb.zhonguo8118.cn

[Q20] IN 列表
来源：https://fd.zhonguo3118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://xh.zhonguo5118.cn

[Q21] 空值判断
来源：https://yv.zhonguo1118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://od.zhonguo5118.cn

[Q22] 排序
来源：https://cr.zhonguo8118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://od.zhonguo3118.cn

[Q23] 分页
来源：https://td.zhonguo1118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://vl.zhonguo5118.cn

[Q24] 去重
来源：https://wz.zhonguo1118.cn

SELECT DISTINCT city FROM users;
来源：https://wh.zhonguo8118.cn

[Q25] 只取前 N 条
来源：https://bl.zhonguo1118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://ay.zhonguo3118.cn

[Q26] 计数
来源：https://lh.zhonguo2118.cn

SELECT COUNT(*) FROM users;
来源：https://kl.zhonguo3118.cn

[Q27] 条件计数
来源：https://vp.zhonguo7118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://ey.zhonguo2118.cn

[Q28] 求和与平均
来源：https://ie.zhonguo7118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://te.zhonguo3118.cn

[Q29] 最大最小值
来源：https://qe.zhonguo8118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://dj.zhonguo5118.cn

[Q30] 分组统计
来源：https://dx.zhonguo3118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://ud.zhonguo2118.cn

[Q31] 分组后过滤
来源：https://cq.zhonguo3118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://be.zhonguo8118.cn

[Q32] 分组拼接字符串
来源：https://ga.zhonguo6118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://nr.zhonguo6118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://vg.zhonguo1118.cn

[Q33] 多列分组
来源：https://tw.zhonguo1118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://yl.zhonguo1118.cn

[Q34] 每组取第一条
来源：https://wm.zhonguo2118.cn

SELECT * FROM (
来源：https://qv.zhonguo3118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://ky.zhonguo5118.cn

) t WHERE rn = 1;
来源：https://yx.zhonguo8118.cn

[Q35] 内连接
来源：https://jy.zhonguo2118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://is.zhonguo8118.cn

[Q36] 左连接
来源：https://ae.zhonguo3118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://gl.zhonguo6118.cn

[Q37] 右连接
来源：https://el.zhonguo5118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://zy.zhonguo6118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://wy.zhonguo7118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://rh.zhonguo4118.cn

[Q39] 自连接（查上下级）
来源：https://kd.zhonguo5118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://gx.zhonguo1118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://hl.zhonguo2118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://wt.zhonguo1118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://hu.zhonguo3118.cn

[Q41] 多表连接
来源：https://qg.zhonguo6118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://gd.zhonguo6118.cn

JOIN users u ON u.id = o.user_id
来源：https://uk.zhonguo2118.cn

JOIN products p ON p.id = o.product_id;
来源：https://hs.zhonguo5118.cn

[Q42] 连接条件附加过滤
来源：https://ek.zhonguo6118.cn

SELECT u.name, o.amount FROM users u
来源：https://vw.zhonguo1118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://sn.zhonguo6118.cn

[Q43] 标量子查询
来源：https://se.zhonguo4118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://xx.zhonguo5118.cn

[Q44] IN 子查询
来源：https://pw.zhonguo5118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://ls.zhonguo7118.cn

[Q45] EXISTS 判断存在
来源：https://bo.zhonguo2118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://qn.zhonguo7118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://dz.zhonguo8118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://ld.zhonguo6118.cn

[Q47] 与平均值比较
来源：https://lf.zhonguo3118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://gc.zhonguo3118.cn

[Q48] CTE 公用表表达式
来源：https://sg.zhonguo6118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://xb.zhonguo2118.cn

SELECT * FROM t WHERE c > 5;
来源：https://oi.zhonguo8118.cn

[Q49] 更新单行
来源：https://rt.zhonguo8118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://eg.zhonguo3118.cn

[Q50] 批量更新
来源：https://tw.zhonguo7118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://cl.zhonguo2118.cn

[Q51] 用子查询更新
来源：https://wt.zhonguo2118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://kp.zhonguo3118.cn

[Q52] 删除指定行
来源：https://pm.zhonguo7118.cn

DELETE FROM users WHERE id = 10;
来源：https://vb.zhonguo1118.cn

[Q53] 按条件删除
来源：https://cj.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://xp.zhonguo2118.cn

[Q54] 清空表
来源：https://za.zhonguo6118.cn

TRUNCATE TABLE logs;
来源：https://jh.zhonguo2118.cn

[Q55] 排名（并列占位）
来源：https://fd.zhonguo1118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://qo.zhonguo3118.cn

[Q56] 密集排名（并列不占位）
来源：https://ey.zhonguo4118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://xw.zhonguo6118.cn

[Q57] 行号
来源：https://kt.zhonguo4118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://db.zhonguo6118.cn

[Q58] 累计求和
来源：https://ow.zhonguo8118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://pg.zhonguo6118.cn

[Q59] 分组内累计
来源：https://os.zhonguo2118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://tx.zhonguo7118.cn

[Q60] 取上一行 / 下一行
来源：https://vn.zhonguo2118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://co.zhonguo4118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://ba.zhonguo2118.cn

[Q61] 移动平均
来源：https://pw.zhonguo7118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://of.zhonguo8118.cn

[Q62] 分组占比
来源：https://wj.zhonguo8118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://pq.zhonguo2118.cn

[Q63] 开启事务
来源：https://oa.zhonguo3118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://wl.zhonguo1118.cn

[Q64] 提交事务
来源：https://zx.zhonguo5118.cn

COMMIT;
来源：https://ge.zhonguo6118.cn

[Q65] 回滚事务
来源：https://jn.zhonguo1118.cn

ROLLBACK;
来源：https://ew.zhonguo5118.cn

[Q66] 行锁查询
来源：https://iv.zhonguo5118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://pg.zhonguo6118.cn

[Q67] 设置隔离级别
来源：https://tw.zhonguo2118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://mc.zhonguo7118.cn

[Q68] 保存点
来源：https://rh.zhonguo1118.cn

SAVEPOINT sp1;
来源：https://gq.zhonguo3118.cn

ROLLBACK TO sp1;
来源：https://ij.zhonguo3118.cn

[Q69] 查看执行计划
来源：https://ho.zhonguo8118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://si.zhonguo3118.cn

[Q70] 更新统计信息
来源：https://ui.zhonguo5118.cn

ANALYZE TABLE users;
来源：https://fp.zhonguo5118.cn

[Q71] 查看建表语句
来源：https://yh.zhonguo1118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://wk.zhonguo3118.cn

[Q72] 查看索引
来源：https://op.zhonguo5118.cn

SHOW INDEX FROM users;
来源：https://jr.zhonguo7118.cn

[Q73] 查看表状态
来源：https://ci.zhonguo3118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://ue.zhonguo8118.cn

[Q74] 强制使用索引
来源：https://pt.zhonguo2118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://rz.zhonguo2118.cn

[Q75] 日期格式化
来源：https://me.zhonguo8118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://hm.zhonguo3118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://nd.zhonguo7118.cn

[Q76] 按天统计
来源：https://tk.zhonguo4118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://sk.zhonguo1118.cn

[Q77] 时间加减
来源：https://bw.zhonguo2118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://kv.zhonguo8118.cn

[Q78] 当前时间
来源：https://sz.zhonguo3118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://me.zhonguo4118.cn

[Q79] 字符串拼接
来源：https://sw.zhonguo5118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://aa.zhonguo6118.cn

[Q80] 字符串截取
来源：https://mm.zhonguo6118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://at.zhonguo6118.cn

[Q81] 字符串替换
来源：https://ki.zhonguo4118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://dc.zhonguo6118.cn


<!-- 参考信息 -->