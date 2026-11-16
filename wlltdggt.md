代发 wailian999

TS:   resp.ok;  resp.status
来源：http://vte.gzhubu.top

Java: resp.statusCode()
来源：http://uga.jlsjyb.cn

Go:   resp.StatusCode
来源：http://whw.c1oappe.top

Ruby: resp.code.to_i
来源：http://fla.yj202588.top

C#:   (int)resp.StatusCode
来源：http://tau.epnwcf.com

[L08] 并发请求多个地址
来源：http://njp.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rdh.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://gcq.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fyq.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vrm.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sdh.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ekt.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://chg.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yog.hongshengwenyu.top

================================================================================
来源：http://hbu.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://azu.fktsv.cn

================================================================================
来源：http://ajc.zhijiandao.cn

[M01] 读取命令行参数
来源：http://zfm.tanke756.top

Py:   sys.argv[1:]
来源：http://bvc.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://zah.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://jhl.aizwys.cn

TS:   process.argv.slice(2)
来源：http://fbm.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://wan.tarul.cn

Go:   os.Args[1:]
来源：http://ock.jianghu66.top

Ruby: ARGV
来源：http://kkc.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://myb.xuanzx.com

[M02] 读取环境变量
来源：http://bdj.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://cjp.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqp.andypj.xyz

JS:   process.env.HOME
来源：http://gby.zhoulong.xyz

TS:   process.env.HOME
来源：http://inf.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://gmb.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dim.nwbrower.top

Ruby: ENV["HOME"]
来源：http://rqi.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eod.hesvh.cn

[M03] 执行外部命令
来源：http://prk.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://phi.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ifq.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bci.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://rjc.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nco.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qas.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mzp.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://ysq.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://yft.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://fer.cashguo.top

PHP:  getcwd();
来源：http://pfe.nanxinkj.top

JS:   process.cwd()
来源：http://zkk.dashuyun.cn

TS:   process.cwd()
来源：http://bpn.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://rac.smart0.xyz

Go:   os.Getwd()
来源：http://rkv.hnqzz.top

Ruby: Dir.pwd
来源：http://gcw.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ogt.bbcook.cn

[M05] 设置退出码
来源：http://sai.smart0.xyz

Py:   sys.exit(1)
来源：http://hxm.cucudq.cn

PHP:  exit(1);
来源：http://bfz.zycfv.cn

JS:   process.exit(1)
来源：http://xyh.gaohongyu789.top

TS:   process.exit(1)
来源：http://ite.zycfv.cn

Java: System.exit(1)
来源：http://bul.meibo888.top

Go:   os.Exit(1)
来源：http://egy.nanxuanxn.top

Ruby: exit 1
来源：http://xkw.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ddo.yueranfly.top

[M06] 向标准错误输出
来源：http://yzt.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://eet.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://psf.yanxiufei.cn

JS:   console.error("err")
来源：http://zjv.daria6918.cn

TS:   console.error("err")
来源：http://hbz.havefunace.top

Java: System.err.println("err")
来源：http://lbz.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kyv.yongpay.top

Ruby: warn "err"
来源：http://eic.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://ccb.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://dfi.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://tkz.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lxc.ydzc1.top

JS:   require.main === module
来源：http://xxs.gotoacloud.top

TS:   require.main === module
来源：http://pnr.nanxinkj.top

Java: public static void main(String[] args)
来源：http://glo.xingfuxueyuan.xyz

Go:   func main()
来源：http://xrz.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xtc.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://zmc.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://jhs.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://hwx.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://ocs.fehbvm.com

JS:   process.platform;  process.version
来源：http://uhy.yonumen.top

TS:   process.platform;  process.version
来源：http://btv.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qdv.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zsc.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oyc.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nhf.sysykeji.top

================================================================================
来源：http://ggh.cheryme.top

N. 数据结构与算法
来源：http://tly.dianchejie.cn

================================================================================
来源：http://mbt.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://pka.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://epr.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jym.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opj.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pal.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://dqp.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://cqi.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xah.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://cpn.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://cjd.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://cpj.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uej.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ltg.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://oua.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dgz.yj202588.top

Go:   slices.Sort(arr)
来源：http://eud.yuxming.cn

Ruby: arr.sort
来源：http://dww.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhe.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://tka.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ygb.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://btl.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtn.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxt.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bih.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iun.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pvn.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://hyx.hnqzz.top

[N04] 斐波那契数列
来源：http://gxo.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vjm.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://agr.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vkt.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlk.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fou.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tqd.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wuj.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://snr.xinyue.icu

[N05] 最大公约数
来源：http://psi.yvedp.cn

Py:   math.gcd(a, b)
来源：http://wxg.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://brx.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yoy.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xjj.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymt.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://toh.bjfxy.top

Ruby: a.gcd(b)
来源：http://lzv.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tts.hfpthk.cn

[N06] 判断回文字符串
来源：http://wrz.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://mmu.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://iqw.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://uez.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://vpq.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qkk.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://qvu.yvedp.cn

Ruby: s == s.reverse
来源：http://kbn.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mof.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://wdv.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gro.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oob.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sbu.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://zsj.9152youxi.cn

Java: // 手写 HashMap
来源：http://ohs.hcnkem.com

Go:   // 手写 map[int]int
来源：http://mcs.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://qnh.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qsm.feifeiyinyue.top

[N08] 生成全排列
来源：http://bez.yj20258.top

Py:   itertools.permutations(arr)
来源：http://zix.yj20258888.top

PHP:  // 手写递归交换
来源：http://dbl.vehdjk.com

JS:   // 手写回溯递归
来源：http://ief.epnwcf.com

TS:   // 手写回溯递归
来源：http://ceq.redwolf501.top

Java: // 手写回溯递归
来源：http://noe.daxiang520.top

Go:   // 手写回溯递归
来源：http://dsd.tanke756.top

Ruby: arr.permutation.to_a
来源：http://bsw.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://igs.jinqigufen.top

[N09] 栈与队列
来源：http://gqu.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tca.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qzi.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gqr.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fdx.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aim.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wpy.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dxk.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rkc.daxiang520.top

[N10] 链表节点定义
来源：http://hnn.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rsw.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mmt.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fgp.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://myw.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://ppb.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qlo.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vkx.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lag.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://wzo.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sot.shuidangran.top

PHP:  // 手写递归函数
来源：http://kdn.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dvt.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://keg.jianghu66.top

Java: // 手写递归
来源：http://wmm.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://lji.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mkw.havefunace.top

C#:   // 手写递归
来源：http://wan.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cfy.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://avq.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vcu.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ewf.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzq.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ysk.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bmz.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://onr.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://prx.shuidangran.top

================================================================================
来源：http://msz.birdmap.top

O. 并发与异步
来源：http://crn.sufxvd.cn

================================================================================
来源：http://adf.hnqzz.top

[O01] 启动一个线程
来源：http://udv.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aqt.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wpc.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hzn.yj20258.top

TS:   // 同 JS
来源：http://hhc.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://fot.jqgfzy.top

Go:   go f()
来源：http://qpm.dashuyun.cn

Ruby: Thread.new { f }
来源：http://qqb.mhx1999.top

C#:   Task.Run(() => F());
来源：http://zss.ydjk.org.cn

[O02] 使用线程池
来源：http://ftq.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ejt.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gus.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://zxq.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://yth.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://vrz.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oti.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tik.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aum.andypj.xyz

[O03] 加锁保护共享数据
来源：http://son.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://hpl.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://rhz.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zow.haohaochexian.top

TS:   // 同 JS
来源：http://twy.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://nez.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tfi.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vjv.sweek.top

C#:   lock (gate) { shared++; }
来源：http://ooq.hnqzz.top

[O04] 定义异步函数并等待
来源：http://tdg.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://lmu.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sns.316326.xyz

JS:   async function f() { await g(); }
来源：http://les.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ctq.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://keh.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://itc.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://nrm.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://ggv.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://xos.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://aqo.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://klb.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://dfs.316326.xyz

TS:   await Promise.all(tasks)
来源：http://ked.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fiw.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://avn.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://yar.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lbw.andypj.xyz

[O06] 使用进程池
来源：http://gqc.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ecz.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gdk.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://xym.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://ztb.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ljv.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hnu.c1oappe.top

Ruby: // fork 块
来源：http://kwe.zhoulong.xyz

C#:   Parallel.For
来源：http://opf.jlsjyb.cn

================================================================================
来源：http://bhv.shzxlz.cn

P. 常用工具函数
来源：http://tob.ydzc1.top

================================================================================
来源：http://ryd.guowangkeji.top

[P01] 生成 UUID
来源：http://wqy.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://oyq.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jhb.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://tuq.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://svl.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://tjd.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://igu.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://nhf.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://rxq.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://kfi.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://irh.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hiy.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qgl.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zni.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://htt.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://apg.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://brk.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://amm.cqqwz.cn

[P03] 生成短随机字符串
来源：http://dad.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mxw.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gvy.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kua.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jwf.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xco.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://azu.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vdj.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hzx.yfazqb.com

[P04] 求长度
来源：http://klq.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ilv.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oju.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uom.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kkv.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://dpx.yuxming.cn

Go:   len(arr);  len(m)
来源：http://qyj.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://ctd.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jqi.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://wfp.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kqo.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pxf.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uep.shanyushiyangtech.top


<!-- 参考信息 -->