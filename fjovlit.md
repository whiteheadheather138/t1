代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://lp.zhonguo3118.cn

JS:   process.env.HOME
来源：https://co.zhonguo2118.cn

TS:   process.env.HOME
来源：https://sa.zhonguo4118.cn

Java: System.getenv("HOME")
来源：https://ee.zhonguo8118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://fn.zhonguo5118.cn

Ruby: ENV["HOME"]
来源：https://ub.zhonguo7118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://ze.zhonguo4118.cn

[M03] 执行外部命令
来源：https://js.zhonguo4118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://ke.zhonguo2118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://sl.zhonguo4118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://hh.zhonguo6118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://sc.zhonguo2118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://xo.zhonguo1118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://bu.zhonguo8118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://hq.zhonguo3118.cn

C#:   Process.Start("ls", "-l");
来源：https://lh.zhonguo3118.cn

[M04] 获取当前工作目录
来源：https://gx.zhonguo1118.cn

Py:   os.getcwd()
来源：https://pw.zhonguo6118.cn

PHP:  getcwd();
来源：https://tk.zhonguo1118.cn

JS:   process.cwd()
来源：https://fd.zhonguo8118.cn

TS:   process.cwd()
来源：https://aj.zhonguo5118.cn

Java: Path.of("").toAbsolutePath()
来源：https://se.zhonguo3118.cn

Go:   os.Getwd()
来源：https://li.zhonguo1118.cn

Ruby: Dir.pwd
来源：https://jf.zhonguo2118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ce.zhonguo6118.cn

[M05] 设置退出码
来源：https://as.zhonguo5118.cn

Py:   sys.exit(1)
来源：https://ol.zhonguo1118.cn

PHP:  exit(1);
来源：https://zn.zhonguo6118.cn

JS:   process.exit(1)
来源：https://mt.zhonguo3118.cn

TS:   process.exit(1)
来源：https://sg.zhonguo5118.cn

Java: System.exit(1)
来源：https://xv.zhonguo8118.cn

Go:   os.Exit(1)
来源：https://rc.zhonguo6118.cn

Ruby: exit 1
来源：https://sj.zhonguo3118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://fm.zhonguo3118.cn

[M06] 向标准错误输出
来源：https://nv.zhonguo6118.cn

Py:   print("err", file=sys.stderr)
来源：https://hu.zhonguo5118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://dl.zhonguo7118.cn

JS:   console.error("err")
来源：https://jd.zhonguo7118.cn

TS:   console.error("err")
来源：https://as.zhonguo6118.cn

Java: System.err.println("err")
来源：https://lp.zhonguo6118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://ql.zhonguo3118.cn

Ruby: warn "err"
来源：https://fu.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://od.zhonguo6118.cn

[M07] 判断是否为主入口
来源：https://qt.zhonguo7118.cn

Py:   if __name__ == "__main__":
来源：https://hy.zhonguo5118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://yv.zhonguo5118.cn

JS:   require.main === module
来源：https://hq.zhonguo4118.cn

TS:   require.main === module
来源：https://mj.zhonguo1118.cn

Java: public static void main(String[] args)
来源：https://un.zhonguo1118.cn

Go:   func main()
来源：https://wj.zhonguo8118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://sv.zhonguo3118.cn

C#:   static void Main(string[] args)
来源：https://gc.zhonguo7118.cn

[M08] 获取系统与运行时信息
来源：https://xn.zhonguo7118.cn

Py:   platform.system();  platform.python_version()
来源：https://nz.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://cq.zhonguo8118.cn

JS:   process.platform;  process.version
来源：https://yq.zhonguo2118.cn

TS:   process.platform;  process.version
来源：https://bp.zhonguo4118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://xn.zhonguo4118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://wl.zhonguo4118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://zn.zhonguo4118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://fz.zhonguo4118.cn

================================================================================
来源：https://bt.zhonguo6118.cn

N. 数据结构与算法
来源：https://ax.zhonguo2118.cn

================================================================================
来源：https://lt.zhonguo2118.cn

[N01] 二分查找（有序数组）
来源：https://rw.zhonguo1118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://ws.zhonguo6118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://wr.zhonguo8118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://qa.zhonguo2118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://pi.zhonguo6118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://tg.zhonguo5118.cn

Go:   sort.SearchInts(arr, x)
来源：https://fe.zhonguo2118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://eb.zhonguo2118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://xo.zhonguo4118.cn

[N02] 排序（工程实践用内置实现）
来源：https://zt.zhonguo8118.cn

Py:   sorted(arr);  arr.sort()
来源：https://dp.zhonguo7118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://dt.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://wf.zhonguo7118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://rg.zhonguo7118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://yz.zhonguo2118.cn

Go:   slices.Sort(arr)
来源：https://ys.zhonguo3118.cn

Ruby: arr.sort
来源：https://ys.zhonguo8118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://ih.zhonguo6118.cn

[N03] 快速排序（分治示例）
来源：https://lt.zhonguo5118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://mi.zhonguo4118.cn

PHP:  // 递归实现，或用 usort
来源：https://fh.zhonguo4118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://ft.zhonguo1118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://kn.zhonguo6118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://or.zhonguo8118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://hk.zhonguo3118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://fp.zhonguo2118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://lh.zhonguo4118.cn

[N04] 斐波那契数列
来源：https://ot.zhonguo3118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://rt.zhonguo6118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://bv.zhonguo8118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://do.zhonguo3118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ef.zhonguo1118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://ga.zhonguo4118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://hw.zhonguo5118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://my.zhonguo5118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://kb.zhonguo1118.cn

[N05] 最大公约数
来源：https://gj.zhonguo7118.cn

Py:   math.gcd(a, b)
来源：https://nd.zhonguo7118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://my.zhonguo1118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://fa.zhonguo5118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://ac.zhonguo2118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://zv.zhonguo6118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://yq.zhonguo4118.cn

Ruby: a.gcd(b)
来源：https://ia.zhonguo7118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://wk.zhonguo1118.cn

[N06] 判断回文字符串
来源：https://vj.zhonguo4118.cn

Py:   s == s[::-1]
来源：https://dr.zhonguo6118.cn

PHP:  $s === strrev($s);
来源：https://wg.zhonguo2118.cn

JS:   s === [...s].reverse().join("")
来源：https://jc.zhonguo4118.cn

TS:   s === [...s].reverse().join("")
来源：https://dv.zhonguo6118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://pn.zhonguo2118.cn

Go:   // 双指针从两端比较
来源：https://kk.zhonguo1118.cn

Ruby: s == s.reverse
来源：https://fk.zhonguo4118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://jg.zhonguo3118.cn

[N07] 两数之和（返回下标）
来源：https://tb.zhonguo5118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://nf.zhonguo3118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://hl.zhonguo1118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://pa.zhonguo1118.cn

TS:   // 手写 Map<string, number>
来源：https://na.zhonguo7118.cn

Java: // 手写 HashMap
来源：https://zd.zhonguo2118.cn

Go:   // 手写 map[int]int
来源：https://ud.zhonguo8118.cn

Ruby: // 手写 Hash
来源：https://ci.zhonguo3118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://fl.zhonguo5118.cn

[N08] 生成全排列
来源：https://kw.zhonguo8118.cn

Py:   itertools.permutations(arr)
来源：https://bq.zhonguo2118.cn

PHP:  // 手写递归交换
来源：https://xc.zhonguo4118.cn

JS:   // 手写回溯递归
来源：https://vj.zhonguo6118.cn

TS:   // 手写回溯递归
来源：https://hj.zhonguo8118.cn

Java: // 手写回溯递归
来源：https://qd.zhonguo4118.cn

Go:   // 手写回溯递归
来源：https://rh.zhonguo5118.cn

Ruby: arr.permutation.to_a
来源：https://uv.zhonguo6118.cn

C#:   // 手写回溯递归
来源：https://zj.zhonguo1118.cn

[N09] 栈与队列
来源：https://jo.zhonguo1118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://lo.zhonguo2118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://kj.zhonguo8118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://iq.zhonguo8118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://sy.zhonguo2118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://dc.zhonguo4118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://hn.zhonguo5118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://dt.zhonguo4118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://gc.zhonguo2118.cn

[N10] 链表节点定义
来源：https://qm.zhonguo7118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://wu.zhonguo2118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://ch.zhonguo4118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://lf.zhonguo1118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://qp.zhonguo5118.cn

Java: class Node { int v; Node next; }
来源：https://yz.zhonguo2118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://ez.zhonguo8118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://tb.zhonguo8118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://zw.zhonguo4118.cn

[N11] 二叉树中序遍历
来源：https://xy.zhonguo2118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://tr.zhonguo4118.cn

PHP:  // 手写递归函数
来源：https://qy.zhonguo3118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://cq.zhonguo7118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://pi.zhonguo2118.cn

Java: // 手写递归
来源：https://rr.zhonguo8118.cn

Go:   // 手写递归
来源：https://kb.zhonguo2118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://dj.zhonguo1118.cn

C#:   // 手写递归
来源：https://zv.zhonguo2118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://hi.zhonguo1118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://ox.zhonguo3118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://ez.zhonguo3118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://uh.zhonguo7118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://cn.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://qb.zhonguo3118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://iy.zhonguo6118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://ey.zhonguo8118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://kb.zhonguo7118.cn

================================================================================
来源：https://gb.zhonguo1118.cn

O. 并发与异步
来源：https://ov.zhonguo1118.cn

================================================================================
来源：https://pl.zhonguo1118.cn

[O01] 启动一个线程
来源：https://zt.zhonguo3118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://dv.zhonguo7118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://lt.zhonguo1118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://yj.zhonguo4118.cn

TS:   // 同 JS
来源：https://uj.zhonguo1118.cn

Java: new Thread(() -> f()).start()
来源：https://nc.zhonguo8118.cn

Go:   go f()
来源：https://vu.zhonguo5118.cn

Ruby: Thread.new { f }
来源：https://ad.zhonguo3118.cn

C#:   Task.Run(() => F());
来源：https://bm.zhonguo5118.cn

[O02] 使用线程池
来源：https://wi.zhonguo4118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://ne.zhonguo2118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://dd.zhonguo4118.cn

JS:   // worker_threads 线程池
来源：https://ut.zhonguo6118.cn

TS:   // worker_threads 线程池
来源：https://tm.zhonguo2118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://sg.zhonguo3118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://xo.zhonguo5118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://ex.zhonguo1118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://xq.zhonguo7118.cn

[O03] 加锁保护共享数据
来源：https://lt.zhonguo6118.cn

Py:   with lock: shared += 1
来源：https://rh.zhonguo6118.cn

PHP:  // 用 flock() 做文件锁
来源：https://fp.zhonguo2118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://sa.zhonguo4118.cn

TS:   // 同 JS
来源：https://cp.zhonguo8118.cn

Java: synchronized (this) { shared++; }
来源：https://du.zhonguo7118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://ld.zhonguo5118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://vf.zhonguo5118.cn

C#:   lock (gate) { shared++; }
来源：https://xz.zhonguo2118.cn

[O04] 定义异步函数并等待
来源：https://lq.zhonguo6118.cn

Py:   async def f():⏎    await g()
来源：https://ql.zhonguo5118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://ns.zhonguo8118.cn

JS:   async function f() { await g(); }
来源：https://et.zhonguo6118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://xp.zhonguo8118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://yr.zhonguo7118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://up.zhonguo8118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://mg.zhonguo7118.cn

C#:   async Task F() { await G(); }
来源：https://uo.zhonguo6118.cn

[O05] 并发执行并等待全部完成
来源：https://dj.zhonguo6118.cn

Py:   asyncio.gather(*tasks)
来源：https://ec.zhonguo3118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://nv.zhonguo6118.cn

JS:   await Promise.all(tasks)
来源：https://gq.zhonguo3118.cn

TS:   await Promise.all(tasks)
来源：https://it.zhonguo4118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://mu.zhonguo8118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://iq.zhonguo4118.cn

Ruby: threads.map(&:join)
来源：https://qq.zhonguo8118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://cj.zhonguo8118.cn

[O06] 使用进程池
来源：https://bx.zhonguo7118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://qd.zhonguo2118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://tu.zhonguo8118.cn

JS:   // child_process / cluster 模块
来源：https://ul.zhonguo6118.cn

TS:   // child_process / cluster 模块
来源：https://qs.zhonguo4118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://ir.zhonguo4118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://ec.zhonguo3118.cn

Ruby: // fork 块
来源：https://qg.zhonguo2118.cn

C#:   Parallel.For
来源：https://in.zhonguo8118.cn

================================================================================
来源：https://ny.zhonguo8118.cn

P. 常用工具函数
来源：https://ay.zhonguo1118.cn

================================================================================
来源：https://om.zhonguo3118.cn

[P01] 生成 UUID
来源：https://zi.zhonguo4118.cn

Py:   str(uuid.uuid4())
来源：https://xe.zhonguo3118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://fg.zhonguo8118.cn

JS:   crypto.randomUUID()
来源：https://rh.zhonguo6118.cn

TS:   crypto.randomUUID()
来源：https://ei.zhonguo6118.cn

Java: UUID.randomUUID().toString()
来源：https://vc.zhonguo1118.cn

Go:   // 用 github.com/google/uuid
来源：https://wt.zhonguo7118.cn

Ruby: SecureRandom.uuid
来源：https://vy.zhonguo8118.cn

C#:   Guid.NewGuid().ToString()
来源：https://tk.zhonguo4118.cn

[P02] MD5 / SHA256 摘要
来源：https://yd.zhonguo2118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://ow.zhonguo6118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://xc.zhonguo7118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://hl.zhonguo8118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://xl.zhonguo7118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://tp.zhonguo5118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://sv.zhonguo3118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://wc.zhonguo6118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://oc.zhonguo3118.cn

[P03] 生成短随机字符串
来源：https://vx.zhonguo6118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://om.zhonguo5118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://fc.zhonguo5118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://jq.zhonguo1118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://bu.zhonguo6118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://mt.zhonguo5118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://wl.zhonguo2118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://jl.zhonguo8118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://vs.zhonguo6118.cn

[P04] 求长度
来源：https://yo.zhonguo4118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://wy.zhonguo3118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ra.zhonguo8118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://wt.zhonguo8118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ts.zhonguo7118.cn

Java: list.size();  map.size();  s.length()
来源：https://bn.zhonguo6118.cn

Go:   len(arr);  len(m)
来源：https://os.zhonguo7118.cn

Ruby: x.length;  x.size
来源：https://qw.zhonguo6118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://wb.zhonguo7118.cn

[P05] 判断两个对象内容是否相等
来源：https://jh.zhonguo3118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://gk.zhonguo3118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://wf.zhonguo6118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://ko.zhonguo5118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://ld.zhonguo5118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://hq.zhonguo6118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://io.zhonguo3118.cn

Ruby: a == b
来源：https://vk.zhonguo2118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://zx.zhonguo5118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://og.zhonguo2118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://mc.zhonguo8118.cn

PHP:  if (empty($x)) {}
来源：https://qn.zhonguo2118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://xn.zhonguo7118.cn

TS:   if (x == null) {}
来源：https://lh.zhonguo8118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://qd.zhonguo3118.cn

Go:   if x == nil {}
来源：https://gv.zhonguo2118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://hy.zhonguo5118.cn

C#:   if (x is null) {}
来源：https://xu.zhonguo8118.cn

[P07] 防抖与节流
来源：https://xn.zhonguo4118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://gl.zhonguo4118.cn

PHP:  // 手写时间戳比较
来源：https://as.zhonguo3118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://iu.zhonguo3118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://fm.zhonguo2118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://lr.zhonguo4118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://sf.zhonguo6118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://pz.zhonguo7118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://yb.zhonguo2118.cn

[P08] 处理浮点精度问题
来源：https://hn.zhonguo4118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://hf.zhonguo2118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://gs.zhonguo8118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://mu.zhonguo4118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://eg.zhonguo6118.cn


<!-- 参考信息 -->