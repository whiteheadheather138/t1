代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ecw.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bpz.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qgk.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://afh.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ucu.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jmc.xziqi.cn

================================================================================
来源：http://rzj.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://xuw.52xcode.cn

================================================================================
来源：http://bhn.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://eav.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://gqp.daria6918.cn

PHP:  $argv;  $argc;
来源：http://pto.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://tdm.redwolf501.top

TS:   process.argv.slice(2)
来源：http://ixm.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://yfr.zhixingplan.top

Go:   os.Args[1:]
来源：http://xfd.0kj1m.cn

Ruby: ARGV
来源：http://isv.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://bdr.feifeiyinyue.top

[M02] 读取环境变量
来源：http://odt.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://sjp.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fqs.pengpengdd.cyou

JS:   process.env.HOME
来源：http://qpr.nanxuanxn.top

TS:   process.env.HOME
来源：http://ncf.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://prr.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fwi.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://jcq.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://msv.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://lfb.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fow.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gye.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pls.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mcg.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mqy.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lpb.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ndt.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://oew.jiagoushi.top

[M04] 获取当前工作目录
来源：http://sqa.yuanzhike.top

Py:   os.getcwd()
来源：http://glx.zhongyouzk.top

PHP:  getcwd();
来源：http://fnq.shzxlz.cn

JS:   process.cwd()
来源：http://yci.ehwqpu.com

TS:   process.cwd()
来源：http://ijv.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://jqg.gaohongyu789.top

Go:   os.Getwd()
来源：http://dwk.birdmap.top

Ruby: Dir.pwd
来源：http://wyd.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://iwn.jyoumei.cn

[M05] 设置退出码
来源：http://nuq.bbcook.cn

Py:   sys.exit(1)
来源：http://zzs.hesvh.cn

PHP:  exit(1);
来源：http://hyj.xylfe.cn

JS:   process.exit(1)
来源：http://ebb.xinyue.icu

TS:   process.exit(1)
来源：http://vrz.hysaishi.cn

Java: System.exit(1)
来源：http://hni.kuanghao11.cn

Go:   os.Exit(1)
来源：http://awa.zdqjudy.top

Ruby: exit 1
来源：http://ilj.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rkg.ehwqpu.com

[M06] 向标准错误输出
来源：http://jsy.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://qdr.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vlc.zhixingplan.top

JS:   console.error("err")
来源：http://uup.jqgfzy.top

TS:   console.error("err")
来源：http://qfh.dianchejie.cn

Java: System.err.println("err")
来源：http://jmp.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tzw.nanxuanxn.top

Ruby: warn "err"
来源：http://ena.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://tuz.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://ztt.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://kmp.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qlb.chenzaomai.com

JS:   require.main === module
来源：http://xac.ctjpmb.com

TS:   require.main === module
来源：http://qhv.yvedp.cn

Java: public static void main(String[] args)
来源：http://xgc.dashuyun.cn

Go:   func main()
来源：http://zgi.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fej.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://mia.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://wov.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://cta.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://gtt.yuanzhike.top

JS:   process.platform;  process.version
来源：http://gtp.nanxinkj.top

TS:   process.platform;  process.version
来源：http://fox.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uuw.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ihr.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tsm.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://slm.yuxming.cn

================================================================================
来源：http://olx.fengsongda.top

N. 数据结构与算法
来源：http://bfo.kuanghao11.cn

================================================================================
来源：http://zto.316326.xyz

[N01] 二分查找（有序数组）
来源：http://viy.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://ssc.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bie.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sgd.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tgc.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://soy.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://mth.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://itc.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://yct.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://vkn.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://srp.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ilg.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lcw.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mrc.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://elc.havefunace.top

Go:   slices.Sort(arr)
来源：http://cvv.vqdsnc.cn

Ruby: arr.sort
来源：http://tmt.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lwu.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://etj.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yvk.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://vzc.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aze.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://muc.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://prc.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tuq.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rrc.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://wys.iojbl.cn

[N04] 斐波那契数列
来源：http://owv.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xbl.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nnx.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zah.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vou.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cnx.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kgk.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nan.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zcp.epnwcf.com

[N05] 最大公约数
来源：http://hmi.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://fzi.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lvs.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nqg.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ear.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ujc.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eax.yuanzhike.top

Ruby: a.gcd(b)
来源：http://csc.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cjs.52xcode.cn

[N06] 判断回文字符串
来源：http://zrt.nwbrower.top

Py:   s == s[::-1]
来源：http://jsj.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://wwf.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://gto.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://mty.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uee.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://srm.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://ftt.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wgb.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://rri.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xgn.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sgx.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://zab.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://tjc.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://kjv.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://tlr.nanxinkj.top

Ruby: // 手写 Hash
来源：http://iha.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wtm.sweek.top

[N08] 生成全排列
来源：http://gds.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://nlr.ctjpmb.com

PHP:  // 手写递归交换
来源：http://zys.daxiang520.top

JS:   // 手写回溯递归
来源：http://otl.fehbvm.com

TS:   // 手写回溯递归
来源：http://mza.sufxvd.cn

Java: // 手写回溯递归
来源：http://spy.iojbl.cn

Go:   // 手写回溯递归
来源：http://vwv.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://wdw.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://lld.hnqzz.top

[N09] 栈与队列
来源：http://iuw.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iig.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://okv.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xmu.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ftd.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qdc.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ova.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wky.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jtm.tianlin.xyz

[N10] 链表节点定义
来源：http://dcw.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pxj.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bjv.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjg.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hdu.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://opo.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eud.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vfy.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://dqh.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://jxx.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jje.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://kdl.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rfb.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hps.gotoacloud.top

Java: // 手写递归
来源：http://uur.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://rpx.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lty.guannengcc.top

C#:   // 手写递归
来源：http://zla.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zgk.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xsu.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ueu.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sxk.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mbt.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vok.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ywk.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://npe.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dww.haohaochexian.top

================================================================================
来源：http://urs.kuanghao11.cn

O. 并发与异步
来源：http://ajc.hywenlv.cn

================================================================================
来源：http://pkp.mhx1999.top

[O01] 启动一个线程
来源：http://tdq.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zos.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lnp.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lal.fehbvm.com

TS:   // 同 JS
来源：http://tbn.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://mnf.9152youxi.cn

Go:   go f()
来源：http://bnm.sxryk.cn

Ruby: Thread.new { f }
来源：http://iud.ivvv.top

C#:   Task.Run(() => F());
来源：http://wux.svipenyu.cn

[O02] 使用线程池
来源：http://ekm.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uey.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vdt.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://wfo.sysykeji.top

TS:   // worker_threads 线程池
来源：http://ihr.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://pbp.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uzn.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jsy.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://enj.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://hpa.tarul.cn

Py:   with lock: shared += 1
来源：http://uzh.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://uct.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tkw.hesvh.cn

TS:   // 同 JS
来源：http://efg.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://isk.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bmi.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pjq.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://yel.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://cwu.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://fzl.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ncy.fehbvm.com

JS:   async function f() { await g(); }
来源：http://lla.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cri.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pqo.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mie.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://bcw.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://qds.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://tgv.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://ggf.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vfn.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://ilg.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://ugs.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hso.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tbo.gzhubu.top

Ruby: threads.map(&:join)
来源：http://vzm.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zde.xinyue.icu

[O06] 使用进程池
来源：http://une.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://efo.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jbg.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://jhh.ivvv.top

TS:   // child_process / cluster 模块
来源：http://ypm.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://spf.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ggm.xylfe.cn

Ruby: // fork 块
来源：http://qto.quarkkingdee.top

C#:   Parallel.For
来源：http://aag.yj20258888.top

================================================================================
来源：http://upe.yuxming.cn

P. 常用工具函数
来源：http://cwa.zhixingplan.top

================================================================================
来源：http://oha.epnwcf.com

[P01] 生成 UUID
来源：http://eid.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://uib.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uhd.yueranfly.top

JS:   crypto.randomUUID()
来源：http://onh.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://ime.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://keo.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://yno.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://svc.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://wqr.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://ufo.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fxj.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cqe.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wkl.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://omw.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hrs.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://znv.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gcg.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://krw.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://nif.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cjt.guowangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zuq.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tgc.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrt.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xlw.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bje.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://wqq.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lms.yfazqb.com

[P04] 求长度
来源：http://xpv.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://idw.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggc.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stv.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rzm.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://lat.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://zhc.wangdashe.top

Ruby: x.length;  x.size
来源：http://aco.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://pit.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://bru.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://bap.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nql.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wdg.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aoi.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://weh.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://bnl.yvedp.cn

Ruby: a == b
来源：http://gls.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kjq.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bdl.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gma.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://gal.zhijiandao.cn


<!-- 参考信息 -->