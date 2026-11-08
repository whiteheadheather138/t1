代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://zp.zhonguo2118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://st.zhonguo3118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://mo.zhonguo6118.cn

Ruby: a.gcd(b)
来源：https://ue.zhonguo5118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://ed.zhonguo3118.cn

[N06] 判断回文字符串
来源：https://wt.zhonguo1118.cn

Py:   s == s[::-1]
来源：https://ij.zhonguo8118.cn

PHP:  $s === strrev($s);
来源：https://xd.zhonguo7118.cn

JS:   s === [...s].reverse().join("")
来源：https://pi.zhonguo5118.cn

TS:   s === [...s].reverse().join("")
来源：https://uh.zhonguo8118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://sb.zhonguo2118.cn

Go:   // 双指针从两端比较
来源：https://gw.zhonguo3118.cn

Ruby: s == s.reverse
来源：https://ny.zhonguo1118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://kx.zhonguo4118.cn

[N07] 两数之和（返回下标）
来源：https://lx.zhonguo6118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://wf.zhonguo3118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://xe.zhonguo2118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://vc.zhonguo5118.cn

TS:   // 手写 Map<string, number>
来源：https://sr.zhonguo5118.cn

Java: // 手写 HashMap
来源：https://pi.zhonguo7118.cn

Go:   // 手写 map[int]int
来源：https://uf.zhonguo2118.cn

Ruby: // 手写 Hash
来源：https://ae.zhonguo4118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://nu.zhonguo8118.cn

[N08] 生成全排列
来源：https://ro.zhonguo3118.cn

Py:   itertools.permutations(arr)
来源：https://rv.zhonguo1118.cn

PHP:  // 手写递归交换
来源：https://ej.zhonguo7118.cn

JS:   // 手写回溯递归
来源：https://ki.zhonguo1118.cn

TS:   // 手写回溯递归
来源：https://sw.zhonguo3118.cn

Java: // 手写回溯递归
来源：https://mm.zhonguo3118.cn

Go:   // 手写回溯递归
来源：https://ro.zhonguo4118.cn

Ruby: arr.permutation.to_a
来源：https://mm.zhonguo6118.cn

C#:   // 手写回溯递归
来源：https://ig.zhonguo5118.cn

[N09] 栈与队列
来源：https://qc.zhonguo8118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://zv.zhonguo6118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://fj.zhonguo3118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://ei.zhonguo2118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://ln.zhonguo8118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://bi.zhonguo5118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://zm.zhonguo3118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://up.zhonguo8118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://ls.zhonguo4118.cn

[N10] 链表节点定义
来源：https://zc.zhonguo2118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://kq.zhonguo1118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://rz.zhonguo1118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://rx.zhonguo5118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://sg.zhonguo4118.cn

Java: class Node { int v; Node next; }
来源：https://zx.zhonguo6118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://vf.zhonguo5118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://qh.zhonguo3118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://xd.zhonguo1118.cn

[N11] 二叉树中序遍历
来源：https://gs.zhonguo3118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://ak.zhonguo4118.cn

PHP:  // 手写递归函数
来源：https://hu.zhonguo4118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://hr.zhonguo3118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://wj.zhonguo4118.cn

Java: // 手写递归
来源：https://mv.zhonguo2118.cn

Go:   // 手写递归
来源：https://cq.zhonguo5118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://mp.zhonguo8118.cn

C#:   // 手写递归
来源：https://bo.zhonguo6118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://lv.zhonguo5118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://wv.zhonguo5118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://vs.zhonguo6118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://mz.zhonguo2118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://ld.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://zs.zhonguo7118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://fh.zhonguo6118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://ib.zhonguo6118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://uq.zhonguo7118.cn

================================================================================
来源：https://em.zhonguo7118.cn

O. 并发与异步
来源：https://zr.zhonguo1118.cn

================================================================================
来源：https://pk.zhonguo3118.cn

[O01] 启动一个线程
来源：https://cz.zhonguo5118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://ph.zhonguo4118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://vw.zhonguo7118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://bb.zhonguo3118.cn

TS:   // 同 JS
来源：https://rz.zhonguo6118.cn

Java: new Thread(() -> f()).start()
来源：https://rh.zhonguo8118.cn

Go:   go f()
来源：https://ju.zhonguo5118.cn

Ruby: Thread.new { f }
来源：https://kp.zhonguo2118.cn

C#:   Task.Run(() => F());
来源：https://ss.zhonguo7118.cn

[O02] 使用线程池
来源：https://mr.zhonguo3118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://ok.zhonguo4118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://bf.zhonguo3118.cn

JS:   // worker_threads 线程池
来源：https://jh.zhonguo8118.cn

TS:   // worker_threads 线程池
来源：https://ac.zhonguo1118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://gk.zhonguo5118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://hi.zhonguo8118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://bq.zhonguo5118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://tf.zhonguo1118.cn

[O03] 加锁保护共享数据
来源：https://dr.zhonguo1118.cn

Py:   with lock: shared += 1
来源：https://xz.zhonguo4118.cn

PHP:  // 用 flock() 做文件锁
来源：https://yc.zhonguo2118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://tv.zhonguo1118.cn

TS:   // 同 JS
来源：https://ij.zhonguo2118.cn

Java: synchronized (this) { shared++; }
来源：https://zd.zhonguo6118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://dv.zhonguo6118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://pc.zhonguo8118.cn

C#:   lock (gate) { shared++; }
来源：https://fl.zhonguo6118.cn

[O04] 定义异步函数并等待
来源：https://qt.zhonguo5118.cn

Py:   async def f():⏎    await g()
来源：https://bg.zhonguo5118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://ip.zhonguo8118.cn

JS:   async function f() { await g(); }
来源：https://jd.zhonguo7118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://uy.zhonguo6118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://as.zhonguo3118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://wd.zhonguo6118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://ff.zhonguo4118.cn

C#:   async Task F() { await G(); }
来源：https://sc.zhonguo5118.cn

[O05] 并发执行并等待全部完成
来源：https://us.zhonguo1118.cn

Py:   asyncio.gather(*tasks)
来源：https://qx.zhonguo1118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://iy.zhonguo5118.cn

JS:   await Promise.all(tasks)
来源：https://eb.zhonguo5118.cn

TS:   await Promise.all(tasks)
来源：https://sy.zhonguo7118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://rb.zhonguo3118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://gl.zhonguo2118.cn

Ruby: threads.map(&:join)
来源：https://wo.zhonguo4118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://fd.zhonguo1118.cn

[O06] 使用进程池
来源：https://qk.zhonguo6118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://as.zhonguo5118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://fi.zhonguo4118.cn

JS:   // child_process / cluster 模块
来源：https://wi.zhonguo8118.cn

TS:   // child_process / cluster 模块
来源：https://ck.zhonguo7118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://tu.zhonguo4118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://pj.zhonguo2118.cn

Ruby: // fork 块
来源：https://lk.zhonguo3118.cn

C#:   Parallel.For
来源：https://ww.zhonguo8118.cn

================================================================================
来源：https://va.zhonguo4118.cn

P. 常用工具函数
来源：https://fp.zhonguo8118.cn

================================================================================
来源：https://on.zhonguo3118.cn

[P01] 生成 UUID
来源：https://vz.zhonguo4118.cn

Py:   str(uuid.uuid4())
来源：https://mw.zhonguo8118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://dx.zhonguo7118.cn

JS:   crypto.randomUUID()
来源：https://jy.zhonguo6118.cn

TS:   crypto.randomUUID()
来源：https://vd.zhonguo7118.cn

Java: UUID.randomUUID().toString()
来源：https://ba.zhonguo5118.cn

Go:   // 用 github.com/google/uuid
来源：https://bk.zhonguo8118.cn

Ruby: SecureRandom.uuid
来源：https://xu.zhonguo8118.cn

C#:   Guid.NewGuid().ToString()
来源：https://ke.zhonguo3118.cn

[P02] MD5 / SHA256 摘要
来源：https://gi.zhonguo8118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://hv.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://lb.zhonguo3118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://iy.zhonguo7118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://me.zhonguo4118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://nx.zhonguo1118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://wm.zhonguo6118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://no.zhonguo7118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://qx.zhonguo2118.cn

[P03] 生成短随机字符串
来源：https://ua.zhonguo8118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://py.zhonguo2118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://hw.zhonguo4118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://hn.zhonguo3118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://oo.zhonguo8118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://sf.zhonguo1118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://ad.zhonguo5118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://qu.zhonguo1118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://bp.zhonguo3118.cn

[P04] 求长度
来源：https://bh.zhonguo8118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://vq.zhonguo3118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://gr.zhonguo8118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ax.zhonguo3118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ia.zhonguo3118.cn

Java: list.size();  map.size();  s.length()
来源：https://vn.zhonguo3118.cn

Go:   len(arr);  len(m)
来源：https://so.zhonguo2118.cn

Ruby: x.length;  x.size
来源：https://bf.zhonguo4118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://gm.zhonguo3118.cn

[P05] 判断两个对象内容是否相等
来源：https://em.zhonguo4118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://wx.zhonguo5118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://nz.zhonguo4118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://iq.zhonguo6118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://ot.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://qx.zhonguo1118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://mu.zhonguo3118.cn

Ruby: a == b
来源：https://nr.zhonguo6118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://wg.zhonguo1118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://of.zhonguo1118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://hr.zhonguo2118.cn

PHP:  if (empty($x)) {}
来源：https://ia.zhonguo6118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://iv.zhonguo5118.cn

TS:   if (x == null) {}
来源：https://wq.zhonguo8118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://xh.zhonguo7118.cn

Go:   if x == nil {}
来源：https://nx.zhonguo2118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://hr.zhonguo1118.cn

C#:   if (x is null) {}
来源：https://gi.zhonguo7118.cn

[P07] 防抖与节流
来源：https://dc.zhonguo8118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://pv.zhonguo1118.cn

PHP:  // 手写时间戳比较
来源：https://yl.zhonguo7118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://io.zhonguo6118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://ok.zhonguo3118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://jp.zhonguo4118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://or.zhonguo3118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://ym.zhonguo6118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://ka.zhonguo3118.cn

[P08] 处理浮点精度问题
来源：https://so.zhonguo6118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://lz.zhonguo7118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://lp.zhonguo3118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://bi.zhonguo7118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://nt.zhonguo1118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://sf.zhonguo1118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://rs.zhonguo6118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://uo.zhonguo5118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://ol.zhonguo6118.cn

================================================================================
来源：https://pd.zhonguo3118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://fc.zhonguo1118.cn

================================================================================
来源：https://ut.zhonguo4118.cn

[Q01] 创建表
来源：https://ik.zhonguo2118.cn

CREATE TABLE users (
来源：https://ms.zhonguo6118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://fp.zhonguo2118.cn

name VARCHAR(50) NOT NULL,
来源：https://uo.zhonguo3118.cn

email VARCHAR(100) UNIQUE,
来源：https://xv.zhonguo2118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://xq.zhonguo8118.cn

);
来源：https://rn.zhonguo1118.cn

[Q02] 创建带外键的表
来源：https://ab.zhonguo8118.cn

CREATE TABLE orders (
来源：https://bt.zhonguo5118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://iy.zhonguo4118.cn

user_id INT NOT NULL,
来源：https://bk.zhonguo1118.cn

amount DECIMAL(10, 2),
来源：https://xl.zhonguo1118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://av.zhonguo5118.cn

);
来源：https://ny.zhonguo6118.cn

[Q03] 增加列
来源：https://nb.zhonguo2118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://cz.zhonguo7118.cn

[Q04] 修改列类型
来源：https://nu.zhonguo5118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://af.zhonguo1118.cn

[Q05] 重命名列
来源：https://nf.zhonguo3118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://pd.zhonguo2118.cn

[Q06] 删除列
来源：https://at.zhonguo3118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://uo.zhonguo6118.cn

[Q07] 删除表
来源：https://ub.zhonguo7118.cn

DROP TABLE IF EXISTS orders;
来源：https://sp.zhonguo6118.cn

[Q08] 创建普通索引
来源：https://za.zhonguo7118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://rk.zhonguo7118.cn

[Q09] 创建唯一索引
来源：https://zl.zhonguo2118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://bn.zhonguo1118.cn

[Q10] 插入单行
来源：https://cj.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://yg.zhonguo1118.cn

[Q11] 一次插入多行
来源：https://db.zhonguo1118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://ip.zhonguo3118.cn

[Q12] 插入后取自增 ID
来源：https://aj.zhonguo2118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://rq.zhonguo8118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://ke.zhonguo4118.cn

[Q13] 忽略重复插入
来源：https://tp.zhonguo3118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://dq.zhonguo6118.cn

[Q14] 存在则更新（upsert）
来源：https://ai.zhonguo2118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://qn.zhonguo3118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://tz.zhonguo2118.cn

[Q15] 查询全部
来源：https://zt.zhonguo2118.cn

SELECT * FROM users;
来源：https://ds.zhonguo7118.cn

[Q16] 查询指定列
来源：https://ty.zhonguo2118.cn

SELECT id, name FROM users;
来源：https://zc.zhonguo3118.cn

[Q17] 条件查询
来源：https://hu.zhonguo4118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://cv.zhonguo8118.cn

[Q18] 模糊匹配
来源：https://ev.zhonguo7118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://hi.zhonguo8118.cn

[Q19] 范围查询
来源：https://md.zhonguo5118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://ew.zhonguo7118.cn

[Q20] IN 列表
来源：https://ag.zhonguo4118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://oq.zhonguo4118.cn

[Q21] 空值判断
来源：https://kt.zhonguo8118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://yi.zhonguo8118.cn

[Q22] 排序
来源：https://jf.zhonguo1118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://ko.zhonguo2118.cn

[Q23] 分页
来源：https://by.zhonguo5118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://sx.zhonguo7118.cn

[Q24] 去重
来源：https://sg.zhonguo7118.cn

SELECT DISTINCT city FROM users;
来源：https://by.zhonguo2118.cn

[Q25] 只取前 N 条
来源：https://we.zhonguo5118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://uy.zhonguo1118.cn

[Q26] 计数
来源：https://un.zhonguo3118.cn

SELECT COUNT(*) FROM users;
来源：https://sj.zhonguo8118.cn

[Q27] 条件计数
来源：https://hw.zhonguo4118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://dv.zhonguo2118.cn

[Q28] 求和与平均
来源：https://fz.zhonguo1118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://ph.zhonguo4118.cn

[Q29] 最大最小值
来源：https://ky.zhonguo2118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://jh.zhonguo5118.cn

[Q30] 分组统计
来源：https://uh.zhonguo4118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://bs.zhonguo4118.cn

[Q31] 分组后过滤
来源：https://ju.zhonguo8118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://cc.zhonguo4118.cn

[Q32] 分组拼接字符串
来源：https://qj.zhonguo4118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://yb.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://jy.zhonguo1118.cn

[Q33] 多列分组
来源：https://rb.zhonguo1118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://ks.zhonguo7118.cn

[Q34] 每组取第一条
来源：https://mb.zhonguo5118.cn

SELECT * FROM (
来源：https://ay.zhonguo7118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://xk.zhonguo4118.cn

) t WHERE rn = 1;
来源：https://jq.zhonguo8118.cn

[Q35] 内连接
来源：https://xw.zhonguo3118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://dy.zhonguo1118.cn

[Q36] 左连接
来源：https://ud.zhonguo3118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://ws.zhonguo7118.cn

[Q37] 右连接
来源：https://lm.zhonguo3118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://kz.zhonguo1118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://ge.zhonguo7118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://bf.zhonguo1118.cn

[Q39] 自连接（查上下级）
来源：https://on.zhonguo5118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://km.zhonguo1118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://zt.zhonguo8118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://uw.zhonguo1118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://sg.zhonguo2118.cn

[Q41] 多表连接
来源：https://pq.zhonguo5118.cn


<!-- 参考信息 -->