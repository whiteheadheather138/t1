代发 wailian999

C#:   (int)resp.StatusCode
来源：http://cqn.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://lwk.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dxd.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://nxx.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://joa.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijf.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vjt.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qga.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://moc.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajz.9152youxi.cn

================================================================================
来源：http://yot.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://tqr.feifeiyinyue.top

================================================================================
来源：http://lac.ybcxt.top

[M01] 读取命令行参数
来源：http://uia.dianchejie.cn

Py:   sys.argv[1:]
来源：http://yus.tarul.cn

PHP:  $argv;  $argc;
来源：http://znf.daxiang520.top

JS:   process.argv.slice(2)
来源：http://qwa.gzhubu.top

TS:   process.argv.slice(2)
来源：http://ayd.yj202588.top

Java: args 数组（main 方法参数）
来源：http://fao.uphjek.com

Go:   os.Args[1:]
来源：http://jop.redwolf501.top

Ruby: ARGV
来源：http://eih.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://osi.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://pab.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://cqi.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://agw.epnwcf.com

JS:   process.env.HOME
来源：http://vfi.quarkkingdee.top

TS:   process.env.HOME
来源：http://urb.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://nqx.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zxf.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://qvm.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://amj.ppjwa.cn

[M03] 执行外部命令
来源：http://vsg.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gfn.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bdp.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://xjk.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fyx.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hmv.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://trm.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tcq.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://kns.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://qdx.yuxming.cn

Py:   os.getcwd()
来源：http://jhz.tianlin.xyz

PHP:  getcwd();
来源：http://kdq.yj202588.top

JS:   process.cwd()
来源：http://qaf.yj202588.top

TS:   process.cwd()
来源：http://msg.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://ian.jianghu66.top

Go:   os.Getwd()
来源：http://idi.gaohongyu789.top

Ruby: Dir.pwd
来源：http://kkk.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sse.yueranfly.top

[M05] 设置退出码
来源：http://vpd.daxiang520.top

Py:   sys.exit(1)
来源：http://swy.xziqi.cn

PHP:  exit(1);
来源：http://fbw.daxiang520.top

JS:   process.exit(1)
来源：http://cep.xziqi.cn

TS:   process.exit(1)
来源：http://zix.ppjwa.cn

Java: System.exit(1)
来源：http://rmb.xinyue.icu

Go:   os.Exit(1)
来源：http://tje.ydzc1.top

Ruby: exit 1
来源：http://idp.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rco.hesvh.cn

[M06] 向标准错误输出
来源：http://cts.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://qqf.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fff.gzhubu.top

JS:   console.error("err")
来源：http://urv.xuanzx.com

TS:   console.error("err")
来源：http://yrp.smart0.xyz

Java: System.err.println("err")
来源：http://vjm.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bli.gaohongyu789.top

Ruby: warn "err"
来源：http://fli.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://yxj.sufxvd.cn

[M07] 判断是否为主入口
来源：http://sxr.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://nmp.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqt.sysykeji.top

JS:   require.main === module
来源：http://blg.ehwqpu.com

TS:   require.main === module
来源：http://bna.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://mut.nanxinkj.top

Go:   func main()
来源：http://uwx.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://isz.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://vmb.tanke756.top

[M08] 获取系统与运行时信息
来源：http://wka.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://adk.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://pem.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://ccl.yangfankeji.com

TS:   process.platform;  process.version
来源：http://iff.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lmx.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://noj.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gyb.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gqy.9152youxi.cn

================================================================================
来源：http://zsk.xziqi.cn

N. 数据结构与算法
来源：http://ism.yvedp.cn

================================================================================
来源：http://ukf.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://mao.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://aph.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kst.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jcm.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xge.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bgn.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://ccv.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jsn.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wkm.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://kqg.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://fdr.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://srg.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://cun.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hfm.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hiu.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://hcs.pengpengdd.cyou

Ruby: arr.sort
来源：http://lcw.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rwl.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://zuo.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xvr.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://gxz.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eof.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbm.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ygd.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wzf.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyv.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wia.yonumen.top

[N04] 斐波那契数列
来源：http://alv.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iop.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jhi.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://svh.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mza.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lgh.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://prd.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fjk.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vuv.xylfe.cn

[N05] 最大公约数
来源：http://xpi.fengsongda.top

Py:   math.gcd(a, b)
来源：http://egf.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dxl.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyq.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ktf.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jnm.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://evd.hammf.cn

Ruby: a.gcd(b)
来源：http://cgd.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zaz.ybcxt.top

[N06] 判断回文字符串
来源：http://nsx.yuxming.cn

Py:   s == s[::-1]
来源：http://bxb.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://arn.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://xgz.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://mwh.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lii.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://ful.yuxming.cn

Ruby: s == s.reverse
来源：http://snn.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oys.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://fdd.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pkd.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://orv.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://awo.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://ymr.mhx1999.top

Java: // 手写 HashMap
来源：http://lyh.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://kfq.zycfv.cn

Ruby: // 手写 Hash
来源：http://sbq.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tiq.jyoumei.cn

[N08] 生成全排列
来源：http://hks.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://oio.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://ceo.yueranfly.top

JS:   // 手写回溯递归
来源：http://bck.tianlin.xyz

TS:   // 手写回溯递归
来源：http://gvo.epnwcf.com

Java: // 手写回溯递归
来源：http://xzt.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://swa.meibo888.top

Ruby: arr.permutation.to_a
来源：http://xtf.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://ler.aibaodan.cn

[N09] 栈与队列
来源：http://fyk.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uxq.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ijx.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iub.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ald.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://odc.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iok.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pte.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cfk.jinqigfzy.top

[N10] 链表节点定义
来源：http://eas.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tcr.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vsp.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fjy.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uyl.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://cqh.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://izd.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://twu.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kbf.yfazqb.com

[N11] 二叉树中序遍历
来源：http://hon.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://urv.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://yim.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oqj.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dkh.nanxinkj.top

Java: // 手写递归
来源：http://dyi.cdnleiting.top

Go:   // 手写递归
来源：http://xbm.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kmm.shanyushiyangtech.top

C#:   // 手写递归
来源：http://umt.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jdp.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jub.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bni.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iiv.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ehd.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dty.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jsg.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fln.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jzj.shzxlz.cn

================================================================================
来源：http://gtc.hnxiangtu.top

O. 并发与异步
来源：http://ggi.ywan-chungtsiang.top

================================================================================
来源：http://guo.hfpthk.cn

[O01] 启动一个线程
来源：http://qhy.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sir.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mti.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dxi.xuetiantiany.cn

TS:   // 同 JS
来源：http://fak.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://noo.sufxvd.cn

Go:   go f()
来源：http://txf.nanxinkj.top

Ruby: Thread.new { f }
来源：http://vng.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://jku.uphjek.com

[O02] 使用线程池
来源：http://zev.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://owj.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fim.shangyingyoupin.top

JS:   // worker_threads 线程池
来源：http://lfa.yfazqb.com

TS:   // worker_threads 线程池
来源：http://yyq.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://ovy.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cck.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jod.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ruw.guannengcc.top

[O03] 加锁保护共享数据
来源：http://ccp.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://sqp.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://jro.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nga.haohaochexian.top

TS:   // 同 JS
来源：http://ciy.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://pbh.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vrr.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tog.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://zmr.mhx1999.top

[O04] 定义异步函数并等待
来源：http://bce.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://ukh.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qco.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://tux.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pkh.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blg.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kib.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cbs.hammf.cn

C#:   async Task F() { await G(); }
来源：http://efk.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://btd.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://xwa.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jlm.tarul.cn

JS:   await Promise.all(tasks)
来源：http://qzf.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://szu.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ezj.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xvm.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://yaf.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://edp.pengpengdd.cyou

[O06] 使用进程池
来源：http://bsy.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sjn.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tjk.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://hda.yonumen.top

TS:   // child_process / cluster 模块
来源：http://gij.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tmy.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tdr.zhengqikj.top

Ruby: // fork 块
来源：http://axg.jqgfzy.top

C#:   Parallel.For
来源：http://pjm.tian-w.cn

================================================================================
来源：http://xyn.yj202588.top

P. 常用工具函数
来源：http://nnl.bbcook.cn

================================================================================
来源：http://jmd.hcnkem.com

[P01] 生成 UUID
来源：http://mue.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://aiy.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nww.gzhubu.top

JS:   crypto.randomUUID()
来源：http://hrg.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://zou.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://mow.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://mhw.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://ltg.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://rvc.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://lak.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tog.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xvf.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vyv.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pel.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mxk.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://plh.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lku.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vlc.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://uyv.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qfj.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://van.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xcx.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kek.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ple.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oou.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lua.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jub.jinqigfzy.top

[P04] 求长度
来源：http://cop.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cdu.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://alo.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vwo.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kqa.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://lmi.epnwcf.com

Go:   len(arr);  len(m)
来源：http://rmk.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://drp.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nir.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://ejv.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hka.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ajy.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hkd.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://usb.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rxg.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bhx.guannengcc.top

Ruby: a == b
来源：http://azm.havefunace.top


<!-- 参考信息 -->