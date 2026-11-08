代发 wailian999

C#:   (int)resp.StatusCode
来源：https://nm.zhonguo3118.cn

[L08] 并发请求多个地址
来源：https://nl.zhonguo2118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://li.zhonguo2118.cn

PHP:  curl_multi_init() 系列
来源：https://hb.zhonguo8118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ps.zhonguo3118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://tp.zhonguo7118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://kx.zhonguo1118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://fq.zhonguo7118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://ux.zhonguo1118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://ez.zhonguo3118.cn

================================================================================
来源：https://ug.zhonguo3118.cn

M. 命令行 / 进程 / 环境
来源：https://po.zhonguo3118.cn

================================================================================
来源：https://fi.zhonguo8118.cn

[M01] 读取命令行参数
来源：https://qz.zhonguo7118.cn

Py:   sys.argv[1:]
来源：https://xj.zhonguo8118.cn

PHP:  $argv;  $argc;
来源：https://ge.zhonguo8118.cn

JS:   process.argv.slice(2)
来源：https://zw.zhonguo4118.cn

TS:   process.argv.slice(2)
来源：https://ee.zhonguo5118.cn

Java: args 数组（main 方法参数）
来源：https://tp.zhonguo2118.cn

Go:   os.Args[1:]
来源：https://lp.zhonguo7118.cn

Ruby: ARGV
来源：https://qe.zhonguo8118.cn

C#:   args 数组（Main 方法参数）
来源：https://eg.zhonguo2118.cn

[M02] 读取环境变量
来源：https://ck.zhonguo2118.cn

Py:   os.environ.get("HOME")
来源：https://lv.zhonguo4118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://xg.zhonguo1118.cn

JS:   process.env.HOME
来源：https://wi.zhonguo3118.cn

TS:   process.env.HOME
来源：https://cn.zhonguo7118.cn

Java: System.getenv("HOME")
来源：https://ev.zhonguo3118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://es.zhonguo4118.cn

Ruby: ENV["HOME"]
来源：https://mr.zhonguo5118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://fn.zhonguo4118.cn

[M03] 执行外部命令
来源：https://um.zhonguo2118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://we.zhonguo7118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://xf.zhonguo7118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://id.zhonguo2118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://cm.zhonguo2118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://qp.zhonguo5118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://ij.zhonguo5118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://ck.zhonguo7118.cn

C#:   Process.Start("ls", "-l");
来源：https://uz.zhonguo3118.cn

[M04] 获取当前工作目录
来源：https://ok.zhonguo4118.cn

Py:   os.getcwd()
来源：https://em.zhonguo4118.cn

PHP:  getcwd();
来源：https://ff.zhonguo7118.cn

JS:   process.cwd()
来源：https://nv.zhonguo1118.cn

TS:   process.cwd()
来源：https://iy.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://rq.zhonguo4118.cn

Go:   os.Getwd()
来源：https://fx.zhonguo5118.cn

Ruby: Dir.pwd
来源：https://el.zhonguo1118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://hp.zhonguo6118.cn

[M05] 设置退出码
来源：https://ip.zhonguo6118.cn

Py:   sys.exit(1)
来源：https://ou.zhonguo4118.cn

PHP:  exit(1);
来源：https://zn.zhonguo1118.cn

JS:   process.exit(1)
来源：https://hv.zhonguo3118.cn

TS:   process.exit(1)
来源：https://tp.zhonguo2118.cn

Java: System.exit(1)
来源：https://bq.zhonguo4118.cn

Go:   os.Exit(1)
来源：https://sq.zhonguo1118.cn

Ruby: exit 1
来源：https://yf.zhonguo3118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://dy.zhonguo1118.cn

[M06] 向标准错误输出
来源：https://ue.zhonguo2118.cn

Py:   print("err", file=sys.stderr)
来源：https://ve.zhonguo1118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://vg.zhonguo8118.cn

JS:   console.error("err")
来源：https://mz.zhonguo4118.cn

TS:   console.error("err")
来源：https://mh.zhonguo3118.cn

Java: System.err.println("err")
来源：https://ul.zhonguo8118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://pv.zhonguo1118.cn

Ruby: warn "err"
来源：https://xl.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://up.zhonguo3118.cn

[M07] 判断是否为主入口
来源：https://ho.zhonguo2118.cn

Py:   if __name__ == "__main__":
来源：https://uq.zhonguo6118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://uy.zhonguo8118.cn

JS:   require.main === module
来源：https://ft.zhonguo2118.cn

TS:   require.main === module
来源：https://yx.zhonguo7118.cn

Java: public static void main(String[] args)
来源：https://uo.zhonguo7118.cn

Go:   func main()
来源：https://xw.zhonguo1118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://th.zhonguo2118.cn

C#:   static void Main(string[] args)
来源：https://vl.zhonguo3118.cn

[M08] 获取系统与运行时信息
来源：https://dg.zhonguo5118.cn

Py:   platform.system();  platform.python_version()
来源：https://ni.zhonguo8118.cn

PHP:  PHP_OS;  phpversion();
来源：https://tr.zhonguo5118.cn

JS:   process.platform;  process.version
来源：https://bk.zhonguo5118.cn

TS:   process.platform;  process.version
来源：https://qx.zhonguo5118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://tn.zhonguo3118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://dj.zhonguo8118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://dy.zhonguo2118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://ng.zhonguo2118.cn

================================================================================
来源：https://fp.zhonguo3118.cn

N. 数据结构与算法
来源：https://wj.zhonguo8118.cn

================================================================================
来源：https://xp.zhonguo1118.cn

[N01] 二分查找（有序数组）
来源：https://gf.zhonguo2118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://uy.zhonguo8118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://sd.zhonguo8118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://iy.zhonguo4118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://vj.zhonguo2118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://se.zhonguo1118.cn

Go:   sort.SearchInts(arr, x)
来源：https://cf.zhonguo2118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://tn.zhonguo2118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://ov.zhonguo6118.cn

[N02] 排序（工程实践用内置实现）
来源：https://fn.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://hj.zhonguo4118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://yg.zhonguo5118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://fx.zhonguo3118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://uh.zhonguo7118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://fp.zhonguo3118.cn

Go:   slices.Sort(arr)
来源：https://yc.zhonguo1118.cn

Ruby: arr.sort
来源：https://uz.zhonguo7118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://gg.zhonguo6118.cn

[N03] 快速排序（分治示例）
来源：https://xs.zhonguo5118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://vb.zhonguo4118.cn

PHP:  // 递归实现，或用 usort
来源：https://kk.zhonguo1118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://bx.zhonguo7118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://la.zhonguo4118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://zv.zhonguo6118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://fu.zhonguo7118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://mc.zhonguo8118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://sp.zhonguo7118.cn

[N04] 斐波那契数列
来源：https://mn.zhonguo1118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://mr.zhonguo7118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://sl.zhonguo6118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ae.zhonguo2118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://he.zhonguo5118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://as.zhonguo2118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://zl.zhonguo6118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://pb.zhonguo6118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://ts.zhonguo2118.cn

[N05] 最大公约数
来源：https://gw.zhonguo6118.cn

Py:   math.gcd(a, b)
来源：https://ud.zhonguo3118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://vt.zhonguo6118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://ch.zhonguo6118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://xb.zhonguo6118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://pg.zhonguo6118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://mr.zhonguo2118.cn

Ruby: a.gcd(b)
来源：https://dy.zhonguo6118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://kq.zhonguo6118.cn

[N06] 判断回文字符串
来源：https://ne.zhonguo7118.cn

Py:   s == s[::-1]
来源：https://fj.zhonguo8118.cn

PHP:  $s === strrev($s);
来源：https://eu.zhonguo1118.cn

JS:   s === [...s].reverse().join("")
来源：https://gv.zhonguo3118.cn

TS:   s === [...s].reverse().join("")
来源：https://bu.zhonguo7118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://yl.zhonguo1118.cn

Go:   // 双指针从两端比较
来源：https://rw.zhonguo4118.cn

Ruby: s == s.reverse
来源：https://mh.zhonguo4118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://hv.zhonguo2118.cn

[N07] 两数之和（返回下标）
来源：https://yg.zhonguo6118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://ka.zhonguo7118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://uh.zhonguo8118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://ph.zhonguo1118.cn

TS:   // 手写 Map<string, number>
来源：https://ah.zhonguo6118.cn

Java: // 手写 HashMap
来源：https://fv.zhonguo2118.cn

Go:   // 手写 map[int]int
来源：https://sc.zhonguo6118.cn

Ruby: // 手写 Hash
来源：https://sc.zhonguo2118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://bo.zhonguo3118.cn

[N08] 生成全排列
来源：https://pi.zhonguo7118.cn

Py:   itertools.permutations(arr)
来源：https://qw.zhonguo6118.cn

PHP:  // 手写递归交换
来源：https://na.zhonguo5118.cn

JS:   // 手写回溯递归
来源：https://bo.zhonguo4118.cn

TS:   // 手写回溯递归
来源：https://nv.zhonguo6118.cn

Java: // 手写回溯递归
来源：https://vt.zhonguo8118.cn

Go:   // 手写回溯递归
来源：https://wh.zhonguo7118.cn

Ruby: arr.permutation.to_a
来源：https://la.zhonguo1118.cn

C#:   // 手写回溯递归
来源：https://xn.zhonguo4118.cn

[N09] 栈与队列
来源：https://pn.zhonguo2118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://po.zhonguo7118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://qq.zhonguo7118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://ga.zhonguo8118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://ws.zhonguo7118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://sl.zhonguo6118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://gj.zhonguo4118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://qp.zhonguo6118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://uf.zhonguo5118.cn

[N10] 链表节点定义
来源：https://zz.zhonguo5118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://fq.zhonguo4118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://sz.zhonguo2118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://pt.zhonguo2118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://bx.zhonguo8118.cn

Java: class Node { int v; Node next; }
来源：https://bb.zhonguo3118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://zq.zhonguo2118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://qd.zhonguo7118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://fm.zhonguo4118.cn

[N11] 二叉树中序遍历
来源：https://fx.zhonguo7118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://cr.zhonguo5118.cn

PHP:  // 手写递归函数
来源：https://yj.zhonguo7118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ur.zhonguo5118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://wb.zhonguo6118.cn

Java: // 手写递归
来源：https://io.zhonguo2118.cn

Go:   // 手写递归
来源：https://bl.zhonguo4118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://rv.zhonguo1118.cn

C#:   // 手写递归
来源：https://jo.zhonguo1118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://wv.zhonguo1118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://le.zhonguo8118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://ub.zhonguo6118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://xs.zhonguo6118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://od.zhonguo4118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://nn.zhonguo6118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://ga.zhonguo5118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://go.zhonguo8118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://ko.zhonguo1118.cn

================================================================================
来源：https://of.zhonguo7118.cn

O. 并发与异步
来源：https://rm.zhonguo6118.cn

================================================================================
来源：https://qt.zhonguo4118.cn

[O01] 启动一个线程
来源：https://tn.zhonguo2118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://rt.zhonguo6118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://hh.zhonguo1118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://ho.zhonguo2118.cn

TS:   // 同 JS
来源：https://wa.zhonguo7118.cn

Java: new Thread(() -> f()).start()
来源：https://pd.zhonguo6118.cn

Go:   go f()
来源：https://mf.zhonguo8118.cn

Ruby: Thread.new { f }
来源：https://yl.zhonguo7118.cn

C#:   Task.Run(() => F());
来源：https://fg.zhonguo5118.cn

[O02] 使用线程池
来源：https://kz.zhonguo7118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://jo.zhonguo2118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://xw.zhonguo7118.cn

JS:   // worker_threads 线程池
来源：https://pb.zhonguo8118.cn

TS:   // worker_threads 线程池
来源：https://km.zhonguo1118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://md.zhonguo6118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://to.zhonguo2118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://es.zhonguo5118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://bg.zhonguo6118.cn

[O03] 加锁保护共享数据
来源：https://re.zhonguo4118.cn

Py:   with lock: shared += 1
来源：https://pp.zhonguo5118.cn

PHP:  // 用 flock() 做文件锁
来源：https://og.zhonguo2118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://lg.zhonguo6118.cn

TS:   // 同 JS
来源：https://rb.zhonguo3118.cn

Java: synchronized (this) { shared++; }
来源：https://ym.zhonguo5118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://zs.zhonguo6118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://jn.zhonguo2118.cn

C#:   lock (gate) { shared++; }
来源：https://ao.zhonguo2118.cn

[O04] 定义异步函数并等待
来源：https://xl.zhonguo2118.cn

Py:   async def f():⏎    await g()
来源：https://tl.zhonguo8118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://bk.zhonguo4118.cn

JS:   async function f() { await g(); }
来源：https://re.zhonguo8118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://xy.zhonguo7118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://ur.zhonguo8118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://rx.zhonguo7118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://vn.zhonguo5118.cn

C#:   async Task F() { await G(); }
来源：https://au.zhonguo7118.cn

[O05] 并发执行并等待全部完成
来源：https://yt.zhonguo6118.cn

Py:   asyncio.gather(*tasks)
来源：https://ks.zhonguo6118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://jw.zhonguo4118.cn

JS:   await Promise.all(tasks)
来源：https://vl.zhonguo6118.cn

TS:   await Promise.all(tasks)
来源：https://ea.zhonguo6118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://tb.zhonguo8118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://en.zhonguo1118.cn

Ruby: threads.map(&:join)
来源：https://vs.zhonguo3118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://ud.zhonguo7118.cn

[O06] 使用进程池
来源：https://eu.zhonguo7118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://hj.zhonguo1118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://cr.zhonguo8118.cn

JS:   // child_process / cluster 模块
来源：https://sm.zhonguo8118.cn

TS:   // child_process / cluster 模块
来源：https://mi.zhonguo8118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://se.zhonguo1118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://oh.zhonguo8118.cn

Ruby: // fork 块
来源：https://yz.zhonguo1118.cn

C#:   Parallel.For
来源：https://ez.zhonguo6118.cn

================================================================================
来源：https://em.zhonguo6118.cn

P. 常用工具函数
来源：https://sj.zhonguo2118.cn

================================================================================
来源：https://ui.zhonguo6118.cn

[P01] 生成 UUID
来源：https://ot.zhonguo1118.cn

Py:   str(uuid.uuid4())
来源：https://em.zhonguo8118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://qv.zhonguo1118.cn

JS:   crypto.randomUUID()
来源：https://kb.zhonguo7118.cn

TS:   crypto.randomUUID()
来源：https://rn.zhonguo7118.cn

Java: UUID.randomUUID().toString()
来源：https://kf.zhonguo3118.cn

Go:   // 用 github.com/google/uuid
来源：https://qp.zhonguo2118.cn

Ruby: SecureRandom.uuid
来源：https://jm.zhonguo8118.cn

C#:   Guid.NewGuid().ToString()
来源：https://pq.zhonguo8118.cn

[P02] MD5 / SHA256 摘要
来源：https://ci.zhonguo8118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://cr.zhonguo8118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://xo.zhonguo8118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://vm.zhonguo8118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://cf.zhonguo4118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://ml.zhonguo5118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://dz.zhonguo3118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://gq.zhonguo5118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://vk.zhonguo6118.cn

[P03] 生成短随机字符串
来源：https://mv.zhonguo7118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://iw.zhonguo6118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://cs.zhonguo5118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://jl.zhonguo8118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://do.zhonguo5118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://nw.zhonguo5118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://ys.zhonguo1118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://jl.zhonguo1118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://qs.zhonguo1118.cn

[P04] 求长度
来源：https://nr.zhonguo1118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://qx.zhonguo1118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://fs.zhonguo8118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://mg.zhonguo5118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ej.zhonguo4118.cn

Java: list.size();  map.size();  s.length()
来源：https://as.zhonguo7118.cn

Go:   len(arr);  len(m)
来源：https://yz.zhonguo4118.cn

Ruby: x.length;  x.size
来源：https://ql.zhonguo1118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://ap.zhonguo6118.cn

[P05] 判断两个对象内容是否相等
来源：https://pa.zhonguo3118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://hd.zhonguo2118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://ns.zhonguo7118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://as.zhonguo1118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://os.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://mk.zhonguo4118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://ti.zhonguo7118.cn

Ruby: a == b
来源：https://xw.zhonguo1118.cn


<!-- 参考信息 -->