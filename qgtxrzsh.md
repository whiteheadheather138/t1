代发 wailian999

C#:   (int)resp.StatusCode
来源：http://wie.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ths.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mbr.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://tqa.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lqj.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iuc.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mtn.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lwp.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kvl.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hpl.zhiwuduotai.top

================================================================================
来源：http://vko.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://yiv.shzxlz.cn

================================================================================
来源：http://apt.yueranfly.top

[M01] 读取命令行参数
来源：http://zys.smart0.xyz

Py:   sys.argv[1:]
来源：http://eek.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://tmv.uphjek.com

JS:   process.argv.slice(2)
来源：http://wyp.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://gvz.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://ayu.sxryk.cn

Go:   os.Args[1:]
来源：http://zaf.xuetiantiany.cn

Ruby: ARGV
来源：http://rpt.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://isb.chenzaomai.com

[M02] 读取环境变量
来源：http://muh.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://xfm.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kic.birdmap.top

JS:   process.env.HOME
来源：http://ggx.jqgufenzy.top

TS:   process.env.HOME
来源：http://bmz.xuanzx.com

Java: System.getenv("HOME")
来源：http://myr.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpl.cashguo.top

Ruby: ENV["HOME"]
来源：http://kmv.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gle.zhengqikj.top

[M03] 执行外部命令
来源：http://vmj.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wip.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cqh.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nrb.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rri.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iab.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yuk.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://fdt.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://cko.zdqjudy.top

[M04] 获取当前工作目录
来源：http://wnx.dashuyun.cn

Py:   os.getcwd()
来源：http://gru.shangyingyoupin.top

PHP:  getcwd();
来源：http://orq.jyoumei.cn

JS:   process.cwd()
来源：http://ade.pengpengdd.cyou

TS:   process.cwd()
来源：http://jlw.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://pzc.gotoacloud.top

Go:   os.Getwd()
来源：http://kzs.sweek.top

Ruby: Dir.pwd
来源：http://xou.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://mhq.zhiwuduotai.top

[M05] 设置退出码
来源：http://odq.fktsv.cn

Py:   sys.exit(1)
来源：http://osn.sweek.top

PHP:  exit(1);
来源：http://yfs.gogol.net.cn

JS:   process.exit(1)
来源：http://fwl.daxiang520.top

TS:   process.exit(1)
来源：http://lvr.yj20258.top

Java: System.exit(1)
来源：http://itp.fzhhl.top

Go:   os.Exit(1)
来源：http://orm.jinqigufen.top

Ruby: exit 1
来源：http://neg.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mgl.ivvv.top

[M06] 向标准错误输出
来源：http://tqj.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://omx.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://thn.nwbrower.top

JS:   console.error("err")
来源：http://dvy.tarul.cn

TS:   console.error("err")
来源：http://vuu.yongpay.top

Java: System.err.println("err")
来源：http://ktw.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qqg.zhoulong.xyz

Ruby: warn "err"
来源：http://mat.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://mox.smart0.xyz

[M07] 判断是否为主入口
来源：http://the.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://onj.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hhc.0kj1m.cn

JS:   require.main === module
来源：http://imh.svipenyu.cn

TS:   require.main === module
来源：http://anc.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://fdj.zhixingplan.top

Go:   func main()
来源：http://ozz.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qok.xuanzx.com

C#:   static void Main(string[] args)
来源：http://lqm.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://wkq.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://rqc.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://ywm.yangfankeji.com

JS:   process.platform;  process.version
来源：http://ask.ybcxt.top

TS:   process.platform;  process.version
来源：http://zpr.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://noh.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mck.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vbp.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iqd.tian-w.cn

================================================================================
来源：http://zlr.yvedp.cn

N. 数据结构与算法
来源：http://toz.yongpay.top

================================================================================
来源：http://ngb.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://pso.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hne.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gxq.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dsy.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mrn.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rrs.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://dtb.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ken.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://fpw.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://qzs.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://mib.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fyk.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kzd.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ebh.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ijt.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://bnh.quarkkingdee.top

Ruby: arr.sort
来源：http://izw.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jjd.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://fky.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xnq.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://ckw.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mjl.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nba.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kvi.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://exz.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xsh.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://rah.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://ppy.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wod.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://trk.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdn.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlw.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bga.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mbk.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dov.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oth.zdbjq.cn

[N05] 最大公约数
来源：http://rgh.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://mhf.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ktj.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfa.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sqt.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ibr.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vwb.cdnleiting.top

Ruby: a.gcd(b)
来源：http://oxd.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jel.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://tkv.jianghu66.top

Py:   s == s[::-1]
来源：http://sjj.yuxming.cn

PHP:  $s === strrev($s);
来源：http://wba.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://nwf.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://yrs.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fql.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://msm.zhongyouzk.top

Ruby: s == s.reverse
来源：http://muy.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uln.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://nkx.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kwj.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nxv.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fms.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://waz.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://slm.yvedp.cn

Go:   // 手写 map[int]int
来源：http://arg.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://ore.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://yhn.ppjwa.cn

[N08] 生成全排列
来源：http://zgz.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://gkz.yangfankeji.com

PHP:  // 手写递归交换
来源：http://hbx.gotoacloud.top

JS:   // 手写回溯递归
来源：http://hrx.yangfankeji.com

TS:   // 手写回溯递归
来源：http://igh.316326.xyz

Java: // 手写回溯递归
来源：http://xoc.xinyue.icu

Go:   // 手写回溯递归
来源：http://lhk.tanke756.top

Ruby: arr.permutation.to_a
来源：http://kpw.gotoacloud.top

C#:   // 手写回溯递归
来源：http://ugx.quarkkingdee.top

[N09] 栈与队列
来源：http://uqz.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mnp.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tlr.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xii.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nhi.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ors.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rhr.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://czl.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lbg.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://ros.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bgh.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://esy.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cme.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nwh.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://oot.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://gne.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qdn.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ijo.pycfn.com

[N11] 二叉树中序遍历
来源：http://osx.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pyv.andypj.xyz

PHP:  // 手写递归函数
来源：http://aov.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aiw.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hhc.xziqi.cn

Java: // 手写递归
来源：http://yti.jinqigfzy.top

Go:   // 手写递归
来源：http://mne.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ina.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://lwh.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gdp.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ydq.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mfx.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zsf.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://skw.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zvk.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hsw.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bxv.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xvx.yangfankeji.com

================================================================================
来源：http://lca.ivvv.top

O. 并发与异步
来源：http://rka.52xcode.cn

================================================================================
来源：http://jxg.yueranfly.top

[O01] 启动一个线程
来源：http://jup.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pqb.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jnm.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uka.sweek.top

TS:   // 同 JS
来源：http://ilq.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://pyy.yuanzhike.top

Go:   go f()
来源：http://rkx.cqqwz.cn

Ruby: Thread.new { f }
来源：http://iuv.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://ifs.hywenlv.cn

[O02] 使用线程池
来源：http://cnz.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hfa.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tbg.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://dvz.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://lga.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://gyd.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bva.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ipg.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ift.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://uln.yfazqb.com

Py:   with lock: shared += 1
来源：http://ovj.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://ajj.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wbj.52xcode.cn

TS:   // 同 JS
来源：http://gpz.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://put.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cvw.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ntf.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://bug.yj20258888.top

[O04] 定义异步函数并等待
来源：http://tje.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://pfy.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dvq.mhx1999.top

JS:   async function f() { await g(); }
来源：http://sdx.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eka.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://akb.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyz.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://mpe.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://pja.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://ymu.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://hib.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tkt.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://kbw.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://ztg.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nez.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qmv.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://syi.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://itn.hammf.cn

[O06] 使用进程池
来源：http://dct.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jng.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vhw.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://hti.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://yyc.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yyl.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://skm.hnxiangtu.top

Ruby: // fork 块
来源：http://aeg.jqgufenzy.top

C#:   Parallel.For
来源：http://ymg.havefunace.top

================================================================================
来源：http://hey.zhongyouzk.top

P. 常用工具函数
来源：http://zde.xylfe.cn

================================================================================
来源：http://gzu.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://wep.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://dfz.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xux.fzhhl.top

JS:   crypto.randomUUID()
来源：http://ndf.meibo888.top

TS:   crypto.randomUUID()
来源：http://sat.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://vba.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://ehk.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://tjf.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://hdn.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://jrb.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bcj.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://rpc.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yfl.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tpy.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tlb.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mni.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tym.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lqi.cucudq.cn

[P03] 生成短随机字符串
来源：http://wrk.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://klq.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ofd.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iik.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uxf.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qwo.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eee.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hsq.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://skp.svipenyu.cn

[P04] 求长度
来源：http://dgb.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xln.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ual.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qke.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mtt.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://hfz.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://vqc.bbcook.cn

Ruby: x.length;  x.size
来源：http://eol.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fay.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://uml.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jwp.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mso.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cqw.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fmg.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wua.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xcd.gotoacloud.top

Ruby: a == b
来源：http://qke.svipenyu.cn


<!-- 参考信息 -->