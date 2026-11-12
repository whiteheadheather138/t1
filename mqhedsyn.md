代发 wailian999

TS:   resp.ok;  resp.status
来源：http://whx.fktsv.cn

Java: resp.statusCode()
来源：http://zbw.smart0.xyz

Go:   resp.StatusCode
来源：http://utk.aizwys.cn

Ruby: resp.code.to_i
来源：http://lrs.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://hfs.aizwys.cn

[L08] 并发请求多个地址
来源：http://pbh.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lcu.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://dtz.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lcc.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hin.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zrz.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://avt.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kpm.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uea.shangyingyoupin.top

================================================================================
来源：http://cca.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://ggi.zhongyouzk.top

================================================================================
来源：http://vyr.gogol.net.cn

[M01] 读取命令行参数
来源：http://xyp.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://owa.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://aqd.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://tag.316326.xyz

TS:   process.argv.slice(2)
来源：http://xfw.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://pba.sweek.top

Go:   os.Args[1:]
来源：http://xmx.jinghuilouyu.cn

Ruby: ARGV
来源：http://hxn.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://qmi.cqqwz.cn

[M02] 读取环境变量
来源：http://imv.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://lwu.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://upt.hcnkem.com

JS:   process.env.HOME
来源：http://hqi.xziqi.cn

TS:   process.env.HOME
来源：http://fak.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://whv.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wvb.birdmap.top

Ruby: ENV["HOME"]
来源：http://txy.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kta.jyoumei.cn

[M03] 执行外部命令
来源：http://bhc.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xlc.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ick.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pyl.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gab.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hlk.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ang.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://alb.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://myo.zycfv.cn

[M04] 获取当前工作目录
来源：http://ptg.gogol.net.cn

Py:   os.getcwd()
来源：http://hwi.yj202588.top

PHP:  getcwd();
来源：http://ghl.sufxvd.cn

JS:   process.cwd()
来源：http://jad.yangfankeji.com

TS:   process.cwd()
来源：http://fzf.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://jau.nanxuanxn.top

Go:   os.Getwd()
来源：http://biu.cucudq.cn

Ruby: Dir.pwd
来源：http://bst.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://flv.sysykeji.top

[M05] 设置退出码
来源：http://mep.smart0.xyz

Py:   sys.exit(1)
来源：http://pva.shzxlz.cn

PHP:  exit(1);
来源：http://ziz.pengpengdd.cyou

JS:   process.exit(1)
来源：http://zmx.bjfxy.top

TS:   process.exit(1)
来源：http://lrk.316326.xyz

Java: System.exit(1)
来源：http://bfs.tian-w.cn

Go:   os.Exit(1)
来源：http://zjn.cqqwz.cn

Ruby: exit 1
来源：http://chz.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ucf.ybcxt.top

[M06] 向标准错误输出
来源：http://zxv.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://fqr.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gdy.zdqjudy.top

JS:   console.error("err")
来源：http://dxp.sufxvd.cn

TS:   console.error("err")
来源：http://eok.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://wcd.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xiy.yanxiufei.cn

Ruby: warn "err"
来源：http://wjz.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://ada.xylfe.cn

[M07] 判断是否为主入口
来源：http://roj.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://hoi.vqdsnc.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mle.cheryme.top

JS:   require.main === module
来源：http://tcu.feifeiyinyue.top

TS:   require.main === module
来源：http://ryd.yj202588.top

Java: public static void main(String[] args)
来源：http://bpd.aibaodan.cn

Go:   func main()
来源：http://eww.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uwc.uphjek.com

C#:   static void Main(string[] args)
来源：http://ewx.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://kfu.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://bcr.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://kdj.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://dvw.hywenlv.cn

TS:   process.platform;  process.version
来源：http://bpw.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nnx.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://igx.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pzy.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jkq.aibaodan.cn

================================================================================
来源：http://qcf.hnqzz.top

N. 数据结构与算法
来源：http://ren.ctjpmb.com

================================================================================
来源：http://ofq.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://lpb.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://wge.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sjl.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vyn.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eiu.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://ypq.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://xiz.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ikz.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://pmt.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://bsv.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://lgy.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gst.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qmt.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ijh.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nym.yonumen.top

Go:   slices.Sort(arr)
来源：http://itb.shangyingyoupin.top

Ruby: arr.sort
来源：http://jjv.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dzl.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://wnu.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zzg.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://vbz.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://chm.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxj.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yfg.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gig.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pld.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wno.sufxvd.cn

[N04] 斐波那契数列
来源：http://eim.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vwo.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lnf.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vsx.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://evc.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zhh.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ftp.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ptc.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eff.shzxlz.cn

[N05] 最大公约数
来源：http://akj.sxryk.cn

Py:   math.gcd(a, b)
来源：http://xdm.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qok.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ily.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlu.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iqg.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bzy.yonumen.top

Ruby: a.gcd(b)
来源：http://dce.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tyl.zhijiandao.cn

[N06] 判断回文字符串
来源：http://myj.hesvh.cn

Py:   s == s[::-1]
来源：http://zmf.cucudq.cn

PHP:  $s === strrev($s);
来源：http://zjs.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://vwr.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://wmb.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tlb.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://ujc.zhijiandao.cn

Ruby: s == s.reverse
来源：http://oqq.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://cnw.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://chz.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zze.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rrg.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fuh.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://kyn.daxiang520.top

Java: // 手写 HashMap
来源：http://zaf.meibo888.top

Go:   // 手写 map[int]int
来源：http://jcf.cqqwz.cn

Ruby: // 手写 Hash
来源：http://jbb.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://etq.fktsv.cn

[N08] 生成全排列
来源：http://ops.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://pjz.jqgfzy.top

PHP:  // 手写递归交换
来源：http://nyq.ydzc1.top

JS:   // 手写回溯递归
来源：http://pct.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://sqh.cheryme.top

Java: // 手写回溯递归
来源：http://typ.xuanzx.com

Go:   // 手写回溯递归
来源：http://fwq.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://ckp.jqgfzy.top

C#:   // 手写回溯递归
来源：http://slu.ehwqpu.com

[N09] 栈与队列
来源：http://vau.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sud.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://afp.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvn.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://saf.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ghl.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kst.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vvs.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vmy.fehbvm.com

[N10] 链表节点定义
来源：http://qwy.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yln.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://squ.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xrl.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://smb.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://vsm.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://xiu.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://roc.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://unc.aizwys.cn

[N11] 二叉树中序遍历
来源：http://ujh.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://flc.guowangkeji.top

PHP:  // 手写递归函数
来源：http://ggh.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfd.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpp.feifeiyinyue.top

Java: // 手写递归
来源：http://lip.dianchejie.cn

Go:   // 手写递归
来源：http://dzj.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xpw.yvedp.cn

C#:   // 手写递归
来源：http://gfe.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vjw.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbr.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vcp.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gsx.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xuv.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lxt.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lvb.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://snx.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zxg.uphjek.com

================================================================================
来源：http://omn.yonumen.top

O. 并发与异步
来源：http://hcz.fanxiaobao.xyz

================================================================================
来源：http://dlk.52xcode.cn

[O01] 启动一个线程
来源：http://zps.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jfr.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wyc.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hdt.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://owz.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://eot.ppjwa.cn

Go:   go f()
来源：http://clk.hesvh.cn

Ruby: Thread.new { f }
来源：http://bzq.xziqi.cn

C#:   Task.Run(() => F());
来源：http://tud.bjfxy.top

[O02] 使用线程池
来源：http://zqy.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ukm.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kar.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://trl.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://evk.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://msd.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mtu.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cap.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://imx.jianghu66.top

[O03] 加锁保护共享数据
来源：http://ijq.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://kva.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://qcd.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rnd.hnqzz.top

TS:   // 同 JS
来源：http://dok.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://gbe.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qnz.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://syr.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://cmk.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://gmx.cheryme.top

Py:   async def f():⏎    await g()
来源：http://ykf.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lnn.yueranfly.top

JS:   async function f() { await g(); }
来源：http://kjz.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ogr.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yoq.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://raz.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://byu.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://ttd.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://sfi.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://oiz.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://epi.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://nml.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://ejk.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uuj.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ckp.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://esh.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://nah.yj202588.top

[O06] 使用进程池
来源：http://nkt.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tcc.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://chu.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://fql.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://vwf.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ewx.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bbz.ctjpmb.com

Ruby: // fork 块
来源：http://byy.andypj.xyz

C#:   Parallel.For
来源：http://nfh.guannengcc.top

================================================================================
来源：http://coq.meibo888.top

P. 常用工具函数
来源：http://fat.ydzc1.top

================================================================================
来源：http://amh.sufxvd.cn

[P01] 生成 UUID
来源：http://ttj.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://pld.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://imx.bjfxy.top

JS:   crypto.randomUUID()
来源：http://phe.yj20258.top

TS:   crypto.randomUUID()
来源：http://mqi.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://bqm.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://gul.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://vkd.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://cwe.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://euy.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kpx.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eam.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://stn.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vlg.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://shm.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ncc.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lvx.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ids.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://byq.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://krs.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tec.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfq.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dum.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://htl.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ypz.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nbv.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iug.jinqigfzy.top

[P04] 求长度
来源：http://mtz.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pdi.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zkg.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hga.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zyk.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://nif.birdmap.top

Go:   len(arr);  len(m)
来源：http://fhc.yj20258.top

Ruby: x.length;  x.size
来源：http://uqa.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xpl.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://ans.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://ama.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eze.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rlg.316326.xyz


<!-- 参考信息 -->