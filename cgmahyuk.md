代发 wailian999

JS:   process.argv.slice(2)
来源：http://izj.yvedp.cn

TS:   process.argv.slice(2)
来源：http://xvp.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://aqe.chenlongwang.top

Go:   os.Args[1:]
来源：http://udo.jqgfzy.top

Ruby: ARGV
来源：http://ajg.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://kzz.tarul.cn

[M02] 读取环境变量
来源：http://rci.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://qtf.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sau.smart0.xyz

JS:   process.env.HOME
来源：http://tjx.tanke756.top

TS:   process.env.HOME
来源：http://kbt.zhixingplan.top

Java: System.getenv("HOME")
来源：http://htk.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hkb.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://dom.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vsn.quarkkingdee.top

[M03] 执行外部命令
来源：http://hnq.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nun.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nxm.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hpv.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://coh.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jqj.fengsongda.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fxr.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ubv.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://hce.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://ytj.daria6918.cn

Py:   os.getcwd()
来源：http://hfa.dashuyun.cn

PHP:  getcwd();
来源：http://xgx.dashuyun.cn

JS:   process.cwd()
来源：http://ayy.gogol.net.cn

TS:   process.cwd()
来源：http://hfi.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://adv.sjlbkw.cn

Go:   os.Getwd()
来源：http://nql.yj202588.top

Ruby: Dir.pwd
来源：http://mdp.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uei.nanxuanxn.top

[M05] 设置退出码
来源：http://wju.hnxiangtu.top

Py:   sys.exit(1)
来源：http://gcv.sweek.top

PHP:  exit(1);
来源：http://zno.nanxuanxn.top

JS:   process.exit(1)
来源：http://hnd.tianlin.xyz

TS:   process.exit(1)
来源：http://fpd.gaohongyu789.top

Java: System.exit(1)
来源：http://oms.svipenyu.cn

Go:   os.Exit(1)
来源：http://ypt.mhx1999.top

Ruby: exit 1
来源：http://msq.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vdl.hcnkem.com

[M06] 向标准错误输出
来源：http://buv.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://mgi.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eon.hesvh.cn

JS:   console.error("err")
来源：http://pue.sxryk.cn

TS:   console.error("err")
来源：http://wfh.bbcook.cn

Java: System.err.println("err")
来源：http://stm.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vfe.316326.xyz

Ruby: warn "err"
来源：http://yug.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://cik.guowangkeji.top

[M07] 判断是否为主入口
来源：http://sel.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://asw.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qra.gotoacloud.top

JS:   require.main === module
来源：http://wny.gzhubu.top

TS:   require.main === module
来源：http://lxa.chenzaomai.com

Java: public static void main(String[] args)
来源：http://zjh.52xcode.cn

Go:   func main()
来源：http://piq.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ifu.hnqzz.top

C#:   static void Main(string[] args)
来源：http://wpw.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://pdr.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://ith.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://qll.tarul.cn

JS:   process.platform;  process.version
来源：http://noq.uphjek.com

TS:   process.platform;  process.version
来源：http://meu.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qrp.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hgp.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bdw.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wdo.guannengcc.top

================================================================================
来源：http://arp.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://ime.epnwcf.com

================================================================================
来源：http://zla.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://xgf.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://plw.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zjg.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idf.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qdn.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://umu.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://cvh.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nxh.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://zqu.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://vsp.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zei.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vof.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rsr.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uwm.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gmn.ybcxt.top

Go:   slices.Sort(arr)
来源：http://xka.ehwqpu.com

Ruby: arr.sort
来源：http://qqr.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tkl.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://cvg.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bek.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://qux.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eed.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tqk.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qus.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mbo.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://npl.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hyb.zhongyouzk.top

[N04] 斐波那契数列
来源：http://fgd.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aug.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gaw.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://quy.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qvb.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ukf.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://poh.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lbh.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qou.andypj.xyz

[N05] 最大公约数
来源：http://nst.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://nuo.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bvi.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zch.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nmh.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xtz.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://chq.epnwcf.com

Ruby: a.gcd(b)
来源：http://asb.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fnf.guannengcc.top

[N06] 判断回文字符串
来源：http://ypd.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://cuc.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://ohb.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://lvu.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://mwz.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cbf.nwbrower.top

Go:   // 双指针从两端比较
来源：http://wxc.316326.xyz

Ruby: s == s.reverse
来源：http://muz.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jxa.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://bai.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lnj.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xag.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cbg.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://eqh.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://don.daxiang520.top

Go:   // 手写 map[int]int
来源：http://tmw.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://xek.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://qdu.vehdjk.com

[N08] 生成全排列
来源：http://qxj.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://mbz.nanxinkj.top

PHP:  // 手写递归交换
来源：http://xie.hfpthk.cn

JS:   // 手写回溯递归
来源：http://hhl.vehdjk.com

TS:   // 手写回溯递归
来源：http://agi.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://hrf.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://vse.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://gvp.jyoumei.cn

C#:   // 手写回溯递归
来源：http://duk.fzhhl.top

[N09] 栈与队列
来源：http://dvv.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://don.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pdc.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ohn.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pyu.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hxv.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qde.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kqi.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lfg.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://lwv.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mpq.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://prm.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lec.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xug.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://xky.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://iow.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yeo.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vwf.birdmap.top

[N11] 二叉树中序遍历
来源：http://yev.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aod.tanke756.top

PHP:  // 手写递归函数
来源：http://qns.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mwt.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hvq.iojbl.cn

Java: // 手写递归
来源：http://inm.sufxvd.cn

Go:   // 手写递归
来源：http://oav.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xrb.zdbjq.cn

C#:   // 手写递归
来源：http://gmr.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vfz.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dmw.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wmy.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kyh.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhr.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wgp.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xcf.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://exw.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kay.uphjek.com

================================================================================
来源：http://czq.daria6918.cn

O. 并发与异步
来源：http://tyk.vehdjk.com

================================================================================
来源：http://jlt.xuanzx.com

[O01] 启动一个线程
来源：http://vul.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jaa.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ygr.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pyq.jiagoushi.top

TS:   // 同 JS
来源：http://vby.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://ise.shanyushiyangkeji.top

Go:   go f()
来源：http://isf.meibo888.top

Ruby: Thread.new { f }
来源：http://zhk.wangdashe.top

C#:   Task.Run(() => F());
来源：http://emk.wangdashe.top

[O02] 使用线程池
来源：http://lyj.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cmz.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cxv.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://pfq.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://eto.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hiv.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bno.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://taf.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kkr.ivvv.top

[O03] 加锁保护共享数据
来源：http://lgz.yuxming.cn

Py:   with lock: shared += 1
来源：http://rkg.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://muc.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dvb.gzhubu.top

TS:   // 同 JS
来源：http://tmp.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://lgy.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bfr.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sho.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://xmk.vehdjk.com

[O04] 定义异步函数并等待
来源：http://pwi.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://ouk.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vik.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://rpt.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xmp.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gkb.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mpf.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qju.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://xnw.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://bns.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://gqf.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qcy.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://drg.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://bje.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://toa.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://adw.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://car.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://yac.zycfv.cn

[O06] 使用进程池
来源：http://obx.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wyy.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jop.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://umj.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://fvk.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nwj.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ozf.bbcook.cn

Ruby: // fork 块
来源：http://nbc.shangyingyoupin.top

C#:   Parallel.For
来源：http://bgr.zhijiandao.cn

================================================================================
来源：http://rrk.mhx1999.top

P. 常用工具函数
来源：http://lsv.zhongyouzk.top

================================================================================
来源：http://uvn.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://liq.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://ytj.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://atv.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://nwu.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://tsf.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://dcs.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://glo.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://ivg.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://axh.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://ybl.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://igj.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iuj.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xez.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ask.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rdj.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gfs.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ery.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zrd.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://zmf.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zdc.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://byg.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://slb.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bbm.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://icw.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zaz.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rlq.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wbc.pycfn.com

[P04] 求长度
来源：http://mll.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lyc.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://biv.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hsb.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tvk.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://stu.cheryme.top

Go:   len(arr);  len(m)
来源：http://njb.sufxvd.cn

Ruby: x.length;  x.size
来源：http://ewv.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ukp.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://qle.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pvc.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fqx.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ulw.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pns.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iuq.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aka.9152youxi.cn

Ruby: a == b
来源：http://nxl.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ojw.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kor.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dje.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://rlb.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fon.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://ucx.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lio.gogol.net.cn

Go:   if x == nil {}
来源：http://apf.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kic.zhijiandao.cn

C#:   if (x is null) {}
来源：http://mdt.hywenlv.cn

[P07] 防抖与节流
来源：http://hqd.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pum.xylfe.cn

PHP:  // 手写时间戳比较
来源：http://gha.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rai.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffp.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://whs.tian-w.cn


<!-- 参考信息 -->