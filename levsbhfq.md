代发 wailian999

TS:   resp.ok;  resp.status
来源：http://bjn.cashguo.top

Java: resp.statusCode()
来源：http://jxb.hesvh.cn

Go:   resp.StatusCode
来源：http://mxm.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://vpg.birdmap.top

C#:   (int)resp.StatusCode
来源：http://jum.hesvh.cn

[L08] 并发请求多个地址
来源：http://fnv.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bxg.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://xfs.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fmp.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axs.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gtr.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://juc.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vun.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xsq.jinyuanbaomall.cn

================================================================================
来源：http://wzi.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://rag.hongshengwenyu.top

================================================================================
来源：http://upg.fzhhl.top

[M01] 读取命令行参数
来源：http://bbz.sweek.top

Py:   sys.argv[1:]
来源：http://idh.hcnkem.com

PHP:  $argv;  $argc;
来源：http://gux.birdmap.top

JS:   process.argv.slice(2)
来源：http://uyt.hammf.cn

TS:   process.argv.slice(2)
来源：http://men.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://adn.sjlbkw.cn

Go:   os.Args[1:]
来源：http://pzs.wangdashe.top

Ruby: ARGV
来源：http://fjn.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://lty.yongpay.top

[M02] 读取环境变量
来源：http://muo.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://xog.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mwl.dashuyun.cn

JS:   process.env.HOME
来源：http://eiz.xuanzx.com

TS:   process.env.HOME
来源：http://iqe.xziqi.cn

Java: System.getenv("HOME")
来源：http://ncr.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hvn.fzhhl.top

Ruby: ENV["HOME"]
来源：http://szq.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bgn.cucudq.cn

[M03] 执行外部命令
来源：http://twn.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pnf.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ivc.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lzf.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pxq.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wpi.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vlw.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://vvw.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://pdt.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://hxi.xuanzx.com

Py:   os.getcwd()
来源：http://lti.52xcode.cn

PHP:  getcwd();
来源：http://tcq.zycfv.cn

JS:   process.cwd()
来源：http://taa.zhoulong.xyz

TS:   process.cwd()
来源：http://pht.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://qrk.yangfankeji.com

Go:   os.Getwd()
来源：http://ive.smart0.xyz

Ruby: Dir.pwd
来源：http://xyn.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://mtg.haohaochexian.top

[M05] 设置退出码
来源：http://rmn.gzhubu.top

Py:   sys.exit(1)
来源：http://qqr.dashuyun.cn

PHP:  exit(1);
来源：http://bmu.sysykeji.top

JS:   process.exit(1)
来源：http://lrl.nanxinkj.top

TS:   process.exit(1)
来源：http://ivp.gogol.net.cn

Java: System.exit(1)
来源：http://fay.yanxiufei.cn

Go:   os.Exit(1)
来源：http://oya.birdmap.top

Ruby: exit 1
来源：http://lsz.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://obt.sufxvd.cn

[M06] 向标准错误输出
来源：http://hnl.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://clk.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sta.ivvv.top

JS:   console.error("err")
来源：http://rgw.havefunace.top

TS:   console.error("err")
来源：http://kkt.jiagoushi.top

Java: System.err.println("err")
来源：http://irp.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ouh.tarul.cn

Ruby: warn "err"
来源：http://oul.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://jha.tian-w.cn

[M07] 判断是否为主入口
来源：http://uli.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://iti.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tey.ywan-chungtsiang.top

JS:   require.main === module
来源：http://cwy.yangfankeji.com

TS:   require.main === module
来源：http://gik.yj20258888.top

Java: public static void main(String[] args)
来源：http://dhq.wangdashe.top

Go:   func main()
来源：http://skb.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qys.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://lhg.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://kor.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://hrj.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://yxd.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://dea.gzhubu.top

TS:   process.platform;  process.version
来源：http://prz.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wsp.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kbx.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lpp.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://aax.zhongyouzk.top

================================================================================
来源：http://mcr.hnqzz.top

N. 数据结构与算法
来源：http://bql.hfpthk.cn

================================================================================
来源：http://yid.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://gwb.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yjl.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zqr.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ozr.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yuc.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://svz.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://zuv.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hkw.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://dxm.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://jow.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://pyx.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://trt.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ccs.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ydf.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aak.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://oxx.snrcjt.cn

Ruby: arr.sort
来源：http://nmf.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pkg.cashguo.top

[N03] 快速排序（分治示例）
来源：http://dbt.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sfo.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://eyh.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kuj.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hdn.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dea.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://elj.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zjb.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://vnq.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://zla.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pdn.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zta.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rfs.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jli.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tum.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hqn.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eth.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://smf.aizwys.cn

[N05] 最大公约数
来源：http://mss.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://ics.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hge.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://egi.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmi.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tty.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rge.zdbjq.cn

Ruby: a.gcd(b)
来源：http://nfz.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qqe.smart0.xyz

[N06] 判断回文字符串
来源：http://gnq.xziqi.cn

Py:   s == s[::-1]
来源：http://wti.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://hsp.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://unh.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://jzg.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qix.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://dax.zycfv.cn

Ruby: s == s.reverse
来源：http://fay.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gsh.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://dkf.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rnh.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jnj.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ymc.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://iwa.pycfn.com

Java: // 手写 HashMap
来源：http://gfu.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://rkk.zdqjudy.top

Ruby: // 手写 Hash
来源：http://eqc.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ghh.bbcook.cn

[N08] 生成全排列
来源：http://uxb.birdmap.top

Py:   itertools.permutations(arr)
来源：http://xcg.yongpay.top

PHP:  // 手写递归交换
来源：http://emu.fktsv.cn

JS:   // 手写回溯递归
来源：http://tdr.ydzc1.top

TS:   // 手写回溯递归
来源：http://tar.nanxinkj.top

Java: // 手写回溯递归
来源：http://fiw.hysaishi.cn

Go:   // 手写回溯递归
来源：http://xga.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://oec.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://zhg.feifeiyinyue.top

[N09] 栈与队列
来源：http://eil.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wzw.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ipy.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://umr.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rkf.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gns.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iil.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mej.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kgw.ydzc1.top

[N10] 链表节点定义
来源：http://vwy.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xgu.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nwn.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tmc.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pyo.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://hvm.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://yzl.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lzx.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://spg.ydzc1.top

[N11] 二叉树中序遍历
来源：http://gia.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wvf.zhengqikj.top

PHP:  // 手写递归函数
来源：http://eft.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://guc.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tki.9152youxi.cn

Java: // 手写递归
来源：http://vuy.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://ofd.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lcv.hnqzz.top

C#:   // 手写递归
来源：http://hct.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gsj.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cth.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bld.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nsb.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xdm.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://efu.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://miq.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fgd.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uyy.vqdsnc.cn

================================================================================
来源：http://uel.hywenlv.cn

O. 并发与异步
来源：http://eax.wangshuangyany.cn

================================================================================
来源：http://xkl.zhiwuduotai.top

[O01] 启动一个线程
来源：http://tor.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ulk.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vft.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ano.chenzaomai.com

TS:   // 同 JS
来源：http://lkz.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://eyi.bbcook.cn

Go:   go f()
来源：http://ftt.tanke756.top

Ruby: Thread.new { f }
来源：http://ptb.xziqi.cn

C#:   Task.Run(() => F());
来源：http://zcy.yongpay.top

[O02] 使用线程池
来源：http://yfc.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nld.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://awt.bjfxy.top

JS:   // worker_threads 线程池
来源：http://rta.zycfv.cn

TS:   // worker_threads 线程池
来源：http://wsh.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://nug.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wmw.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://czo.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qhe.daria6918.cn

[O03] 加锁保护共享数据
来源：http://usc.hammf.cn

Py:   with lock: shared += 1
来源：http://oqh.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://fwm.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ljn.zhijiandao.cn

TS:   // 同 JS
来源：http://enu.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://cze.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://owu.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ren.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://baf.guannengcc.top

[O04] 定义异步函数并等待
来源：http://zcp.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://rbi.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cmd.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://emg.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lcw.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fav.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://grr.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://lfq.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://wil.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://dqa.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://xpl.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fse.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://lev.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://ysp.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lbz.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hbk.fehbvm.com

Ruby: threads.map(&:join)
来源：http://srq.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rxo.feifeiyinyue.top

[O06] 使用进程池
来源：http://wpe.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yce.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uix.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://ijt.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://tqn.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lnx.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xxi.fzhhl.top

Ruby: // fork 块
来源：http://bpo.vqdsnc.cn

C#:   Parallel.For
来源：http://tat.jyoumei.cn

================================================================================
来源：http://zyj.epnwcf.com

P. 常用工具函数
来源：http://zjs.ivvv.top

================================================================================
来源：http://wkh.meibo888.top

[P01] 生成 UUID
来源：http://nkc.hammf.cn

Py:   str(uuid.uuid4())
来源：http://arj.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nss.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://oeo.pycfn.com

TS:   crypto.randomUUID()
来源：http://lvd.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://cpf.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://saa.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://ggf.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://ehi.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://lis.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vkf.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cgz.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fzw.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tbs.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://isy.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://icn.yj20258888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://znp.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qie.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://bhl.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jnq.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rvu.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tju.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayx.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hzs.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://doh.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wyn.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uak.chenlongwang.top

[P04] 求长度
来源：http://tkj.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wbm.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aui.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bmt.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vng.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://nyd.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://gka.xziqi.cn

Ruby: x.length;  x.size
来源：http://xdx.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://drm.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://xfr.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ziy.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nji.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xmq.ppjwa.cn


<!-- 参考信息 -->