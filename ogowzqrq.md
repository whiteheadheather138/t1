代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://tjz.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lod.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kgg.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://isg.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://flv.guowangkeji.top

Java: resp.statusCode()
来源：http://atm.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://tsq.yj202588.top

Ruby: resp.code.to_i
来源：http://nbu.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://mos.yj202588.top

[L08] 并发请求多个地址
来源：http://qca.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zuk.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://jao.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rnc.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfo.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ejf.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dzs.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oav.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yig.bbcook.cn

================================================================================
来源：http://ruj.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://tku.xingfuxueyuan.xyz

================================================================================
来源：http://rpv.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://byw.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://fmf.yonumen.top

PHP:  $argv;  $argc;
来源：http://qal.mhx1999.top

JS:   process.argv.slice(2)
来源：http://yno.smart0.xyz

TS:   process.argv.slice(2)
来源：http://hpu.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://cxm.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://yqb.fanxiaobao.xyz

Ruby: ARGV
来源：http://tsq.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://qec.cashguo.top

[M02] 读取环境变量
来源：http://fzh.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://qki.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rjd.epnwcf.com

JS:   process.env.HOME
来源：http://acv.52xcode.cn

TS:   process.env.HOME
来源：http://hwg.ppjwa.cn

Java: System.getenv("HOME")
来源：http://uve.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://opl.daxiang520.top

Ruby: ENV["HOME"]
来源：http://ukv.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://smr.zhoulong.xyz

[M03] 执行外部命令
来源：http://ech.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eec.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kft.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://mfx.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yoa.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mbr.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://shg.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://zns.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://ral.wangdashe.top

[M04] 获取当前工作目录
来源：http://krs.9152youxi.cn

Py:   os.getcwd()
来源：http://brw.gaohongyu789.top

PHP:  getcwd();
来源：http://mav.zycfv.cn

JS:   process.cwd()
来源：http://qkf.iojbl.cn

TS:   process.cwd()
来源：http://jjw.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://uxi.epnwcf.com

Go:   os.Getwd()
来源：http://rsu.ydzc1.top

Ruby: Dir.pwd
来源：http://jlz.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tvz.zdqjudy.top

[M05] 设置退出码
来源：http://sjg.sysykeji.top

Py:   sys.exit(1)
来源：http://sgx.gaohongyu789.top

PHP:  exit(1);
来源：http://een.tian-w.cn

JS:   process.exit(1)
来源：http://okd.xuanzx.com

TS:   process.exit(1)
来源：http://vxr.tianlin.xyz

Java: System.exit(1)
来源：http://cjk.ydzc1.top

Go:   os.Exit(1)
来源：http://vub.cheryme.top

Ruby: exit 1
来源：http://qlq.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rnq.jqgfzy.top

[M06] 向标准错误输出
来源：http://wxv.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://uwh.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aod.jinqigfzy.top

JS:   console.error("err")
来源：http://udt.sjlbkw.cn

TS:   console.error("err")
来源：http://dcn.fzhhl.top

Java: System.err.println("err")
来源：http://ybl.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xfi.sweek.top

Ruby: warn "err"
来源：http://ukf.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://izc.hfpthk.cn

[M07] 判断是否为主入口
来源：http://rjm.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://gui.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nmk.wangdashe.top

JS:   require.main === module
来源：http://adh.tian-w.cn

TS:   require.main === module
来源：http://sqm.hysaishi.cn

Java: public static void main(String[] args)
来源：http://aej.vqdsnc.cn

Go:   func main()
来源：http://alf.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hhx.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://vle.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://ntp.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://oio.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://cfv.pycfn.com

JS:   process.platform;  process.version
来源：http://aoc.hfpthk.cn

TS:   process.platform;  process.version
来源：http://int.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lta.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yrb.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xil.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xjw.zycfv.cn

================================================================================
来源：http://ywz.fengsongda.top

N. 数据结构与算法
来源：http://svk.yj20258888.top

================================================================================
来源：http://ttp.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://weq.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cdw.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qzs.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmb.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lqq.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://rnd.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://lye.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mvc.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://dcn.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://zzp.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://ixk.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rnj.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kia.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ooe.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dzj.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://wgm.yfazqb.com

Ruby: arr.sort
来源：http://xje.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jsk.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://ksp.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vsc.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://aip.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hkg.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gib.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bsp.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lxr.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vtc.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://obl.cqqwz.cn

[N04] 斐波那契数列
来源：http://gvh.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://drw.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://afl.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vxn.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bep.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fag.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pld.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxw.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fmd.vqdsnc.cn

[N05] 最大公约数
来源：http://noz.hammf.cn

Py:   math.gcd(a, b)
来源：http://dbv.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qip.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jcu.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eff.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://awm.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://utm.svipenyu.cn

Ruby: a.gcd(b)
来源：http://nrd.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://imp.guowangkeji.top

[N06] 判断回文字符串
来源：http://shw.dianchejie.cn

Py:   s == s[::-1]
来源：http://pll.yvedp.cn

PHP:  $s === strrev($s);
来源：http://qrj.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://bua.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://dgy.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cqt.gzhubu.top

Go:   // 双指针从两端比较
来源：http://nbw.zycfv.cn

Ruby: s == s.reverse
来源：http://wva.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ghq.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://oqa.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zly.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mlw.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nop.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://til.dianchejie.cn

Java: // 手写 HashMap
来源：http://vxd.vehdjk.com

Go:   // 手写 map[int]int
来源：http://evr.meibo888.top

Ruby: // 手写 Hash
来源：http://zdz.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oyr.gaohongyu789.top

[N08] 生成全排列
来源：http://kwe.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://hja.aizwys.cn

PHP:  // 手写递归交换
来源：http://zjs.tanke756.top

JS:   // 手写回溯递归
来源：http://boj.yueranfly.top

TS:   // 手写回溯递归
来源：http://kal.zhoulong.xyz

Java: // 手写回溯递归
来源：http://bty.52xcode.cn

Go:   // 手写回溯递归
来源：http://cay.sweek.top

Ruby: arr.permutation.to_a
来源：http://uyt.yangfankeji.com

C#:   // 手写回溯递归
来源：http://xae.gogol.net.cn

[N09] 栈与队列
来源：http://sog.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mgd.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wfd.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ojg.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lwi.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iug.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hip.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yma.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qzd.svipenyu.cn

[N10] 链表节点定义
来源：http://goi.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bzo.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wbm.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qzm.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ypl.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://rbn.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://gtk.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wdi.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iln.bbcook.cn

[N11] 二叉树中序遍历
来源：http://bsb.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jun.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://bub.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zag.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czm.daria6918.cn

Java: // 手写递归
来源：http://uph.wangdashe.top

Go:   // 手写递归
来源：http://kkw.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vus.hysaishi.cn

C#:   // 手写递归
来源：http://hft.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lol.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bth.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nbg.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zpn.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ysr.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nwk.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rnz.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://toz.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cyw.hfpthk.cn

================================================================================
来源：http://nut.wangdashe.top

O. 并发与异步
来源：http://paw.uphjek.com

================================================================================
来源：http://vsw.yanxiufei.cn

[O01] 启动一个线程
来源：http://joj.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dae.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pmo.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yqt.uphjek.com

TS:   // 同 JS
来源：http://orz.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://ahe.zhaomingkeji.xyz

Go:   go f()
来源：http://hgl.aibaodan.cn

Ruby: Thread.new { f }
来源：http://dqw.vehdjk.com

C#:   Task.Run(() => F());
来源：http://rgo.shanyushiyangtech.top

[O02] 使用线程池
来源：http://zyn.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bhv.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fne.yongpay.top

JS:   // worker_threads 线程池
来源：http://wda.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://uep.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://bjw.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vax.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kld.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jki.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://vzv.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://qcg.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://tas.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wdm.sxryk.cn

TS:   // 同 JS
来源：http://tnw.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://egs.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://reu.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://akz.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://oof.hesvh.cn

[O04] 定义异步函数并等待
来源：http://hib.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://udc.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xia.smart0.xyz

JS:   async function f() { await g(); }
来源：http://rkm.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kcq.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qrl.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jlv.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nvt.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://fgm.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://ufv.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://mbs.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://woo.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://ozi.ivvv.top

TS:   await Promise.all(tasks)
来源：http://epp.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dvj.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nvq.uphjek.com

Ruby: threads.map(&:join)
来源：http://poz.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ffx.ybcxt.top

[O06] 使用进程池
来源：http://abp.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wra.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ayo.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://ucj.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://jcd.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pli.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mmn.pycfn.com

Ruby: // fork 块
来源：http://tnx.redwolf501.top

C#:   Parallel.For
来源：http://uil.xziqi.cn

================================================================================
来源：http://jzl.xuanzx.com

P. 常用工具函数
来源：http://lbu.redwolf501.top

================================================================================
来源：http://vwo.tian-w.cn

[P01] 生成 UUID
来源：http://grm.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://wea.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xqz.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://ikf.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://lzo.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://fnc.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://xef.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://ysd.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://vnb.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://vgg.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kef.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://agv.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wrw.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fgb.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ksv.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rai.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://age.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ntz.pycfn.com

[P03] 生成短随机字符串
来源：http://yqz.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qdg.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iwj.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lck.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwt.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oaz.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xpv.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gbf.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qjl.yongpay.top

[P04] 求长度
来源：http://xuu.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://enm.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wdh.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xks.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fli.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://joe.316326.xyz

Go:   len(arr);  len(m)
来源：http://cqu.sweek.top

Ruby: x.length;  x.size
来源：http://ilp.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pft.ybcxt.top


<!-- 参考信息 -->