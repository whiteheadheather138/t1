代发 wailian999

C#:   (int)resp.StatusCode
来源：http://itw.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://rmd.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzy.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://uas.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pkg.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cxc.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pmg.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nnf.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yyx.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tme.xylfe.cn

================================================================================
来源：http://gfm.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://tvs.zycfv.cn

================================================================================
来源：http://jhq.epnwcf.com

[M01] 读取命令行参数
来源：http://mbe.daxiang520.top

Py:   sys.argv[1:]
来源：http://nbr.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://wtk.uphjek.com

JS:   process.argv.slice(2)
来源：http://txm.bbcook.cn

TS:   process.argv.slice(2)
来源：http://mwk.uphjek.com

Java: args 数组（main 方法参数）
来源：http://ibq.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://nsv.iojbl.cn

Ruby: ARGV
来源：http://gby.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://mcb.daxiang520.top

[M02] 读取环境变量
来源：http://gln.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://gin.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://amg.gotoacloud.top

JS:   process.env.HOME
来源：http://agr.yfazqb.com

TS:   process.env.HOME
来源：http://gyc.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://tjs.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sog.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://gyg.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://idj.ydjk.org.cn

[M03] 执行外部命令
来源：http://gtk.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uxr.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jod.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://thb.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kdb.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hkc.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://cun.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://plj.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://wxy.zhengqikj.top

[M04] 获取当前工作目录
来源：http://ysm.gotoacloud.top

Py:   os.getcwd()
来源：http://wrq.yj202588.top

PHP:  getcwd();
来源：http://zem.nwbrower.top

JS:   process.cwd()
来源：http://yng.ydjk.org.cn

TS:   process.cwd()
来源：http://pxk.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://slh.fehbvm.com

Go:   os.Getwd()
来源：http://hql.shuidangran.top

Ruby: Dir.pwd
来源：http://efj.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ysi.jiagoushi.top

[M05] 设置退出码
来源：http://mrt.jqgfzy.top

Py:   sys.exit(1)
来源：http://dex.yj202588.top

PHP:  exit(1);
来源：http://vat.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://sws.hnxiangtu.top

TS:   process.exit(1)
来源：http://xfq.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://ckj.aizwys.cn

Go:   os.Exit(1)
来源：http://xgl.havefunace.top

Ruby: exit 1
来源：http://xkz.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cee.cheryme.top

[M06] 向标准错误输出
来源：http://mbx.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://zvo.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://yjw.sjlbkw.cn

JS:   console.error("err")
来源：http://coe.hnqzz.top

TS:   console.error("err")
来源：http://wvh.smart0.xyz

Java: System.err.println("err")
来源：http://pzq.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ego.guannengcc.top

Ruby: warn "err"
来源：http://mhu.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://vgo.zhixingplan.top

[M07] 判断是否为主入口
来源：http://udi.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://kjo.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dqi.snrcjt.cn

JS:   require.main === module
来源：http://mhs.ehwqpu.com

TS:   require.main === module
来源：http://mex.smart0.xyz

Java: public static void main(String[] args)
来源：http://dib.fengsongda.top

Go:   func main()
来源：http://uzf.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vmy.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://ddo.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://dwl.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://uck.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://gzb.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://pgu.zhengqikj.top

TS:   process.platform;  process.version
来源：http://xct.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://een.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://jni.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hvh.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ayf.jlsjyb.cn

================================================================================
来源：http://agd.hysaishi.cn

N. 数据结构与算法
来源：http://kht.vqdsnc.cn

================================================================================
来源：http://opu.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://glr.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://bmj.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qmk.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jil.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrg.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://uvy.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://onj.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zmz.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://mxb.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://asm.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://omn.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qad.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rik.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://djk.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ckf.tarul.cn

Go:   slices.Sort(arr)
来源：http://wwc.shuidangran.top

Ruby: arr.sort
来源：http://syr.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nfr.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://pgy.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sen.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://obs.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://agh.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ivp.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qcd.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dbq.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://krw.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://fjm.cucudq.cn

[N04] 斐波那契数列
来源：http://jjg.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zbr.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ofj.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhl.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rrb.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ynm.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ifz.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zva.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://flo.gotoacloud.top

[N05] 最大公约数
来源：http://xxo.ivvv.top

Py:   math.gcd(a, b)
来源：http://gqq.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jvt.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aso.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ofs.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ysr.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iqz.cdnleiting.top

Ruby: a.gcd(b)
来源：http://uxw.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qeg.hesvh.cn

[N06] 判断回文字符串
来源：http://qpt.jianghu66.top

Py:   s == s[::-1]
来源：http://oiz.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://pew.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://rpp.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://see.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rkj.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://dmn.yj202588.top

Ruby: s == s.reverse
来源：http://rzr.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rfb.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://iee.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tmd.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iym.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xps.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://skp.cdnleiting.top

Java: // 手写 HashMap
来源：http://gdu.tarul.cn

Go:   // 手写 map[int]int
来源：http://wsi.tianlin.xyz

Ruby: // 手写 Hash
来源：http://efe.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://tny.jinghuilouyu.cn

[N08] 生成全排列
来源：http://zhc.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://div.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://pai.dianchejie.cn

JS:   // 手写回溯递归
来源：http://hjy.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://guc.sxryk.cn

Java: // 手写回溯递归
来源：http://bzq.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://jnz.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://jrs.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://znq.316326.xyz

[N09] 栈与队列
来源：http://ppy.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wqq.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://spd.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xwo.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jfh.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jdj.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jic.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qok.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xpi.redwolf501.top

[N10] 链表节点定义
来源：http://jgh.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nnh.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eix.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ldw.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bab.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://cby.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://yhz.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wba.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rxq.sysykeji.top

[N11] 二叉树中序遍历
来源：http://qsg.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ojy.zdqjudy.top

PHP:  // 手写递归函数
来源：http://znf.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yyi.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xrm.nanxuanxn.top

Java: // 手写递归
来源：http://jbz.vqdsnc.cn

Go:   // 手写递归
来源：http://yef.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zzr.yfazqb.com

C#:   // 手写递归
来源：http://vhj.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ixq.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gng.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygr.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rhw.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://plx.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mzb.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xhs.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kxb.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://riu.wangshuangyany.cn

================================================================================
来源：http://zsg.yuanzhike.top

O. 并发与异步
来源：http://qen.fanxiaobao.xyz

================================================================================
来源：http://oke.gaohongyu789.top

[O01] 启动一个线程
来源：http://kdd.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ine.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mcn.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hnc.yanxiufei.cn

TS:   // 同 JS
来源：http://oiq.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://cyt.sufxvd.cn

Go:   go f()
来源：http://kic.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://ity.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://cts.yueranfly.top

[O02] 使用线程池
来源：http://zzz.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cho.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gfl.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://uke.aizwys.cn

TS:   // worker_threads 线程池
来源：http://ahq.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://slm.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abf.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iky.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gui.c1oappe.top

[O03] 加锁保护共享数据
来源：http://dxe.yuanzhike.top

Py:   with lock: shared += 1
来源：http://tor.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://aho.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mjn.jianghu66.top

TS:   // 同 JS
来源：http://vou.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://ync.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gsr.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lhb.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://ogp.hesvh.cn

[O04] 定义异步函数并等待
来源：http://gac.sweek.top

Py:   async def f():⏎    await g()
来源：http://zmp.xuetiantiany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kwf.yj202588.top

JS:   async function f() { await g(); }
来源：http://cqv.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fan.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mzr.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pvc.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://dcz.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://iue.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://rvf.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://txm.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ufk.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://jdr.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://hwa.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dhb.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mnl.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://ffe.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://igh.gotoacloud.top

[O06] 使用进程池
来源：http://gjy.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tof.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xyl.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://vas.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://fbk.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jtx.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jcg.smart0.xyz

Ruby: // fork 块
来源：http://jtr.uphjek.com

C#:   Parallel.For
来源：http://hzi.zhiwuduotai.top

================================================================================
来源：http://crd.zhiwuduotai.top

P. 常用工具函数
来源：http://xhn.yangfankeji.com

================================================================================
来源：http://syr.iojbl.cn

[P01] 生成 UUID
来源：http://ggj.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://ojj.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cof.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://unf.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://axr.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://tcw.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://mkm.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://tcm.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://xkc.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://lfu.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hwc.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kzz.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oga.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://opc.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qsb.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://krs.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cyt.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qnd.snrcjt.cn

[P03] 生成短随机字符串
来源：http://kka.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://but.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ioa.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lhn.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wbx.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yay.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tlw.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bvj.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://njj.gogol.net.cn

[P04] 求长度
来源：http://ztz.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zet.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wkx.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yko.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jra.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://iud.ydzc1.top

Go:   len(arr);  len(m)
来源：http://gte.jqgfzy.top

Ruby: x.length;  x.size
来源：http://nva.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lnm.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://jim.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lcu.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ujp.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rsh.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vow.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kbl.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://umg.yj20258888.top

Ruby: a == b
来源：http://oom.yongpay.top


<!-- 参考信息 -->