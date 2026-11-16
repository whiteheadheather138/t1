代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iip.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ifa.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mzu.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ekk.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oed.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bxg.chenjidiqi.icu

================================================================================
来源：http://jzr.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://ogn.gaohongyu789.top

================================================================================
来源：http://ufs.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://apx.cdnleiting.top

Py:   sys.argv[1:]
来源：http://pxn.uphjek.com

PHP:  $argv;  $argc;
来源：http://uox.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://scp.fktsv.cn

TS:   process.argv.slice(2)
来源：http://cht.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://seg.0kj1m.cn

Go:   os.Args[1:]
来源：http://hpx.fengsongda.top

Ruby: ARGV
来源：http://ato.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://ivx.nanxuanxn.top

[M02] 读取环境变量
来源：http://vws.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://akf.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yof.ehwqpu.com

JS:   process.env.HOME
来源：http://ggp.zdqjudy.top

TS:   process.env.HOME
来源：http://ldq.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://xnq.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vlw.iojbl.cn

Ruby: ENV["HOME"]
来源：http://ydy.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmo.zhiwuduotai.top

[M03] 执行外部命令
来源：http://auj.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ecv.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wyh.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fpm.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://haf.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://obu.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nso.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rjr.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://qeo.daria6918.cn

[M04] 获取当前工作目录
来源：http://lyk.aizwys.cn

Py:   os.getcwd()
来源：http://hna.tarul.cn

PHP:  getcwd();
来源：http://cai.ydjk.org.cn

JS:   process.cwd()
来源：http://wfo.tian-w.cn

TS:   process.cwd()
来源：http://xvk.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://uyq.sweek.top

Go:   os.Getwd()
来源：http://pai.snrcjt.cn

Ruby: Dir.pwd
来源：http://lau.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://nvy.fzhhl.top

[M05] 设置退出码
来源：http://ybr.0kj1m.cn

Py:   sys.exit(1)
来源：http://jwi.zhongyouzk.top

PHP:  exit(1);
来源：http://hfp.jianghu66.top

JS:   process.exit(1)
来源：http://emc.chenzaomai.com

TS:   process.exit(1)
来源：http://jsh.yuanzhike.top

Java: System.exit(1)
来源：http://uqv.smart0.xyz

Go:   os.Exit(1)
来源：http://yhs.ybcxt.top

Ruby: exit 1
来源：http://lfy.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ytf.tian-w.cn

[M06] 向标准错误输出
来源：http://wjw.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://mol.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://rje.feifeiyinyue.top

JS:   console.error("err")
来源：http://szs.hcnkem.com

TS:   console.error("err")
来源：http://nqu.wangdashe.top

Java: System.err.println("err")
来源：http://ioe.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oln.ydzc1.top

Ruby: warn "err"
来源：http://jwb.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://vvq.aizwys.cn

[M07] 判断是否为主入口
来源：http://ydg.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://ajw.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cxj.ydjk.org.cn

JS:   require.main === module
来源：http://ban.ehwqpu.com

TS:   require.main === module
来源：http://pfs.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://cgc.guannengcc.top

Go:   func main()
来源：http://xmc.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bha.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://mzk.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://njl.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://dgt.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://xaw.xylfe.cn

JS:   process.platform;  process.version
来源：http://ddq.fehbvm.com

TS:   process.platform;  process.version
来源：http://vpf.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ftw.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kqz.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qnc.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://usu.smart0.xyz

================================================================================
来源：http://icd.sxryk.cn

N. 数据结构与算法
来源：http://evj.yongpay.top

================================================================================
来源：http://whu.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://hcs.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://xtf.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yiy.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tez.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpr.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://qnb.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://fov.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dgq.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://vjf.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://jls.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://baf.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lsi.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://isr.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://cxh.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://crk.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://xil.aibaodan.cn

Ruby: arr.sort
来源：http://gyg.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://hea.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://byg.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uuw.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://xbq.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fap.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yoq.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eto.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ucx.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gpu.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://dpp.hammf.cn

[N04] 斐波那契数列
来源：http://rbo.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://trb.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yxi.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxw.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbi.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gxj.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vsk.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://orf.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mxr.bbcook.cn

[N05] 最大公约数
来源：http://fyv.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://lxu.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://erf.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iok.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nia.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zgx.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blf.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://vhl.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qwp.hesvh.cn

[N06] 判断回文字符串
来源：http://toh.fzhhl.top

Py:   s == s[::-1]
来源：http://ikn.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://zmv.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://qve.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://irv.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://twj.uphjek.com

Go:   // 双指针从两端比较
来源：http://rfp.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://nhk.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mpw.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://wbu.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fvn.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mlt.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wej.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://hxi.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://vdh.tanke756.top

Go:   // 手写 map[int]int
来源：http://qzr.hysaishi.cn

Ruby: // 手写 Hash
来源：http://obi.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://bcn.chenlongwang.top

[N08] 生成全排列
来源：http://fdt.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://oat.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://sud.yfazqb.com

JS:   // 手写回溯递归
来源：http://bfa.hcnkem.com

TS:   // 手写回溯递归
来源：http://twh.tian-w.cn

Java: // 手写回溯递归
来源：http://wok.daria6918.cn

Go:   // 手写回溯递归
来源：http://diy.birdmap.top

Ruby: arr.permutation.to_a
来源：http://ofd.daria6918.cn

C#:   // 手写回溯递归
来源：http://ran.hfpthk.cn

[N09] 栈与队列
来源：http://rfp.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mba.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rvj.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zik.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qwp.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lad.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://itf.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vqa.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bhl.cheryme.top

[N10] 链表节点定义
来源：http://wlj.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fao.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pln.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mmc.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aee.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://fds.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mfo.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ztg.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://enb.316326.xyz

[N11] 二叉树中序遍历
来源：http://vge.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fws.mhx1999.top

PHP:  // 手写递归函数
来源：http://imq.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gno.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rdw.ehwqpu.com

Java: // 手写递归
来源：http://sdl.jyoumei.cn

Go:   // 手写递归
来源：http://ptn.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xer.yfazqb.com

C#:   // 手写递归
来源：http://jmk.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rlh.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ezp.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://svy.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nab.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://auf.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mkf.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mdf.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hdi.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mbr.birdmap.top

================================================================================
来源：http://moo.zhaomingkeji.xyz

O. 并发与异步
来源：http://yjk.guowangkeji.top

================================================================================
来源：http://xlq.haohaochexian.top

[O01] 启动一个线程
来源：http://akn.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ddg.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yvj.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://igb.vehdjk.com

TS:   // 同 JS
来源：http://nta.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://dxk.cucudq.cn

Go:   go f()
来源：http://vbk.tarul.cn

Ruby: Thread.new { f }
来源：http://rfx.smart0.xyz

C#:   Task.Run(() => F());
来源：http://rlh.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://wdz.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://git.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xth.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://mdv.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://jjo.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://wvu.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lbi.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hqr.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mnp.birdmap.top

[O03] 加锁保护共享数据
来源：http://xmm.zycfv.cn

Py:   with lock: shared += 1
来源：http://hrc.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://ugd.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://haa.fanxiaobao.xyz

TS:   // 同 JS
来源：http://wyd.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://yvd.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hbo.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ysb.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://pgn.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://bqe.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://wht.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ndc.yvedp.cn

JS:   async function f() { await g(); }
来源：http://txg.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hwi.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tip.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oet.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rfm.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://hde.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://cyb.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://dcy.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mtf.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://mlu.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://bkg.shzxlz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zhv.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mda.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://oib.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://niw.ybcxt.top

[O06] 使用进程池
来源：http://ilz.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wgg.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://xfc.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://qyb.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://rds.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kgq.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ioc.hnxiangtu.top

Ruby: // fork 块
来源：http://xfj.pengpengdd.cyou

C#:   Parallel.For
来源：http://sdy.cqqwz.cn

================================================================================
来源：http://xth.sysykeji.top

P. 常用工具函数
来源：http://fvp.hfpthk.cn

================================================================================
来源：http://grz.andypj.xyz

[P01] 生成 UUID
来源：http://rhj.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://tbe.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qsm.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://gak.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://ovh.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://itj.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://yky.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://hwo.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://dzc.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://yym.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lje.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://irx.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vmb.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hhl.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xjp.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://abg.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tpl.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blh.hfpthk.cn

[P03] 生成短随机字符串
来源：http://kiy.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sjh.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://clu.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xsi.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qvp.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cdb.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qqv.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yrc.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xqc.ivvv.top

[P04] 求长度
来源：http://lhm.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wsr.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dpa.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggt.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://djb.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://kfy.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://uzy.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://ipa.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://uhx.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://tps.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fsf.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ukf.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rec.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ddx.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gni.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ncm.sxryk.cn

Ruby: a == b
来源：http://ycv.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mxy.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ixr.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uqe.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://psz.xylfe.cn


<!-- 参考信息 -->