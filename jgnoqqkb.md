代发 wailian999

TS:   resp.ok;  resp.status
来源：http://jmi.pengpengdd.cyou

Java: resp.statusCode()
来源：http://yuz.yangfankeji.com

Go:   resp.StatusCode
来源：http://qcb.epnwcf.com

Ruby: resp.code.to_i
来源：http://shh.yj20258.top

C#:   (int)resp.StatusCode
来源：http://vze.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://wjd.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tdi.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://gnq.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxv.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dbf.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gtq.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yph.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://koj.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wbm.yueranfly.top

================================================================================
来源：http://vtu.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://icc.yongpay.top

================================================================================
来源：http://avm.hnxiangtu.top

[M01] 读取命令行参数
来源：http://kiv.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://hfj.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://hfg.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://emi.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://mft.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://ady.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://rix.52xcode.cn

Ruby: ARGV
来源：http://epz.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://jbv.yuanzhike.top

[M02] 读取环境变量
来源：http://xqb.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://gvd.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gsq.chenzaomai.com

JS:   process.env.HOME
来源：http://ony.cdnleiting.top

TS:   process.env.HOME
来源：http://yxe.fzhhl.top

Java: System.getenv("HOME")
来源：http://uvk.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iny.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://jxc.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gza.cdnleiting.top

[M03] 执行外部命令
来源：http://jdx.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ano.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uaz.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://glj.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rqd.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fbl.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yfs.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://wzh.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://opp.aizwys.cn

[M04] 获取当前工作目录
来源：http://ehm.zycfv.cn

Py:   os.getcwd()
来源：http://jtk.hnxiangtu.top

PHP:  getcwd();
来源：http://hei.guannengcc.top

JS:   process.cwd()
来源：http://lou.pycfn.com

TS:   process.cwd()
来源：http://ikr.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://kpn.snrcjt.cn

Go:   os.Getwd()
来源：http://bsw.nwbrower.top

Ruby: Dir.pwd
来源：http://ojs.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://eqa.zdbjq.cn

[M05] 设置退出码
来源：http://riv.smart0.xyz

Py:   sys.exit(1)
来源：http://lwv.hnqzz.top

PHP:  exit(1);
来源：http://eeb.yvedp.cn

JS:   process.exit(1)
来源：http://nxr.sxryk.cn

TS:   process.exit(1)
来源：http://moq.gzhubu.top

Java: System.exit(1)
来源：http://vcl.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://yzn.shanyushiyangtech.top

Ruby: exit 1
来源：http://udl.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ajt.yuxming.cn

[M06] 向标准错误输出
来源：http://olg.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://pil.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lhp.yvedp.cn

JS:   console.error("err")
来源：http://bhd.kuanghao11.cn

TS:   console.error("err")
来源：http://ieo.zhongyouzk.top

Java: System.err.println("err")
来源：http://asq.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eve.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://ftc.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://ntf.yuanzhike.top

[M07] 判断是否为主入口
来源：http://ssu.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://tsn.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rzd.daxiang520.top

JS:   require.main === module
来源：http://gic.feifeiyinyue.top

TS:   require.main === module
来源：http://eqs.nwbrower.top

Java: public static void main(String[] args)
来源：http://qve.xylfe.cn

Go:   func main()
来源：http://kxo.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdt.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://lcz.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://lto.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://uhh.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://knu.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://htv.zdqjudy.top

TS:   process.platform;  process.version
来源：http://zlh.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fff.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wis.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fur.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgt.jlsjyb.cn

================================================================================
来源：http://fdf.quarkkingdee.top

N. 数据结构与算法
来源：http://npq.shanyushiyangkeji.top

================================================================================
来源：http://sic.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://mfv.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://vgc.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://czl.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wru.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjb.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://nra.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://pai.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zgv.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://jqp.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://hyi.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://jnm.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gtt.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://aqu.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gpr.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ebj.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://fio.hesvh.cn

Ruby: arr.sort
来源：http://hje.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pll.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://ttr.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mpl.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://bfq.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbk.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghh.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://que.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cvp.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wsj.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://grx.hfpthk.cn

[N04] 斐波那契数列
来源：http://xhz.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tfg.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://glj.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://msp.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oiq.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://guo.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vno.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pzq.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sfi.haohaochexian.top

[N05] 最大公约数
来源：http://adw.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://fgc.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kjq.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://enq.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edv.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uuy.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://elk.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://hpv.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vny.ydjk.org.cn

[N06] 判断回文字符串
来源：http://jne.gogol.net.cn

Py:   s == s[::-1]
来源：http://pde.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://ekr.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://awh.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://zyx.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ibf.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://vyy.quarkkingdee.top

Ruby: s == s.reverse
来源：http://ssw.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://okj.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://hkt.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pku.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ftz.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xcc.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://jye.xuanzx.com

Java: // 手写 HashMap
来源：http://soe.xuanzx.com

Go:   // 手写 map[int]int
来源：http://icj.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://idq.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://gnj.nanxinkj.top

[N08] 生成全排列
来源：http://glt.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://aoy.jyoumei.cn

PHP:  // 手写递归交换
来源：http://ggt.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://jwr.hywenlv.cn

TS:   // 手写回溯递归
来源：http://nyw.yueranfly.top

Java: // 手写回溯递归
来源：http://ijy.jqgfzy.top

Go:   // 手写回溯递归
来源：http://eeu.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://nbi.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://zkq.fktsv.cn

[N09] 栈与队列
来源：http://gxi.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://znh.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dqo.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ern.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yyq.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sjk.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://shy.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xjf.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://akm.cucudq.cn

[N10] 链表节点定义
来源：http://pga.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lic.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jfu.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ujd.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pyh.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://sfn.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://tdn.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wxm.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ulg.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://nvy.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kla.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://elc.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tyn.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndt.cdnleiting.top

Java: // 手写递归
来源：http://vmt.jqgufenzy.top

Go:   // 手写递归
来源：http://ddl.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vwk.zhijiandao.cn

C#:   // 手写递归
来源：http://dxm.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://chp.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hrj.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vlq.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pan.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gyi.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qpw.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ewn.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gdw.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jdi.zhengqikj.top

================================================================================
来源：http://tqi.yongpay.top

O. 并发与异步
来源：http://gbq.chenlongwang.top

================================================================================
来源：http://bbk.0kj1m.cn

[O01] 启动一个线程
来源：http://lij.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kfi.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://syv.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://euy.guannengcc.top

TS:   // 同 JS
来源：http://ark.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://zvm.vqdsnc.cn

Go:   go f()
来源：http://tda.jyoumei.cn

Ruby: Thread.new { f }
来源：http://tmy.xuanzx.com

C#:   Task.Run(() => F());
来源：http://qee.yvedp.cn

[O02] 使用线程池
来源：http://feu.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fhn.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rer.uphjek.com

JS:   // worker_threads 线程池
来源：http://iot.cashguo.top

TS:   // worker_threads 线程池
来源：http://tfi.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zeu.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://djg.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ynr.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wgz.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://jdx.sweek.top

Py:   with lock: shared += 1
来源：http://sef.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://vcb.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://imd.wangshuangyany.cn

TS:   // 同 JS
来源：http://ncb.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://hnj.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zrb.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://njv.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://sqc.c1oappe.top

[O04] 定义异步函数并等待
来源：http://ohl.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://bbx.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nya.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://okx.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kka.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zku.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://npz.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://mnn.tarul.cn

C#:   async Task F() { await G(); }
来源：http://vli.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://hgd.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://gfp.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ahj.yj20258.top

JS:   await Promise.all(tasks)
来源：http://cil.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://bfq.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uzt.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rod.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://ygs.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ojp.pengpengdd.cyou

[O06] 使用进程池
来源：http://tpt.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://exi.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://xno.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://wvp.pycfn.com

TS:   // child_process / cluster 模块
来源：http://uni.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wdb.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://taf.bjfxy.top

Ruby: // fork 块
来源：http://yks.pengpengdd.cyou

C#:   Parallel.For
来源：http://art.bbcook.cn

================================================================================
来源：http://zrw.yueranfly.top

P. 常用工具函数
来源：http://gra.meibo888.top

================================================================================
来源：http://bmd.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://usb.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://lpl.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mpv.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://snp.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://eeg.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://uhy.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://oxp.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://vmq.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://wpv.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://mde.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ryb.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tms.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vsi.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ptd.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zsy.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zyb.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upi.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bzo.redwolf501.top

[P03] 生成短随机字符串
来源：http://ecw.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yyn.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qzw.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://epd.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://icz.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gsa.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://euz.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fwh.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://osj.shuidangran.top

[P04] 求长度
来源：http://opo.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lfk.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qec.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oju.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uqv.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://urm.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://mjy.chenlongwang.top

Ruby: x.length;  x.size
来源：http://gnj.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jdc.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://gre.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://abp.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://akz.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qvg.wangdashe.top


<!-- 参考信息 -->