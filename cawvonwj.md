代发 wailian999

================================================================================
来源：http://kuw.yuxming.cn

[M01] 读取命令行参数
来源：http://ctz.yonumen.top

Py:   sys.argv[1:]
来源：http://yhn.cucudq.cn

PHP:  $argv;  $argc;
来源：http://lmx.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://aio.yonumen.top

TS:   process.argv.slice(2)
来源：http://vye.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://ewh.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://qxk.tanke756.top

Ruby: ARGV
来源：http://zgb.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://swu.guannengcc.top

[M02] 读取环境变量
来源：http://apv.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://kfa.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zrl.bjfxy.top

JS:   process.env.HOME
来源：http://lqp.jyoumei.cn

TS:   process.env.HOME
来源：http://itd.ydzc1.top

Java: System.getenv("HOME")
来源：http://hlv.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nyn.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://akq.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fob.aizwys.cn

[M03] 执行外部命令
来源：http://amc.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uiq.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://quc.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kxq.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://fyq.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uoz.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://noy.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ydq.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://pyg.shuidangran.top

[M04] 获取当前工作目录
来源：http://bwd.aizwys.cn

Py:   os.getcwd()
来源：http://abp.zhengqikj.top

PHP:  getcwd();
来源：http://afu.zdqjudy.top

JS:   process.cwd()
来源：http://duy.hcnkem.com

TS:   process.cwd()
来源：http://ssu.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://mfe.kuanghao11.cn

Go:   os.Getwd()
来源：http://tkk.jinqigufen.top

Ruby: Dir.pwd
来源：http://aow.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://umd.gaohongyu789.top

[M05] 设置退出码
来源：http://rbu.gotoacloud.top

Py:   sys.exit(1)
来源：http://xga.epnwcf.com

PHP:  exit(1);
来源：http://seu.hammf.cn

JS:   process.exit(1)
来源：http://vlx.cdnleiting.top

TS:   process.exit(1)
来源：http://nvv.mhx1999.top

Java: System.exit(1)
来源：http://hwj.yfazqb.com

Go:   os.Exit(1)
来源：http://lix.jinqigfzy.top

Ruby: exit 1
来源：http://usg.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://stn.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://gzy.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://qyy.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://swg.jinghuilouyu.cn

JS:   console.error("err")
来源：http://zoa.daxiang520.top

TS:   console.error("err")
来源：http://mzi.hnqzz.top

Java: System.err.println("err")
来源：http://shy.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qui.yongpay.top

Ruby: warn "err"
来源：http://fny.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://hfp.jinqigufen.top

[M07] 判断是否为主入口
来源：http://gir.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://nsm.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eye.redwolf501.top

JS:   require.main === module
来源：http://vzz.9152youxi.cn

TS:   require.main === module
来源：http://bhk.haohaochexian.top

Java: public static void main(String[] args)
来源：http://kiv.shzxlz.cn

Go:   func main()
来源：http://wnd.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hdd.aizwys.cn

C#:   static void Main(string[] args)
来源：http://jkh.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://ctx.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://qha.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://wul.ybcxt.top

JS:   process.platform;  process.version
来源：http://kbc.redwolf501.top

TS:   process.platform;  process.version
来源：http://gad.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rfc.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zkz.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qtu.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eli.guowangkeji.top

================================================================================
来源：http://huj.gzhubu.top

N. 数据结构与算法
来源：http://dso.xinyue.icu

================================================================================
来源：http://dsa.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://fws.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://igr.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wpa.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sun.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hsv.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bew.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://xpq.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wby.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fin.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://jxc.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://hpz.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xik.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vjv.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tck.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uhb.yuxming.cn

Go:   slices.Sort(arr)
来源：http://faz.cucudq.cn

Ruby: arr.sort
来源：http://nou.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zkw.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://kir.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vqa.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://vpr.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vfz.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://owe.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gzz.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rcw.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ife.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://euy.gogol.net.cn

[N04] 斐波那契数列
来源：http://lwk.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rrf.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzn.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zqn.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kei.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yvx.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oao.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hqb.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mkq.hysaishi.cn

[N05] 最大公约数
来源：http://mld.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://qzu.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ntu.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvv.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zoo.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vyj.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jrf.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://gji.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zmc.cucudq.cn

[N06] 判断回文字符串
来源：http://hie.tarul.cn

Py:   s == s[::-1]
来源：http://upv.bjfxy.top

PHP:  $s === strrev($s);
来源：http://qqr.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://ned.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://you.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bim.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://ykc.zhijiandao.cn

Ruby: s == s.reverse
来源：http://bqw.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yfk.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://wyi.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://soo.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nvc.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ppw.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://zhs.xinyue.icu

Java: // 手写 HashMap
来源：http://pir.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://ast.meibo888.top

Ruby: // 手写 Hash
来源：http://qjy.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mhg.jinghuilouyu.cn

[N08] 生成全排列
来源：http://ccg.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://wwf.cucudq.cn

PHP:  // 手写递归交换
来源：http://yoc.uphjek.com

JS:   // 手写回溯递归
来源：http://fdd.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://cdn.nanxinkj.top

Java: // 手写回溯递归
来源：http://fwm.yangfankeji.com

Go:   // 手写回溯递归
来源：http://ppv.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://tei.xinyue.icu

C#:   // 手写回溯递归
来源：http://flb.dashuyun.cn

[N09] 栈与队列
来源：http://mrz.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iar.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lda.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ejv.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eua.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pxf.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wri.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sag.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvx.tianlin.xyz

[N10] 链表节点定义
来源：http://hkh.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pxf.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vxx.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vfl.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mcs.yongpay.top

Java: class Node { int v; Node next; }
来源：http://rid.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://qvn.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hlc.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ohf.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://oqh.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vlp.mhx1999.top

PHP:  // 手写递归函数
来源：http://ttf.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itg.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivq.gotoacloud.top

Java: // 手写递归
来源：http://vgp.andypj.xyz

Go:   // 手写递归
来源：http://wcm.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oof.zhijiandao.cn

C#:   // 手写递归
来源：http://jka.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pyx.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nlk.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gby.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://auh.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thv.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dii.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kfv.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xwc.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ouv.birdmap.top

================================================================================
来源：http://jgy.zhixingplan.top

O. 并发与异步
来源：http://lje.yonumen.top

================================================================================
来源：http://vqg.xuanzx.com

[O01] 启动一个线程
来源：http://fyy.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sug.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://odo.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ceh.jiagoushi.top

TS:   // 同 JS
来源：http://bhc.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://ret.fanxiaobao.xyz

Go:   go f()
来源：http://wgv.fehbvm.com

Ruby: Thread.new { f }
来源：http://djj.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://ojo.zhijiandao.cn

[O02] 使用线程池
来源：http://ryu.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dhc.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qqo.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://aed.xuanzx.com

TS:   // worker_threads 线程池
来源：http://pzj.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uuh.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zbv.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bjk.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aps.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://rrz.zdbjq.cn

Py:   with lock: shared += 1
来源：http://uvm.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://cok.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sts.yfazqb.com

TS:   // 同 JS
来源：http://mdh.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://tbu.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zrn.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wwm.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://rar.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://sfc.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://gab.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hwk.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://shc.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aox.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gpu.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lkd.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://sgt.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://hyo.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://cof.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://tib.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vsc.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://nwv.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://arf.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjy.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://afh.fktsv.cn

Ruby: threads.map(&:join)
来源：http://jdk.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://gwi.yangfankeji.com

[O06] 使用进程池
来源：http://cfl.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pxb.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://llb.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://rgj.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://tuk.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dmj.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xpv.yonumen.top

Ruby: // fork 块
来源：http://ljo.0kj1m.cn

C#:   Parallel.For
来源：http://hgl.andypj.xyz

================================================================================
来源：http://akq.shuidangran.top

P. 常用工具函数
来源：http://vpy.ctjpmb.com

================================================================================
来源：http://cye.fzhhl.top

[P01] 生成 UUID
来源：http://tzv.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://zpj.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://etw.redwolf501.top

JS:   crypto.randomUUID()
来源：http://pes.ybcxt.top

TS:   crypto.randomUUID()
来源：http://eky.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://dtc.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://mcy.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://tij.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://tsi.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://wad.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://guw.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pnj.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sas.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lhc.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pyv.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gsn.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://grv.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gtr.zhixingplan.top

[P03] 生成短随机字符串
来源：http://csd.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mpb.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://drt.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgv.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uax.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xkx.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://frz.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iym.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ffg.tanke756.top

[P04] 求长度
来源：http://xtg.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://djr.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://icw.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oqk.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzg.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://lqq.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://gld.316326.xyz

Ruby: x.length;  x.size
来源：http://hsq.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gdb.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://kds.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gnn.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eoy.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mtq.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jnb.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://egk.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://vap.ydjk.org.cn

Ruby: a == b
来源：http://mab.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dxr.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qer.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://css.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://bxx.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gwv.daxiang520.top

TS:   if (x == null) {}
来源：http://jkd.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qcb.quarkkingdee.top

Go:   if x == nil {}
来源：http://tvx.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sai.meibo888.top

C#:   if (x is null) {}
来源：http://fwv.yfazqb.com

[P07] 防抖与节流
来源：http://ote.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pof.shuidangran.top


<!-- 参考信息 -->