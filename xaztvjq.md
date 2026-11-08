代发 wailian999

Ruby: arr.sort
来源：https://kh.zhonguo2118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://ng.zhonguo2118.cn

[N03] 快速排序（分治示例）
来源：https://bt.zhonguo2118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://au.zhonguo7118.cn

PHP:  // 递归实现，或用 usort
来源：https://rg.zhonguo5118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://qb.zhonguo4118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://wu.zhonguo4118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://qt.zhonguo1118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://jg.zhonguo5118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://sq.zhonguo6118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://ic.zhonguo6118.cn

[N04] 斐波那契数列
来源：https://bk.zhonguo3118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://bv.zhonguo6118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://qu.zhonguo5118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://gk.zhonguo1118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://at.zhonguo6118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://so.zhonguo6118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://tj.zhonguo4118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://il.zhonguo4118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://hz.zhonguo3118.cn

[N05] 最大公约数
来源：https://gb.zhonguo4118.cn

Py:   math.gcd(a, b)
来源：https://tu.zhonguo2118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://vj.zhonguo2118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://oo.zhonguo4118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://gj.zhonguo4118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://ht.zhonguo1118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://pb.zhonguo8118.cn

Ruby: a.gcd(b)
来源：https://mk.zhonguo5118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://wk.zhonguo7118.cn

[N06] 判断回文字符串
来源：https://si.zhonguo2118.cn

Py:   s == s[::-1]
来源：https://pf.zhonguo4118.cn

PHP:  $s === strrev($s);
来源：https://ar.zhonguo4118.cn

JS:   s === [...s].reverse().join("")
来源：https://ep.zhonguo7118.cn

TS:   s === [...s].reverse().join("")
来源：https://hi.zhonguo6118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://gn.zhonguo5118.cn

Go:   // 双指针从两端比较
来源：https://ik.zhonguo1118.cn

Ruby: s == s.reverse
来源：https://fb.zhonguo8118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://za.zhonguo4118.cn

[N07] 两数之和（返回下标）
来源：https://eq.zhonguo6118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://zt.zhonguo2118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://pe.zhonguo4118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://en.zhonguo5118.cn

TS:   // 手写 Map<string, number>
来源：https://ms.zhonguo4118.cn

Java: // 手写 HashMap
来源：https://di.zhonguo7118.cn

Go:   // 手写 map[int]int
来源：https://cs.zhonguo6118.cn

Ruby: // 手写 Hash
来源：https://eh.zhonguo7118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://zi.zhonguo7118.cn

[N08] 生成全排列
来源：https://qm.zhonguo1118.cn

Py:   itertools.permutations(arr)
来源：https://ps.zhonguo7118.cn

PHP:  // 手写递归交换
来源：https://ai.zhonguo2118.cn

JS:   // 手写回溯递归
来源：https://zb.zhonguo4118.cn

TS:   // 手写回溯递归
来源：https://hm.zhonguo3118.cn

Java: // 手写回溯递归
来源：https://id.zhonguo8118.cn

Go:   // 手写回溯递归
来源：https://gk.zhonguo4118.cn

Ruby: arr.permutation.to_a
来源：https://xi.zhonguo7118.cn

C#:   // 手写回溯递归
来源：https://ol.zhonguo5118.cn

[N09] 栈与队列
来源：https://du.zhonguo7118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://fd.zhonguo2118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://bw.zhonguo6118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://at.zhonguo8118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://qu.zhonguo5118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://rs.zhonguo4118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://zo.zhonguo2118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://fj.zhonguo6118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://db.zhonguo7118.cn

[N10] 链表节点定义
来源：https://gx.zhonguo2118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://st.zhonguo7118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://pr.zhonguo5118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://xq.zhonguo4118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://oj.zhonguo1118.cn

Java: class Node { int v; Node next; }
来源：https://ut.zhonguo3118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://eh.zhonguo5118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://ja.zhonguo6118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://zr.zhonguo2118.cn

[N11] 二叉树中序遍历
来源：https://xv.zhonguo1118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://bb.zhonguo6118.cn

PHP:  // 手写递归函数
来源：https://om.zhonguo2118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://fn.zhonguo5118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://wl.zhonguo6118.cn

Java: // 手写递归
来源：https://iw.zhonguo2118.cn

Go:   // 手写递归
来源：https://bw.zhonguo3118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://wb.zhonguo2118.cn

C#:   // 手写递归
来源：https://qt.zhonguo5118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://ch.zhonguo2118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://ef.zhonguo8118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://je.zhonguo7118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://qe.zhonguo6118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://br.zhonguo2118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://aq.zhonguo1118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://ij.zhonguo1118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://rg.zhonguo5118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://xg.zhonguo4118.cn

================================================================================
来源：https://oy.zhonguo1118.cn

O. 并发与异步
来源：https://pq.zhonguo8118.cn

================================================================================
来源：https://wg.zhonguo2118.cn

[O01] 启动一个线程
来源：https://bx.zhonguo2118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://ja.zhonguo6118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://rx.zhonguo3118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://hj.zhonguo5118.cn

TS:   // 同 JS
来源：https://rw.zhonguo5118.cn

Java: new Thread(() -> f()).start()
来源：https://vr.zhonguo8118.cn

Go:   go f()
来源：https://hk.zhonguo1118.cn

Ruby: Thread.new { f }
来源：https://wa.zhonguo1118.cn

C#:   Task.Run(() => F());
来源：https://aq.zhonguo3118.cn

[O02] 使用线程池
来源：https://qj.zhonguo4118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://ed.zhonguo3118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://ts.zhonguo3118.cn

JS:   // worker_threads 线程池
来源：https://xl.zhonguo2118.cn

TS:   // worker_threads 线程池
来源：https://wx.zhonguo7118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://sy.zhonguo4118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://np.zhonguo8118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://np.zhonguo3118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://su.zhonguo1118.cn

[O03] 加锁保护共享数据
来源：https://fs.zhonguo7118.cn

Py:   with lock: shared += 1
来源：https://up.zhonguo6118.cn

PHP:  // 用 flock() 做文件锁
来源：https://pv.zhonguo1118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://gu.zhonguo8118.cn

TS:   // 同 JS
来源：https://hp.zhonguo2118.cn

Java: synchronized (this) { shared++; }
来源：https://tx.zhonguo5118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://fa.zhonguo4118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://vv.zhonguo8118.cn

C#:   lock (gate) { shared++; }
来源：https://ua.zhonguo1118.cn

[O04] 定义异步函数并等待
来源：https://hm.zhonguo7118.cn

Py:   async def f():⏎    await g()
来源：https://xn.zhonguo8118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://cc.zhonguo6118.cn

JS:   async function f() { await g(); }
来源：https://yg.zhonguo3118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://lh.zhonguo4118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://ps.zhonguo3118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://an.zhonguo7118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://al.zhonguo2118.cn

C#:   async Task F() { await G(); }
来源：https://lk.zhonguo5118.cn

[O05] 并发执行并等待全部完成
来源：https://ny.zhonguo8118.cn

Py:   asyncio.gather(*tasks)
来源：https://ss.zhonguo6118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://oi.zhonguo1118.cn

JS:   await Promise.all(tasks)
来源：https://qe.zhonguo3118.cn

TS:   await Promise.all(tasks)
来源：https://ew.zhonguo5118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://nu.zhonguo6118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://kw.zhonguo4118.cn

Ruby: threads.map(&:join)
来源：https://cw.zhonguo6118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://ff.zhonguo3118.cn

[O06] 使用进程池
来源：https://sj.zhonguo6118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://et.zhonguo8118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://uq.zhonguo2118.cn

JS:   // child_process / cluster 模块
来源：https://no.zhonguo4118.cn

TS:   // child_process / cluster 模块
来源：https://ki.zhonguo2118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://tq.zhonguo1118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://mx.zhonguo3118.cn

Ruby: // fork 块
来源：https://vw.zhonguo8118.cn

C#:   Parallel.For
来源：https://hn.zhonguo7118.cn

================================================================================
来源：https://ou.zhonguo1118.cn

P. 常用工具函数
来源：https://lp.zhonguo5118.cn

================================================================================
来源：https://us.zhonguo6118.cn

[P01] 生成 UUID
来源：https://ok.zhonguo6118.cn

Py:   str(uuid.uuid4())
来源：https://uf.zhonguo1118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://si.zhonguo2118.cn

JS:   crypto.randomUUID()
来源：https://dj.zhonguo5118.cn

TS:   crypto.randomUUID()
来源：https://zp.zhonguo3118.cn

Java: UUID.randomUUID().toString()
来源：https://og.zhonguo4118.cn

Go:   // 用 github.com/google/uuid
来源：https://kc.zhonguo4118.cn

Ruby: SecureRandom.uuid
来源：https://xs.zhonguo4118.cn

C#:   Guid.NewGuid().ToString()
来源：https://se.zhonguo2118.cn

[P02] MD5 / SHA256 摘要
来源：https://rj.zhonguo6118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://vx.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://fc.zhonguo2118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://ld.zhonguo8118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://dx.zhonguo8118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://um.zhonguo2118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://af.zhonguo4118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://ex.zhonguo1118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://th.zhonguo4118.cn

[P03] 生成短随机字符串
来源：https://uv.zhonguo6118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://rt.zhonguo3118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://ue.zhonguo4118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://vs.zhonguo3118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://bd.zhonguo4118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://dp.zhonguo1118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://fq.zhonguo3118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://sg.zhonguo5118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://so.zhonguo7118.cn

[P04] 求长度
来源：https://yz.zhonguo4118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://mf.zhonguo4118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://fq.zhonguo6118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://is.zhonguo7118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://oj.zhonguo5118.cn

Java: list.size();  map.size();  s.length()
来源：https://ok.zhonguo5118.cn

Go:   len(arr);  len(m)
来源：https://wg.zhonguo7118.cn

Ruby: x.length;  x.size
来源：https://bo.zhonguo4118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://da.zhonguo8118.cn

[P05] 判断两个对象内容是否相等
来源：https://dv.zhonguo2118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://og.zhonguo7118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://ss.zhonguo7118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://nd.zhonguo5118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://mk.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://sh.zhonguo7118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://xv.zhonguo7118.cn

Ruby: a == b
来源：https://ka.zhonguo5118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://ew.zhonguo2118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://bw.zhonguo1118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://ce.zhonguo3118.cn

PHP:  if (empty($x)) {}
来源：https://xf.zhonguo6118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://jc.zhonguo7118.cn

TS:   if (x == null) {}
来源：https://yo.zhonguo2118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://lm.zhonguo5118.cn

Go:   if x == nil {}
来源：https://qq.zhonguo3118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://nr.zhonguo6118.cn

C#:   if (x is null) {}
来源：https://sa.zhonguo4118.cn

[P07] 防抖与节流
来源：https://wb.zhonguo7118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://ja.zhonguo5118.cn

PHP:  // 手写时间戳比较
来源：https://gv.zhonguo1118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://rv.zhonguo2118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://bq.zhonguo5118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://vb.zhonguo6118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://rv.zhonguo5118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://dk.zhonguo1118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://uj.zhonguo5118.cn

[P08] 处理浮点精度问题
来源：https://lo.zhonguo4118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://ce.zhonguo5118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://so.zhonguo1118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://zv.zhonguo5118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://az.zhonguo7118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://bm.zhonguo5118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://uu.zhonguo2118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://wl.zhonguo6118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://qw.zhonguo2118.cn

================================================================================
来源：https://lh.zhonguo5118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://xb.zhonguo1118.cn

================================================================================
来源：https://zw.zhonguo1118.cn

[Q01] 创建表
来源：https://hg.zhonguo1118.cn

CREATE TABLE users (
来源：https://yz.zhonguo7118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://re.zhonguo2118.cn

name VARCHAR(50) NOT NULL,
来源：https://cy.zhonguo2118.cn

email VARCHAR(100) UNIQUE,
来源：https://tv.zhonguo6118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://xi.zhonguo6118.cn

);
来源：https://qv.zhonguo8118.cn

[Q02] 创建带外键的表
来源：https://mf.zhonguo4118.cn

CREATE TABLE orders (
来源：https://sq.zhonguo1118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://tg.zhonguo1118.cn

user_id INT NOT NULL,
来源：https://db.zhonguo4118.cn

amount DECIMAL(10, 2),
来源：https://ge.zhonguo1118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://hb.zhonguo6118.cn

);
来源：https://ku.zhonguo5118.cn

[Q03] 增加列
来源：https://na.zhonguo1118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://tc.zhonguo8118.cn

[Q04] 修改列类型
来源：https://mh.zhonguo4118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://dx.zhonguo2118.cn

[Q05] 重命名列
来源：https://yb.zhonguo6118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://jn.zhonguo1118.cn

[Q06] 删除列
来源：https://sf.zhonguo2118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://bl.zhonguo2118.cn

[Q07] 删除表
来源：https://lu.zhonguo3118.cn

DROP TABLE IF EXISTS orders;
来源：https://fi.zhonguo3118.cn

[Q08] 创建普通索引
来源：https://bt.zhonguo6118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://gk.zhonguo2118.cn

[Q09] 创建唯一索引
来源：https://ge.zhonguo5118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://un.zhonguo5118.cn

[Q10] 插入单行
来源：https://za.zhonguo8118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://ly.zhonguo4118.cn

[Q11] 一次插入多行
来源：https://ev.zhonguo2118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://iu.zhonguo7118.cn

[Q12] 插入后取自增 ID
来源：https://wk.zhonguo3118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://la.zhonguo3118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://tc.zhonguo6118.cn

[Q13] 忽略重复插入
来源：https://gy.zhonguo5118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://xw.zhonguo7118.cn

[Q14] 存在则更新（upsert）
来源：https://ck.zhonguo2118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://ne.zhonguo4118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://jm.zhonguo6118.cn

[Q15] 查询全部
来源：https://ev.zhonguo7118.cn

SELECT * FROM users;
来源：https://lm.zhonguo7118.cn

[Q16] 查询指定列
来源：https://cj.zhonguo5118.cn

SELECT id, name FROM users;
来源：https://wl.zhonguo6118.cn

[Q17] 条件查询
来源：https://cl.zhonguo4118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://ys.zhonguo7118.cn

[Q18] 模糊匹配
来源：https://ju.zhonguo5118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://fj.zhonguo7118.cn

[Q19] 范围查询
来源：https://id.zhonguo4118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://aw.zhonguo4118.cn

[Q20] IN 列表
来源：https://vk.zhonguo5118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://ti.zhonguo7118.cn

[Q21] 空值判断
来源：https://uw.zhonguo6118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://va.zhonguo3118.cn

[Q22] 排序
来源：https://gc.zhonguo3118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://zz.zhonguo4118.cn

[Q23] 分页
来源：https://lo.zhonguo3118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://mn.zhonguo1118.cn

[Q24] 去重
来源：https://oo.zhonguo1118.cn

SELECT DISTINCT city FROM users;
来源：https://qm.zhonguo6118.cn

[Q25] 只取前 N 条
来源：https://xv.zhonguo7118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://ee.zhonguo6118.cn

[Q26] 计数
来源：https://kw.zhonguo5118.cn

SELECT COUNT(*) FROM users;
来源：https://zy.zhonguo8118.cn

[Q27] 条件计数
来源：https://ab.zhonguo3118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://py.zhonguo4118.cn

[Q28] 求和与平均
来源：https://td.zhonguo6118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://bz.zhonguo7118.cn

[Q29] 最大最小值
来源：https://pq.zhonguo3118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://bs.zhonguo4118.cn

[Q30] 分组统计
来源：https://gy.zhonguo3118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://wz.zhonguo6118.cn

[Q31] 分组后过滤
来源：https://jg.zhonguo3118.cn


<!-- 参考信息 -->