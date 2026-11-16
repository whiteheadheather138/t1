代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xsh.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uzk.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uic.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gyh.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bcn.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rqy.pengpengdd.cyou

================================================================================
来源：http://eym.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://tdx.guannengcc.top

================================================================================
来源：http://fiw.ehwqpu.com

[M01] 读取命令行参数
来源：http://xim.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://kgm.ydzc1.top

PHP:  $argv;  $argc;
来源：http://wwj.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://qiz.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://jkk.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://dld.jiagoushi.top

Go:   os.Args[1:]
来源：http://bab.aizwys.cn

Ruby: ARGV
来源：http://omt.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://rle.tianlin.xyz

[M02] 读取环境变量
来源：http://xwl.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://vhh.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zwi.hywenlv.cn

JS:   process.env.HOME
来源：http://nak.quarkkingdee.top

TS:   process.env.HOME
来源：http://arw.guannengcc.top

Java: System.getenv("HOME")
来源：http://bqb.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zpv.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://fld.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ynt.xylfe.cn

[M03] 执行外部命令
来源：http://xgf.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fld.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mlv.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nwh.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qpx.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jtn.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://tvn.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://trn.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://svj.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://lpn.tanke756.top

Py:   os.getcwd()
来源：http://dho.9152youxi.cn

PHP:  getcwd();
来源：http://gpn.tarul.cn

JS:   process.cwd()
来源：http://buy.sweek.top

TS:   process.cwd()
来源：http://kpg.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://cun.zhiwuduotai.top

Go:   os.Getwd()
来源：http://cwk.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://woc.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://ddz.jinqigufen.top

[M05] 设置退出码
来源：http://eil.redwolf501.top

Py:   sys.exit(1)
来源：http://jhc.gzhubu.top

PHP:  exit(1);
来源：http://bgg.uphjek.com

JS:   process.exit(1)
来源：http://pxd.52xcode.cn

TS:   process.exit(1)
来源：http://ugs.nanxuanxn.top

Java: System.exit(1)
来源：http://pty.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://lor.ehwqpu.com

Ruby: exit 1
来源：http://mqa.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vjd.tanke756.top

[M06] 向标准错误输出
来源：http://pkt.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://jsa.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://gnh.havefunace.top

JS:   console.error("err")
来源：http://mbs.hnqzz.top

TS:   console.error("err")
来源：http://vpq.cashguo.top

Java: System.err.println("err")
来源：http://vkg.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ioo.gaohongyu789.top

Ruby: warn "err"
来源：http://imd.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://kvd.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://roe.cheryme.top

Py:   if __name__ == "__main__":
来源：http://gox.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nam.svipenyu.cn

JS:   require.main === module
来源：http://mvz.dianchejie.cn

TS:   require.main === module
来源：http://nxx.havefunace.top

Java: public static void main(String[] args)
来源：http://aqs.jiagoushi.top

Go:   func main()
来源：http://xjg.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hvp.guannengcc.top

C#:   static void Main(string[] args)
来源：http://qjj.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://xed.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://dra.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://wjs.sysykeji.top

JS:   process.platform;  process.version
来源：http://dmi.tian-w.cn

TS:   process.platform;  process.version
来源：http://ctp.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qey.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dwj.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xcm.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zbk.pengpengdd.cyou

================================================================================
来源：http://zrj.pengpengdd.cyou

N. 数据结构与算法
来源：http://qbm.xylfe.cn

================================================================================
来源：http://xvm.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://ruj.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://zmg.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gkn.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zwr.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ncn.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cpv.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://ooa.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ssv.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://qol.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://ziz.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ukf.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eof.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cqa.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zzw.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zpe.vehdjk.com

Go:   slices.Sort(arr)
来源：http://ebd.sysykeji.top

Ruby: arr.sort
来源：http://vau.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fry.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://xsc.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://znr.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://egm.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zzw.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jce.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baf.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jqn.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dqy.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://urh.shuidangran.top

[N04] 斐波那契数列
来源：http://fip.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jhl.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wpo.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rio.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mel.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dlw.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nvu.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://klz.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tee.9152youxi.cn

[N05] 最大公约数
来源：http://apa.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://qra.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oqy.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nsp.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://epy.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://slw.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xee.fehbvm.com

Ruby: a.gcd(b)
来源：http://rln.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://llw.andypj.xyz

[N06] 判断回文字符串
来源：http://nls.redwolf501.top

Py:   s == s[::-1]
来源：http://cho.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://nyt.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://cxp.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://crp.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lvu.sysykeji.top

Go:   // 双指针从两端比较
来源：http://cpy.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://yzw.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://khw.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://qlf.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ccx.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dvm.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ivo.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://cnb.tarul.cn

Java: // 手写 HashMap
来源：http://quc.fktsv.cn

Go:   // 手写 map[int]int
来源：http://vcb.yonumen.top

Ruby: // 手写 Hash
来源：http://wag.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://ehj.yueranfly.top

[N08] 生成全排列
来源：http://pbn.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://bxj.yuxming.cn

PHP:  // 手写递归交换
来源：http://qac.hysaishi.cn

JS:   // 手写回溯递归
来源：http://sor.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://etl.nwbrower.top

Java: // 手写回溯递归
来源：http://voy.hysaishi.cn

Go:   // 手写回溯递归
来源：http://xrw.yonumen.top

Ruby: arr.permutation.to_a
来源：http://bbz.guannengcc.top

C#:   // 手写回溯递归
来源：http://ahb.yj202588.top

[N09] 栈与队列
来源：http://irq.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lxt.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qbx.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fhr.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pdy.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nvm.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://smo.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://whk.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://adi.sysykeji.top

[N10] 链表节点定义
来源：http://dwj.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nrq.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qpg.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qde.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gsp.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://wiv.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://utb.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vkj.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ffp.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://obk.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ovf.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://axf.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nsw.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnt.guannengcc.top

Java: // 手写递归
来源：http://gkq.xylfe.cn

Go:   // 手写递归
来源：http://rcx.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hrg.dianchejie.cn

C#:   // 手写递归
来源：http://zoq.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://htt.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tbs.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jwi.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dzk.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qjv.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iza.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yde.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://saa.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hpd.zhijiandao.cn

================================================================================
来源：http://crx.tian-w.cn

O. 并发与异步
来源：http://fnx.epnwcf.com

================================================================================
来源：http://opp.tanke756.top

[O01] 启动一个线程
来源：http://ygo.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hhv.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cpj.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aei.zhixingplan.top

TS:   // 同 JS
来源：http://jpa.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://wng.yj20258888.top

Go:   go f()
来源：http://vex.cdnleiting.top

Ruby: Thread.new { f }
来源：http://cix.mhx1999.top

C#:   Task.Run(() => F());
来源：http://tut.bbcook.cn

[O02] 使用线程池
来源：http://lfo.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dkn.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ckz.shuidangran.top

JS:   // worker_threads 线程池
来源：http://xgb.guannengcc.top

TS:   // worker_threads 线程池
来源：http://iga.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rvr.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://own.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://keh.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rrn.uphjek.com

[O03] 加锁保护共享数据
来源：http://eyq.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://eve.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://hwo.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nyv.dianchejie.cn

TS:   // 同 JS
来源：http://lnm.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://buk.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hmq.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mkd.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://egj.andypj.xyz

[O04] 定义异步函数并等待
来源：http://uou.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://yhb.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vqx.xinyue.icu

JS:   async function f() { await g(); }
来源：http://tjz.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mew.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yew.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://duj.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://kkk.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://jwn.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://ztl.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://upq.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sab.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://nmn.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://npo.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yep.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ffg.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://bsp.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://cec.jqgfzy.top

[O06] 使用进程池
来源：http://tde.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ssh.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cih.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://jom.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://sjw.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nzs.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pos.hammf.cn

Ruby: // fork 块
来源：http://tak.zdbjq.cn

C#:   Parallel.For
来源：http://rde.xziqi.cn

================================================================================
来源：http://fub.epnwcf.com

P. 常用工具函数
来源：http://dpj.zhiwuduotai.top

================================================================================
来源：http://act.chenjidiqi.icu

[P01] 生成 UUID
来源：http://fpa.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://wke.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://euo.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://ifm.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://wev.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://gje.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://ngr.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://ubw.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://ajf.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://rdo.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hor.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lhj.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gbx.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://twg.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lgu.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vrk.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dkx.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kkl.aizwys.cn

[P03] 生成短随机字符串
来源：http://rpw.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sob.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://edk.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ptf.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nwo.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ija.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vte.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wiw.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://omv.sysykeji.top

[P04] 求长度
来源：http://icr.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mvr.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axo.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vfp.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rfm.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://pjb.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://naw.yuxming.cn

Ruby: x.length;  x.size
来源：http://uel.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iep.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://uby.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dla.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bcr.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kjf.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://slh.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uev.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://uyp.meibo888.top

Ruby: a == b
来源：http://ltv.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sxw.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aiv.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jqj.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://akh.haohaochexian.top


<!-- 参考信息 -->