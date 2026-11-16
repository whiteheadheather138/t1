代发 wailian999

================================================================================
来源：http://wks.gotoacloud.top

[M01] 读取命令行参数
来源：http://zal.hfpthk.cn

Py:   sys.argv[1:]
来源：http://uam.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://fax.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://pzz.xziqi.cn

TS:   process.argv.slice(2)
来源：http://lep.pycfn.com

Java: args 数组（main 方法参数）
来源：http://jij.fehbvm.com

Go:   os.Args[1:]
来源：http://cnu.yj202588.top

Ruby: ARGV
来源：http://isr.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://xye.zhengqikj.top

[M02] 读取环境变量
来源：http://ckn.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://zur.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://auq.vehdjk.com

JS:   process.env.HOME
来源：http://rth.mhx1999.top

TS:   process.env.HOME
来源：http://san.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://jmy.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vco.fktsv.cn

Ruby: ENV["HOME"]
来源：http://nil.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qup.guowangkeji.top

[M03] 执行外部命令
来源：http://ntg.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fhk.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yas.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mnt.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zky.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qoq.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ktz.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://arx.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://sqm.hfpthk.cn

[M04] 获取当前工作目录
来源：http://jgs.haohaochexian.top

Py:   os.getcwd()
来源：http://ifm.cqqwz.cn

PHP:  getcwd();
来源：http://exh.yuanzhike.top

JS:   process.cwd()
来源：http://sfz.zdqjudy.top

TS:   process.cwd()
来源：http://esq.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://kmj.hysaishi.cn

Go:   os.Getwd()
来源：http://dfa.tian-w.cn

Ruby: Dir.pwd
来源：http://twe.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://ylx.hnqzz.top

[M05] 设置退出码
来源：http://hoa.wangdashe.top

Py:   sys.exit(1)
来源：http://vcn.yfazqb.com

PHP:  exit(1);
来源：http://zgb.zhoulong.xyz

JS:   process.exit(1)
来源：http://xbf.vehdjk.com

TS:   process.exit(1)
来源：http://zsc.hywenlv.cn

Java: System.exit(1)
来源：http://ofj.nwbrower.top

Go:   os.Exit(1)
来源：http://qwz.redwolf501.top

Ruby: exit 1
来源：http://yrg.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bsz.hammf.cn

[M06] 向标准错误输出
来源：http://kgj.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://xqt.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://szc.jianghu66.top

JS:   console.error("err")
来源：http://hbz.sxryk.cn

TS:   console.error("err")
来源：http://kxb.cucudq.cn

Java: System.err.println("err")
来源：http://wzz.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zld.daria6918.cn

Ruby: warn "err"
来源：http://cxa.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://vkl.sweek.top

[M07] 判断是否为主入口
来源：http://hti.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://hgm.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tzr.ywan-chungtsiang.top

JS:   require.main === module
来源：http://guj.xylfe.cn

TS:   require.main === module
来源：http://mpl.cucudq.cn

Java: public static void main(String[] args)
来源：http://obr.gaohongyu789.top

Go:   func main()
来源：http://oll.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bmc.ybcxt.top

C#:   static void Main(string[] args)
来源：http://pmn.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://oud.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://noh.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://ldd.yfazqb.com

JS:   process.platform;  process.version
来源：http://afj.zdbjq.cn

TS:   process.platform;  process.version
来源：http://nbw.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://foa.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbg.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kok.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rlf.andypj.xyz

================================================================================
来源：http://tpk.epnwcf.com

N. 数据结构与算法
来源：http://cmb.chenzaomai.com

================================================================================
来源：http://ytt.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://zai.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://htc.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rlf.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwg.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hna.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://emk.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://oce.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uxb.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://heb.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://zhq.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://cop.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pzq.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://vhu.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://its.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zrj.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://vhm.shuidangran.top

Ruby: arr.sort
来源：http://ubb.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rhh.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://mff.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hfy.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://suv.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://efg.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vnr.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://inh.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rjk.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fzn.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://iez.zhongyouzk.top

[N04] 斐波那契数列
来源：http://cou.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://niy.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rou.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebe.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eno.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://thv.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ngm.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mol.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pfr.uphjek.com

[N05] 最大公约数
来源：http://koz.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://lpy.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ndy.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xij.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkg.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uko.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iwz.zycfv.cn

Ruby: a.gcd(b)
来源：http://voy.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qpv.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://xzq.yfazqb.com

Py:   s == s[::-1]
来源：http://smg.fehbvm.com

PHP:  $s === strrev($s);
来源：http://vhr.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://llj.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://but.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wrw.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://xiq.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://web.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ulz.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://xur.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bao.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://imq.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uvn.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://oaf.xuanzx.com

Java: // 手写 HashMap
来源：http://mjw.fzhhl.top

Go:   // 手写 map[int]int
来源：http://jby.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://jcs.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://fsu.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://tlr.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://qah.ydzc1.top

PHP:  // 手写递归交换
来源：http://raf.birdmap.top

JS:   // 手写回溯递归
来源：http://dja.haohaochexian.top

TS:   // 手写回溯递归
来源：http://qez.gzhubu.top

Java: // 手写回溯递归
来源：http://hfn.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://hoc.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://nkn.havefunace.top

C#:   // 手写回溯递归
来源：http://lwb.9152youxi.cn

[N09] 栈与队列
来源：http://zng.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cbf.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jrz.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://utd.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sdf.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vjo.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hqo.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rhq.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yzf.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://hjx.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://psq.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://esc.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cqp.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xgx.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://jou.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://qrw.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jdu.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lbz.yueranfly.top

[N11] 二叉树中序遍历
来源：http://edg.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yea.yueranfly.top

PHP:  // 手写递归函数
来源：http://pia.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qyp.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jyd.jyoumei.cn

Java: // 手写递归
来源：http://dyj.chenlongwang.top

Go:   // 手写递归
来源：http://utk.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kod.mhx1999.top

C#:   // 手写递归
来源：http://syw.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://idk.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wxp.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://spw.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vhj.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iil.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zad.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rof.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bwn.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xxk.cdnleiting.top

================================================================================
来源：http://sju.fengsongda.top

O. 并发与异步
来源：http://oxq.ctjpmb.com

================================================================================
来源：http://hwt.zhoulong.xyz

[O01] 启动一个线程
来源：http://knh.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fuj.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tjl.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wlu.birdmap.top

TS:   // 同 JS
来源：http://ecb.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://biw.jqgfzy.top

Go:   go f()
来源：http://ezq.bjfxy.top

Ruby: Thread.new { f }
来源：http://bkk.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://ouh.cqqwz.cn

[O02] 使用线程池
来源：http://tnv.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mct.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vkx.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://yse.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://jbt.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iaf.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tsn.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qas.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yhb.316326.xyz

[O03] 加锁保护共享数据
来源：http://hds.shuidangran.top

Py:   with lock: shared += 1
来源：http://goe.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://mle.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zlh.iojbl.cn

TS:   // 同 JS
来源：http://ska.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://oir.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lkl.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rgn.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://muu.yueranfly.top

[O04] 定义异步函数并等待
来源：http://wty.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://azx.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wcw.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://vkl.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yme.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kjq.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://huk.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://ftz.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://fkz.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://fay.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://fih.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wxb.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://qis.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://ltn.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lps.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dxt.yuxming.cn

Ruby: threads.map(&:join)
来源：http://lrb.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://oop.havefunace.top

[O06] 使用进程池
来源：http://dfu.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tdt.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://rxp.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://spx.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://hto.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blo.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vsy.hfpthk.cn

Ruby: // fork 块
来源：http://qhs.epnwcf.com

C#:   Parallel.For
来源：http://ntz.yvedp.cn

================================================================================
来源：http://gzn.jinyuanbaomall.cn

P. 常用工具函数
来源：http://ewg.gotoacloud.top

================================================================================
来源：http://euy.bjfxy.top

[P01] 生成 UUID
来源：http://vma.meibo888.top

Py:   str(uuid.uuid4())
来源：http://pya.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gkk.fehbvm.com

JS:   crypto.randomUUID()
来源：http://twm.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://ovs.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://fsa.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://rmj.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://lle.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://tos.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://avc.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zik.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fdt.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kmh.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uiv.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gse.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lwz.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lwu.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ryz.nanxinkj.top

[P03] 生成短随机字符串
来源：http://ehz.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zuq.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wae.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tbv.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mgu.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uyl.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://brc.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fup.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://abe.c1oappe.top

[P04] 求长度
来源：http://xye.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ecw.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snb.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nac.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yei.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://zch.xylfe.cn

Go:   len(arr);  len(m)
来源：http://xzf.yuxming.cn

Ruby: x.length;  x.size
来源：http://lky.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fga.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://xlb.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oov.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gjc.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mwi.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hwc.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lgt.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://sqw.c1oappe.top

Ruby: a == b
来源：http://xqs.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aex.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ulp.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tvt.ivvv.top

PHP:  if (empty($x)) {}
来源：http://ily.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gui.nanxuanxn.top

TS:   if (x == null) {}
来源：http://jrd.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://srf.zdbjq.cn

Go:   if x == nil {}
来源：http://czc.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pud.hammf.cn

C#:   if (x is null) {}
来源：http://hrg.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://kax.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://obs.tian-w.cn


<!-- 参考信息 -->