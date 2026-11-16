代发 wailian999

C#:   (int)resp.StatusCode
来源：http://nlt.cqqwz.cn

[L08] 并发请求多个地址
来源：http://txx.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qyz.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://cxy.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://azb.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iud.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rza.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aug.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kct.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hph.cqqwz.cn

================================================================================
来源：http://pqm.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://mef.havefunace.top

================================================================================
来源：http://hhm.ybcxt.top

[M01] 读取命令行参数
来源：http://ijt.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://wun.gotoacloud.top

PHP:  $argv;  $argc;
来源：http://qos.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://gxf.xziqi.cn

TS:   process.argv.slice(2)
来源：http://ruj.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://zhl.yuxming.cn

Go:   os.Args[1:]
来源：http://pex.quarkkingdee.top

Ruby: ARGV
来源：http://iun.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://pjc.fehbvm.com

[M02] 读取环境变量
来源：http://pkw.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://fdk.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://edp.cheryme.top

JS:   process.env.HOME
来源：http://qol.52xcode.cn

TS:   process.env.HOME
来源：http://ahb.tian-w.cn

Java: System.getenv("HOME")
来源：http://ahj.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://brd.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://yfq.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rab.ybcxt.top

[M03] 执行外部命令
来源：http://rce.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://udj.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fwp.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lqf.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yau.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pej.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cmi.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://gbf.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://hjw.jiagoushi.top

[M04] 获取当前工作目录
来源：http://fxj.cheryme.top

Py:   os.getcwd()
来源：http://mpq.jqgfzy.top

PHP:  getcwd();
来源：http://iwt.pycfn.com

JS:   process.cwd()
来源：http://dds.hongshengwenyu.top

TS:   process.cwd()
来源：http://uti.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://cse.c1oappe.top

Go:   os.Getwd()
来源：http://mnp.hywenlv.cn

Ruby: Dir.pwd
来源：http://fwx.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://fvj.yuxming.cn

[M05] 设置退出码
来源：http://qtw.zhijiandao.cn

Py:   sys.exit(1)
来源：http://fdb.yuanzhike.top

PHP:  exit(1);
来源：http://jlu.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://mnz.shzxlz.cn

TS:   process.exit(1)
来源：http://pqi.fktsv.cn

Java: System.exit(1)
来源：http://pge.yuxming.cn

Go:   os.Exit(1)
来源：http://fqx.feifeiyinyue.top

Ruby: exit 1
来源：http://jgh.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://amv.snrcjt.cn

[M06] 向标准错误输出
来源：http://zto.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://eka.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nhd.hysaishi.cn

JS:   console.error("err")
来源：http://ski.meibo888.top

TS:   console.error("err")
来源：http://fzo.tarul.cn

Java: System.err.println("err")
来源：http://dvw.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://njf.cdnleiting.top

Ruby: warn "err"
来源：http://zyk.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://irf.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://ufu.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://wkd.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vdn.sweek.top

JS:   require.main === module
来源：http://fby.nanxuanxn.top

TS:   require.main === module
来源：http://uuf.cashguo.top

Java: public static void main(String[] args)
来源：http://ace.hongshengwenyu.top

Go:   func main()
来源：http://iin.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qmv.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://jax.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://wna.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://tqs.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://equ.9152youxi.cn

JS:   process.platform;  process.version
来源：http://orl.bjfxy.top

TS:   process.platform;  process.version
来源：http://btr.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pws.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fev.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dkc.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xsf.cucudq.cn

================================================================================
来源：http://jxh.hnqzz.top

N. 数据结构与算法
来源：http://wwa.kuanghao11.cn

================================================================================
来源：http://dlo.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://gev.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://opj.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rqh.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://znd.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://irr.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://hok.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://rpy.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://edd.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bss.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://ixe.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://eoy.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ssx.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zdo.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kzp.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wfq.fengsongda.top

Go:   slices.Sort(arr)
来源：http://yxa.guowangkeji.top

Ruby: arr.sort
来源：http://xvd.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uec.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://lnb.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nju.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://dss.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xot.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mba.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mfm.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rhh.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zef.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://igc.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://ppw.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dmx.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iby.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xbx.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqb.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lcm.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ead.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://prk.52xcode.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cxh.zhongyouzk.top

[N05] 最大公约数
来源：http://ruc.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://cvf.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tex.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygl.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bqn.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avc.nanxinkj.top

Ruby: a.gcd(b)
来源：http://yox.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dfd.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://sbh.xziqi.cn

Py:   s == s[::-1]
来源：http://bzk.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://lln.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://rrd.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://onn.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://knz.uphjek.com

Go:   // 双指针从两端比较
来源：http://jax.daria6918.cn

Ruby: s == s.reverse
来源：http://uyp.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nvl.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://hho.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gze.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hjz.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ayo.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://zrc.epnwcf.com

Java: // 手写 HashMap
来源：http://zgy.uphjek.com

Go:   // 手写 map[int]int
来源：http://bys.zhixingplan.top

Ruby: // 手写 Hash
来源：http://uww.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://byz.kuanghao11.cn

[N08] 生成全排列
来源：http://oeh.cheryme.top

Py:   itertools.permutations(arr)
来源：http://tlo.nanxinkj.top

PHP:  // 手写递归交换
来源：http://pci.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://fjg.xinyue.icu

TS:   // 手写回溯递归
来源：http://myn.yuxming.cn

Java: // 手写回溯递归
来源：http://cle.yuxming.cn

Go:   // 手写回溯递归
来源：http://hhz.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://rbi.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://xzg.fehbvm.com

[N09] 栈与队列
来源：http://exe.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jho.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://chy.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wki.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vaq.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cat.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mcd.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rbb.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xdw.svipenyu.cn

[N10] 链表节点定义
来源：http://uoi.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uwh.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://itj.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ycu.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wgm.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://hrw.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ehx.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wcw.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zyq.gzhubu.top

[N11] 二叉树中序遍历
来源：http://bgy.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kay.aibaodan.cn

PHP:  // 手写递归函数
来源：http://qzx.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jna.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://buy.shzxlz.cn

Java: // 手写递归
来源：http://clk.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://tes.gotoacloud.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zfl.hongshengwenyu.top

C#:   // 手写递归
来源：http://btv.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lau.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vmi.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vfu.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jul.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rjb.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fmu.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyp.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nnp.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dtv.xuetiantiany.cn

================================================================================
来源：http://dbb.jyoumei.cn

O. 并发与异步
来源：http://sjl.chenjidiqi.icu

================================================================================
来源：http://pxn.vehdjk.com

[O01] 启动一个线程
来源：http://yji.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ohk.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ltk.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kje.yj202588.top

TS:   // 同 JS
来源：http://bnz.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://dzg.tarul.cn

Go:   go f()
来源：http://ule.bjfxy.top

Ruby: Thread.new { f }
来源：http://mzx.guannengcc.top

C#:   Task.Run(() => F());
来源：http://ujh.cdnleiting.top

[O02] 使用线程池
来源：http://yei.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qmz.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iog.c1oappe.top

JS:   // worker_threads 线程池
来源：http://ukj.daria6918.cn

TS:   // worker_threads 线程池
来源：http://xpu.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://cqp.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sfm.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yzn.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gkk.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://cee.cheryme.top

Py:   with lock: shared += 1
来源：http://baq.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://sub.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdd.yongpay.top

TS:   // 同 JS
来源：http://rgd.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://ktm.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qor.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lsy.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://lnp.cheryme.top

[O04] 定义异步函数并等待
来源：http://ywn.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://ipt.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xtq.andypj.xyz

JS:   async function f() { await g(); }
来源：http://rbb.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tya.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zus.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xeb.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://xdp.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://mnj.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://ltx.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://cnm.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://alj.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://jbz.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://aor.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ubg.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pcf.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://mkl.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uhh.ctjpmb.com

[O06] 使用进程池
来源：http://iux.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tbt.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xkf.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://vnu.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://hro.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dhy.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mdu.andypj.xyz

Ruby: // fork 块
来源：http://iav.zhijiandao.cn

C#:   Parallel.For
来源：http://enc.gzhubu.top

================================================================================
来源：http://osh.quarkkingdee.top

P. 常用工具函数
来源：http://jfk.iojbl.cn

================================================================================
来源：http://vcx.nanxinkj.top

[P01] 生成 UUID
来源：http://snm.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://bdz.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ntl.ivvv.top

JS:   crypto.randomUUID()
来源：http://ehc.yonumen.top

TS:   crypto.randomUUID()
来源：http://tga.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://tzj.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://rsm.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://qwq.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://jdg.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://fnd.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fjh.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://ovr.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xah.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fzd.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://owe.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://svs.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kjm.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bih.zhengqikj.top

[P03] 生成短随机字符串
来源：http://aex.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fns.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jgs.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fnr.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kyi.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nka.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zaq.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://gey.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://htd.fktsv.cn

[P04] 求长度
来源：http://anl.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qbe.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nkh.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aqi.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wod.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://qep.yuxming.cn

Go:   len(arr);  len(m)
来源：http://wpc.bbcook.cn

Ruby: x.length;  x.size
来源：http://lsq.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jcb.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://uad.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zuy.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xdr.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dxs.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eix.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ejr.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://psx.fehbvm.com

Ruby: a == b
来源：http://krl.tarul.cn


<!-- 参考信息 -->