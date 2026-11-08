代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：https://os.zhonguo3118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://zq.zhonguo3118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://ej.zhonguo2118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://ry.zhonguo7118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://hy.zhonguo6118.cn

[N10] 链表节点定义
来源：https://nx.zhonguo7118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://vi.zhonguo7118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://sa.zhonguo4118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://vr.zhonguo1118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://nl.zhonguo8118.cn

Java: class Node { int v; Node next; }
来源：https://bq.zhonguo7118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://xj.zhonguo5118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://oc.zhonguo8118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://mf.zhonguo1118.cn

[N11] 二叉树中序遍历
来源：https://df.zhonguo7118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://ck.zhonguo4118.cn

PHP:  // 手写递归函数
来源：https://tt.zhonguo5118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://di.zhonguo1118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ui.zhonguo6118.cn

Java: // 手写递归
来源：https://vi.zhonguo8118.cn

Go:   // 手写递归
来源：https://wn.zhonguo2118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://aq.zhonguo5118.cn

C#:   // 手写递归
来源：https://pr.zhonguo4118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://vm.zhonguo5118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://kr.zhonguo7118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://md.zhonguo6118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://en.zhonguo8118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://qf.zhonguo5118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://kb.zhonguo3118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://qm.zhonguo2118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://vb.zhonguo3118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://ce.zhonguo8118.cn

================================================================================
来源：https://dq.zhonguo3118.cn

O. 并发与异步
来源：https://tx.zhonguo7118.cn

================================================================================
来源：https://jq.zhonguo5118.cn

[O01] 启动一个线程
来源：https://et.zhonguo4118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://ud.zhonguo4118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://nf.zhonguo3118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://gx.zhonguo4118.cn

TS:   // 同 JS
来源：https://tt.zhonguo6118.cn

Java: new Thread(() -> f()).start()
来源：https://sf.zhonguo1118.cn

Go:   go f()
来源：https://ct.zhonguo6118.cn

Ruby: Thread.new { f }
来源：https://dh.zhonguo4118.cn

C#:   Task.Run(() => F());
来源：https://tj.zhonguo2118.cn

[O02] 使用线程池
来源：https://dx.zhonguo7118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://fq.zhonguo4118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://gi.zhonguo2118.cn

JS:   // worker_threads 线程池
来源：https://gh.zhonguo3118.cn

TS:   // worker_threads 线程池
来源：https://oj.zhonguo8118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://hw.zhonguo3118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://qx.zhonguo8118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://je.zhonguo2118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://zd.zhonguo3118.cn

[O03] 加锁保护共享数据
来源：https://sh.zhonguo2118.cn

Py:   with lock: shared += 1
来源：https://xo.zhonguo4118.cn

PHP:  // 用 flock() 做文件锁
来源：https://vu.zhonguo3118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://op.zhonguo6118.cn

TS:   // 同 JS
来源：https://zg.zhonguo1118.cn

Java: synchronized (this) { shared++; }
来源：https://tu.zhonguo4118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://wo.zhonguo3118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://oy.zhonguo6118.cn

C#:   lock (gate) { shared++; }
来源：https://na.zhonguo4118.cn

[O04] 定义异步函数并等待
来源：https://yq.zhonguo7118.cn

Py:   async def f():⏎    await g()
来源：https://ba.zhonguo3118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://oa.zhonguo8118.cn

JS:   async function f() { await g(); }
来源：https://md.zhonguo2118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://jl.zhonguo2118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://mb.zhonguo6118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://av.zhonguo7118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://mu.zhonguo4118.cn

C#:   async Task F() { await G(); }
来源：https://lr.zhonguo8118.cn

[O05] 并发执行并等待全部完成
来源：https://tn.zhonguo6118.cn

Py:   asyncio.gather(*tasks)
来源：https://uy.zhonguo8118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://mu.zhonguo4118.cn

JS:   await Promise.all(tasks)
来源：https://la.zhonguo7118.cn

TS:   await Promise.all(tasks)
来源：https://ox.zhonguo1118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://fb.zhonguo2118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://mf.zhonguo2118.cn

Ruby: threads.map(&:join)
来源：https://qo.zhonguo3118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://cb.zhonguo1118.cn

[O06] 使用进程池
来源：https://cd.zhonguo1118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://hp.zhonguo6118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://es.zhonguo4118.cn

JS:   // child_process / cluster 模块
来源：https://et.zhonguo2118.cn

TS:   // child_process / cluster 模块
来源：https://ks.zhonguo5118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://wp.zhonguo3118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://fw.zhonguo5118.cn

Ruby: // fork 块
来源：https://hr.zhonguo7118.cn

C#:   Parallel.For
来源：https://yt.zhonguo6118.cn

================================================================================
来源：https://sd.zhonguo8118.cn

P. 常用工具函数
来源：https://np.zhonguo2118.cn

================================================================================
来源：https://mf.zhonguo2118.cn

[P01] 生成 UUID
来源：https://ex.zhonguo1118.cn

Py:   str(uuid.uuid4())
来源：https://ji.zhonguo5118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://gl.zhonguo4118.cn

JS:   crypto.randomUUID()
来源：https://rq.zhonguo8118.cn

TS:   crypto.randomUUID()
来源：https://wp.zhonguo5118.cn

Java: UUID.randomUUID().toString()
来源：https://df.zhonguo1118.cn

Go:   // 用 github.com/google/uuid
来源：https://sz.zhonguo8118.cn

Ruby: SecureRandom.uuid
来源：https://zl.zhonguo3118.cn

C#:   Guid.NewGuid().ToString()
来源：https://uu.zhonguo6118.cn

[P02] MD5 / SHA256 摘要
来源：https://ei.zhonguo8118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://om.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://hm.zhonguo1118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://wl.zhonguo1118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://gb.zhonguo1118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://en.zhonguo8118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://tp.zhonguo3118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://sa.zhonguo5118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://yy.zhonguo7118.cn

[P03] 生成短随机字符串
来源：https://yz.zhonguo5118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://oz.zhonguo5118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://wl.zhonguo2118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://bu.zhonguo6118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://jg.zhonguo8118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://uz.zhonguo4118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://un.zhonguo4118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://rh.zhonguo6118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://su.zhonguo7118.cn

[P04] 求长度
来源：https://df.zhonguo1118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://wd.zhonguo4118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ti.zhonguo7118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://oa.zhonguo4118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://df.zhonguo3118.cn

Java: list.size();  map.size();  s.length()
来源：https://ml.zhonguo5118.cn

Go:   len(arr);  len(m)
来源：https://yb.zhonguo5118.cn

Ruby: x.length;  x.size
来源：https://fd.zhonguo8118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://cw.zhonguo8118.cn

[P05] 判断两个对象内容是否相等
来源：https://iy.zhonguo1118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://co.zhonguo8118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://nc.zhonguo2118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://tw.zhonguo7118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://yq.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://fp.zhonguo6118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://st.zhonguo7118.cn

Ruby: a == b
来源：https://lv.zhonguo1118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://uc.zhonguo1118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://sd.zhonguo4118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://ds.zhonguo3118.cn

PHP:  if (empty($x)) {}
来源：https://db.zhonguo7118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://hw.zhonguo3118.cn

TS:   if (x == null) {}
来源：https://cl.zhonguo2118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://rd.zhonguo5118.cn

Go:   if x == nil {}
来源：https://qu.zhonguo4118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://be.zhonguo6118.cn

C#:   if (x is null) {}
来源：https://ua.zhonguo8118.cn

[P07] 防抖与节流
来源：https://xt.zhonguo8118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://ut.zhonguo7118.cn

PHP:  // 手写时间戳比较
来源：https://fg.zhonguo1118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://al.zhonguo2118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://xa.zhonguo5118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://qp.zhonguo5118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://ja.zhonguo8118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://jh.zhonguo2118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://xi.zhonguo6118.cn

[P08] 处理浮点精度问题
来源：https://qf.zhonguo1118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://nl.zhonguo5118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://ae.zhonguo2118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://gy.zhonguo6118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://tz.zhonguo4118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://wc.zhonguo8118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://eu.zhonguo5118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://tf.zhonguo2118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://ub.zhonguo2118.cn

================================================================================
来源：https://tp.zhonguo8118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://zr.zhonguo2118.cn

================================================================================
来源：https://jd.zhonguo3118.cn

[Q01] 创建表
来源：https://fj.zhonguo7118.cn

CREATE TABLE users (
来源：https://xd.zhonguo1118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://dc.zhonguo6118.cn

name VARCHAR(50) NOT NULL,
来源：https://yx.zhonguo6118.cn

email VARCHAR(100) UNIQUE,
来源：https://xs.zhonguo4118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://zl.zhonguo2118.cn

);
来源：https://lk.zhonguo8118.cn

[Q02] 创建带外键的表
来源：https://jt.zhonguo7118.cn

CREATE TABLE orders (
来源：https://hz.zhonguo7118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://vz.zhonguo6118.cn

user_id INT NOT NULL,
来源：https://rm.zhonguo3118.cn

amount DECIMAL(10, 2),
来源：https://un.zhonguo2118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://tf.zhonguo3118.cn

);
来源：https://uu.zhonguo7118.cn

[Q03] 增加列
来源：https://iq.zhonguo3118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://eu.zhonguo1118.cn

[Q04] 修改列类型
来源：https://nu.zhonguo3118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://dn.zhonguo7118.cn

[Q05] 重命名列
来源：https://bm.zhonguo7118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://ic.zhonguo3118.cn

[Q06] 删除列
来源：https://wi.zhonguo3118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://vz.zhonguo1118.cn

[Q07] 删除表
来源：https://cz.zhonguo5118.cn

DROP TABLE IF EXISTS orders;
来源：https://rl.zhonguo6118.cn

[Q08] 创建普通索引
来源：https://dp.zhonguo6118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://ig.zhonguo1118.cn

[Q09] 创建唯一索引
来源：https://kq.zhonguo1118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://fe.zhonguo1118.cn

[Q10] 插入单行
来源：https://pk.zhonguo2118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://xd.zhonguo4118.cn

[Q11] 一次插入多行
来源：https://hz.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://tu.zhonguo5118.cn

[Q12] 插入后取自增 ID
来源：https://lz.zhonguo7118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://bj.zhonguo6118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://bn.zhonguo2118.cn

[Q13] 忽略重复插入
来源：https://vo.zhonguo3118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://sb.zhonguo2118.cn

[Q14] 存在则更新（upsert）
来源：https://pl.zhonguo7118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://io.zhonguo2118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://us.zhonguo7118.cn

[Q15] 查询全部
来源：https://ot.zhonguo8118.cn

SELECT * FROM users;
来源：https://pa.zhonguo6118.cn

[Q16] 查询指定列
来源：https://la.zhonguo3118.cn

SELECT id, name FROM users;
来源：https://on.zhonguo5118.cn

[Q17] 条件查询
来源：https://me.zhonguo3118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://xz.zhonguo4118.cn

[Q18] 模糊匹配
来源：https://vx.zhonguo1118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://ex.zhonguo6118.cn

[Q19] 范围查询
来源：https://ka.zhonguo7118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://jz.zhonguo2118.cn

[Q20] IN 列表
来源：https://ji.zhonguo8118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://sh.zhonguo4118.cn

[Q21] 空值判断
来源：https://za.zhonguo6118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://eh.zhonguo8118.cn

[Q22] 排序
来源：https://qz.zhonguo3118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://lu.zhonguo4118.cn

[Q23] 分页
来源：https://ql.zhonguo6118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://jc.zhonguo4118.cn

[Q24] 去重
来源：https://zs.zhonguo3118.cn

SELECT DISTINCT city FROM users;
来源：https://ih.zhonguo8118.cn

[Q25] 只取前 N 条
来源：https://qh.zhonguo8118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://hu.zhonguo2118.cn

[Q26] 计数
来源：https://xn.zhonguo4118.cn

SELECT COUNT(*) FROM users;
来源：https://vr.zhonguo3118.cn

[Q27] 条件计数
来源：https://os.zhonguo8118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://rq.zhonguo4118.cn

[Q28] 求和与平均
来源：https://gt.zhonguo7118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://ab.zhonguo1118.cn

[Q29] 最大最小值
来源：https://rn.zhonguo8118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://xs.zhonguo1118.cn

[Q30] 分组统计
来源：https://ex.zhonguo1118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://ld.zhonguo7118.cn

[Q31] 分组后过滤
来源：https://oo.zhonguo5118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://ld.zhonguo3118.cn

[Q32] 分组拼接字符串
来源：https://cb.zhonguo7118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://pv.zhonguo6118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://ub.zhonguo7118.cn

[Q33] 多列分组
来源：https://nm.zhonguo7118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://mp.zhonguo7118.cn

[Q34] 每组取第一条
来源：https://uc.zhonguo1118.cn

SELECT * FROM (
来源：https://wj.zhonguo3118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://lb.zhonguo7118.cn

) t WHERE rn = 1;
来源：https://ob.zhonguo1118.cn

[Q35] 内连接
来源：https://oe.zhonguo8118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://wp.zhonguo3118.cn

[Q36] 左连接
来源：https://th.zhonguo4118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://pj.zhonguo3118.cn

[Q37] 右连接
来源：https://id.zhonguo1118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://dd.zhonguo6118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://xj.zhonguo8118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://mt.zhonguo3118.cn

[Q39] 自连接（查上下级）
来源：https://hu.zhonguo6118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://is.zhonguo1118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://zi.zhonguo6118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://oj.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://hz.zhonguo1118.cn

[Q41] 多表连接
来源：https://ed.zhonguo3118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://xc.zhonguo3118.cn

JOIN users u ON u.id = o.user_id
来源：https://cn.zhonguo8118.cn

JOIN products p ON p.id = o.product_id;
来源：https://dn.zhonguo4118.cn

[Q42] 连接条件附加过滤
来源：https://do.zhonguo7118.cn

SELECT u.name, o.amount FROM users u
来源：https://sq.zhonguo2118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://zs.zhonguo3118.cn

[Q43] 标量子查询
来源：https://pb.zhonguo1118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://wm.zhonguo4118.cn

[Q44] IN 子查询
来源：https://yc.zhonguo2118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://xx.zhonguo4118.cn

[Q45] EXISTS 判断存在
来源：https://vk.zhonguo3118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://de.zhonguo5118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://ws.zhonguo1118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://mo.zhonguo3118.cn

[Q47] 与平均值比较
来源：https://ih.zhonguo5118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://no.zhonguo1118.cn

[Q48] CTE 公用表表达式
来源：https://na.zhonguo3118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://iy.zhonguo5118.cn

SELECT * FROM t WHERE c > 5;
来源：https://rf.zhonguo8118.cn

[Q49] 更新单行
来源：https://bb.zhonguo1118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://dz.zhonguo3118.cn

[Q50] 批量更新
来源：https://bv.zhonguo5118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://py.zhonguo4118.cn

[Q51] 用子查询更新
来源：https://sd.zhonguo5118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://ei.zhonguo6118.cn

[Q52] 删除指定行
来源：https://zo.zhonguo3118.cn

DELETE FROM users WHERE id = 10;
来源：https://uu.zhonguo8118.cn

[Q53] 按条件删除
来源：https://mx.zhonguo3118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://zc.zhonguo6118.cn

[Q54] 清空表
来源：https://ar.zhonguo4118.cn

TRUNCATE TABLE logs;
来源：https://hp.zhonguo2118.cn

[Q55] 排名（并列占位）
来源：https://uu.zhonguo8118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://bq.zhonguo3118.cn

[Q56] 密集排名（并列不占位）
来源：https://ah.zhonguo7118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://ih.zhonguo6118.cn

[Q57] 行号
来源：https://dn.zhonguo6118.cn


<!-- 参考信息 -->