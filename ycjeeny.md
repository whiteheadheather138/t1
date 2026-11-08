代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：https://so.zhonguo7118.cn

JS:   console.error("err")
来源：https://ar.zhonguo7118.cn

TS:   console.error("err")
来源：https://fz.zhonguo2118.cn

Java: System.err.println("err")
来源：https://vu.zhonguo2118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://lr.zhonguo7118.cn

Ruby: warn "err"
来源：https://wz.zhonguo4118.cn

C#:   Console.Error.WriteLine("err")
来源：https://yc.zhonguo7118.cn

[M07] 判断是否为主入口
来源：https://xj.zhonguo3118.cn

Py:   if __name__ == "__main__":
来源：https://wg.zhonguo5118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://wz.zhonguo6118.cn

JS:   require.main === module
来源：https://hr.zhonguo2118.cn

TS:   require.main === module
来源：https://tf.zhonguo7118.cn

Java: public static void main(String[] args)
来源：https://ck.zhonguo1118.cn

Go:   func main()
来源：https://if.zhonguo7118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://kv.zhonguo2118.cn

C#:   static void Main(string[] args)
来源：https://yo.zhonguo6118.cn

[M08] 获取系统与运行时信息
来源：https://gb.zhonguo2118.cn

Py:   platform.system();  platform.python_version()
来源：https://ub.zhonguo2118.cn

PHP:  PHP_OS;  phpversion();
来源：https://xj.zhonguo7118.cn

JS:   process.platform;  process.version
来源：https://xj.zhonguo2118.cn

TS:   process.platform;  process.version
来源：https://gi.zhonguo5118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://rc.zhonguo7118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://yl.zhonguo6118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://tr.zhonguo1118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://uo.zhonguo1118.cn

================================================================================
来源：https://pc.zhonguo6118.cn

N. 数据结构与算法
来源：https://gu.zhonguo1118.cn

================================================================================
来源：https://sy.zhonguo4118.cn

[N01] 二分查找（有序数组）
来源：https://lu.zhonguo1118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://fv.zhonguo7118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://cz.zhonguo5118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://ca.zhonguo7118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://ar.zhonguo4118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://vk.zhonguo5118.cn

Go:   sort.SearchInts(arr, x)
来源：https://wg.zhonguo3118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://ui.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://ak.zhonguo3118.cn

[N02] 排序（工程实践用内置实现）
来源：https://cb.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://sb.zhonguo5118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://sa.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://zz.zhonguo2118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://tj.zhonguo4118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://wj.zhonguo4118.cn

Go:   slices.Sort(arr)
来源：https://gg.zhonguo2118.cn

Ruby: arr.sort
来源：https://ta.zhonguo8118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://xq.zhonguo2118.cn

[N03] 快速排序（分治示例）
来源：https://lm.zhonguo4118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://mm.zhonguo8118.cn

PHP:  // 递归实现，或用 usort
来源：https://lw.zhonguo7118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://zf.zhonguo4118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://fi.zhonguo8118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://ss.zhonguo7118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://fi.zhonguo1118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://hu.zhonguo2118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://rw.zhonguo5118.cn

[N04] 斐波那契数列
来源：https://vq.zhonguo2118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://co.zhonguo3118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://at.zhonguo7118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://fz.zhonguo2118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://lf.zhonguo3118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://ob.zhonguo4118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://sv.zhonguo7118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://kw.zhonguo1118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://ss.zhonguo4118.cn

[N05] 最大公约数
来源：https://rz.zhonguo6118.cn

Py:   math.gcd(a, b)
来源：https://ga.zhonguo6118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://rz.zhonguo2118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://yd.zhonguo2118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://rg.zhonguo4118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://sp.zhonguo1118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://wi.zhonguo6118.cn

Ruby: a.gcd(b)
来源：https://nu.zhonguo7118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://qx.zhonguo5118.cn

[N06] 判断回文字符串
来源：https://uj.zhonguo4118.cn

Py:   s == s[::-1]
来源：https://bu.zhonguo2118.cn

PHP:  $s === strrev($s);
来源：https://yg.zhonguo1118.cn

JS:   s === [...s].reverse().join("")
来源：https://or.zhonguo3118.cn

TS:   s === [...s].reverse().join("")
来源：https://bv.zhonguo4118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://qo.zhonguo1118.cn

Go:   // 双指针从两端比较
来源：https://rx.zhonguo7118.cn

Ruby: s == s.reverse
来源：https://bg.zhonguo1118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://sv.zhonguo6118.cn

[N07] 两数之和（返回下标）
来源：https://hc.zhonguo3118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://uj.zhonguo4118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://ib.zhonguo2118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://ye.zhonguo2118.cn

TS:   // 手写 Map<string, number>
来源：https://vg.zhonguo5118.cn

Java: // 手写 HashMap
来源：https://re.zhonguo4118.cn

Go:   // 手写 map[int]int
来源：https://la.zhonguo6118.cn

Ruby: // 手写 Hash
来源：https://sh.zhonguo5118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://jc.zhonguo5118.cn

[N08] 生成全排列
来源：https://fv.zhonguo7118.cn

Py:   itertools.permutations(arr)
来源：https://gc.zhonguo4118.cn

PHP:  // 手写递归交换
来源：https://ml.zhonguo8118.cn

JS:   // 手写回溯递归
来源：https://ut.zhonguo2118.cn

TS:   // 手写回溯递归
来源：https://ms.zhonguo5118.cn

Java: // 手写回溯递归
来源：https://dy.zhonguo1118.cn

Go:   // 手写回溯递归
来源：https://sl.zhonguo3118.cn

Ruby: arr.permutation.to_a
来源：https://wk.zhonguo8118.cn

C#:   // 手写回溯递归
来源：https://up.zhonguo3118.cn

[N09] 栈与队列
来源：https://vu.zhonguo7118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://ej.zhonguo2118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://qh.zhonguo5118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://xo.zhonguo4118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://nc.zhonguo4118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://hh.zhonguo5118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://ud.zhonguo8118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://uo.zhonguo5118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://oy.zhonguo1118.cn

[N10] 链表节点定义
来源：https://sn.zhonguo5118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://xd.zhonguo2118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://lt.zhonguo5118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://ks.zhonguo5118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://fi.zhonguo3118.cn

Java: class Node { int v; Node next; }
来源：https://yn.zhonguo4118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://um.zhonguo2118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://nm.zhonguo8118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://sj.zhonguo8118.cn

[N11] 二叉树中序遍历
来源：https://pa.zhonguo7118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://mx.zhonguo6118.cn

PHP:  // 手写递归函数
来源：https://fq.zhonguo7118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://kg.zhonguo6118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://tv.zhonguo5118.cn

Java: // 手写递归
来源：https://vy.zhonguo8118.cn

Go:   // 手写递归
来源：https://sr.zhonguo2118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://dw.zhonguo6118.cn

C#:   // 手写递归
来源：https://zh.zhonguo3118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://kx.zhonguo3118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://ty.zhonguo5118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://zv.zhonguo6118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://of.zhonguo1118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://xt.zhonguo7118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://we.zhonguo5118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://bn.zhonguo2118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://ig.zhonguo6118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://ur.zhonguo4118.cn

================================================================================
来源：https://lz.zhonguo2118.cn

O. 并发与异步
来源：https://wv.zhonguo4118.cn

================================================================================
来源：https://ml.zhonguo6118.cn

[O01] 启动一个线程
来源：https://jv.zhonguo1118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://lj.zhonguo8118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://sg.zhonguo5118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://ne.zhonguo4118.cn

TS:   // 同 JS
来源：https://vh.zhonguo1118.cn

Java: new Thread(() -> f()).start()
来源：https://pq.zhonguo2118.cn

Go:   go f()
来源：https://gu.zhonguo4118.cn

Ruby: Thread.new { f }
来源：https://ir.zhonguo1118.cn

C#:   Task.Run(() => F());
来源：https://yo.zhonguo4118.cn

[O02] 使用线程池
来源：https://fu.zhonguo2118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://tu.zhonguo3118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://bg.zhonguo2118.cn

JS:   // worker_threads 线程池
来源：https://qm.zhonguo6118.cn

TS:   // worker_threads 线程池
来源：https://ao.zhonguo3118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://el.zhonguo6118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://df.zhonguo1118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://fy.zhonguo4118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://oz.zhonguo4118.cn

[O03] 加锁保护共享数据
来源：https://lg.zhonguo2118.cn

Py:   with lock: shared += 1
来源：https://nf.zhonguo3118.cn

PHP:  // 用 flock() 做文件锁
来源：https://yn.zhonguo2118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://ct.zhonguo4118.cn

TS:   // 同 JS
来源：https://fi.zhonguo8118.cn

Java: synchronized (this) { shared++; }
来源：https://vn.zhonguo3118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://il.zhonguo4118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://jw.zhonguo7118.cn

C#:   lock (gate) { shared++; }
来源：https://pq.zhonguo7118.cn

[O04] 定义异步函数并等待
来源：https://hx.zhonguo1118.cn

Py:   async def f():⏎    await g()
来源：https://iy.zhonguo7118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://qd.zhonguo4118.cn

JS:   async function f() { await g(); }
来源：https://yj.zhonguo4118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://gm.zhonguo3118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://dl.zhonguo2118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://mb.zhonguo6118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://dg.zhonguo5118.cn

C#:   async Task F() { await G(); }
来源：https://tl.zhonguo7118.cn

[O05] 并发执行并等待全部完成
来源：https://jf.zhonguo8118.cn

Py:   asyncio.gather(*tasks)
来源：https://jc.zhonguo1118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://pi.zhonguo4118.cn

JS:   await Promise.all(tasks)
来源：https://iu.zhonguo6118.cn

TS:   await Promise.all(tasks)
来源：https://vl.zhonguo5118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://kv.zhonguo7118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://sy.zhonguo8118.cn

Ruby: threads.map(&:join)
来源：https://bp.zhonguo5118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://ub.zhonguo7118.cn

[O06] 使用进程池
来源：https://uy.zhonguo1118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://jn.zhonguo6118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://mi.zhonguo7118.cn

JS:   // child_process / cluster 模块
来源：https://cu.zhonguo8118.cn

TS:   // child_process / cluster 模块
来源：https://lx.zhonguo3118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://an.zhonguo2118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://jf.zhonguo1118.cn

Ruby: // fork 块
来源：https://sd.zhonguo6118.cn

C#:   Parallel.For
来源：https://hl.zhonguo2118.cn

================================================================================
来源：https://se.zhonguo8118.cn

P. 常用工具函数
来源：https://kj.zhonguo4118.cn

================================================================================
来源：https://si.zhonguo2118.cn

[P01] 生成 UUID
来源：https://bv.zhonguo3118.cn

Py:   str(uuid.uuid4())
来源：https://ln.zhonguo6118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://pj.zhonguo6118.cn

JS:   crypto.randomUUID()
来源：https://zh.zhonguo8118.cn

TS:   crypto.randomUUID()
来源：https://ke.zhonguo5118.cn

Java: UUID.randomUUID().toString()
来源：https://tj.zhonguo3118.cn

Go:   // 用 github.com/google/uuid
来源：https://zd.zhonguo1118.cn

Ruby: SecureRandom.uuid
来源：https://gz.zhonguo1118.cn

C#:   Guid.NewGuid().ToString()
来源：https://qx.zhonguo5118.cn

[P02] MD5 / SHA256 摘要
来源：https://ee.zhonguo7118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://lf.zhonguo3118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://kg.zhonguo1118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://zi.zhonguo7118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://gn.zhonguo1118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://hd.zhonguo5118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://aa.zhonguo1118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://dh.zhonguo5118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://vb.zhonguo4118.cn

[P03] 生成短随机字符串
来源：https://qb.zhonguo6118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://ij.zhonguo4118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://ma.zhonguo3118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://px.zhonguo1118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://hm.zhonguo1118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://wx.zhonguo7118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://cp.zhonguo3118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://wq.zhonguo1118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://ev.zhonguo5118.cn

[P04] 求长度
来源：https://ap.zhonguo4118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://gu.zhonguo5118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://qh.zhonguo2118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://my.zhonguo1118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://fn.zhonguo5118.cn

Java: list.size();  map.size();  s.length()
来源：https://dv.zhonguo2118.cn

Go:   len(arr);  len(m)
来源：https://sd.zhonguo5118.cn

Ruby: x.length;  x.size
来源：https://iq.zhonguo8118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://ul.zhonguo7118.cn

[P05] 判断两个对象内容是否相等
来源：https://eg.zhonguo4118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://ez.zhonguo1118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://bx.zhonguo4118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://za.zhonguo5118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://cj.zhonguo3118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://kg.zhonguo5118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://rj.zhonguo6118.cn

Ruby: a == b
来源：https://gv.zhonguo3118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://qq.zhonguo3118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://dz.zhonguo3118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://ch.zhonguo8118.cn

PHP:  if (empty($x)) {}
来源：https://ig.zhonguo5118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://zt.zhonguo6118.cn

TS:   if (x == null) {}
来源：https://ya.zhonguo1118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://xb.zhonguo5118.cn

Go:   if x == nil {}
来源：https://ft.zhonguo2118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://wz.zhonguo2118.cn

C#:   if (x is null) {}
来源：https://us.zhonguo4118.cn

[P07] 防抖与节流
来源：https://nj.zhonguo7118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://gv.zhonguo8118.cn

PHP:  // 手写时间戳比较
来源：https://no.zhonguo2118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://le.zhonguo3118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://bu.zhonguo3118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://wx.zhonguo5118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://wi.zhonguo3118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://jc.zhonguo1118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://bf.zhonguo8118.cn

[P08] 处理浮点精度问题
来源：https://sb.zhonguo4118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://gt.zhonguo6118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://vl.zhonguo4118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://jj.zhonguo8118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://af.zhonguo3118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://dr.zhonguo7118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://he.zhonguo5118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://ac.zhonguo3118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://uu.zhonguo1118.cn

================================================================================
来源：https://tn.zhonguo8118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://qd.zhonguo1118.cn

================================================================================
来源：https://tl.zhonguo3118.cn

[Q01] 创建表
来源：https://mi.zhonguo6118.cn

CREATE TABLE users (
来源：https://nm.zhonguo3118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://zk.zhonguo4118.cn

name VARCHAR(50) NOT NULL,
来源：https://rf.zhonguo4118.cn

email VARCHAR(100) UNIQUE,
来源：https://gp.zhonguo4118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://xq.zhonguo8118.cn

);
来源：https://cj.zhonguo8118.cn

[Q02] 创建带外键的表
来源：https://ms.zhonguo3118.cn

CREATE TABLE orders (
来源：https://xv.zhonguo2118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://gh.zhonguo1118.cn

user_id INT NOT NULL,
来源：https://re.zhonguo5118.cn

amount DECIMAL(10, 2),
来源：https://zw.zhonguo5118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://br.zhonguo8118.cn

);
来源：https://lb.zhonguo7118.cn

[Q03] 增加列
来源：https://tb.zhonguo1118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://wr.zhonguo1118.cn

[Q04] 修改列类型
来源：https://bh.zhonguo2118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://nv.zhonguo2118.cn

[Q05] 重命名列
来源：https://on.zhonguo8118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://vp.zhonguo3118.cn

[Q06] 删除列
来源：https://av.zhonguo8118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://aj.zhonguo3118.cn

[Q07] 删除表
来源：https://hg.zhonguo4118.cn

DROP TABLE IF EXISTS orders;
来源：https://jt.zhonguo8118.cn

[Q08] 创建普通索引
来源：https://wt.zhonguo1118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://xo.zhonguo4118.cn

[Q09] 创建唯一索引
来源：https://pe.zhonguo5118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://do.zhonguo8118.cn

[Q10] 插入单行
来源：https://ed.zhonguo4118.cn


<!-- 参考信息 -->