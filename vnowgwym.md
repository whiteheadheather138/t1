代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xei.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xzv.cdnleiting.top

================================================================================
来源：http://eho.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://vde.zhixingplan.top

================================================================================
来源：http://ypg.sweek.top

[M01] 读取命令行参数
来源：http://wkh.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://gdp.yj20258.top

PHP:  $argv;  $argc;
来源：http://dah.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://bja.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://gew.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://mgd.yueranfly.top

Go:   os.Args[1:]
来源：http://sdu.zhaomingkeji.xyz

Ruby: ARGV
来源：http://kte.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://nse.cucudq.cn

[M02] 读取环境变量
来源：http://nmn.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://jgc.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wix.yueranfly.top

JS:   process.env.HOME
来源：http://kdj.yj20258888.top

TS:   process.env.HOME
来源：http://rcw.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://pqj.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lws.uphjek.com

Ruby: ENV["HOME"]
来源：http://pdh.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rkn.shzxlz.cn

[M03] 执行外部命令
来源：http://gxh.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mwi.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pdd.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ylw.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zrb.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zhu.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ebv.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://nvi.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://fca.hammf.cn

[M04] 获取当前工作目录
来源：http://xsy.chenlongwang.top

Py:   os.getcwd()
来源：http://ohs.fehbvm.com

PHP:  getcwd();
来源：http://qhf.uphjek.com

JS:   process.cwd()
来源：http://vrx.jinghuilouyu.cn

TS:   process.cwd()
来源：http://bwq.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://xfb.sysykeji.top

Go:   os.Getwd()
来源：http://eka.jqgfzy.top

Ruby: Dir.pwd
来源：http://bnp.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sow.jqgufenzy.top

[M05] 设置退出码
来源：http://ilv.smart0.xyz

Py:   sys.exit(1)
来源：http://wgx.zdqjudy.top

PHP:  exit(1);
来源：http://rdy.snrcjt.cn

JS:   process.exit(1)
来源：http://tfe.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://zka.birdmap.top

Java: System.exit(1)
来源：http://ora.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://kab.aizwys.cn

Ruby: exit 1
来源：http://dsg.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://egy.quarkkingdee.top

[M06] 向标准错误输出
来源：http://vdw.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://dkv.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nxc.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://gkf.haohaochexian.top

TS:   console.error("err")
来源：http://iok.zhengqikj.top

Java: System.err.println("err")
来源：http://kzd.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eor.aizwys.cn

Ruby: warn "err"
来源：http://wwm.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://lgj.cqqwz.cn

[M07] 判断是否为主入口
来源：http://yvp.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://qxw.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rts.shuidangran.top

JS:   require.main === module
来源：http://ist.hnxiangtu.top

TS:   require.main === module
来源：http://xcf.yangfankeji.com

Java: public static void main(String[] args)
来源：http://xvw.cheryme.top

Go:   func main()
来源：http://djf.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wzu.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://oyx.tanke756.top

[M08] 获取系统与运行时信息
来源：http://tpb.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://ocg.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://kvn.havefunace.top

JS:   process.platform;  process.version
来源：http://pln.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://lgl.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cjj.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cqs.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ins.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bhm.jyoumei.cn

================================================================================
来源：http://rpb.chenzaomai.com

N. 数据结构与算法
来源：http://sjd.yj20258888.top

================================================================================
来源：http://qau.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://tjs.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://bhj.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ban.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qis.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jbl.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fyh.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://mak.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://soa.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://tyo.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://iyx.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://emc.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zgn.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vup.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dxf.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fmp.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://bcu.shangyingyoupin.top

Ruby: arr.sort
来源：http://wid.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ohl.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://uoz.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yxq.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://jbe.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esg.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbh.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sgx.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lqo.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://caj.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://spf.gotoacloud.top

[N04] 斐波那契数列
来源：http://vih.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://phm.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xmf.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxj.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebj.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yxt.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wts.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://awl.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mso.xuetiantiany.cn

[N05] 最大公约数
来源：http://ssw.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://mjy.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://brs.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://syw.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vyi.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bxq.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gim.meibo888.top

Ruby: a.gcd(b)
来源：http://jkv.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mhv.bbcook.cn

[N06] 判断回文字符串
来源：http://tce.xziqi.cn

Py:   s == s[::-1]
来源：http://fuc.hcnkem.com

PHP:  $s === strrev($s);
来源：http://urd.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://wth.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://lex.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cfa.wangdashe.top

Go:   // 双指针从两端比较
来源：http://loh.kuanghao11.cn

Ruby: s == s.reverse
来源：http://bkz.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nit.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://zkp.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bsk.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pbx.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tqi.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://coq.aibaodan.cn

Java: // 手写 HashMap
来源：http://gfy.yfazqb.com

Go:   // 手写 map[int]int
来源：http://dvg.svipenyu.cn

Ruby: // 手写 Hash
来源：http://laj.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://sdx.bbcook.cn

[N08] 生成全排列
来源：http://eag.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://vva.cashguo.top

PHP:  // 手写递归交换
来源：http://tok.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://kch.redwolf501.top

TS:   // 手写回溯递归
来源：http://xcp.zdqjudy.top

Java: // 手写回溯递归
来源：http://otq.yangfankeji.com

Go:   // 手写回溯递归
来源：http://xfj.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://iag.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://twg.zhijiandao.cn

[N09] 栈与队列
来源：http://uob.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qtn.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bax.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tvw.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pld.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://omd.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sxl.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iet.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://syd.yanxiufei.cn

[N10] 链表节点定义
来源：http://axr.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnk.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wex.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lez.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mlj.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://muc.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mwd.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ljh.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://roe.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://sms.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rrx.c1oappe.top

PHP:  // 手写递归函数
来源：http://anz.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hkk.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzn.xuanzx.com

Java: // 手写递归
来源：http://sdo.52xcode.cn

Go:   // 手写递归
来源：http://uhe.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zgn.epnwcf.com

C#:   // 手写递归
来源：http://ngc.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kyn.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yvx.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dwn.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://byu.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ycx.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xee.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dgk.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kym.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nfj.dashuyun.cn

================================================================================
来源：http://ztf.sjlbkw.cn

O. 并发与异步
来源：http://cri.tian-w.cn

================================================================================
来源：http://rca.fengsongda.top

[O01] 启动一个线程
来源：http://eja.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yxa.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qae.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vpw.yangfankeji.com

TS:   // 同 JS
来源：http://uud.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://irb.wangdashe.top

Go:   go f()
来源：http://gez.jianghu66.top

Ruby: Thread.new { f }
来源：http://kcm.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://lex.iojbl.cn

[O02] 使用线程池
来源：http://qgf.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ayd.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cul.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://poj.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://ohi.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://rrd.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://why.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xuy.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cfb.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://akb.cheryme.top

Py:   with lock: shared += 1
来源：http://dzq.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://qed.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jfk.wangdashe.top

TS:   // 同 JS
来源：http://orj.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://erf.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kwq.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qkp.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://zlf.xylfe.cn

[O04] 定义异步函数并等待
来源：http://wbp.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://kbq.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xhr.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://fkn.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://iwy.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gfj.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kjs.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://flz.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://bme.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://cks.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://nut.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fuv.yonumen.top

JS:   await Promise.all(tasks)
来源：http://zwr.pycfn.com

TS:   await Promise.all(tasks)
来源：http://apr.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vpt.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tyr.tarul.cn

Ruby: threads.map(&:join)
来源：http://lgg.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://yrb.tianlin.xyz

[O06] 使用进程池
来源：http://lcp.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bfc.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://eqc.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://hgo.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://jww.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cwi.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lug.316326.xyz

Ruby: // fork 块
来源：http://bdc.fzhhl.top

C#:   Parallel.For
来源：http://djn.ehwqpu.com

================================================================================
来源：http://hqt.ctjpmb.com

P. 常用工具函数
来源：http://shc.kuanghao11.cn

================================================================================
来源：http://pxl.wangshuangyany.cn

[P01] 生成 UUID
来源：http://psw.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://ypq.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hdu.shuidangran.top

JS:   crypto.randomUUID()
来源：http://avu.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://mqh.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://uzm.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://vco.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://ibt.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://bdx.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://dfw.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zrl.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mtb.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tvz.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://izo.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mjw.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sql.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://roh.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lhl.yj20258888.top

[P03] 生成短随机字符串
来源：http://zrh.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gjt.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rsj.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oba.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qop.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vqr.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://koe.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yrr.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aji.redwolf501.top

[P04] 求长度
来源：http://ugo.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dso.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vin.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uwg.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ccs.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://ibe.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://gkj.sysykeji.top

Ruby: x.length;  x.size
来源：http://zrt.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hig.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://xoe.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bhd.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fex.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kfw.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dmm.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lyk.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://viw.zycfv.cn

Ruby: a == b
来源：http://okw.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bay.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gip.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mdp.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://dbp.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vam.shzxlz.cn

TS:   if (x == null) {}
来源：http://qmb.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pla.chenlongwang.top

Go:   if x == nil {}
来源：http://etb.0kj1m.cn


<!-- 参考信息 -->