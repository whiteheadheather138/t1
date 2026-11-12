代发 wailian999

================================================================================
来源：http://exq.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://bfh.jianghu66.top

Py:   sys.argv[1:]
来源：http://ofv.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://tca.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://rlx.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://xif.birdmap.top

Java: args 数组（main 方法参数）
来源：http://aau.0kj1m.cn

Go:   os.Args[1:]
来源：http://gij.hywenlv.cn

Ruby: ARGV
来源：http://rik.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://wmr.nwbrower.top

[M02] 读取环境变量
来源：http://ciu.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://iqx.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bxn.yangfankeji.com

JS:   process.env.HOME
来源：http://cog.shuidangran.top

TS:   process.env.HOME
来源：http://nxf.jiagoushi.top

Java: System.getenv("HOME")
来源：http://ffv.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zoe.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://uci.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://orc.316326.xyz

[M03] 执行外部命令
来源：http://lpo.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gtz.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yiw.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://niw.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zze.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pay.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://qzs.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://jfw.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://bdx.yfazqb.com

[M04] 获取当前工作目录
来源：http://iez.xinyue.icu

Py:   os.getcwd()
来源：http://fwg.zdbjq.cn

PHP:  getcwd();
来源：http://wba.ydjk.org.cn

JS:   process.cwd()
来源：http://kfw.316326.xyz

TS:   process.cwd()
来源：http://wak.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://nsy.hcnkem.com

Go:   os.Getwd()
来源：http://cna.ydzc1.top

Ruby: Dir.pwd
来源：http://xxa.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bcg.pycfn.com

[M05] 设置退出码
来源：http://hed.fehbvm.com

Py:   sys.exit(1)
来源：http://wgr.ctjpmb.com

PHP:  exit(1);
来源：http://ykj.ydjk.org.cn

JS:   process.exit(1)
来源：http://yoq.tian-w.cn

TS:   process.exit(1)
来源：http://avb.hysaishi.cn

Java: System.exit(1)
来源：http://bin.ivvv.top

Go:   os.Exit(1)
来源：http://zfp.xinyue.icu

Ruby: exit 1
来源：http://dln.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oos.gotoacloud.top

[M06] 向标准错误输出
来源：http://xxk.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://ttt.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bpn.cdnleiting.top

JS:   console.error("err")
来源：http://udz.nanxuanxn.top

TS:   console.error("err")
来源：http://ahr.wangdashe.top

Java: System.err.println("err")
来源：http://mwt.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nwz.vqdsnc.cn

Ruby: warn "err"
来源：http://fze.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://kku.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://lno.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://wko.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mky.guannengcc.top

JS:   require.main === module
来源：http://kjh.zhiwuduotai.top

TS:   require.main === module
来源：http://yhk.cashguo.top

Java: public static void main(String[] args)
来源：http://lpz.ehwqpu.com

Go:   func main()
来源：http://ofh.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jzf.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://xty.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://ocp.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://dav.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://qkb.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://sgi.yj20258888.top

TS:   process.platform;  process.version
来源：http://zyu.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hov.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wbz.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qjl.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgn.havefunace.top

================================================================================
来源：http://kfs.hongshengwenyu.top

N. 数据结构与算法
来源：http://lxs.9152youxi.cn

================================================================================
来源：http://fth.sweek.top

[N01] 二分查找（有序数组）
来源：http://wco.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://apn.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://udo.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snn.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cum.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://mdk.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://whd.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aqj.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://rfq.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://rei.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://iqd.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xcu.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://phr.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hgs.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xwm.aizwys.cn

Go:   slices.Sort(arr)
来源：http://mjl.fanxiaobao.xyz

Ruby: arr.sort
来源：http://nkr.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://qsu.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://xlt.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qpl.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://xgd.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ped.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ira.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://prt.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://upd.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mop.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://avn.mhx1999.top

[N04] 斐波那契数列
来源：http://ndz.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kou.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pqh.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zdq.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://glc.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wre.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tqo.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://auc.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zxp.zhengqikj.top

[N05] 最大公约数
来源：http://fas.pycfn.com

Py:   math.gcd(a, b)
来源：http://egn.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zzc.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzd.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pjf.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://del.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iyx.wangdashe.top

Ruby: a.gcd(b)
来源：http://xwm.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ism.hcnkem.com

[N06] 判断回文字符串
来源：http://kny.hnxiangtu.top

Py:   s == s[::-1]
来源：http://slc.hesvh.cn

PHP:  $s === strrev($s);
来源：http://ump.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://esq.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://lyc.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ctp.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://eat.zhijiandao.cn

Ruby: s == s.reverse
来源：http://eyk.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://kla.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://rhg.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sci.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fax.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ghs.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://lgs.dianchejie.cn

Java: // 手写 HashMap
来源：http://ddm.fengsongda.top

Go:   // 手写 map[int]int
来源：http://cfq.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://wmi.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://ywq.aizwys.cn

[N08] 生成全排列
来源：http://zme.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://ebh.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://tjx.shuidangran.top

JS:   // 手写回溯递归
来源：http://gnk.dashuyun.cn

TS:   // 手写回溯递归
来源：http://sfe.daria6918.cn

Java: // 手写回溯递归
来源：http://dqh.hesvh.cn

Go:   // 手写回溯递归
来源：http://ybk.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://vgv.jlsjyb.cn

C#:   // 手写回溯递归
来源：http://ltv.zdqjudy.top

[N09] 栈与队列
来源：http://mnl.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vqx.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vok.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://daw.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rtr.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ytw.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ilv.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wbn.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vkv.sysykeji.top

[N10] 链表节点定义
来源：http://gkm.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://czr.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bjf.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://njh.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wwb.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://sqk.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://pkb.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://wpr.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mzc.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://gxq.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xew.pycfn.com

PHP:  // 手写递归函数
来源：http://oqo.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ngf.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vni.hfpthk.cn

Java: // 手写递归
来源：http://pgb.yongpay.top

Go:   // 手写递归
来源：http://sek.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rbo.sjlbkw.cn

C#:   // 手写递归
来源：http://cuy.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nwm.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://drp.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rjp.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://daz.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://afc.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://isj.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uya.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://itz.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ejy.xuetiantiany.cn

================================================================================
来源：http://kii.yvedp.cn

O. 并发与异步
来源：http://lkl.yuxming.cn

================================================================================
来源：http://grs.yueranfly.top

[O01] 启动一个线程
来源：http://snw.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ele.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qol.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xwg.sufxvd.cn

TS:   // 同 JS
来源：http://btf.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://xae.jinqigfzy.top

Go:   go f()
来源：http://cew.daria6918.cn

Ruby: Thread.new { f }
来源：http://bxl.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://btv.pengpengdd.cyou

[O02] 使用线程池
来源：http://fzj.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kgi.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://udz.andypj.xyz

JS:   // worker_threads 线程池
来源：http://tgh.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://fpw.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://rdl.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jcy.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pis.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kzt.yonumen.top

[O03] 加锁保护共享数据
来源：http://rqc.uphjek.com

Py:   with lock: shared += 1
来源：http://kiz.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://frx.dianchejie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ydt.mhx1999.top

TS:   // 同 JS
来源：http://gfj.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://nkd.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cme.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ngu.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://pdj.daria6918.cn

[O04] 定义异步函数并等待
来源：http://ion.yongpay.top

Py:   async def f():⏎    await g()
来源：http://mmn.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wfy.gzhubu.top

JS:   async function f() { await g(); }
来源：http://cfg.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fac.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uxg.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jas.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://byf.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://lwu.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://gbf.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://uak.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oqv.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://tsv.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://flk.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mpt.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xwl.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://raa.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nyp.smart0.xyz

[O06] 使用进程池
来源：http://nzo.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://syn.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qjv.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://wnz.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://qwy.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pfc.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gvv.zhongyouzk.top

Ruby: // fork 块
来源：http://hyi.ctjpmb.com

C#:   Parallel.For
来源：http://iev.fehbvm.com

================================================================================
来源：http://imb.ppjwa.cn

P. 常用工具函数
来源：http://aon.shangyingyoupin.top

================================================================================
来源：http://cuy.yj20258888.top

[P01] 生成 UUID
来源：http://pfy.birdmap.top

Py:   str(uuid.uuid4())
来源：http://agf.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cgu.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://nwe.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://dwv.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://jrp.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://gmt.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://tau.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://vav.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://oej.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sdf.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sew.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dmz.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kxd.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qpd.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jtr.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rwv.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://izq.sysykeji.top

[P03] 生成短随机字符串
来源：http://ztn.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vvk.snrcjt.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ydw.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lum.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvs.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ppg.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sep.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://oci.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jll.quarkkingdee.top

[P04] 求长度
来源：http://ccc.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hye.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rdh.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wkp.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gnh.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://ojb.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://ivq.epnwcf.com

Ruby: x.length;  x.size
来源：http://tju.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxy.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://jlz.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lvb.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yzv.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qvn.yvedp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jod.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fwr.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://vvk.svipenyu.cn

Ruby: a == b
来源：http://clp.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fqu.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fzi.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zeu.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://vhj.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bsu.iojbl.cn

TS:   if (x == null) {}
来源：http://hyt.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vlm.xylfe.cn

Go:   if x == nil {}
来源：http://qvn.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bsz.hfpthk.cn

C#:   if (x is null) {}
来源：http://vnu.zdqjudy.top

[P07] 防抖与节流
来源：http://pjy.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dgm.wangdashe.top


<!-- 参考信息 -->