代发 wailian999

C#:   (int)resp.StatusCode
来源：http://rsb.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://mow.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://itj.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://dcc.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sgw.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oma.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cha.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bdm.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rop.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xdw.fanxiaobao.xyz

================================================================================
来源：http://qqx.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://ovc.zhaomingkeji.xyz

================================================================================
来源：http://jjz.9152youxi.cn

[M01] 读取命令行参数
来源：http://ozt.xziqi.cn

Py:   sys.argv[1:]
来源：http://kgy.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://wdv.shuidangran.top

JS:   process.argv.slice(2)
来源：http://yvw.bbcook.cn

TS:   process.argv.slice(2)
来源：http://mpx.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://ogz.zhongyouzk.top

Go:   os.Args[1:]
来源：http://sxv.shangyingyoupin.top

Ruby: ARGV
来源：http://kpu.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://wue.xinyue.icu

[M02] 读取环境变量
来源：http://tfx.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://rds.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ezc.hysaishi.cn

JS:   process.env.HOME
来源：http://kwy.c1oappe.top

TS:   process.env.HOME
来源：http://mhm.9152youxi.cn

Java: System.getenv("HOME")
来源：http://mhf.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jyp.bjfxy.top

Ruby: ENV["HOME"]
来源：http://zme.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cvu.hnqzz.top

[M03] 执行外部命令
来源：http://hwj.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lys.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://irp.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://nmr.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ozb.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ucs.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xfx.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ojt.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://rkt.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://xne.hongshengwenyu.top

Py:   os.getcwd()
来源：http://nez.wangdashe.top

PHP:  getcwd();
来源：http://oab.jqgfzy.top

JS:   process.cwd()
来源：http://xtw.feifeiyinyue.top

TS:   process.cwd()
来源：http://cxh.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://cna.9152youxi.cn

Go:   os.Getwd()
来源：http://ecp.vqdsnc.cn

Ruby: Dir.pwd
来源：http://iyp.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://xcw.cheryme.top

[M05] 设置退出码
来源：http://zff.hcnkem.com

Py:   sys.exit(1)
来源：http://wte.yuanzhike.top

PHP:  exit(1);
来源：http://mkw.aibaodan.cn

JS:   process.exit(1)
来源：http://qxp.hysaishi.cn

TS:   process.exit(1)
来源：http://chp.sjlbkw.cn

Java: System.exit(1)
来源：http://gtt.fehbvm.com

Go:   os.Exit(1)
来源：http://amy.ctjpmb.com

Ruby: exit 1
来源：http://kkm.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cda.uphjek.com

[M06] 向标准错误输出
来源：http://oox.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://oij.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rpp.uphjek.com

JS:   console.error("err")
来源：http://aqb.jlsjyb.cn

TS:   console.error("err")
来源：http://wuk.havefunace.top

Java: System.err.println("err")
来源：http://qlg.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fge.jyoumei.cn

Ruby: warn "err"
来源：http://mci.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://kya.jqgfzy.top

[M07] 判断是否为主入口
来源：http://xdu.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://uqw.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mdl.sweek.top

JS:   require.main === module
来源：http://wkv.iojbl.cn

TS:   require.main === module
来源：http://dqk.daria6918.cn

Java: public static void main(String[] args)
来源：http://tlu.gzhubu.top

Go:   func main()
来源：http://iie.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ucx.cucudq.cn

C#:   static void Main(string[] args)
来源：http://mvm.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://irh.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://mbf.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ohb.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://pxy.yvedp.cn

TS:   process.platform;  process.version
来源：http://rpq.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zgo.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wrq.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ldi.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tzf.sxryk.cn

================================================================================
来源：http://jam.yanxiufei.cn

N. 数据结构与算法
来源：http://bxx.yj20258888.top

================================================================================
来源：http://oyc.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://aqx.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ikn.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://acw.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgh.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wxg.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://gij.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://rfw.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://wsc.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://byq.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://zar.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://nds.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vjc.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://agw.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://jcy.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wfv.tanke756.top

Go:   slices.Sort(arr)
来源：http://lcl.jlsjyb.cn

Ruby: arr.sort
来源：http://pfg.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xaj.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://wtq.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mwl.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://pqu.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ywb.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://owp.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://suu.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qkj.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nuj.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://svq.xziqi.cn

[N04] 斐波那契数列
来源：http://yrs.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxh.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dyt.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sjz.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sii.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rtt.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xon.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iub.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umr.yueranfly.top

[N05] 最大公约数
来源：http://jee.yj202588.top

Py:   math.gcd(a, b)
来源：http://qat.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oxr.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ldh.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gad.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dfu.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wzb.cashguo.top

Ruby: a.gcd(b)
来源：http://nqk.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://drd.0kj1m.cn

[N06] 判断回文字符串
来源：http://ztr.cdnleiting.top

Py:   s == s[::-1]
来源：http://qol.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://yxw.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://ljp.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://ltf.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dvw.yfazqb.com

Go:   // 双指针从两端比较
来源：http://avu.aizwys.cn

Ruby: s == s.reverse
来源：http://bqg.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://kpl.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://cqd.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cvp.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cer.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oje.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://fap.svipenyu.cn

Java: // 手写 HashMap
来源：http://qxr.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://yiy.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://ipk.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mpb.aibaodan.cn

[N08] 生成全排列
来源：http://edh.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://gko.fehbvm.com

PHP:  // 手写递归交换
来源：http://ety.cqqwz.cn

JS:   // 手写回溯递归
来源：http://glz.yuanzhike.top

TS:   // 手写回溯递归
来源：http://bbk.dashuyun.cn

Java: // 手写回溯递归
来源：http://hro.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://pyl.hammf.cn

Ruby: arr.permutation.to_a
来源：http://veb.cucudq.cn

C#:   // 手写回溯递归
来源：http://qwa.zhoulong.xyz

[N09] 栈与队列
来源：http://rle.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ggf.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gvg.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pje.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bns.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lzw.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://obj.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dbg.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yfe.ydzc1.top

[N10] 链表节点定义
来源：http://ltw.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://noz.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://duz.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yhu.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wpz.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://ead.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://cuf.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iru.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ebv.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://iqw.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ylj.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://ihp.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfi.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ztt.jinghuilouyu.cn

Java: // 手写递归
来源：http://hmo.chenjidiqi.icu

Go:   // 手写递归
来源：http://qqc.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eel.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://kwz.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hbi.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baa.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://crw.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hjx.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nzj.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dtz.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://unp.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oiy.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dyr.fktsv.cn

================================================================================
来源：http://ugp.c1oappe.top

O. 并发与异步
来源：http://cef.fehbvm.com

================================================================================
来源：http://wpu.xuanzx.com

[O01] 启动一个线程
来源：http://iae.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ttt.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hlj.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jrv.fktsv.cn

TS:   // 同 JS
来源：http://off.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://riu.guannengcc.top

Go:   go f()
来源：http://isi.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://jzs.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://zqw.sysykeji.top

[O02] 使用线程池
来源：http://pff.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hni.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mtv.zycfv.cn

JS:   // worker_threads 线程池
来源：http://roz.vehdjk.com

TS:   // worker_threads 线程池
来源：http://gut.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://kxx.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vea.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uqr.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://adx.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://lcg.hammf.cn

Py:   with lock: shared += 1
来源：http://eoo.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://ljo.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://doz.kuanghao11.cn

TS:   // 同 JS
来源：http://swb.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://abl.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://khm.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hqb.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://wus.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://xta.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://kvo.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xvw.jianghu66.top

JS:   async function f() { await g(); }
来源：http://mtf.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gvc.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ymk.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://piq.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://jzj.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://qaf.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://gcr.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://amr.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qhz.meibo888.top

JS:   await Promise.all(tasks)
来源：http://qvo.yonumen.top

TS:   await Promise.all(tasks)
来源：http://aqq.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ydm.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://upg.hammf.cn

Ruby: threads.map(&:join)
来源：http://iow.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dvt.daria6918.cn

[O06] 使用进程池
来源：http://aei.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xhh.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jza.tarul.cn

JS:   // child_process / cluster 模块
来源：http://zak.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://fnz.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dpc.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mmw.fanxiaobao.xyz

Ruby: // fork 块
来源：http://tcp.fktsv.cn

C#:   Parallel.For
来源：http://xlr.yuxming.cn

================================================================================
来源：http://ecj.xuetiantiany.cn

P. 常用工具函数
来源：http://kdf.jinyuanbaomall.cn

================================================================================
来源：http://avd.shuidangran.top

[P01] 生成 UUID
来源：http://boi.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://iti.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yej.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://ngm.daxiang520.top

TS:   crypto.randomUUID()
来源：http://ajw.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://mhj.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://mno.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://peu.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://bdc.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://kod.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aeq.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tmz.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wlu.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yto.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fbk.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://txp.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fyj.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lrs.havefunace.top

[P03] 生成短随机字符串
来源：http://voh.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lkc.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qjq.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rbn.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://czq.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tsi.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kdj.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yjd.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vhk.chenjidiqi.icu

[P04] 求长度
来源：http://icg.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://acg.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wkz.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kde.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urx.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://yzl.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://rdm.xuanzx.com

Ruby: x.length;  x.size
来源：http://hwu.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://udd.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://dit.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://riz.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kvj.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dvw.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dtf.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xdp.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://vix.cdnleiting.top

Ruby: a == b
来源：http://zky.c1oappe.top


<!-- 参考信息 -->