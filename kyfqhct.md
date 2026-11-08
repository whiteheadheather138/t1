代发 wailian999

Java: // 手写回溯递归
来源：https://ys.zhonguo3118.cn

Go:   // 手写回溯递归
来源：https://xb.zhonguo7118.cn

Ruby: arr.permutation.to_a
来源：https://kj.zhonguo4118.cn

C#:   // 手写回溯递归
来源：https://qa.zhonguo7118.cn

[N09] 栈与队列
来源：https://jw.zhonguo5118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://cc.zhonguo1118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://ci.zhonguo8118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://se.zhonguo2118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://uq.zhonguo7118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://kj.zhonguo3118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://zw.zhonguo6118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://wh.zhonguo3118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://fz.zhonguo7118.cn

[N10] 链表节点定义
来源：https://hv.zhonguo4118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://pg.zhonguo8118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://ov.zhonguo6118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://ci.zhonguo2118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://rp.zhonguo2118.cn

Java: class Node { int v; Node next; }
来源：https://ip.zhonguo8118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://ch.zhonguo1118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://kz.zhonguo6118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://rf.zhonguo5118.cn

[N11] 二叉树中序遍历
来源：https://dd.zhonguo7118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://pe.zhonguo2118.cn

PHP:  // 手写递归函数
来源：https://ca.zhonguo2118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://wo.zhonguo7118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://wv.zhonguo8118.cn

Java: // 手写递归
来源：https://ek.zhonguo2118.cn

Go:   // 手写递归
来源：https://lw.zhonguo1118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://ci.zhonguo3118.cn

C#:   // 手写递归
来源：https://jj.zhonguo8118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://mz.zhonguo1118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://ge.zhonguo6118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://qj.zhonguo2118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://tn.zhonguo7118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://ge.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://aq.zhonguo3118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://jx.zhonguo2118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://wx.zhonguo5118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://ab.zhonguo3118.cn

================================================================================
来源：https://bk.zhonguo8118.cn

O. 并发与异步
来源：https://bm.zhonguo6118.cn

================================================================================
来源：https://ii.zhonguo7118.cn

[O01] 启动一个线程
来源：https://jf.zhonguo2118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://sl.zhonguo8118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://ib.zhonguo5118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://bc.zhonguo5118.cn

TS:   // 同 JS
来源：https://oq.zhonguo2118.cn

Java: new Thread(() -> f()).start()
来源：https://ym.zhonguo3118.cn

Go:   go f()
来源：https://zl.zhonguo3118.cn

Ruby: Thread.new { f }
来源：https://tq.zhonguo8118.cn

C#:   Task.Run(() => F());
来源：https://zz.zhonguo5118.cn

[O02] 使用线程池
来源：https://no.zhonguo3118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://kf.zhonguo8118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://lo.zhonguo6118.cn

JS:   // worker_threads 线程池
来源：https://ic.zhonguo3118.cn

TS:   // worker_threads 线程池
来源：https://ay.zhonguo7118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://ki.zhonguo7118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://wi.zhonguo4118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://to.zhonguo4118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://oz.zhonguo4118.cn

[O03] 加锁保护共享数据
来源：https://wk.zhonguo2118.cn

Py:   with lock: shared += 1
来源：https://ke.zhonguo6118.cn

PHP:  // 用 flock() 做文件锁
来源：https://yx.zhonguo1118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://xq.zhonguo2118.cn

TS:   // 同 JS
来源：https://ln.zhonguo3118.cn

Java: synchronized (this) { shared++; }
来源：https://dd.zhonguo8118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://cx.zhonguo8118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://ca.zhonguo4118.cn

C#:   lock (gate) { shared++; }
来源：https://dh.zhonguo8118.cn

[O04] 定义异步函数并等待
来源：https://kp.zhonguo6118.cn

Py:   async def f():⏎    await g()
来源：https://tp.zhonguo5118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://ho.zhonguo8118.cn

JS:   async function f() { await g(); }
来源：https://hl.zhonguo3118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://yo.zhonguo3118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://pl.zhonguo3118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://om.zhonguo3118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://tn.zhonguo1118.cn

C#:   async Task F() { await G(); }
来源：https://tk.zhonguo2118.cn

[O05] 并发执行并等待全部完成
来源：https://eo.zhonguo2118.cn

Py:   asyncio.gather(*tasks)
来源：https://ij.zhonguo3118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://kw.zhonguo1118.cn

JS:   await Promise.all(tasks)
来源：https://ft.zhonguo1118.cn

TS:   await Promise.all(tasks)
来源：https://fb.zhonguo2118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://as.zhonguo6118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://ah.zhonguo1118.cn

Ruby: threads.map(&:join)
来源：https://en.zhonguo2118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://em.zhonguo4118.cn

[O06] 使用进程池
来源：https://qh.zhonguo1118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://li.zhonguo1118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://yk.zhonguo7118.cn

JS:   // child_process / cluster 模块
来源：https://sh.zhonguo2118.cn

TS:   // child_process / cluster 模块
来源：https://ju.zhonguo2118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://ns.zhonguo3118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://xz.zhonguo5118.cn

Ruby: // fork 块
来源：https://hv.zhonguo1118.cn

C#:   Parallel.For
来源：https://tx.zhonguo1118.cn

================================================================================
来源：https://ke.zhonguo1118.cn

P. 常用工具函数
来源：https://ka.zhonguo2118.cn

================================================================================
来源：https://sx.zhonguo7118.cn

[P01] 生成 UUID
来源：https://kl.zhonguo4118.cn

Py:   str(uuid.uuid4())
来源：https://zt.zhonguo6118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://wf.zhonguo2118.cn

JS:   crypto.randomUUID()
来源：https://nn.zhonguo3118.cn

TS:   crypto.randomUUID()
来源：https://lg.zhonguo7118.cn

Java: UUID.randomUUID().toString()
来源：https://ug.zhonguo6118.cn

Go:   // 用 github.com/google/uuid
来源：https://rs.zhonguo6118.cn

Ruby: SecureRandom.uuid
来源：https://qr.zhonguo7118.cn

C#:   Guid.NewGuid().ToString()
来源：https://ya.zhonguo7118.cn

[P02] MD5 / SHA256 摘要
来源：https://sb.zhonguo3118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://pw.zhonguo6118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://gm.zhonguo5118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://qm.zhonguo4118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://ki.zhonguo6118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://tj.zhonguo8118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://jn.zhonguo1118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://iu.zhonguo3118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://sv.zhonguo6118.cn

[P03] 生成短随机字符串
来源：https://wp.zhonguo4118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://bp.zhonguo6118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://bg.zhonguo3118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://kt.zhonguo1118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://vt.zhonguo6118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://sm.zhonguo2118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://we.zhonguo5118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://me.zhonguo8118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://yi.zhonguo2118.cn

[P04] 求长度
来源：https://xl.zhonguo6118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://fr.zhonguo1118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://bt.zhonguo3118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://xq.zhonguo2118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://cf.zhonguo7118.cn

Java: list.size();  map.size();  s.length()
来源：https://ht.zhonguo4118.cn

Go:   len(arr);  len(m)
来源：https://oy.zhonguo7118.cn

Ruby: x.length;  x.size
来源：https://eb.zhonguo8118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://fo.zhonguo5118.cn

[P05] 判断两个对象内容是否相等
来源：https://cb.zhonguo3118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://hx.zhonguo2118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://lt.zhonguo6118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://aw.zhonguo5118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://ts.zhonguo2118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://sh.zhonguo7118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://fw.zhonguo1118.cn

Ruby: a == b
来源：https://fe.zhonguo5118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://yu.zhonguo2118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://yd.zhonguo5118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://qn.zhonguo7118.cn

PHP:  if (empty($x)) {}
来源：https://bf.zhonguo4118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://xn.zhonguo5118.cn

TS:   if (x == null) {}
来源：https://xh.zhonguo2118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://rr.zhonguo3118.cn

Go:   if x == nil {}
来源：https://uh.zhonguo7118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://rm.zhonguo5118.cn

C#:   if (x is null) {}
来源：https://ig.zhonguo4118.cn

[P07] 防抖与节流
来源：https://cg.zhonguo7118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://ui.zhonguo3118.cn

PHP:  // 手写时间戳比较
来源：https://vo.zhonguo2118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://mk.zhonguo8118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://tg.zhonguo4118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://kt.zhonguo5118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://xc.zhonguo1118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://fr.zhonguo3118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://iy.zhonguo4118.cn

[P08] 处理浮点精度问题
来源：https://lz.zhonguo8118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://lz.zhonguo2118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://px.zhonguo5118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://fs.zhonguo2118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://bb.zhonguo6118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://mm.zhonguo7118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://dg.zhonguo3118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://jf.zhonguo2118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://hf.zhonguo4118.cn

================================================================================
来源：https://jp.zhonguo6118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://zd.zhonguo7118.cn

================================================================================
来源：https://ab.zhonguo6118.cn

[Q01] 创建表
来源：https://yk.zhonguo8118.cn

CREATE TABLE users (
来源：https://wl.zhonguo5118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://yb.zhonguo7118.cn

name VARCHAR(50) NOT NULL,
来源：https://nx.zhonguo7118.cn

email VARCHAR(100) UNIQUE,
来源：https://im.zhonguo8118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://az.zhonguo5118.cn

);
来源：https://zj.zhonguo3118.cn

[Q02] 创建带外键的表
来源：https://or.zhonguo4118.cn

CREATE TABLE orders (
来源：https://lc.zhonguo2118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://ts.zhonguo5118.cn

user_id INT NOT NULL,
来源：https://ca.zhonguo5118.cn

amount DECIMAL(10, 2),
来源：https://ij.zhonguo8118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://oz.zhonguo6118.cn

);
来源：https://rz.zhonguo6118.cn

[Q03] 增加列
来源：https://ij.zhonguo2118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://xg.zhonguo3118.cn

[Q04] 修改列类型
来源：https://lf.zhonguo5118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://nm.zhonguo3118.cn

[Q05] 重命名列
来源：https://kp.zhonguo6118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://cz.zhonguo2118.cn

[Q06] 删除列
来源：https://cn.zhonguo5118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://xw.zhonguo4118.cn

[Q07] 删除表
来源：https://kn.zhonguo2118.cn

DROP TABLE IF EXISTS orders;
来源：https://tl.zhonguo6118.cn

[Q08] 创建普通索引
来源：https://vg.zhonguo1118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://le.zhonguo3118.cn

[Q09] 创建唯一索引
来源：https://bv.zhonguo5118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://xi.zhonguo4118.cn

[Q10] 插入单行
来源：https://ak.zhonguo3118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://dv.zhonguo3118.cn

[Q11] 一次插入多行
来源：https://iu.zhonguo3118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://nq.zhonguo8118.cn

[Q12] 插入后取自增 ID
来源：https://mg.zhonguo4118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://ns.zhonguo7118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://gt.zhonguo5118.cn

[Q13] 忽略重复插入
来源：https://bb.zhonguo1118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://cm.zhonguo3118.cn

[Q14] 存在则更新（upsert）
来源：https://jg.zhonguo4118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://up.zhonguo5118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://xf.zhonguo7118.cn

[Q15] 查询全部
来源：https://vx.zhonguo1118.cn

SELECT * FROM users;
来源：https://sx.zhonguo7118.cn

[Q16] 查询指定列
来源：https://xo.zhonguo5118.cn

SELECT id, name FROM users;
来源：https://md.zhonguo3118.cn

[Q17] 条件查询
来源：https://jp.zhonguo5118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://zk.zhonguo8118.cn

[Q18] 模糊匹配
来源：https://ij.zhonguo7118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://aq.zhonguo2118.cn

[Q19] 范围查询
来源：https://gd.zhonguo3118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://zw.zhonguo4118.cn

[Q20] IN 列表
来源：https://il.zhonguo7118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://ve.zhonguo5118.cn

[Q21] 空值判断
来源：https://ru.zhonguo2118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://yl.zhonguo8118.cn

[Q22] 排序
来源：https://al.zhonguo1118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://mx.zhonguo6118.cn

[Q23] 分页
来源：https://zb.zhonguo7118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://gw.zhonguo6118.cn

[Q24] 去重
来源：https://nt.zhonguo1118.cn

SELECT DISTINCT city FROM users;
来源：https://rg.zhonguo1118.cn

[Q25] 只取前 N 条
来源：https://sp.zhonguo8118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://um.zhonguo3118.cn

[Q26] 计数
来源：https://xa.zhonguo8118.cn

SELECT COUNT(*) FROM users;
来源：https://az.zhonguo8118.cn

[Q27] 条件计数
来源：https://sd.zhonguo5118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://nb.zhonguo4118.cn

[Q28] 求和与平均
来源：https://qh.zhonguo6118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://fp.zhonguo4118.cn

[Q29] 最大最小值
来源：https://pw.zhonguo8118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://ek.zhonguo5118.cn

[Q30] 分组统计
来源：https://tp.zhonguo5118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://bq.zhonguo2118.cn

[Q31] 分组后过滤
来源：https://zf.zhonguo7118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://oi.zhonguo8118.cn

[Q32] 分组拼接字符串
来源：https://ru.zhonguo1118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://hs.zhonguo3118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://fo.zhonguo8118.cn

[Q33] 多列分组
来源：https://gh.zhonguo7118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://sl.zhonguo3118.cn

[Q34] 每组取第一条
来源：https://vl.zhonguo3118.cn

SELECT * FROM (
来源：https://ig.zhonguo4118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://jp.zhonguo3118.cn

) t WHERE rn = 1;
来源：https://kw.zhonguo6118.cn

[Q35] 内连接
来源：https://do.zhonguo4118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://ir.zhonguo6118.cn

[Q36] 左连接
来源：https://fa.zhonguo4118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://lq.zhonguo5118.cn

[Q37] 右连接
来源：https://gx.zhonguo8118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://eb.zhonguo6118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://kj.zhonguo8118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://cg.zhonguo4118.cn

[Q39] 自连接（查上下级）
来源：https://cw.zhonguo8118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://hp.zhonguo6118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://nm.zhonguo8118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://zf.zhonguo4118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://me.zhonguo3118.cn

[Q41] 多表连接
来源：https://da.zhonguo2118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://kj.zhonguo5118.cn

JOIN users u ON u.id = o.user_id
来源：https://oi.zhonguo4118.cn

JOIN products p ON p.id = o.product_id;
来源：https://id.zhonguo1118.cn

[Q42] 连接条件附加过滤
来源：https://vc.zhonguo5118.cn

SELECT u.name, o.amount FROM users u
来源：https://zt.zhonguo3118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://lu.zhonguo4118.cn

[Q43] 标量子查询
来源：https://dv.zhonguo7118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://sq.zhonguo3118.cn

[Q44] IN 子查询
来源：https://os.zhonguo3118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://hu.zhonguo1118.cn

[Q45] EXISTS 判断存在
来源：https://cv.zhonguo1118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://va.zhonguo1118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://yb.zhonguo1118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://pw.zhonguo5118.cn

[Q47] 与平均值比较
来源：https://jx.zhonguo6118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://fr.zhonguo8118.cn

[Q48] CTE 公用表表达式
来源：https://yk.zhonguo1118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://lz.zhonguo2118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ap.zhonguo2118.cn

[Q49] 更新单行
来源：https://oc.zhonguo1118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://lw.zhonguo5118.cn

[Q50] 批量更新
来源：https://oh.zhonguo1118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://uw.zhonguo3118.cn

[Q51] 用子查询更新
来源：https://nd.zhonguo7118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://bi.zhonguo4118.cn

[Q52] 删除指定行
来源：https://sy.zhonguo8118.cn

DELETE FROM users WHERE id = 10;
来源：https://nk.zhonguo1118.cn

[Q53] 按条件删除
来源：https://pn.zhonguo4118.cn


<!-- 参考信息 -->