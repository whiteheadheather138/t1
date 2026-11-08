代发 wailian999

Java: public static void main(String[] args)
来源：https://qd.zhonguo5118.cn

Go:   func main()
来源：https://ll.zhonguo7118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://ly.zhonguo3118.cn

C#:   static void Main(string[] args)
来源：https://pb.zhonguo5118.cn

[M08] 获取系统与运行时信息
来源：https://yr.zhonguo5118.cn

Py:   platform.system();  platform.python_version()
来源：https://iz.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://hg.zhonguo4118.cn

JS:   process.platform;  process.version
来源：https://vd.zhonguo4118.cn

TS:   process.platform;  process.version
来源：https://rr.zhonguo4118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://uq.zhonguo1118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://xy.zhonguo1118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://sq.zhonguo8118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://cz.zhonguo7118.cn

================================================================================
来源：https://qo.zhonguo7118.cn

N. 数据结构与算法
来源：https://xc.zhonguo6118.cn

================================================================================
来源：https://pr.zhonguo1118.cn

[N01] 二分查找（有序数组）
来源：https://rx.zhonguo6118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://mt.zhonguo1118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://mi.zhonguo7118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://lx.zhonguo3118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://rr.zhonguo8118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://ad.zhonguo2118.cn

Go:   sort.SearchInts(arr, x)
来源：https://ua.zhonguo3118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://uf.zhonguo1118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://lz.zhonguo7118.cn

[N02] 排序（工程实践用内置实现）
来源：https://fj.zhonguo2118.cn

Py:   sorted(arr);  arr.sort()
来源：https://tz.zhonguo5118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://ml.zhonguo8118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://um.zhonguo2118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://hn.zhonguo5118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://jm.zhonguo8118.cn

Go:   slices.Sort(arr)
来源：https://sb.zhonguo6118.cn

Ruby: arr.sort
来源：https://tc.zhonguo4118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://xs.zhonguo2118.cn

[N03] 快速排序（分治示例）
来源：https://eb.zhonguo1118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://um.zhonguo3118.cn

PHP:  // 递归实现，或用 usort
来源：https://cn.zhonguo1118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://sh.zhonguo7118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://rw.zhonguo8118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://wn.zhonguo5118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://tb.zhonguo4118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://lh.zhonguo6118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://wo.zhonguo6118.cn

[N04] 斐波那契数列
来源：https://jp.zhonguo2118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://cf.zhonguo1118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://ms.zhonguo4118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://mz.zhonguo5118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://wx.zhonguo5118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://fy.zhonguo6118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://og.zhonguo8118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://ue.zhonguo5118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://ya.zhonguo4118.cn

[N05] 最大公约数
来源：https://fy.zhonguo5118.cn

Py:   math.gcd(a, b)
来源：https://fp.zhonguo1118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://bn.zhonguo6118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://zy.zhonguo5118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://ue.zhonguo3118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://zx.zhonguo5118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://ba.zhonguo8118.cn

Ruby: a.gcd(b)
来源：https://yi.zhonguo3118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://an.zhonguo6118.cn

[N06] 判断回文字符串
来源：https://mj.zhonguo4118.cn

Py:   s == s[::-1]
来源：https://ym.zhonguo1118.cn

PHP:  $s === strrev($s);
来源：https://rq.zhonguo7118.cn

JS:   s === [...s].reverse().join("")
来源：https://jd.zhonguo1118.cn

TS:   s === [...s].reverse().join("")
来源：https://qu.zhonguo2118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://rt.zhonguo7118.cn

Go:   // 双指针从两端比较
来源：https://xu.zhonguo2118.cn

Ruby: s == s.reverse
来源：https://oe.zhonguo7118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://rr.zhonguo1118.cn

[N07] 两数之和（返回下标）
来源：https://cr.zhonguo1118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://cc.zhonguo7118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://xt.zhonguo4118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://kv.zhonguo3118.cn

TS:   // 手写 Map<string, number>
来源：https://up.zhonguo7118.cn

Java: // 手写 HashMap
来源：https://fs.zhonguo3118.cn

Go:   // 手写 map[int]int
来源：https://uv.zhonguo3118.cn

Ruby: // 手写 Hash
来源：https://se.zhonguo5118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://ky.zhonguo6118.cn

[N08] 生成全排列
来源：https://yf.zhonguo1118.cn

Py:   itertools.permutations(arr)
来源：https://cp.zhonguo8118.cn

PHP:  // 手写递归交换
来源：https://tf.zhonguo7118.cn

JS:   // 手写回溯递归
来源：https://un.zhonguo4118.cn

TS:   // 手写回溯递归
来源：https://ft.zhonguo4118.cn

Java: // 手写回溯递归
来源：https://zq.zhonguo3118.cn

Go:   // 手写回溯递归
来源：https://ei.zhonguo2118.cn

Ruby: arr.permutation.to_a
来源：https://wf.zhonguo8118.cn

C#:   // 手写回溯递归
来源：https://mm.zhonguo6118.cn

[N09] 栈与队列
来源：https://bc.zhonguo2118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://au.zhonguo5118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://vn.zhonguo5118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://ia.zhonguo3118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://vj.zhonguo7118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://jm.zhonguo2118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://rv.zhonguo4118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://ny.zhonguo1118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://ht.zhonguo8118.cn

[N10] 链表节点定义
来源：https://fm.zhonguo5118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://nn.zhonguo2118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://kf.zhonguo4118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://tj.zhonguo7118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://nv.zhonguo1118.cn

Java: class Node { int v; Node next; }
来源：https://ov.zhonguo1118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://sb.zhonguo3118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://bw.zhonguo5118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://ao.zhonguo1118.cn

[N11] 二叉树中序遍历
来源：https://dj.zhonguo5118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://oo.zhonguo6118.cn

PHP:  // 手写递归函数
来源：https://sv.zhonguo2118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ok.zhonguo8118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://uy.zhonguo5118.cn

Java: // 手写递归
来源：https://of.zhonguo7118.cn

Go:   // 手写递归
来源：https://lj.zhonguo8118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://ve.zhonguo5118.cn

C#:   // 手写递归
来源：https://hr.zhonguo8118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://do.zhonguo2118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://eq.zhonguo8118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://bl.zhonguo5118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://bc.zhonguo2118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://qc.zhonguo6118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://od.zhonguo6118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://xj.zhonguo5118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://yk.zhonguo6118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://oy.zhonguo2118.cn

================================================================================
来源：https://pd.zhonguo1118.cn

O. 并发与异步
来源：https://ob.zhonguo5118.cn

================================================================================
来源：https://ce.zhonguo3118.cn

[O01] 启动一个线程
来源：https://ry.zhonguo7118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://jo.zhonguo1118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://oh.zhonguo5118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://yz.zhonguo2118.cn

TS:   // 同 JS
来源：https://iz.zhonguo4118.cn

Java: new Thread(() -> f()).start()
来源：https://lu.zhonguo6118.cn

Go:   go f()
来源：https://sh.zhonguo7118.cn

Ruby: Thread.new { f }
来源：https://ze.zhonguo5118.cn

C#:   Task.Run(() => F());
来源：https://gf.zhonguo1118.cn

[O02] 使用线程池
来源：https://zg.zhonguo6118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://kr.zhonguo2118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://rm.zhonguo2118.cn

JS:   // worker_threads 线程池
来源：https://do.zhonguo8118.cn

TS:   // worker_threads 线程池
来源：https://jn.zhonguo7118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://uq.zhonguo1118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://md.zhonguo6118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://ug.zhonguo6118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://zx.zhonguo7118.cn

[O03] 加锁保护共享数据
来源：https://dv.zhonguo7118.cn

Py:   with lock: shared += 1
来源：https://oz.zhonguo5118.cn

PHP:  // 用 flock() 做文件锁
来源：https://ro.zhonguo3118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://ea.zhonguo7118.cn

TS:   // 同 JS
来源：https://dl.zhonguo3118.cn

Java: synchronized (this) { shared++; }
来源：https://ay.zhonguo6118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://tp.zhonguo4118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://ns.zhonguo2118.cn

C#:   lock (gate) { shared++; }
来源：https://yj.zhonguo1118.cn

[O04] 定义异步函数并等待
来源：https://sv.zhonguo6118.cn

Py:   async def f():⏎    await g()
来源：https://fr.zhonguo1118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://be.zhonguo1118.cn

JS:   async function f() { await g(); }
来源：https://vu.zhonguo7118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://lg.zhonguo5118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://hl.zhonguo3118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://jn.zhonguo4118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://iy.zhonguo5118.cn

C#:   async Task F() { await G(); }
来源：https://nb.zhonguo1118.cn

[O05] 并发执行并等待全部完成
来源：https://ev.zhonguo6118.cn

Py:   asyncio.gather(*tasks)
来源：https://bp.zhonguo4118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://ra.zhonguo1118.cn

JS:   await Promise.all(tasks)
来源：https://yj.zhonguo1118.cn

TS:   await Promise.all(tasks)
来源：https://si.zhonguo6118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://ro.zhonguo2118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://lc.zhonguo6118.cn

Ruby: threads.map(&:join)
来源：https://lf.zhonguo1118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://np.zhonguo4118.cn

[O06] 使用进程池
来源：https://nk.zhonguo4118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://lz.zhonguo5118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://gn.zhonguo8118.cn

JS:   // child_process / cluster 模块
来源：https://pv.zhonguo1118.cn

TS:   // child_process / cluster 模块
来源：https://xh.zhonguo4118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://ma.zhonguo7118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://pj.zhonguo2118.cn

Ruby: // fork 块
来源：https://mg.zhonguo1118.cn

C#:   Parallel.For
来源：https://sh.zhonguo6118.cn

================================================================================
来源：https://on.zhonguo1118.cn

P. 常用工具函数
来源：https://um.zhonguo5118.cn

================================================================================
来源：https://zv.zhonguo6118.cn

[P01] 生成 UUID
来源：https://lk.zhonguo8118.cn

Py:   str(uuid.uuid4())
来源：https://ig.zhonguo3118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://ej.zhonguo5118.cn

JS:   crypto.randomUUID()
来源：https://kj.zhonguo2118.cn

TS:   crypto.randomUUID()
来源：https://lz.zhonguo1118.cn

Java: UUID.randomUUID().toString()
来源：https://iu.zhonguo5118.cn

Go:   // 用 github.com/google/uuid
来源：https://qc.zhonguo5118.cn

Ruby: SecureRandom.uuid
来源：https://lz.zhonguo3118.cn

C#:   Guid.NewGuid().ToString()
来源：https://bi.zhonguo7118.cn

[P02] MD5 / SHA256 摘要
来源：https://cl.zhonguo5118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://xh.zhonguo4118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://yp.zhonguo2118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://ij.zhonguo2118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://cd.zhonguo5118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://fs.zhonguo6118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://cs.zhonguo8118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://rn.zhonguo4118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://cj.zhonguo7118.cn

[P03] 生成短随机字符串
来源：https://if.zhonguo1118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://kj.zhonguo6118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://eg.zhonguo3118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://ge.zhonguo4118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://en.zhonguo3118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://wd.zhonguo5118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://wu.zhonguo7118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://ke.zhonguo8118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://fs.zhonguo3118.cn

[P04] 求长度
来源：https://ij.zhonguo4118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://mg.zhonguo4118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://oi.zhonguo1118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://wu.zhonguo5118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://nr.zhonguo2118.cn

Java: list.size();  map.size();  s.length()
来源：https://we.zhonguo1118.cn

Go:   len(arr);  len(m)
来源：https://ut.zhonguo8118.cn

Ruby: x.length;  x.size
来源：https://ik.zhonguo2118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://dx.zhonguo6118.cn

[P05] 判断两个对象内容是否相等
来源：https://dy.zhonguo1118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://jg.zhonguo2118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://mp.zhonguo7118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://iq.zhonguo6118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://ot.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://hc.zhonguo2118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://ke.zhonguo1118.cn

Ruby: a == b
来源：https://tq.zhonguo6118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://cr.zhonguo1118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://mt.zhonguo3118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://cj.zhonguo6118.cn

PHP:  if (empty($x)) {}
来源：https://mp.zhonguo6118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://ct.zhonguo2118.cn

TS:   if (x == null) {}
来源：https://hg.zhonguo2118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://fa.zhonguo2118.cn

Go:   if x == nil {}
来源：https://uu.zhonguo8118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://zv.zhonguo7118.cn

C#:   if (x is null) {}
来源：https://gg.zhonguo7118.cn

[P07] 防抖与节流
来源：https://uv.zhonguo6118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://yr.zhonguo8118.cn

PHP:  // 手写时间戳比较
来源：https://lr.zhonguo4118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://dd.zhonguo3118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://ya.zhonguo8118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://yj.zhonguo4118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://of.zhonguo2118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://mk.zhonguo1118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://xd.zhonguo8118.cn

[P08] 处理浮点精度问题
来源：https://bo.zhonguo4118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://ja.zhonguo2118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://cq.zhonguo2118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://sy.zhonguo8118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://rb.zhonguo3118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://sp.zhonguo4118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://lp.zhonguo1118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://km.zhonguo7118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://ww.zhonguo3118.cn

================================================================================
来源：https://st.zhonguo3118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://ls.zhonguo8118.cn

================================================================================
来源：https://gv.zhonguo2118.cn

[Q01] 创建表
来源：https://oj.zhonguo6118.cn

CREATE TABLE users (
来源：https://vx.zhonguo8118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://pd.zhonguo3118.cn

name VARCHAR(50) NOT NULL,
来源：https://ly.zhonguo2118.cn

email VARCHAR(100) UNIQUE,
来源：https://fo.zhonguo5118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://cr.zhonguo8118.cn

);
来源：https://gx.zhonguo5118.cn

[Q02] 创建带外键的表
来源：https://ha.zhonguo7118.cn

CREATE TABLE orders (
来源：https://kb.zhonguo1118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://ql.zhonguo5118.cn

user_id INT NOT NULL,
来源：https://gk.zhonguo8118.cn

amount DECIMAL(10, 2),
来源：https://cd.zhonguo5118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://hm.zhonguo2118.cn

);
来源：https://uk.zhonguo7118.cn

[Q03] 增加列
来源：https://qq.zhonguo1118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://hu.zhonguo5118.cn

[Q04] 修改列类型
来源：https://tg.zhonguo5118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://nc.zhonguo6118.cn

[Q05] 重命名列
来源：https://ex.zhonguo7118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://jw.zhonguo2118.cn

[Q06] 删除列
来源：https://zs.zhonguo4118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://xp.zhonguo6118.cn

[Q07] 删除表
来源：https://kl.zhonguo5118.cn

DROP TABLE IF EXISTS orders;
来源：https://ew.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://tw.zhonguo7118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://cf.zhonguo5118.cn

[Q09] 创建唯一索引
来源：https://yj.zhonguo5118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://qd.zhonguo4118.cn

[Q10] 插入单行
来源：https://kf.zhonguo7118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://ai.zhonguo7118.cn

[Q11] 一次插入多行
来源：https://yj.zhonguo3118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://lf.zhonguo7118.cn

[Q12] 插入后取自增 ID
来源：https://wf.zhonguo8118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://bj.zhonguo4118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://mg.zhonguo8118.cn

[Q13] 忽略重复插入
来源：https://xf.zhonguo8118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://yj.zhonguo8118.cn

[Q14] 存在则更新（upsert）
来源：https://zk.zhonguo4118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://av.zhonguo2118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://do.zhonguo3118.cn

[Q15] 查询全部
来源：https://gt.zhonguo4118.cn


<!-- 参考信息 -->