代发 wailian999

TS:   resp.ok;  resp.status
来源：http://xmh.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://mho.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://hch.cdnleiting.top

Ruby: resp.code.to_i
来源：http://fmy.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://ode.ehwqpu.com

[L08] 并发请求多个地址
来源：http://tqo.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ivc.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://fdt.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npw.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nqt.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dpg.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://chp.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://luc.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://glu.hfpthk.cn

================================================================================
来源：http://fzv.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://hts.sweek.top

================================================================================
来源：http://wxq.havefunace.top

[M01] 读取命令行参数
来源：http://qzk.hywenlv.cn

Py:   sys.argv[1:]
来源：http://frj.xinyue.icu

PHP:  $argv;  $argc;
来源：http://yti.sxryk.cn

JS:   process.argv.slice(2)
来源：http://ydy.tanke756.top

TS:   process.argv.slice(2)
来源：http://cxx.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://nnz.hnqzz.top

Go:   os.Args[1:]
来源：http://mer.zdbjq.cn

Ruby: ARGV
来源：http://oqs.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://maz.xuanzx.com

[M02] 读取环境变量
来源：http://rtg.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://jhw.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ntw.yuanzhike.top

JS:   process.env.HOME
来源：http://ipy.guowangkeji.top

TS:   process.env.HOME
来源：http://vue.wangdashe.top

Java: System.getenv("HOME")
来源：http://gfb.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gkw.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://mls.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lfj.guannengcc.top

[M03] 执行外部命令
来源：http://tgf.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ypa.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qbl.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://fmb.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cyf.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kos.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mld.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kaa.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://idb.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://iit.jinqigufen.top

Py:   os.getcwd()
来源：http://bdg.redwolf501.top

PHP:  getcwd();
来源：http://imc.epnwcf.com

JS:   process.cwd()
来源：http://kcv.yj20258888.top

TS:   process.cwd()
来源：http://oum.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://qke.cqqwz.cn

Go:   os.Getwd()
来源：http://tor.zhengqikj.top

Ruby: Dir.pwd
来源：http://qpn.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://uer.fengsongda.top

[M05] 设置退出码
来源：http://ufl.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://obo.hesvh.cn

PHP:  exit(1);
来源：http://nlz.xuanzx.com

JS:   process.exit(1)
来源：http://lzl.sysykeji.top

TS:   process.exit(1)
来源：http://fgo.jianghu66.top

Java: System.exit(1)
来源：http://sch.316326.xyz

Go:   os.Exit(1)
来源：http://yzl.c1oappe.top

Ruby: exit 1
来源：http://fan.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sbc.jqgfzy.top

[M06] 向标准错误输出
来源：http://was.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://luk.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tnj.guannengcc.top

JS:   console.error("err")
来源：http://vfk.feifeiyinyue.top

TS:   console.error("err")
来源：http://eyn.ybcxt.top

Java: System.err.println("err")
来源：http://lqt.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qpp.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://ozu.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://fjk.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://aqy.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://yvd.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://epy.jqgufenzy.top

JS:   require.main === module
来源：http://abc.dashuyun.cn

TS:   require.main === module
来源：http://fsv.andypj.xyz

Java: public static void main(String[] args)
来源：http://wvo.zhaomingkeji.xyz

Go:   func main()
来源：http://tqa.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jwv.pycfn.com

C#:   static void Main(string[] args)
来源：http://ajo.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://rff.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://oyx.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://mtd.zdbjq.cn

JS:   process.platform;  process.version
来源：http://ijy.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://hjn.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qtj.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://drq.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bob.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://who.fktsv.cn

================================================================================
来源：http://ykm.jinqigufen.top

N. 数据结构与算法
来源：http://uiw.nanxinkj.top

================================================================================
来源：http://wiw.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://khv.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cyg.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sli.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://upf.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmy.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tll.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://uwo.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cyy.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://hli.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qul.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://wja.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogh.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xkd.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ryf.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jrv.pycfn.com

Go:   slices.Sort(arr)
来源：http://nbp.fktsv.cn

Ruby: arr.sort
来源：http://sny.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jmb.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://vnh.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dwz.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://gtd.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://agk.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://saz.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bqw.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vdh.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cbq.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://lbt.vehdjk.com

[N04] 斐波那契数列
来源：http://lgd.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vwr.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ahq.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tcg.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bnr.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rqw.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://chz.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rqk.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aac.yanxiufei.cn

[N05] 最大公约数
来源：http://tts.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://wom.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qao.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wyn.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://brb.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cob.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eoj.tian-w.cn

Ruby: a.gcd(b)
来源：http://mrf.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zhf.vqdsnc.cn

[N06] 判断回文字符串
来源：http://rmr.0kj1m.cn

Py:   s == s[::-1]
来源：http://oyz.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://zdv.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://ewi.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://kji.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fzd.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://zlc.chenzaomai.com

Ruby: s == s.reverse
来源：http://qoy.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://xxo.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://vqo.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lgc.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ehd.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ohs.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://ixj.vqdsnc.cn

Java: // 手写 HashMap
来源：http://npn.yj20258.top

Go:   // 手写 map[int]int
来源：http://iwm.jinqigufen.top

Ruby: // 手写 Hash
来源：http://esu.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://udu.316326.xyz

[N08] 生成全排列
来源：http://mnd.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://zlz.mhx1999.top

PHP:  // 手写递归交换
来源：http://zwv.vehdjk.com

JS:   // 手写回溯递归
来源：http://alu.fzhhl.top

TS:   // 手写回溯递归
来源：http://lvt.xylfe.cn

Java: // 手写回溯递归
来源：http://etf.birdmap.top

Go:   // 手写回溯递归
来源：http://mvv.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://add.yj20258.top

C#:   // 手写回溯递归
来源：http://wxe.zdbjq.cn

[N09] 栈与队列
来源：http://twc.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zos.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dxo.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jvl.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ydc.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://urj.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://myw.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zot.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://etb.yueranfly.top

[N10] 链表节点定义
来源：http://pfv.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zcp.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://edh.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ygf.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pwh.ivvv.top

Java: class Node { int v; Node next; }
来源：http://kek.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ufs.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://krv.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oez.redwolf501.top

[N11] 二叉树中序遍历
来源：http://qpw.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oce.ybcxt.top

PHP:  // 手写递归函数
来源：http://hdh.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pee.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyv.gogol.net.cn

Java: // 手写递归
来源：http://osq.tianlin.xyz

Go:   // 手写递归
来源：http://bbm.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xoe.dashuyun.cn

C#:   // 手写递归
来源：http://gah.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sig.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qdh.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://erz.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pmy.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://inc.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bjk.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hkv.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qgp.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://anc.gogol.net.cn

================================================================================
来源：http://pzu.hesvh.cn

O. 并发与异步
来源：http://izf.zdbjq.cn

================================================================================
来源：http://bcz.jlsjyb.cn

[O01] 启动一个线程
来源：http://ajx.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dwa.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gao.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tol.shangyingyoupin.top

TS:   // 同 JS
来源：http://byh.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://vlu.fehbvm.com

Go:   go f()
来源：http://zjy.hywenlv.cn

Ruby: Thread.new { f }
来源：http://gib.hammf.cn

C#:   Task.Run(() => F());
来源：http://axk.shangyingyoupin.top

[O02] 使用线程池
来源：http://lkt.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pzk.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wnv.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://yye.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://zdi.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://ufy.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zps.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://smp.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ywj.jianghu66.top

[O03] 加锁保护共享数据
来源：http://pud.iojbl.cn

Py:   with lock: shared += 1
来源：http://vwx.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://tsq.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iaz.hnqzz.top

TS:   // 同 JS
来源：http://quy.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://vgb.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lky.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wnt.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://vvv.yj20258.top

[O04] 定义异步函数并等待
来源：http://cnj.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://pyo.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ncd.yvedp.cn

JS:   async function f() { await g(); }
来源：http://sxb.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cat.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xtt.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://izi.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wyo.tanke756.top

C#:   async Task F() { await G(); }
来源：http://mvq.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://rem.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://utt.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gps.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://ihy.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://vdb.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://okl.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ync.epnwcf.com

Ruby: threads.map(&:join)
来源：http://dab.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eoc.yvedp.cn

[O06] 使用进程池
来源：http://jps.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zhh.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://dnu.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://jdt.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://mhr.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nhp.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ukh.pengpengdd.cyou

Ruby: // fork 块
来源：http://drg.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://wks.birdmap.top

================================================================================
来源：http://qcg.cdnleiting.top

P. 常用工具函数
来源：http://ejw.ppjwa.cn

================================================================================
来源：http://ruu.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://rsl.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://prq.cdnleiting.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xrr.uphjek.com

JS:   crypto.randomUUID()
来源：http://atj.fehbvm.com

TS:   crypto.randomUUID()
来源：http://hrn.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://hzx.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://nbm.tanke756.top

Ruby: SecureRandom.uuid
来源：http://bbi.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://vwa.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://qvg.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fpx.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wov.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jnr.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://znn.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ned.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wgk.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hhx.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cwy.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://zlo.zhoulong.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xcg.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rdn.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zwq.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nzs.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oqf.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gln.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://okb.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wlh.nanxuanxn.top

[P04] 求长度
来源：http://sec.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vdq.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://thr.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smh.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wim.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://mch.pycfn.com

Go:   len(arr);  len(m)
来源：http://orm.xziqi.cn

Ruby: x.length;  x.size
来源：http://keg.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://hve.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://llu.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://edb.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hot.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hij.cashguo.top


<!-- 参考信息 -->