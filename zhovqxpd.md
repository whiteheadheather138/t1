代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eer.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kcp.jianghu66.top

================================================================================
来源：http://crd.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://hbl.jqgufenzy.top

================================================================================
来源：http://bct.hfpthk.cn

[M01] 读取命令行参数
来源：http://jbr.xinyue.icu

Py:   sys.argv[1:]
来源：http://mvt.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://ivs.cucudq.cn

JS:   process.argv.slice(2)
来源：http://cwm.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://atk.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://wxh.yanxiufei.cn

Go:   os.Args[1:]
来源：http://fqv.chenlongwang.top

Ruby: ARGV
来源：http://gqb.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://djt.jinqigufen.top

[M02] 读取环境变量
来源：http://wsk.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://tzf.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lqa.0kj1m.cn

JS:   process.env.HOME
来源：http://xip.tarul.cn

TS:   process.env.HOME
来源：http://spc.sxryk.cn

Java: System.getenv("HOME")
来源：http://ufw.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vre.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://xke.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hir.yj20258888.top

[M03] 执行外部命令
来源：http://jqj.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xso.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://inj.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qbb.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ytl.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://whc.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ucv.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nua.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://tab.guowangkeji.top

[M04] 获取当前工作目录
来源：http://lpe.sweek.top

Py:   os.getcwd()
来源：http://msr.feifeiyinyue.top

PHP:  getcwd();
来源：http://ddz.yj20258888.top

JS:   process.cwd()
来源：http://lyg.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://xic.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://cgb.daxiang520.top

Go:   os.Getwd()
来源：http://pbv.tarul.cn

Ruby: Dir.pwd
来源：http://baq.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ysd.epnwcf.com

[M05] 设置退出码
来源：http://apd.0kj1m.cn

Py:   sys.exit(1)
来源：http://vkc.pycfn.com

PHP:  exit(1);
来源：http://eyt.yonumen.top

JS:   process.exit(1)
来源：http://qht.epnwcf.com

TS:   process.exit(1)
来源：http://yri.smart0.xyz

Java: System.exit(1)
来源：http://wig.zdbjq.cn

Go:   os.Exit(1)
来源：http://ksm.vqdsnc.cn

Ruby: exit 1
来源：http://ajw.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zew.hfpthk.cn

[M06] 向标准错误输出
来源：http://xbv.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://ofo.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uvd.yueranfly.top

JS:   console.error("err")
来源：http://hjv.fengsongda.top

TS:   console.error("err")
来源：http://ngx.hongshengwenyu.top

Java: System.err.println("err")
来源：http://ahr.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bmo.ydzc1.top

Ruby: warn "err"
来源：http://joa.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://xlt.nwbrower.top

[M07] 判断是否为主入口
来源：http://alc.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://lji.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cgy.jinqigufen.top

JS:   require.main === module
来源：http://jnm.hcnkem.com

TS:   require.main === module
来源：http://oip.bjfxy.top

Java: public static void main(String[] args)
来源：http://yka.c1oappe.top

Go:   func main()
来源：http://aii.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aaq.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://mwx.yj20258.top

[M08] 获取系统与运行时信息
来源：http://acx.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://nml.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://qpw.aizwys.cn

JS:   process.platform;  process.version
来源：http://bhs.ivvv.top

TS:   process.platform;  process.version
来源：http://bpv.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ewv.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://won.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zjc.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lhl.zdbjq.cn

================================================================================
来源：http://xps.316326.xyz

N. 数据结构与算法
来源：http://ros.xuetiantiany.cn

================================================================================
来源：http://vla.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://guv.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://zbv.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nbp.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xzj.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ljq.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://xho.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://hgh.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://doq.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://xha.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://bhx.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://cnc.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xdf.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gml.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://pxf.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://neo.yj202588.top

Go:   slices.Sort(arr)
来源：http://ywd.jiagoushi.top

Ruby: arr.sort
来源：http://bzw.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://naz.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://dyi.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rdn.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://fti.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ztz.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vqh.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cmx.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cti.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wxn.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xny.zhijiandao.cn

[N04] 斐波那契数列
来源：http://mvc.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cei.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fxs.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ntp.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iuf.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bsb.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mkc.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ige.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bcl.ppjwa.cn

[N05] 最大公约数
来源：http://nyu.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://wcx.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ysz.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tsm.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iin.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xxn.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rht.gogol.net.cn

Ruby: a.gcd(b)
来源：http://hyo.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wjt.yuxming.cn

[N06] 判断回文字符串
来源：http://baj.tianlin.xyz

Py:   s == s[::-1]
来源：http://cdm.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://dgc.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://cqo.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://vhq.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kjr.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://hrq.andypj.xyz

Ruby: s == s.reverse
来源：http://oqi.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qjt.meibo888.top

[N07] 两数之和（返回下标）
来源：http://lyh.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oma.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://med.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vae.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://rvx.yvedp.cn

Java: // 手写 HashMap
来源：http://ijb.yfazqb.com

Go:   // 手写 map[int]int
来源：http://mua.c1oappe.top

Ruby: // 手写 Hash
来源：http://jpf.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://fus.svipenyu.cn

[N08] 生成全排列
来源：http://xpi.tarul.cn

Py:   itertools.permutations(arr)
来源：http://dnx.hesvh.cn

PHP:  // 手写递归交换
来源：http://kiv.hywenlv.cn

JS:   // 手写回溯递归
来源：http://zjz.yonumen.top

TS:   // 手写回溯递归
来源：http://mda.guowangkeji.top

Java: // 手写回溯递归
来源：http://nkt.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://nts.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://lrr.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://mcb.yj20258888.top

[N09] 栈与队列
来源：http://xte.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://slb.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ybg.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://znz.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wpf.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oxm.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gmb.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ibk.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pyd.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://gup.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nar.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tza.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://izc.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://def.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://ebd.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ywi.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bzy.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uco.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://wcn.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tje.chenlongwang.top

PHP:  // 手写递归函数
来源：http://leg.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xps.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kkk.0kj1m.cn

Java: // 手写递归
来源：http://htl.gogol.net.cn

Go:   // 手写递归
来源：http://hsf.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://woa.jinghuilouyu.cn

C#:   // 手写递归
来源：http://qzw.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ihi.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ljb.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xsa.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ewr.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epq.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ywm.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://byz.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://glv.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dup.yfazqb.com

================================================================================
来源：http://hfe.hnxiangtu.top

O. 并发与异步
来源：http://fwt.yanxiufei.cn

================================================================================
来源：http://toq.redwolf501.top

[O01] 启动一个线程
来源：http://nmm.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qnb.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zyw.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iyd.zdbjq.cn

TS:   // 同 JS
来源：http://azc.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://nkg.yvedp.cn

Go:   go f()
来源：http://bbe.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://bjz.iojbl.cn

C#:   Task.Run(() => F());
来源：http://rgw.ydjk.org.cn

[O02] 使用线程池
来源：http://afl.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uma.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qpd.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://inf.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://jgb.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://jyp.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pbe.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ghf.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bpx.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://glc.hysaishi.cn

Py:   with lock: shared += 1
来源：http://eai.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://fmk.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hnv.0kj1m.cn

TS:   // 同 JS
来源：http://tma.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://nwd.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://daw.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iwh.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://ija.tarul.cn

[O04] 定义异步函数并等待
来源：http://llw.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://gai.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://trs.wangdashe.top

JS:   async function f() { await g(); }
来源：http://crq.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://piz.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xki.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://odl.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://nun.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://dwn.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://upw.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://afd.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jcb.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://bvf.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://lpm.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ctz.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iuu.sxryk.cn

Ruby: threads.map(&:join)
来源：http://usb.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xdh.hysaishi.cn

[O06] 使用进程池
来源：http://zru.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bdp.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://lcl.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://dtv.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://sgq.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wvi.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wpe.epnwcf.com

Ruby: // fork 块
来源：http://ewu.hfpthk.cn

C#:   Parallel.For
来源：http://wvx.sxryk.cn

================================================================================
来源：http://hcq.sufxvd.cn

P. 常用工具函数
来源：http://ezh.hesvh.cn

================================================================================
来源：http://ksm.fzhhl.top

[P01] 生成 UUID
来源：http://mgc.meibo888.top

Py:   str(uuid.uuid4())
来源：http://zdq.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gpk.fzhhl.top

JS:   crypto.randomUUID()
来源：http://qlu.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://oaa.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://ggo.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://wjk.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://kqu.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://wyw.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://qdt.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aku.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://awr.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gel.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://puu.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://scq.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wqi.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lzt.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mhv.smart0.xyz

[P03] 生成短随机字符串
来源：http://dfz.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://axd.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tch.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vyh.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fsr.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ovj.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://njg.yvedp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ekc.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xlv.jyoumei.cn

[P04] 求长度
来源：http://cil.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qza.havefunace.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exl.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwu.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pxu.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://bgs.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://qup.svipenyu.cn

Ruby: x.length;  x.size
来源：http://uov.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xrw.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://zun.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://gcv.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sxi.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ohc.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mew.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mzp.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://eds.jinqigufen.top

Ruby: a == b
来源：http://fcc.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cqv.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qau.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xtc.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://kor.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hhq.jlsjyb.cn

TS:   if (x == null) {}
来源：http://clc.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eug.xuetiantiany.cn

Go:   if x == nil {}
来源：http://lha.yj202588.top


<!-- 参考信息 -->