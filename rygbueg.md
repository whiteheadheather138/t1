代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://yf.zhonguo4118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://hg.zhonguo1118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://dm.zhonguo6118.cn

[L06] 解析响应为 JSON
来源：https://py.zhonguo5118.cn

Py:   resp.json()
来源：https://ls.zhonguo5118.cn

PHP:  json_decode($body, true);
来源：https://dv.zhonguo7118.cn

JS:   await resp.json()
来源：https://kn.zhonguo6118.cn

TS:   await resp.json()
来源：https://nu.zhonguo1118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://fw.zhonguo3118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://az.zhonguo8118.cn

Ruby: JSON.parse(resp.body)
来源：https://vp.zhonguo3118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://xo.zhonguo4118.cn

[L07] 处理 HTTP 状态码
来源：https://um.zhonguo3118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://lf.zhonguo5118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://ue.zhonguo8118.cn

JS:   resp.ok;  resp.status
来源：https://fv.zhonguo2118.cn

TS:   resp.ok;  resp.status
来源：https://dg.zhonguo4118.cn

Java: resp.statusCode()
来源：https://od.zhonguo1118.cn

Go:   resp.StatusCode
来源：https://ue.zhonguo4118.cn

Ruby: resp.code.to_i
来源：https://vx.zhonguo7118.cn

C#:   (int)resp.StatusCode
来源：https://cl.zhonguo7118.cn

[L08] 并发请求多个地址
来源：https://th.zhonguo3118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://iu.zhonguo5118.cn

PHP:  curl_multi_init() 系列
来源：https://qc.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://nx.zhonguo1118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://jh.zhonguo7118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://tg.zhonguo8118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://gk.zhonguo2118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://zh.zhonguo1118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://lp.zhonguo3118.cn

================================================================================
来源：https://uv.zhonguo5118.cn

M. 命令行 / 进程 / 环境
来源：https://mt.zhonguo1118.cn

================================================================================
来源：https://zg.zhonguo8118.cn

[M01] 读取命令行参数
来源：https://zq.zhonguo7118.cn

Py:   sys.argv[1:]
来源：https://rr.zhonguo6118.cn

PHP:  $argv;  $argc;
来源：https://qv.zhonguo8118.cn

JS:   process.argv.slice(2)
来源：https://cu.zhonguo7118.cn

TS:   process.argv.slice(2)
来源：https://ed.zhonguo4118.cn

Java: args 数组（main 方法参数）
来源：https://ys.zhonguo5118.cn

Go:   os.Args[1:]
来源：https://qc.zhonguo1118.cn

Ruby: ARGV
来源：https://cs.zhonguo4118.cn

C#:   args 数组（Main 方法参数）
来源：https://ci.zhonguo2118.cn

[M02] 读取环境变量
来源：https://ey.zhonguo5118.cn

Py:   os.environ.get("HOME")
来源：https://as.zhonguo7118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://qr.zhonguo7118.cn

JS:   process.env.HOME
来源：https://pp.zhonguo2118.cn

TS:   process.env.HOME
来源：https://mx.zhonguo3118.cn

Java: System.getenv("HOME")
来源：https://go.zhonguo3118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://lq.zhonguo5118.cn

Ruby: ENV["HOME"]
来源：https://cc.zhonguo8118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://nm.zhonguo3118.cn

[M03] 执行外部命令
来源：https://ff.zhonguo2118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://dy.zhonguo7118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://vf.zhonguo1118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://jm.zhonguo8118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://gm.zhonguo2118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://ls.zhonguo1118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://ll.zhonguo4118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://cj.zhonguo4118.cn

C#:   Process.Start("ls", "-l");
来源：https://ap.zhonguo5118.cn

[M04] 获取当前工作目录
来源：https://tz.zhonguo3118.cn

Py:   os.getcwd()
来源：https://mj.zhonguo5118.cn

PHP:  getcwd();
来源：https://ez.zhonguo5118.cn

JS:   process.cwd()
来源：https://hr.zhonguo8118.cn

TS:   process.cwd()
来源：https://lq.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://db.zhonguo2118.cn

Go:   os.Getwd()
来源：https://lo.zhonguo8118.cn

Ruby: Dir.pwd
来源：https://cb.zhonguo7118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://yu.zhonguo6118.cn

[M05] 设置退出码
来源：https://er.zhonguo5118.cn

Py:   sys.exit(1)
来源：https://pd.zhonguo6118.cn

PHP:  exit(1);
来源：https://xu.zhonguo6118.cn

JS:   process.exit(1)
来源：https://eq.zhonguo4118.cn

TS:   process.exit(1)
来源：https://kg.zhonguo6118.cn

Java: System.exit(1)
来源：https://fn.zhonguo7118.cn

Go:   os.Exit(1)
来源：https://qp.zhonguo8118.cn

Ruby: exit 1
来源：https://ip.zhonguo4118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://aa.zhonguo2118.cn

[M06] 向标准错误输出
来源：https://km.zhonguo1118.cn

Py:   print("err", file=sys.stderr)
来源：https://nz.zhonguo3118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://ib.zhonguo2118.cn

JS:   console.error("err")
来源：https://qy.zhonguo5118.cn

TS:   console.error("err")
来源：https://ou.zhonguo7118.cn

Java: System.err.println("err")
来源：https://ei.zhonguo6118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://fr.zhonguo3118.cn

Ruby: warn "err"
来源：https://kt.zhonguo3118.cn

C#:   Console.Error.WriteLine("err")
来源：https://nk.zhonguo2118.cn

[M07] 判断是否为主入口
来源：https://fk.zhonguo5118.cn

Py:   if __name__ == "__main__":
来源：https://gg.zhonguo3118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://kk.zhonguo7118.cn

JS:   require.main === module
来源：https://dn.zhonguo5118.cn

TS:   require.main === module
来源：https://hy.zhonguo7118.cn

Java: public static void main(String[] args)
来源：https://oh.zhonguo7118.cn

Go:   func main()
来源：https://ku.zhonguo1118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://xb.zhonguo1118.cn

C#:   static void Main(string[] args)
来源：https://wp.zhonguo2118.cn

[M08] 获取系统与运行时信息
来源：https://fs.zhonguo8118.cn

Py:   platform.system();  platform.python_version()
来源：https://nl.zhonguo6118.cn

PHP:  PHP_OS;  phpversion();
来源：https://mm.zhonguo7118.cn

JS:   process.platform;  process.version
来源：https://bz.zhonguo3118.cn

TS:   process.platform;  process.version
来源：https://bz.zhonguo1118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://vs.zhonguo4118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://ln.zhonguo1118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://vn.zhonguo6118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://bc.zhonguo6118.cn

================================================================================
来源：https://tn.zhonguo2118.cn

N. 数据结构与算法
来源：https://yn.zhonguo6118.cn

================================================================================
来源：https://tg.zhonguo3118.cn

[N01] 二分查找（有序数组）
来源：https://dm.zhonguo5118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://ai.zhonguo5118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://yr.zhonguo1118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://jb.zhonguo4118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://zv.zhonguo1118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://tl.zhonguo1118.cn

Go:   sort.SearchInts(arr, x)
来源：https://qq.zhonguo3118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://ti.zhonguo2118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://zu.zhonguo6118.cn

[N02] 排序（工程实践用内置实现）
来源：https://uc.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://mv.zhonguo4118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://ct.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://xd.zhonguo5118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://or.zhonguo6118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://wx.zhonguo4118.cn

Go:   slices.Sort(arr)
来源：https://lp.zhonguo1118.cn

Ruby: arr.sort
来源：https://qf.zhonguo3118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://wy.zhonguo8118.cn

[N03] 快速排序（分治示例）
来源：https://bc.zhonguo6118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://mz.zhonguo5118.cn

PHP:  // 递归实现，或用 usort
来源：https://tp.zhonguo7118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://gm.zhonguo2118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://my.zhonguo2118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://ui.zhonguo7118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://zo.zhonguo2118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://qo.zhonguo6118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://tl.zhonguo3118.cn

[N04] 斐波那契数列
来源：https://sf.zhonguo3118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://eb.zhonguo8118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://sv.zhonguo8118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ce.zhonguo6118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://la.zhonguo3118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://xx.zhonguo6118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://ui.zhonguo3118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://cc.zhonguo8118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://gq.zhonguo5118.cn

[N05] 最大公约数
来源：https://kx.zhonguo5118.cn

Py:   math.gcd(a, b)
来源：https://xe.zhonguo4118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://qd.zhonguo8118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://km.zhonguo4118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://pd.zhonguo8118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://pq.zhonguo7118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://xz.zhonguo6118.cn

Ruby: a.gcd(b)
来源：https://dv.zhonguo4118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://tt.zhonguo3118.cn

[N06] 判断回文字符串
来源：https://mp.zhonguo2118.cn

Py:   s == s[::-1]
来源：https://vd.zhonguo3118.cn

PHP:  $s === strrev($s);
来源：https://hl.zhonguo3118.cn

JS:   s === [...s].reverse().join("")
来源：https://vh.zhonguo2118.cn

TS:   s === [...s].reverse().join("")
来源：https://fr.zhonguo3118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://tv.zhonguo2118.cn

Go:   // 双指针从两端比较
来源：https://jv.zhonguo7118.cn

Ruby: s == s.reverse
来源：https://qf.zhonguo8118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://fl.zhonguo5118.cn

[N07] 两数之和（返回下标）
来源：https://wt.zhonguo5118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://ro.zhonguo6118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://ge.zhonguo5118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://th.zhonguo8118.cn

TS:   // 手写 Map<string, number>
来源：https://ny.zhonguo6118.cn

Java: // 手写 HashMap
来源：https://br.zhonguo4118.cn

Go:   // 手写 map[int]int
来源：https://gk.zhonguo5118.cn

Ruby: // 手写 Hash
来源：https://ni.zhonguo6118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://zw.zhonguo5118.cn

[N08] 生成全排列
来源：https://sa.zhonguo2118.cn

Py:   itertools.permutations(arr)
来源：https://dr.zhonguo6118.cn

PHP:  // 手写递归交换
来源：https://fv.zhonguo5118.cn

JS:   // 手写回溯递归
来源：https://hf.zhonguo3118.cn

TS:   // 手写回溯递归
来源：https://wn.zhonguo4118.cn

Java: // 手写回溯递归
来源：https://ef.zhonguo6118.cn

Go:   // 手写回溯递归
来源：https://gd.zhonguo5118.cn

Ruby: arr.permutation.to_a
来源：https://kn.zhonguo2118.cn

C#:   // 手写回溯递归
来源：https://ak.zhonguo5118.cn

[N09] 栈与队列
来源：https://jj.zhonguo1118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://zh.zhonguo5118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://ry.zhonguo4118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://yd.zhonguo8118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://kb.zhonguo6118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://ph.zhonguo2118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://bm.zhonguo6118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://lr.zhonguo8118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://jx.zhonguo5118.cn

[N10] 链表节点定义
来源：https://ue.zhonguo8118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://hb.zhonguo1118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://gv.zhonguo3118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://hb.zhonguo2118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://ua.zhonguo6118.cn

Java: class Node { int v; Node next; }
来源：https://vw.zhonguo5118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://wl.zhonguo4118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://do.zhonguo7118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://jg.zhonguo8118.cn

[N11] 二叉树中序遍历
来源：https://ob.zhonguo7118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://cl.zhonguo2118.cn

PHP:  // 手写递归函数
来源：https://jy.zhonguo7118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://xa.zhonguo6118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ao.zhonguo4118.cn

Java: // 手写递归
来源：https://fx.zhonguo1118.cn

Go:   // 手写递归
来源：https://bx.zhonguo6118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://jv.zhonguo6118.cn

C#:   // 手写递归
来源：https://bt.zhonguo1118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://nk.zhonguo8118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://gm.zhonguo3118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://da.zhonguo5118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://yj.zhonguo2118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://nh.zhonguo6118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://dn.zhonguo8118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://xm.zhonguo5118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://yt.zhonguo4118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://xh.zhonguo4118.cn

================================================================================
来源：https://mr.zhonguo4118.cn

O. 并发与异步
来源：https://nk.zhonguo8118.cn

================================================================================
来源：https://rj.zhonguo2118.cn

[O01] 启动一个线程
来源：https://bb.zhonguo5118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://uj.zhonguo3118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://vm.zhonguo2118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://rp.zhonguo7118.cn

TS:   // 同 JS
来源：https://pi.zhonguo5118.cn

Java: new Thread(() -> f()).start()
来源：https://mf.zhonguo2118.cn

Go:   go f()
来源：https://uy.zhonguo2118.cn

Ruby: Thread.new { f }
来源：https://py.zhonguo3118.cn

C#:   Task.Run(() => F());
来源：https://uv.zhonguo5118.cn

[O02] 使用线程池
来源：https://nm.zhonguo4118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://gv.zhonguo8118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://ea.zhonguo8118.cn

JS:   // worker_threads 线程池
来源：https://gi.zhonguo2118.cn

TS:   // worker_threads 线程池
来源：https://ak.zhonguo1118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://hb.zhonguo1118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://li.zhonguo4118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://zy.zhonguo1118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://vz.zhonguo8118.cn

[O03] 加锁保护共享数据
来源：https://xi.zhonguo8118.cn

Py:   with lock: shared += 1
来源：https://mr.zhonguo4118.cn

PHP:  // 用 flock() 做文件锁
来源：https://sj.zhonguo3118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://lg.zhonguo8118.cn

TS:   // 同 JS
来源：https://mc.zhonguo4118.cn

Java: synchronized (this) { shared++; }
来源：https://ma.zhonguo2118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://xd.zhonguo5118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://fg.zhonguo3118.cn

C#:   lock (gate) { shared++; }
来源：https://em.zhonguo5118.cn

[O04] 定义异步函数并等待
来源：https://gh.zhonguo8118.cn

Py:   async def f():⏎    await g()
来源：https://th.zhonguo2118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://ji.zhonguo2118.cn

JS:   async function f() { await g(); }
来源：https://pi.zhonguo6118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://pj.zhonguo5118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://wq.zhonguo1118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://qk.zhonguo6118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://rs.zhonguo3118.cn

C#:   async Task F() { await G(); }
来源：https://ie.zhonguo8118.cn

[O05] 并发执行并等待全部完成
来源：https://xf.zhonguo2118.cn

Py:   asyncio.gather(*tasks)
来源：https://dd.zhonguo1118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://dw.zhonguo6118.cn

JS:   await Promise.all(tasks)
来源：https://gf.zhonguo4118.cn

TS:   await Promise.all(tasks)
来源：https://qv.zhonguo6118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://vf.zhonguo6118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://hi.zhonguo2118.cn

Ruby: threads.map(&:join)
来源：https://hi.zhonguo7118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://sd.zhonguo4118.cn

[O06] 使用进程池
来源：https://vo.zhonguo3118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://zk.zhonguo8118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://sw.zhonguo6118.cn

JS:   // child_process / cluster 模块
来源：https://zp.zhonguo4118.cn

TS:   // child_process / cluster 模块
来源：https://sc.zhonguo5118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://dr.zhonguo1118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://yg.zhonguo2118.cn

Ruby: // fork 块
来源：https://sw.zhonguo7118.cn

C#:   Parallel.For
来源：https://ln.zhonguo5118.cn

================================================================================
来源：https://fp.zhonguo3118.cn

P. 常用工具函数
来源：https://mh.zhonguo8118.cn

================================================================================
来源：https://zw.zhonguo8118.cn

[P01] 生成 UUID
来源：https://vt.zhonguo5118.cn

Py:   str(uuid.uuid4())
来源：https://gj.zhonguo8118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://ry.zhonguo4118.cn

JS:   crypto.randomUUID()
来源：https://xn.zhonguo5118.cn

TS:   crypto.randomUUID()
来源：https://lx.zhonguo1118.cn

Java: UUID.randomUUID().toString()
来源：https://rp.zhonguo5118.cn

Go:   // 用 github.com/google/uuid
来源：https://si.zhonguo4118.cn

Ruby: SecureRandom.uuid
来源：https://hs.zhonguo2118.cn

C#:   Guid.NewGuid().ToString()
来源：https://xr.zhonguo2118.cn

[P02] MD5 / SHA256 摘要
来源：https://id.zhonguo2118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://qd.zhonguo4118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://nh.zhonguo4118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://za.zhonguo1118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://ei.zhonguo4118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://wc.zhonguo5118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://hr.zhonguo5118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://rp.zhonguo1118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://tn.zhonguo2118.cn

[P03] 生成短随机字符串
来源：https://nm.zhonguo6118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://nd.zhonguo8118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://ho.zhonguo7118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://on.zhonguo8118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://ms.zhonguo5118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://vs.zhonguo7118.cn


<!-- 参考信息 -->