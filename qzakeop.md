代发 wailian999

Go:   // 手写 map[int]int
来源：https://yx.zhonguo5118.cn

Ruby: // 手写 Hash
来源：https://xa.zhonguo4118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://uw.zhonguo7118.cn

[N08] 生成全排列
来源：https://ht.zhonguo8118.cn

Py:   itertools.permutations(arr)
来源：https://ol.zhonguo6118.cn

PHP:  // 手写递归交换
来源：https://cj.zhonguo3118.cn

JS:   // 手写回溯递归
来源：https://cq.zhonguo2118.cn

TS:   // 手写回溯递归
来源：https://qb.zhonguo2118.cn

Java: // 手写回溯递归
来源：https://jd.zhonguo1118.cn

Go:   // 手写回溯递归
来源：https://sl.zhonguo1118.cn

Ruby: arr.permutation.to_a
来源：https://pd.zhonguo5118.cn

C#:   // 手写回溯递归
来源：https://ph.zhonguo8118.cn

[N09] 栈与队列
来源：https://up.zhonguo1118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://qk.zhonguo6118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://gy.zhonguo8118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://er.zhonguo2118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://bf.zhonguo7118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://sm.zhonguo5118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://nl.zhonguo8118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://nw.zhonguo7118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://xj.zhonguo6118.cn

[N10] 链表节点定义
来源：https://oc.zhonguo8118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://vk.zhonguo2118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://ag.zhonguo2118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://py.zhonguo3118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://lk.zhonguo7118.cn

Java: class Node { int v; Node next; }
来源：https://kx.zhonguo8118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://tb.zhonguo3118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://rh.zhonguo6118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://iq.zhonguo5118.cn

[N11] 二叉树中序遍历
来源：https://ez.zhonguo8118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://ic.zhonguo8118.cn

PHP:  // 手写递归函数
来源：https://zn.zhonguo6118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ig.zhonguo3118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://pd.zhonguo7118.cn

Java: // 手写递归
来源：https://ge.zhonguo2118.cn

Go:   // 手写递归
来源：https://fu.zhonguo2118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://hd.zhonguo5118.cn

C#:   // 手写递归
来源：https://zp.zhonguo7118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://vs.zhonguo7118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://ac.zhonguo7118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://rn.zhonguo6118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://he.zhonguo5118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://wq.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://wy.zhonguo7118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://jl.zhonguo6118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://am.zhonguo6118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://bi.zhonguo5118.cn

================================================================================
来源：https://jb.zhonguo5118.cn

O. 并发与异步
来源：https://op.zhonguo8118.cn

================================================================================
来源：https://lu.zhonguo1118.cn

[O01] 启动一个线程
来源：https://bp.zhonguo4118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://kk.zhonguo4118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://sb.zhonguo2118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://sg.zhonguo7118.cn

TS:   // 同 JS
来源：https://qt.zhonguo7118.cn

Java: new Thread(() -> f()).start()
来源：https://ti.zhonguo6118.cn

Go:   go f()
来源：https://ki.zhonguo6118.cn

Ruby: Thread.new { f }
来源：https://ad.zhonguo5118.cn

C#:   Task.Run(() => F());
来源：https://cl.zhonguo5118.cn

[O02] 使用线程池
来源：https://uy.zhonguo4118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://iy.zhonguo8118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://gs.zhonguo3118.cn

JS:   // worker_threads 线程池
来源：https://jy.zhonguo7118.cn

TS:   // worker_threads 线程池
来源：https://qp.zhonguo5118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://gb.zhonguo1118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://sy.zhonguo6118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://os.zhonguo6118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://dd.zhonguo7118.cn

[O03] 加锁保护共享数据
来源：https://jk.zhonguo2118.cn

Py:   with lock: shared += 1
来源：https://ms.zhonguo7118.cn

PHP:  // 用 flock() 做文件锁
来源：https://os.zhonguo7118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://uv.zhonguo5118.cn

TS:   // 同 JS
来源：https://sw.zhonguo8118.cn

Java: synchronized (this) { shared++; }
来源：https://ay.zhonguo6118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://jk.zhonguo3118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://mw.zhonguo5118.cn

C#:   lock (gate) { shared++; }
来源：https://ey.zhonguo5118.cn

[O04] 定义异步函数并等待
来源：https://xp.zhonguo5118.cn

Py:   async def f():⏎    await g()
来源：https://dn.zhonguo8118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://gz.zhonguo4118.cn

JS:   async function f() { await g(); }
来源：https://au.zhonguo8118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://da.zhonguo5118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://jq.zhonguo5118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://jz.zhonguo6118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://fa.zhonguo8118.cn

C#:   async Task F() { await G(); }
来源：https://oo.zhonguo6118.cn

[O05] 并发执行并等待全部完成
来源：https://be.zhonguo3118.cn

Py:   asyncio.gather(*tasks)
来源：https://ix.zhonguo3118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://se.zhonguo1118.cn

JS:   await Promise.all(tasks)
来源：https://hk.zhonguo3118.cn

TS:   await Promise.all(tasks)
来源：https://zv.zhonguo5118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://cv.zhonguo5118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://nw.zhonguo6118.cn

Ruby: threads.map(&:join)
来源：https://xr.zhonguo3118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://zk.zhonguo5118.cn

[O06] 使用进程池
来源：https://nh.zhonguo4118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://fk.zhonguo3118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://tm.zhonguo7118.cn

JS:   // child_process / cluster 模块
来源：https://qj.zhonguo1118.cn

TS:   // child_process / cluster 模块
来源：https://cw.zhonguo4118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://mu.zhonguo1118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://ym.zhonguo5118.cn

Ruby: // fork 块
来源：https://vd.zhonguo6118.cn

C#:   Parallel.For
来源：https://hb.zhonguo5118.cn

================================================================================
来源：https://tg.zhonguo6118.cn

P. 常用工具函数
来源：https://eq.zhonguo6118.cn

================================================================================
来源：https://en.zhonguo1118.cn

[P01] 生成 UUID
来源：https://zd.zhonguo5118.cn

Py:   str(uuid.uuid4())
来源：https://fu.zhonguo4118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://zg.zhonguo6118.cn

JS:   crypto.randomUUID()
来源：https://ec.zhonguo6118.cn

TS:   crypto.randomUUID()
来源：https://rv.zhonguo3118.cn

Java: UUID.randomUUID().toString()
来源：https://hz.zhonguo5118.cn

Go:   // 用 github.com/google/uuid
来源：https://me.zhonguo2118.cn

Ruby: SecureRandom.uuid
来源：https://nl.zhonguo1118.cn

C#:   Guid.NewGuid().ToString()
来源：https://qa.zhonguo5118.cn

[P02] MD5 / SHA256 摘要
来源：https://tc.zhonguo5118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://ma.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://ru.zhonguo5118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://ry.zhonguo4118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://mr.zhonguo7118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://yt.zhonguo2118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://gr.zhonguo8118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://zt.zhonguo3118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://de.zhonguo7118.cn

[P03] 生成短随机字符串
来源：https://ke.zhonguo7118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://rs.zhonguo1118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://rp.zhonguo6118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://dh.zhonguo2118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://ud.zhonguo7118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://yr.zhonguo7118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://ep.zhonguo8118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://pf.zhonguo7118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://gz.zhonguo6118.cn

[P04] 求长度
来源：https://cl.zhonguo4118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://vm.zhonguo5118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://sr.zhonguo8118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://to.zhonguo6118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ko.zhonguo2118.cn

Java: list.size();  map.size();  s.length()
来源：https://tz.zhonguo3118.cn

Go:   len(arr);  len(m)
来源：https://et.zhonguo8118.cn

Ruby: x.length;  x.size
来源：https://wj.zhonguo1118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://yz.zhonguo7118.cn

[P05] 判断两个对象内容是否相等
来源：https://gk.zhonguo5118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://ht.zhonguo1118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://fk.zhonguo6118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://lh.zhonguo1118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://hi.zhonguo4118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://yn.zhonguo8118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://zc.zhonguo8118.cn

Ruby: a == b
来源：https://fx.zhonguo4118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://zi.zhonguo4118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://dd.zhonguo1118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://rb.zhonguo6118.cn

PHP:  if (empty($x)) {}
来源：https://np.zhonguo3118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://ow.zhonguo3118.cn

TS:   if (x == null) {}
来源：https://di.zhonguo7118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://ot.zhonguo1118.cn

Go:   if x == nil {}
来源：https://bf.zhonguo2118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://zq.zhonguo1118.cn

C#:   if (x is null) {}
来源：https://rn.zhonguo3118.cn

[P07] 防抖与节流
来源：https://jv.zhonguo8118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://ff.zhonguo3118.cn

PHP:  // 手写时间戳比较
来源：https://av.zhonguo8118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://hn.zhonguo6118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://vd.zhonguo6118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://im.zhonguo6118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://gn.zhonguo8118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://rq.zhonguo7118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://bn.zhonguo2118.cn

[P08] 处理浮点精度问题
来源：https://xw.zhonguo8118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://ql.zhonguo5118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://yn.zhonguo3118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://vt.zhonguo8118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://yg.zhonguo4118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://ce.zhonguo5118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://mk.zhonguo7118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://uo.zhonguo1118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://ql.zhonguo2118.cn

================================================================================
来源：https://ub.zhonguo3118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://yn.zhonguo6118.cn

================================================================================
来源：https://gb.zhonguo4118.cn

[Q01] 创建表
来源：https://eg.zhonguo7118.cn

CREATE TABLE users (
来源：https://yc.zhonguo6118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://hy.zhonguo1118.cn

name VARCHAR(50) NOT NULL,
来源：https://bs.zhonguo4118.cn

email VARCHAR(100) UNIQUE,
来源：https://vz.zhonguo5118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://ro.zhonguo3118.cn

);
来源：https://az.zhonguo6118.cn

[Q02] 创建带外键的表
来源：https://hx.zhonguo4118.cn

CREATE TABLE orders (
来源：https://ht.zhonguo2118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://pl.zhonguo1118.cn

user_id INT NOT NULL,
来源：https://ii.zhonguo4118.cn

amount DECIMAL(10, 2),
来源：https://du.zhonguo1118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://me.zhonguo2118.cn

);
来源：https://hm.zhonguo4118.cn

[Q03] 增加列
来源：https://xq.zhonguo6118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://vw.zhonguo5118.cn

[Q04] 修改列类型
来源：https://wa.zhonguo2118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://nv.zhonguo4118.cn

[Q05] 重命名列
来源：https://dh.zhonguo4118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://pa.zhonguo3118.cn

[Q06] 删除列
来源：https://gt.zhonguo1118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://cy.zhonguo2118.cn

[Q07] 删除表
来源：https://cc.zhonguo1118.cn

DROP TABLE IF EXISTS orders;
来源：https://jo.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://ht.zhonguo8118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://qy.zhonguo5118.cn

[Q09] 创建唯一索引
来源：https://lt.zhonguo7118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://dm.zhonguo2118.cn

[Q10] 插入单行
来源：https://jv.zhonguo2118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://xq.zhonguo8118.cn

[Q11] 一次插入多行
来源：https://lr.zhonguo4118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://de.zhonguo5118.cn

[Q12] 插入后取自增 ID
来源：https://xi.zhonguo7118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://jk.zhonguo5118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://zx.zhonguo7118.cn

[Q13] 忽略重复插入
来源：https://cc.zhonguo6118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://dt.zhonguo6118.cn

[Q14] 存在则更新（upsert）
来源：https://or.zhonguo3118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://dv.zhonguo2118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://ga.zhonguo2118.cn

[Q15] 查询全部
来源：https://zb.zhonguo8118.cn

SELECT * FROM users;
来源：https://sj.zhonguo2118.cn

[Q16] 查询指定列
来源：https://yh.zhonguo2118.cn

SELECT id, name FROM users;
来源：https://il.zhonguo4118.cn

[Q17] 条件查询
来源：https://wx.zhonguo3118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://bk.zhonguo5118.cn

[Q18] 模糊匹配
来源：https://eg.zhonguo6118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://sz.zhonguo6118.cn

[Q19] 范围查询
来源：https://ha.zhonguo8118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://nk.zhonguo6118.cn

[Q20] IN 列表
来源：https://xq.zhonguo3118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://mn.zhonguo7118.cn

[Q21] 空值判断
来源：https://ln.zhonguo2118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://lw.zhonguo2118.cn

[Q22] 排序
来源：https://od.zhonguo5118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://kz.zhonguo3118.cn

[Q23] 分页
来源：https://ys.zhonguo4118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://rb.zhonguo1118.cn

[Q24] 去重
来源：https://ai.zhonguo7118.cn

SELECT DISTINCT city FROM users;
来源：https://tt.zhonguo5118.cn

[Q25] 只取前 N 条
来源：https://qq.zhonguo8118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://ib.zhonguo3118.cn

[Q26] 计数
来源：https://dt.zhonguo6118.cn

SELECT COUNT(*) FROM users;
来源：https://hv.zhonguo7118.cn

[Q27] 条件计数
来源：https://lt.zhonguo5118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://yx.zhonguo5118.cn

[Q28] 求和与平均
来源：https://ck.zhonguo6118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://tm.zhonguo8118.cn

[Q29] 最大最小值
来源：https://ji.zhonguo7118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://yw.zhonguo7118.cn

[Q30] 分组统计
来源：https://fs.zhonguo2118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://vm.zhonguo5118.cn

[Q31] 分组后过滤
来源：https://xf.zhonguo6118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://nk.zhonguo7118.cn

[Q32] 分组拼接字符串
来源：https://lq.zhonguo2118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://yg.zhonguo8118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://hv.zhonguo6118.cn

[Q33] 多列分组
来源：https://nm.zhonguo4118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://ih.zhonguo4118.cn

[Q34] 每组取第一条
来源：https://mm.zhonguo8118.cn

SELECT * FROM (
来源：https://np.zhonguo1118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://nk.zhonguo5118.cn

) t WHERE rn = 1;
来源：https://io.zhonguo8118.cn

[Q35] 内连接
来源：https://ud.zhonguo6118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://ru.zhonguo2118.cn

[Q36] 左连接
来源：https://hx.zhonguo3118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://vx.zhonguo1118.cn

[Q37] 右连接
来源：https://hd.zhonguo2118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://ey.zhonguo7118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://wg.zhonguo2118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://nh.zhonguo7118.cn

[Q39] 自连接（查上下级）
来源：https://md.zhonguo5118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://wu.zhonguo8118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://jo.zhonguo4118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://ly.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://wo.zhonguo6118.cn

[Q41] 多表连接
来源：https://nv.zhonguo2118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://be.zhonguo2118.cn

JOIN users u ON u.id = o.user_id
来源：https://ef.zhonguo1118.cn

JOIN products p ON p.id = o.product_id;
来源：https://km.zhonguo5118.cn

[Q42] 连接条件附加过滤
来源：https://sd.zhonguo8118.cn

SELECT u.name, o.amount FROM users u
来源：https://ev.zhonguo4118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://jy.zhonguo1118.cn

[Q43] 标量子查询
来源：https://zn.zhonguo2118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://nf.zhonguo5118.cn

[Q44] IN 子查询
来源：https://ut.zhonguo3118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://ii.zhonguo5118.cn

[Q45] EXISTS 判断存在
来源：https://xi.zhonguo5118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://yi.zhonguo3118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://cf.zhonguo4118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://cc.zhonguo2118.cn

[Q47] 与平均值比较
来源：https://kz.zhonguo8118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://gz.zhonguo2118.cn

[Q48] CTE 公用表表达式
来源：https://ik.zhonguo7118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://kb.zhonguo5118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ut.zhonguo8118.cn

[Q49] 更新单行
来源：https://dw.zhonguo4118.cn


<!-- 参考信息 -->