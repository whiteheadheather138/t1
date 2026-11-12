代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://ere.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nth.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yru.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://rjx.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://yty.hcnkem.com

Java: resp.statusCode()
来源：http://crg.dashuyun.cn

Go:   resp.StatusCode
来源：http://sdx.sysykeji.top

Ruby: resp.code.to_i
来源：http://cgv.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://blt.ppjwa.cn

[L08] 并发请求多个地址
来源：http://mfa.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dmp.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://oma.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ole.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pve.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hbm.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://emp.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ave.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fdg.kuanghao11.cn

================================================================================
来源：http://vpp.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://rdd.uphjek.com

================================================================================
来源：http://cpb.yj202588.top

[M01] 读取命令行参数
来源：http://put.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://ocd.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://fpd.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://bvj.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://bkg.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://apo.52xcode.cn

Go:   os.Args[1:]
来源：http://ofl.sjlbkw.cn

Ruby: ARGV
来源：http://swv.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://vur.uphjek.com

[M02] 读取环境变量
来源：http://ehl.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://wog.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bbg.havefunace.top

JS:   process.env.HOME
来源：http://qxp.yangfankeji.com

TS:   process.env.HOME
来源：http://oaw.andypj.xyz

Java: System.getenv("HOME")
来源：http://vci.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rsr.meibo888.top

Ruby: ENV["HOME"]
来源：http://cat.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sck.ctjpmb.com

[M03] 执行外部命令
来源：http://ugg.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kma.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xnv.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gic.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ocg.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blr.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nux.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://ehj.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://sdo.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://sjt.kuanghao11.cn

Py:   os.getcwd()
来源：http://ick.sxryk.cn

PHP:  getcwd();
来源：http://wwm.jqgfzy.top

JS:   process.cwd()
来源：http://ezg.shanyushiyangtech.top

TS:   process.cwd()
来源：http://kxg.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://wwg.sweek.top

Go:   os.Getwd()
来源：http://ayu.cdnleiting.top

Ruby: Dir.pwd
来源：http://swq.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ytg.jinghuilouyu.cn

[M05] 设置退出码
来源：http://tcc.nanxinkj.top

Py:   sys.exit(1)
来源：http://bvq.tian-w.cn

PHP:  exit(1);
来源：http://dgx.sysykeji.top

JS:   process.exit(1)
来源：http://xen.chenzaomai.com

TS:   process.exit(1)
来源：http://nhn.vqdsnc.cn

Java: System.exit(1)
来源：http://cez.yuxming.cn

Go:   os.Exit(1)
来源：http://vuo.ydjk.org.cn

Ruby: exit 1
来源：http://hib.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qwq.yj20258888.top

[M06] 向标准错误输出
来源：http://wft.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://ynn.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yyo.cdnleiting.top

JS:   console.error("err")
来源：http://hxp.tianlin.xyz

TS:   console.error("err")
来源：http://gfl.vehdjk.com

Java: System.err.println("err")
来源：http://pmk.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvo.cqqwz.cn

Ruby: warn "err"
来源：http://zhi.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://ztt.zdqjudy.top

[M07] 判断是否为主入口
来源：http://jyd.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://gib.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yhs.ywan-chungtsiang.top

JS:   require.main === module
来源：http://czm.cdnleiting.top

TS:   require.main === module
来源：http://vmy.yj202588.top

Java: public static void main(String[] args)
来源：http://dvw.fehbvm.com

Go:   func main()
来源：http://mqf.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lam.ybcxt.top

C#:   static void Main(string[] args)
来源：http://tst.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://uud.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://qsk.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://mdm.hfpthk.cn

JS:   process.platform;  process.version
来源：http://ofu.dianchejie.cn

TS:   process.platform;  process.version
来源：http://uhe.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gdi.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://avn.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zek.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nbu.havefunace.top

================================================================================
来源：http://qiu.nanxuanxn.top

N. 数据结构与算法
来源：http://fok.316326.xyz

================================================================================
来源：http://xjv.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://bzb.yangfankeji.com

Py:   bisect.bisect_left(arr, x)
来源：http://wip.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nrq.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://djv.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mzx.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tzq.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://idp.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kkp.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dmx.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://nqc.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://jsm.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ilo.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ldt.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://znp.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pak.yvedp.cn

Go:   slices.Sort(arr)
来源：http://dcl.yongpay.top

Ruby: arr.sort
来源：http://ele.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hse.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://qer.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xkk.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://pii.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqv.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://djp.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uzu.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sld.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rtw.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://usk.smart0.xyz

[N04] 斐波那契数列
来源：http://esi.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://duj.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dul.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cfx.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hou.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pty.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ezq.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://grc.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wuw.yueranfly.top

[N05] 最大公约数
来源：http://aoe.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://oeq.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tbh.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xay.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fnd.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jxi.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://poy.ppjwa.cn

Ruby: a.gcd(b)
来源：http://laf.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://erh.ydjk.org.cn

[N06] 判断回文字符串
来源：http://dgf.haohaochexian.top

Py:   s == s[::-1]
来源：http://vhk.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://ibs.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://whu.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://gxl.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jkj.tarul.cn

Go:   // 双指针从两端比较
来源：http://iao.svipenyu.cn

Ruby: s == s.reverse
来源：http://xln.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fdp.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://jvj.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pxg.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gzo.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ixa.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://avz.zycfv.cn

Java: // 手写 HashMap
来源：http://abv.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://ocn.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://hro.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://bct.ctjpmb.com

[N08] 生成全排列
来源：http://rdm.sweek.top

Py:   itertools.permutations(arr)
来源：http://pli.redwolf501.top

PHP:  // 手写递归交换
来源：http://itp.birdmap.top

JS:   // 手写回溯递归
来源：http://fcf.mhx1999.top

TS:   // 手写回溯递归
来源：http://jjm.xylfe.cn

Java: // 手写回溯递归
来源：http://ccn.redwolf501.top

Go:   // 手写回溯递归
来源：http://ont.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://oqt.bbcook.cn

C#:   // 手写回溯递归
来源：http://ivy.chenjidiqi.icu

[N09] 栈与队列
来源：http://lig.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kjb.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bvx.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ynn.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yde.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://msl.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qxq.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://czv.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://riv.ctjpmb.com

[N10] 链表节点定义
来源：http://vhh.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zif.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kzp.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zsf.xuanzx.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qep.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://vvl.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://car.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://aza.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zzi.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://qjk.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fxh.xinyue.icu

PHP:  // 手写递归函数
来源：http://tlh.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fkk.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lcm.jinqigfzy.top

Java: // 手写递归
来源：http://otd.wangshuangyany.cn

Go:   // 手写递归
来源：http://vwc.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vvc.yanxiufei.cn

C#:   // 手写递归
来源：http://oju.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xfd.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cfx.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zqn.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://png.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dud.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wsd.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kpz.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://amr.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dnw.gaohongyu789.top

================================================================================
来源：http://dev.cucudq.cn

O. 并发与异步
来源：http://msd.gzhubu.top

================================================================================
来源：http://wqb.yfazqb.com

[O01] 启动一个线程
来源：http://ssu.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ibe.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cph.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vpc.meibo888.top

TS:   // 同 JS
来源：http://vir.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://adv.gaohongyu789.top

Go:   go f()
来源：http://ovl.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://cqx.316326.xyz

C#:   Task.Run(() => F());
来源：http://pbv.cashguo.top

[O02] 使用线程池
来源：http://buy.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://var.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uae.daxiang520.top

JS:   // worker_threads 线程池
来源：http://jxi.pycfn.com

TS:   // worker_threads 线程池
来源：http://uxm.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://ecx.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xpv.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tpt.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cyw.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://uqg.xinyue.icu

Py:   with lock: shared += 1
来源：http://nbv.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://zds.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ajz.jqgfzy.top

TS:   // 同 JS
来源：http://fpz.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://eqn.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sld.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://orr.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://zwx.redwolf501.top

[O04] 定义异步函数并等待
来源：http://vcw.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://rfl.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dlt.daxiang520.top

JS:   async function f() { await g(); }
来源：http://ait.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://uts.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mge.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fci.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tpo.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://pnb.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://riz.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://fzl.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://juz.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://nbv.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://gqv.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bdy.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aql.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://ayq.yangfankeji.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sas.haohaochexian.top

[O06] 使用进程池
来源：http://pvn.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qhq.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://swl.pycfn.com

JS:   // child_process / cluster 模块
来源：http://deh.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://twj.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qni.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wkn.wangdashe.top

Ruby: // fork 块
来源：http://pyg.andypj.xyz

C#:   Parallel.For
来源：http://opb.yvedp.cn

================================================================================
来源：http://iqf.xylfe.cn

P. 常用工具函数
来源：http://vtq.hywenlv.cn

================================================================================
来源：http://wvh.aibaodan.cn

[P01] 生成 UUID
来源：http://wzz.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://pmx.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sap.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://woy.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://qpr.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://lna.0kj1m.cn

Go:   // 用 github.com/google/uuid
来源：http://dbh.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://ayd.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://koi.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://gsf.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vro.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tsi.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ply.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dkf.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ouu.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lls.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wko.zhaomingkeji.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://enx.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://xfx.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mad.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sbx.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ifh.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wfy.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vor.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xvx.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bar.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lev.havefunace.top

[P04] 求长度
来源：http://fbp.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qvv.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nje.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wkb.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qao.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://hfm.sysykeji.top

Go:   len(arr);  len(m)
来源：http://zlj.yangfankeji.com

Ruby: x.length;  x.size
来源：http://nkc.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://bko.jinqigfzy.top


<!-- 参考信息 -->