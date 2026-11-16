代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fgt.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ckw.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://htu.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hfe.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://ypi.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hoz.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xoj.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://vql.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://ghw.jyoumei.cn

Java: resp.statusCode()
来源：http://iae.zhongyouzk.top

Go:   resp.StatusCode
来源：http://omm.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://vvf.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://aej.hfpthk.cn

[L08] 并发请求多个地址
来源：http://htu.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gvm.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://kpd.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fnz.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmz.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://evo.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mcb.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kmo.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eaz.mhx1999.top

================================================================================
来源：http://coq.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://xoj.c1oappe.top

================================================================================
来源：http://inw.chenzaomai.com

[M01] 读取命令行参数
来源：http://mje.ppjwa.cn

Py:   sys.argv[1:]
来源：http://qhw.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://srk.tarul.cn

JS:   process.argv.slice(2)
来源：http://fhy.aizwys.cn

TS:   process.argv.slice(2)
来源：http://ywy.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://iqn.jinqigfzy.top

Go:   os.Args[1:]
来源：http://uay.ctjpmb.com

Ruby: ARGV
来源：http://ydd.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://aae.9152youxi.cn

[M02] 读取环境变量
来源：http://ljh.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://mwe.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hak.chenlongwang.top

JS:   process.env.HOME
来源：http://fcl.jyoumei.cn

TS:   process.env.HOME
来源：http://sea.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://cqf.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pqe.havefunace.top

Ruby: ENV["HOME"]
来源：http://seh.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pqt.gogol.net.cn

[M03] 执行外部命令
来源：http://mok.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://leg.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rlc.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kgk.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://amc.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qzm.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xqs.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://iuu.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://ciz.sweek.top

[M04] 获取当前工作目录
来源：http://ahw.ehwqpu.com

Py:   os.getcwd()
来源：http://oyk.mhx1999.top

PHP:  getcwd();
来源：http://izk.snrcjt.cn

JS:   process.cwd()
来源：http://cdm.ppjwa.cn

TS:   process.cwd()
来源：http://psx.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://wow.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://urf.cashguo.top

Ruby: Dir.pwd
来源：http://orx.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://zpj.tanke756.top

[M05] 设置退出码
来源：http://vwr.yfazqb.com

Py:   sys.exit(1)
来源：http://wme.hfpthk.cn

PHP:  exit(1);
来源：http://ucu.aibaodan.cn

JS:   process.exit(1)
来源：http://ure.mhx1999.top

TS:   process.exit(1)
来源：http://roh.gotoacloud.top

Java: System.exit(1)
来源：http://dzv.fktsv.cn

Go:   os.Exit(1)
来源：http://vzf.andypj.xyz

Ruby: exit 1
来源：http://qta.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wfx.quarkkingdee.top

[M06] 向标准错误输出
来源：http://jvf.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://knn.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://wac.nanxuanxn.top

JS:   console.error("err")
来源：http://nwt.yvedp.cn

TS:   console.error("err")
来源：http://gps.quarkkingdee.top

Java: System.err.println("err")
来源：http://cii.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dhi.mhx1999.top

Ruby: warn "err"
来源：http://dtq.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://slm.mhx1999.top

[M07] 判断是否为主入口
来源：http://wdn.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://iys.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iws.hammf.cn

JS:   require.main === module
来源：http://aol.ppjwa.cn

TS:   require.main === module
来源：http://ibv.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://gby.daxiang520.top

Go:   func main()
来源：http://sev.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hlv.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://rul.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://uji.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://cmv.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://jsj.fzhhl.top

JS:   process.platform;  process.version
来源：http://qcw.316326.xyz

TS:   process.platform;  process.version
来源：http://dmx.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://knx.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://czq.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bai.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jjp.chenlongwang.top

================================================================================
来源：http://vcz.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://msr.yj20258888.top

================================================================================
来源：http://our.tarul.cn

[N01] 二分查找（有序数组）
来源：http://jpn.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://abs.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ait.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwr.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sec.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xae.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://mpz.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ccf.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://koe.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://ybc.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://wid.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sci.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://jvo.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zrr.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hbt.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://kiq.yj202588.top

Ruby: arr.sort
来源：http://sdl.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qov.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://goh.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zol.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://tra.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vfu.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tut.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cvh.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yhb.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ksz.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fyj.gotoacloud.top

[N04] 斐波那契数列
来源：http://hbe.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nub.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qrt.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://deb.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://beh.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rlw.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ywb.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qxj.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aqg.iojbl.cn

[N05] 最大公约数
来源：http://ydi.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://zxt.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nou.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcc.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygq.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ptk.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wus.cdnleiting.top

Ruby: a.gcd(b)
来源：http://kax.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gvw.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://yqn.zhengqikj.top

Py:   s == s[::-1]
来源：http://yqh.xinyue.icu

PHP:  $s === strrev($s);
来源：http://fdv.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://bzt.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://opr.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qvt.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://onq.zhongyouzk.top

Ruby: s == s.reverse
来源：http://eai.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ihi.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://wig.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zsn.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wzd.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nyo.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://xdx.zhengqikj.top

Java: // 手写 HashMap
来源：http://ask.yj20258888.top

Go:   // 手写 map[int]int
来源：http://grr.yongpay.top

Ruby: // 手写 Hash
来源：http://hsh.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://mpx.hysaishi.cn

[N08] 生成全排列
来源：http://fzq.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://vpu.fktsv.cn

PHP:  // 手写递归交换
来源：http://mlb.yueranfly.top

JS:   // 手写回溯递归
来源：http://umm.vehdjk.com

TS:   // 手写回溯递归
来源：http://nct.ybcxt.top

Java: // 手写回溯递归
来源：http://iff.dianchejie.cn

Go:   // 手写回溯递归
来源：http://qaj.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://jyg.jqgfzy.top

C#:   // 手写回溯递归
来源：http://fnh.aizwys.cn

[N09] 栈与队列
来源：http://uri.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yqf.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ksc.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://woh.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vfe.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nsa.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dfg.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://odn.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://myb.yangfankeji.com

[N10] 链表节点定义
来源：http://wgx.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://twx.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pan.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ghi.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yxc.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://rhc.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://mze.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zyv.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tbq.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://sll.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tkk.sxryk.cn

PHP:  // 手写递归函数
来源：http://giz.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zoi.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fsu.ppjwa.cn

Java: // 手写递归
来源：http://qle.ivvv.top

Go:   // 手写递归
来源：http://dfe.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nes.jinqigfzy.top

C#:   // 手写递归
来源：http://ozv.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oqf.fanxiaobao.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xjq.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhj.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxo.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxl.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xyg.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zpq.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://env.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xnh.shangyingyoupin.top

================================================================================
来源：http://rnk.0kj1m.cn

O. 并发与异步
来源：http://xrt.zhijiandao.cn

================================================================================
来源：http://ueg.feifeiyinyue.top

[O01] 启动一个线程
来源：http://jad.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nax.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://azz.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yun.jyoumei.cn

TS:   // 同 JS
来源：http://kou.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://bgw.xingfuxueyuan.xyz

Go:   go f()
来源：http://zhk.chenlongwang.top

Ruby: Thread.new { f }
来源：http://sro.yfazqb.com

C#:   Task.Run(() => F());
来源：http://htd.ybcxt.top

[O02] 使用线程池
来源：http://tof.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cwq.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cbi.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://ysn.sweek.top

TS:   // worker_threads 线程池
来源：http://xar.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://zxo.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hwm.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aig.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xqa.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://cwd.vehdjk.com

Py:   with lock: shared += 1
来源：http://gej.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://fbz.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oox.daxiang520.top

TS:   // 同 JS
来源：http://rmr.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://vcb.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zdj.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nxl.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://agj.yfazqb.com

[O04] 定义异步函数并等待
来源：http://twk.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://jdq.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jll.yvedp.cn

JS:   async function f() { await g(); }
来源：http://xjg.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xop.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rjb.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wis.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://nyr.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://wdt.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://euy.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://cth.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vev.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://gcq.316326.xyz

TS:   await Promise.all(tasks)
来源：http://agm.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ioe.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://etf.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://ddn.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://uvw.zhoulong.xyz

[O06] 使用进程池
来源：http://yef.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cqm.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zor.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://llz.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://acp.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xhb.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fgv.zhijiandao.cn

Ruby: // fork 块
来源：http://ofh.c1oappe.top

C#:   Parallel.For
来源：http://gwp.xuetiantiany.cn

================================================================================
来源：http://ipt.jiagoushi.top

P. 常用工具函数
来源：http://zzv.yj20258888.top

================================================================================
来源：http://mok.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://kzg.c1oappe.top

Py:   str(uuid.uuid4())
来源：http://ycc.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jum.jianghu66.top

JS:   crypto.randomUUID()
来源：http://hwn.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://ogl.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://teb.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://xei.yj202588.top

Ruby: SecureRandom.uuid
来源：http://scf.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://nyr.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://luc.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oxs.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jrr.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://khj.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lds.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ecz.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jph.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ulv.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vns.sysykeji.top

[P03] 生成短随机字符串
来源：http://jcg.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zqu.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qdk.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zdk.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://giu.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vay.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bmg.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jxj.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rqr.jinqigufen.top

[P04] 求长度
来源：http://cth.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tky.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snr.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stx.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eul.vehdjk.com


<!-- 参考信息 -->