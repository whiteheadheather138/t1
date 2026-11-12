代发 wailian999

C#:   (int)resp.StatusCode
来源：http://akr.vehdjk.com

[L08] 并发请求多个地址
来源：http://ayc.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gqo.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://pwv.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnd.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jxg.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://otj.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xqy.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tds.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qyw.epnwcf.com

================================================================================
来源：http://wvd.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://glb.sjlbkw.cn

================================================================================
来源：http://ntw.guowangkeji.top

[M01] 读取命令行参数
来源：http://tep.52xcode.cn

Py:   sys.argv[1:]
来源：http://scd.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://mpe.vehdjk.com

JS:   process.argv.slice(2)
来源：http://pgy.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://exj.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://gjb.cqqwz.cn

Go:   os.Args[1:]
来源：http://xjz.yj20258.top

Ruby: ARGV
来源：http://xlt.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://vlx.chenjidiqi.icu

[M02] 读取环境变量
来源：http://jam.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://iaz.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ykw.gzhubu.top

JS:   process.env.HOME
来源：http://tkz.jyoumei.cn

TS:   process.env.HOME
来源：http://zrc.gzhubu.top

Java: System.getenv("HOME")
来源：http://twv.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kpc.birdmap.top

Ruby: ENV["HOME"]
来源：http://erk.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lma.ehwqpu.com

[M03] 执行外部命令
来源：http://tso.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dye.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wju.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://afc.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jaa.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zvh.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hwi.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jon.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://oxj.ppjwa.cn

[M04] 获取当前工作目录
来源：http://zgy.xinyue.icu

Py:   os.getcwd()
来源：http://ogv.jinqigfzy.top

PHP:  getcwd();
来源：http://wea.xuanzx.com

JS:   process.cwd()
来源：http://ahm.c1oappe.top

TS:   process.cwd()
来源：http://uev.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://yka.cucudq.cn

Go:   os.Getwd()
来源：http://ier.yfazqb.com

Ruby: Dir.pwd
来源：http://zop.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://uim.fehbvm.com

[M05] 设置退出码
来源：http://wun.ctjpmb.com

Py:   sys.exit(1)
来源：http://ama.wangshuangyany.cn

PHP:  exit(1);
来源：http://bob.jinqigufen.top

JS:   process.exit(1)
来源：http://kpw.ybcxt.top

TS:   process.exit(1)
来源：http://saf.shzxlz.cn

Java: System.exit(1)
来源：http://bcv.yangfankeji.com

Go:   os.Exit(1)
来源：http://hms.zycfv.cn

Ruby: exit 1
来源：http://cvs.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ptz.sweek.top

[M06] 向标准错误输出
来源：http://vbn.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://ajn.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wtf.snrcjt.cn

JS:   console.error("err")
来源：http://cyw.yj202588.top

TS:   console.error("err")
来源：http://eyp.nwbrower.top

Java: System.err.println("err")
来源：http://aqq.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pxk.cqqwz.cn

Ruby: warn "err"
来源：http://czk.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://lac.guowangkeji.top

[M07] 判断是否为主入口
来源：http://xrr.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://jsc.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lla.sxryk.cn

JS:   require.main === module
来源：http://jmx.ydjk.org.cn

TS:   require.main === module
来源：http://sgq.zdqjudy.top

Java: public static void main(String[] args)
来源：http://tif.ctjpmb.com

Go:   func main()
来源：http://voe.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gru.bjfxy.top

C#:   static void Main(string[] args)
来源：http://ziz.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://ycy.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://oke.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://nzx.cashguo.top

JS:   process.platform;  process.version
来源：http://srz.tarul.cn

TS:   process.platform;  process.version
来源：http://daf.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mop.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rvh.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dgo.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lqx.pengpengdd.cyou

================================================================================
来源：http://sbu.yangfankeji.com

N. 数据结构与算法
来源：http://yai.jinqigfzy.top

================================================================================
来源：http://kxy.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://wro.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://knu.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vpq.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gss.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uhk.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://ker.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://rqb.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hwy.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://ivs.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://ykm.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://bbj.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nxa.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yry.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qgc.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gsx.ybcxt.top

Go:   slices.Sort(arr)
来源：http://ekz.gogol.net.cn

Ruby: arr.sort
来源：http://qmb.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tem.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://wgk.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qsb.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://ntn.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zgu.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahp.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nxc.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jdq.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pkl.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://gfg.yj20258888.top

[N04] 斐波那契数列
来源：http://zmr.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bpx.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oap.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mnm.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hwi.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bkm.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yvu.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://isn.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xlh.xuanzx.com

[N05] 最大公约数
来源：http://xhn.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://oll.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bly.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixf.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpm.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zwu.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ejx.meibo888.top

Ruby: a.gcd(b)
来源：http://zfg.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://efm.cashguo.top

[N06] 判断回文字符串
来源：http://hpq.jyoumei.cn

Py:   s == s[::-1]
来源：http://vxc.ybcxt.top

PHP:  $s === strrev($s);
来源：http://zqe.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://tih.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://lln.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xtf.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://lcp.0kj1m.cn

Ruby: s == s.reverse
来源：http://tcl.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gqt.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://msl.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rhd.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yqu.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://whu.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://isc.jinqigufen.top

Java: // 手写 HashMap
来源：http://hxl.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://crs.dianchejie.cn

Ruby: // 手写 Hash
来源：http://lmv.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://bwe.ybcxt.top

[N08] 生成全排列
来源：http://pug.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://lqe.sufxvd.cn

PHP:  // 手写递归交换
来源：http://oju.zdbjq.cn

JS:   // 手写回溯递归
来源：http://efu.cucudq.cn

TS:   // 手写回溯递归
来源：http://kjb.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://fdr.ydzc1.top

Go:   // 手写回溯递归
来源：http://kby.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://fpu.zdqjudy.top

C#:   // 手写回溯递归
来源：http://evw.chenzaomai.com

[N09] 栈与队列
来源：http://mug.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kps.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nlc.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lja.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wkp.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jld.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bqt.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uim.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pzh.hysaishi.cn

[N10] 链表节点定义
来源：http://rcn.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://skr.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lbj.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://noa.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sdp.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://fbc.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://joh.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://pnw.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bny.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://mtx.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zxc.yj20258888.top

PHP:  // 手写递归函数
来源：http://grz.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zly.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dsa.bbcook.cn

Java: // 手写递归
来源：http://mzl.chenzaomai.com

Go:   // 手写递归
来源：http://qbe.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tmn.daxiang520.top

C#:   // 手写递归
来源：http://eaq.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mej.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ypl.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zpb.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvx.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://phm.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uwx.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dnc.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mpm.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xtw.yuxming.cn

================================================================================
来源：http://dqm.bjfxy.top

O. 并发与异步
来源：http://mar.fengsongda.top

================================================================================
来源：http://vvh.guowangkeji.top

[O01] 启动一个线程
来源：http://bew.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ydu.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qum.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gvz.nanxuanxn.top

TS:   // 同 JS
来源：http://nzn.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://ouv.chenjidiqi.icu

Go:   go f()
来源：http://flp.xziqi.cn

Ruby: Thread.new { f }
来源：http://dse.sxryk.cn

C#:   Task.Run(() => F());
来源：http://zme.aizwys.cn

[O02] 使用线程池
来源：http://vdn.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gfd.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qlh.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://zho.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://dil.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nby.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wao.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://knj.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wjj.yfazqb.com

[O03] 加锁保护共享数据
来源：http://rlu.jyoumei.cn

Py:   with lock: shared += 1
来源：http://bgk.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://adq.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mxp.jqgufenzy.top

TS:   // 同 JS
来源：http://eic.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://eve.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eqc.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uqo.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://jrj.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://sjx.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://pue.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gdg.hcnkem.com

JS:   async function f() { await g(); }
来源：http://yho.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ioo.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pyk.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xxi.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://dzg.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://qfs.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://sye.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://ggi.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ywi.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://vuy.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://bfu.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fcm.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyt.bjfxy.top

Ruby: threads.map(&:join)
来源：http://cac.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://twb.nwbrower.top

[O06] 使用进程池
来源：http://zyf.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mhz.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uww.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://rfx.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://joz.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ogi.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqi.xuanzx.com

Ruby: // fork 块
来源：http://faj.snrcjt.cn

C#:   Parallel.For
来源：http://gmo.xuetiantiany.cn

================================================================================
来源：http://yaj.nanxuanxn.top

P. 常用工具函数
来源：http://qgp.zycfv.cn

================================================================================
来源：http://gha.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://xyk.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://pgp.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://avb.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://bds.yj20258888.top

TS:   crypto.randomUUID()
来源：http://jbf.yuxming.cn

Java: UUID.randomUUID().toString()
来源：http://puk.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://ymf.cashguo.top

Ruby: SecureRandom.uuid
来源：http://mvj.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://ubv.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://cin.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tnx.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wiv.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tfd.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ses.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vyk.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jso.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sxc.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://syz.uphjek.com

[P03] 生成短随机字符串
来源：http://wbu.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://she.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vtc.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yhy.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vne.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qkw.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lio.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dtr.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hww.svipenyu.cn

[P04] 求长度
来源：http://jas.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tkp.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://swr.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://haf.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://agu.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://ghl.xinyue.icu

Go:   len(arr);  len(m)
来源：http://xup.xylfe.cn

Ruby: x.length;  x.size
来源：http://vju.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://why.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://ydn.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://awn.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cof.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rgk.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zcn.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tcc.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://ywd.haohaochexian.top

Ruby: a == b
来源：http://qrf.svipenyu.cn


<!-- 参考信息 -->