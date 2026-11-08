代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://st.zhonguo5118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://vw.zhonguo3118.cn

================================================================================
来源：https://ej.zhonguo4118.cn

M. 命令行 / 进程 / 环境
来源：https://pz.zhonguo6118.cn

================================================================================
来源：https://ta.zhonguo1118.cn

[M01] 读取命令行参数
来源：https://fb.zhonguo7118.cn

Py:   sys.argv[1:]
来源：https://sr.zhonguo6118.cn

PHP:  $argv;  $argc;
来源：https://gc.zhonguo3118.cn

JS:   process.argv.slice(2)
来源：https://hd.zhonguo7118.cn

TS:   process.argv.slice(2)
来源：https://uq.zhonguo7118.cn

Java: args 数组（main 方法参数）
来源：https://vp.zhonguo6118.cn

Go:   os.Args[1:]
来源：https://ri.zhonguo8118.cn

Ruby: ARGV
来源：https://dk.zhonguo3118.cn

C#:   args 数组（Main 方法参数）
来源：https://hz.zhonguo5118.cn

[M02] 读取环境变量
来源：https://vn.zhonguo5118.cn

Py:   os.environ.get("HOME")
来源：https://ee.zhonguo1118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://ej.zhonguo7118.cn

JS:   process.env.HOME
来源：https://nf.zhonguo6118.cn

TS:   process.env.HOME
来源：https://qm.zhonguo7118.cn

Java: System.getenv("HOME")
来源：https://oc.zhonguo7118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://lz.zhonguo4118.cn

Ruby: ENV["HOME"]
来源：https://jr.zhonguo2118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://ti.zhonguo3118.cn

[M03] 执行外部命令
来源：https://mc.zhonguo8118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://kz.zhonguo2118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://yx.zhonguo7118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://sa.zhonguo1118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://bc.zhonguo7118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://tk.zhonguo3118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://xh.zhonguo4118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://bs.zhonguo6118.cn

C#:   Process.Start("ls", "-l");
来源：https://vn.zhonguo3118.cn

[M04] 获取当前工作目录
来源：https://rp.zhonguo3118.cn

Py:   os.getcwd()
来源：https://we.zhonguo8118.cn

PHP:  getcwd();
来源：https://rx.zhonguo4118.cn

JS:   process.cwd()
来源：https://sn.zhonguo3118.cn

TS:   process.cwd()
来源：https://sx.zhonguo2118.cn

Java: Path.of("").toAbsolutePath()
来源：https://xl.zhonguo6118.cn

Go:   os.Getwd()
来源：https://dx.zhonguo4118.cn

Ruby: Dir.pwd
来源：https://hi.zhonguo3118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://yw.zhonguo8118.cn

[M05] 设置退出码
来源：https://nu.zhonguo3118.cn

Py:   sys.exit(1)
来源：https://cl.zhonguo1118.cn

PHP:  exit(1);
来源：https://be.zhonguo5118.cn

JS:   process.exit(1)
来源：https://pe.zhonguo1118.cn

TS:   process.exit(1)
来源：https://da.zhonguo7118.cn

Java: System.exit(1)
来源：https://ha.zhonguo4118.cn

Go:   os.Exit(1)
来源：https://yv.zhonguo4118.cn

Ruby: exit 1
来源：https://eu.zhonguo4118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://uu.zhonguo1118.cn

[M06] 向标准错误输出
来源：https://cu.zhonguo3118.cn

Py:   print("err", file=sys.stderr)
来源：https://pc.zhonguo7118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://jw.zhonguo4118.cn

JS:   console.error("err")
来源：https://xa.zhonguo8118.cn

TS:   console.error("err")
来源：https://fl.zhonguo6118.cn

Java: System.err.println("err")
来源：https://ys.zhonguo4118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://rs.zhonguo2118.cn

Ruby: warn "err"
来源：https://pg.zhonguo6118.cn

C#:   Console.Error.WriteLine("err")
来源：https://yk.zhonguo2118.cn

[M07] 判断是否为主入口
来源：https://zu.zhonguo1118.cn

Py:   if __name__ == "__main__":
来源：https://fh.zhonguo8118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://tl.zhonguo8118.cn

JS:   require.main === module
来源：https://nf.zhonguo2118.cn

TS:   require.main === module
来源：https://xr.zhonguo8118.cn

Java: public static void main(String[] args)
来源：https://rh.zhonguo8118.cn

Go:   func main()
来源：https://at.zhonguo8118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://ts.zhonguo7118.cn

C#:   static void Main(string[] args)
来源：https://fu.zhonguo1118.cn

[M08] 获取系统与运行时信息
来源：https://yv.zhonguo4118.cn

Py:   platform.system();  platform.python_version()
来源：https://nw.zhonguo1118.cn

PHP:  PHP_OS;  phpversion();
来源：https://ja.zhonguo5118.cn

JS:   process.platform;  process.version
来源：https://ii.zhonguo1118.cn

TS:   process.platform;  process.version
来源：https://dc.zhonguo3118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://sd.zhonguo1118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://xf.zhonguo2118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://ek.zhonguo1118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://bp.zhonguo8118.cn

================================================================================
来源：https://ve.zhonguo2118.cn

N. 数据结构与算法
来源：https://ta.zhonguo8118.cn

================================================================================
来源：https://br.zhonguo4118.cn

[N01] 二分查找（有序数组）
来源：https://ic.zhonguo3118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://mp.zhonguo3118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://bi.zhonguo3118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://mf.zhonguo1118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://gw.zhonguo2118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://cp.zhonguo8118.cn

Go:   sort.SearchInts(arr, x)
来源：https://gk.zhonguo7118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://od.zhonguo4118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://ke.zhonguo2118.cn

[N02] 排序（工程实践用内置实现）
来源：https://eq.zhonguo2118.cn

Py:   sorted(arr);  arr.sort()
来源：https://dr.zhonguo4118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://ju.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://lo.zhonguo3118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://gw.zhonguo1118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://ah.zhonguo7118.cn

Go:   slices.Sort(arr)
来源：https://ap.zhonguo6118.cn

Ruby: arr.sort
来源：https://uq.zhonguo5118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://bt.zhonguo2118.cn

[N03] 快速排序（分治示例）
来源：https://hv.zhonguo2118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://jb.zhonguo2118.cn

PHP:  // 递归实现，或用 usort
来源：https://om.zhonguo3118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://ey.zhonguo4118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://cp.zhonguo7118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://sq.zhonguo2118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://tf.zhonguo2118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://oy.zhonguo1118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://ot.zhonguo1118.cn

[N04] 斐波那契数列
来源：https://uw.zhonguo4118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://xv.zhonguo8118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://pm.zhonguo6118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ks.zhonguo2118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ra.zhonguo7118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://hq.zhonguo3118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://mb.zhonguo8118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://un.zhonguo1118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://me.zhonguo4118.cn

[N05] 最大公约数
来源：https://id.zhonguo3118.cn

Py:   math.gcd(a, b)
来源：https://ul.zhonguo8118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://av.zhonguo2118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://oc.zhonguo8118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://gp.zhonguo8118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://jf.zhonguo2118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://to.zhonguo4118.cn

Ruby: a.gcd(b)
来源：https://cb.zhonguo5118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://cz.zhonguo4118.cn

[N06] 判断回文字符串
来源：https://rv.zhonguo1118.cn

Py:   s == s[::-1]
来源：https://ta.zhonguo4118.cn

PHP:  $s === strrev($s);
来源：https://lf.zhonguo7118.cn

JS:   s === [...s].reverse().join("")
来源：https://wt.zhonguo8118.cn

TS:   s === [...s].reverse().join("")
来源：https://az.zhonguo8118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://ye.zhonguo6118.cn

Go:   // 双指针从两端比较
来源：https://pg.zhonguo6118.cn

Ruby: s == s.reverse
来源：https://nd.zhonguo3118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://dv.zhonguo7118.cn

[N07] 两数之和（返回下标）
来源：https://zf.zhonguo8118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://oh.zhonguo8118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://mq.zhonguo5118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://cu.zhonguo7118.cn

TS:   // 手写 Map<string, number>
来源：https://my.zhonguo2118.cn

Java: // 手写 HashMap
来源：https://qb.zhonguo7118.cn

Go:   // 手写 map[int]int
来源：https://ah.zhonguo5118.cn

Ruby: // 手写 Hash
来源：https://hq.zhonguo3118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://yt.zhonguo8118.cn

[N08] 生成全排列
来源：https://kb.zhonguo5118.cn

Py:   itertools.permutations(arr)
来源：https://cg.zhonguo8118.cn

PHP:  // 手写递归交换
来源：https://hm.zhonguo3118.cn

JS:   // 手写回溯递归
来源：https://xw.zhonguo8118.cn

TS:   // 手写回溯递归
来源：https://qw.zhonguo5118.cn

Java: // 手写回溯递归
来源：https://la.zhonguo6118.cn

Go:   // 手写回溯递归
来源：https://ug.zhonguo8118.cn

Ruby: arr.permutation.to_a
来源：https://hv.zhonguo7118.cn

C#:   // 手写回溯递归
来源：https://ff.zhonguo4118.cn

[N09] 栈与队列
来源：https://zw.zhonguo7118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://gd.zhonguo5118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://ym.zhonguo8118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://hi.zhonguo8118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://pv.zhonguo7118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://wu.zhonguo1118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://rz.zhonguo5118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://sp.zhonguo8118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://gi.zhonguo6118.cn

[N10] 链表节点定义
来源：https://vk.zhonguo6118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://dn.zhonguo4118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://lw.zhonguo1118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://vx.zhonguo3118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://ev.zhonguo1118.cn

Java: class Node { int v; Node next; }
来源：https://lw.zhonguo4118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://fj.zhonguo8118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://uz.zhonguo1118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://he.zhonguo4118.cn

[N11] 二叉树中序遍历
来源：https://nx.zhonguo5118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://uh.zhonguo6118.cn

PHP:  // 手写递归函数
来源：https://ec.zhonguo2118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://fh.zhonguo3118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ae.zhonguo4118.cn

Java: // 手写递归
来源：https://yi.zhonguo2118.cn

Go:   // 手写递归
来源：https://oy.zhonguo1118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://ny.zhonguo7118.cn

C#:   // 手写递归
来源：https://vr.zhonguo3118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://lm.zhonguo2118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://ko.zhonguo1118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://hy.zhonguo7118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://uk.zhonguo2118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://hp.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://kj.zhonguo3118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://hc.zhonguo3118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://du.zhonguo5118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://fx.zhonguo8118.cn

================================================================================
来源：https://el.zhonguo3118.cn

O. 并发与异步
来源：https://ic.zhonguo7118.cn

================================================================================
来源：https://mx.zhonguo7118.cn

[O01] 启动一个线程
来源：https://or.zhonguo6118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://ni.zhonguo5118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://ip.zhonguo8118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://sl.zhonguo3118.cn

TS:   // 同 JS
来源：https://yo.zhonguo6118.cn

Java: new Thread(() -> f()).start()
来源：https://fl.zhonguo4118.cn

Go:   go f()
来源：https://vd.zhonguo1118.cn

Ruby: Thread.new { f }
来源：https://ld.zhonguo3118.cn

C#:   Task.Run(() => F());
来源：https://rx.zhonguo5118.cn

[O02] 使用线程池
来源：https://rq.zhonguo2118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://xp.zhonguo4118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://qw.zhonguo4118.cn

JS:   // worker_threads 线程池
来源：https://dg.zhonguo3118.cn

TS:   // worker_threads 线程池
来源：https://wj.zhonguo7118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://im.zhonguo5118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://ax.zhonguo8118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://vn.zhonguo1118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://gd.zhonguo4118.cn

[O03] 加锁保护共享数据
来源：https://sl.zhonguo1118.cn

Py:   with lock: shared += 1
来源：https://tw.zhonguo6118.cn

PHP:  // 用 flock() 做文件锁
来源：https://bu.zhonguo3118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://ku.zhonguo7118.cn

TS:   // 同 JS
来源：https://vj.zhonguo1118.cn

Java: synchronized (this) { shared++; }
来源：https://su.zhonguo1118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://yu.zhonguo8118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://zw.zhonguo6118.cn

C#:   lock (gate) { shared++; }
来源：https://uh.zhonguo4118.cn

[O04] 定义异步函数并等待
来源：https://tm.zhonguo6118.cn

Py:   async def f():⏎    await g()
来源：https://pm.zhonguo4118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://mj.zhonguo8118.cn

JS:   async function f() { await g(); }
来源：https://fr.zhonguo3118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://pm.zhonguo5118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://ix.zhonguo8118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://jy.zhonguo1118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://he.zhonguo4118.cn

C#:   async Task F() { await G(); }
来源：https://gs.zhonguo8118.cn

[O05] 并发执行并等待全部完成
来源：https://de.zhonguo6118.cn

Py:   asyncio.gather(*tasks)
来源：https://tz.zhonguo8118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://nt.zhonguo1118.cn

JS:   await Promise.all(tasks)
来源：https://ds.zhonguo6118.cn

TS:   await Promise.all(tasks)
来源：https://np.zhonguo4118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://iu.zhonguo5118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://yg.zhonguo2118.cn

Ruby: threads.map(&:join)
来源：https://ay.zhonguo5118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://qq.zhonguo5118.cn

[O06] 使用进程池
来源：https://kl.zhonguo5118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://qm.zhonguo1118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://sy.zhonguo2118.cn

JS:   // child_process / cluster 模块
来源：https://xy.zhonguo2118.cn

TS:   // child_process / cluster 模块
来源：https://wq.zhonguo6118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://cq.zhonguo5118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://ty.zhonguo7118.cn

Ruby: // fork 块
来源：https://nb.zhonguo5118.cn

C#:   Parallel.For
来源：https://fd.zhonguo3118.cn

================================================================================
来源：https://oa.zhonguo6118.cn

P. 常用工具函数
来源：https://zb.zhonguo3118.cn

================================================================================
来源：https://mp.zhonguo5118.cn

[P01] 生成 UUID
来源：https://ux.zhonguo7118.cn

Py:   str(uuid.uuid4())
来源：https://xo.zhonguo8118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://kl.zhonguo2118.cn

JS:   crypto.randomUUID()
来源：https://pn.zhonguo4118.cn

TS:   crypto.randomUUID()
来源：https://kk.zhonguo6118.cn

Java: UUID.randomUUID().toString()
来源：https://iq.zhonguo1118.cn

Go:   // 用 github.com/google/uuid
来源：https://rf.zhonguo4118.cn

Ruby: SecureRandom.uuid
来源：https://sg.zhonguo3118.cn

C#:   Guid.NewGuid().ToString()
来源：https://nz.zhonguo2118.cn

[P02] MD5 / SHA256 摘要
来源：https://bl.zhonguo5118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://bc.zhonguo4118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://fu.zhonguo2118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://yj.zhonguo8118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://bx.zhonguo1118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://dp.zhonguo3118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://ly.zhonguo6118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://vr.zhonguo8118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://rf.zhonguo8118.cn

[P03] 生成短随机字符串
来源：https://xe.zhonguo8118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://hk.zhonguo2118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://su.zhonguo3118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://qm.zhonguo4118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://tm.zhonguo6118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://gk.zhonguo2118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://je.zhonguo8118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://eo.zhonguo7118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://jk.zhonguo6118.cn

[P04] 求长度
来源：https://rx.zhonguo4118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://zc.zhonguo6118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://ar.zhonguo4118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://da.zhonguo2118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://hc.zhonguo5118.cn

Java: list.size();  map.size();  s.length()
来源：https://es.zhonguo6118.cn

Go:   len(arr);  len(m)
来源：https://fv.zhonguo2118.cn

Ruby: x.length;  x.size
来源：https://hg.zhonguo1118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://xi.zhonguo8118.cn

[P05] 判断两个对象内容是否相等
来源：https://mo.zhonguo2118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://ey.zhonguo5118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://ev.zhonguo7118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://ag.zhonguo2118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://yt.zhonguo2118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://mo.zhonguo5118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://aj.zhonguo3118.cn

Ruby: a == b
来源：https://ut.zhonguo6118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://ro.zhonguo8118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://wm.zhonguo7118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://yz.zhonguo2118.cn

PHP:  if (empty($x)) {}
来源：https://gp.zhonguo5118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://lq.zhonguo1118.cn

TS:   if (x == null) {}
来源：https://we.zhonguo7118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://wl.zhonguo5118.cn

Go:   if x == nil {}
来源：https://ei.zhonguo6118.cn


<!-- 参考信息 -->