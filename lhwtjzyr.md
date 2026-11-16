代发 wailian999

TS:   resp.ok;  resp.status
来源：http://eqx.kuanghao11.cn

Java: resp.statusCode()
来源：http://ezv.kuanghao11.cn

Go:   resp.StatusCode
来源：http://tsj.gzhubu.top

Ruby: resp.code.to_i
来源：http://yad.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://ofn.xylfe.cn

[L08] 并发请求多个地址
来源：http://fzv.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vtn.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://lxq.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnk.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://onr.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ixl.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyo.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bwk.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ihc.birdmap.top

================================================================================
来源：http://hxz.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://vsr.aizwys.cn

================================================================================
来源：http://ohu.shuidangran.top

[M01] 读取命令行参数
来源：http://phx.sweek.top

Py:   sys.argv[1:]
来源：http://ruz.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://cxp.xinyue.icu

JS:   process.argv.slice(2)
来源：http://kwd.fktsv.cn

TS:   process.argv.slice(2)
来源：http://elc.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://yad.haohaochexian.top

Go:   os.Args[1:]
来源：http://wat.nanxuanxn.top

Ruby: ARGV
来源：http://cim.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://uuh.jinqigfzy.top

[M02] 读取环境变量
来源：http://tsp.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://pzt.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://czj.c1oappe.top

JS:   process.env.HOME
来源：http://nvi.nanxinkj.top

TS:   process.env.HOME
来源：http://mnh.gzhubu.top

Java: System.getenv("HOME")
来源：http://hmf.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fyz.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://nyh.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tum.fehbvm.com

[M03] 执行外部命令
来源：http://dlp.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rhi.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zev.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qyv.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxy.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kjm.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://skt.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://hjl.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://kgh.yonumen.top

[M04] 获取当前工作目录
来源：http://gwk.yangfankeji.com

Py:   os.getcwd()
来源：http://gmi.ivvv.top

PHP:  getcwd();
来源：http://gxe.dianchejie.cn

JS:   process.cwd()
来源：http://lrz.shangyingyoupin.top

TS:   process.cwd()
来源：http://fqd.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://bwd.quarkkingdee.top

Go:   os.Getwd()
来源：http://ykx.tarul.cn

Ruby: Dir.pwd
来源：http://iwe.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://zam.pengpengdd.cyou

[M05] 设置退出码
来源：http://ard.shuidangran.top

Py:   sys.exit(1)
来源：http://jmo.zhiwuduotai.top

PHP:  exit(1);
来源：http://mbl.316326.xyz

JS:   process.exit(1)
来源：http://tyu.0kj1m.cn

TS:   process.exit(1)
来源：http://mry.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://seu.sweek.top

Go:   os.Exit(1)
来源：http://zyz.gaohongyu789.top

Ruby: exit 1
来源：http://lgf.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jnd.mhx1999.top

[M06] 向标准错误输出
来源：http://ruq.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://tik.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dvr.svipenyu.cn

JS:   console.error("err")
来源：http://zoh.cqqwz.cn

TS:   console.error("err")
来源：http://hwd.zhiwuduotai.top

Java: System.err.println("err")
来源：http://xfe.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogn.ivvv.top

Ruby: warn "err"
来源：http://dvb.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://zes.zhixingplan.top

[M07] 判断是否为主入口
来源：http://ssw.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://pfc.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sek.yuanzhike.top

JS:   require.main === module
来源：http://cwf.jyoumei.cn

TS:   require.main === module
来源：http://qjw.zhengqikj.top

Java: public static void main(String[] args)
来源：http://kkl.ctjpmb.com

Go:   func main()
来源：http://tgd.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lmu.mhx1999.top

C#:   static void Main(string[] args)
来源：http://wrq.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://hnc.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://lui.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://vze.smart0.xyz

JS:   process.platform;  process.version
来源：http://fmg.yj202588.top

TS:   process.platform;  process.version
来源：http://kyn.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cxf.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cro.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yga.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yig.zhiwuduotai.top

================================================================================
来源：http://cyx.hnxiangtu.top

N. 数据结构与算法
来源：http://ifu.nanxuanxn.top

================================================================================
来源：http://zxn.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://ams.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://lqf.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://meu.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://svl.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zit.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zzt.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://xhb.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kvv.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://fuw.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://ier.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://fcx.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lot.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ycw.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vhc.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://twe.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://zpf.daria6918.cn

Ruby: arr.sort
来源：http://eli.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ptc.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://xiu.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pxo.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://vqt.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://giq.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qav.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kur.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rnc.quarkkingdee.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wok.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://ufh.gzhubu.top

[N04] 斐波那契数列
来源：http://azt.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://awd.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uqt.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pdi.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jdc.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qxa.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hxu.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ekb.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xva.yvedp.cn

[N05] 最大公约数
来源：http://xta.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://isx.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yyg.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bul.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rjx.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pdb.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sqc.tianlin.xyz

Ruby: a.gcd(b)
来源：http://mka.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qxm.c1oappe.top

[N06] 判断回文字符串
来源：http://xmi.hywenlv.cn

Py:   s == s[::-1]
来源：http://kgz.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://hwu.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://dxo.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://tmc.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ynw.ivvv.top

Go:   // 双指针从两端比较
来源：http://njo.haohaochexian.top

Ruby: s == s.reverse
来源：http://tjm.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lse.pycfn.com

[N07] 两数之和（返回下标）
来源：http://pju.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wed.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wvi.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qvr.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://jlt.zhijiandao.cn

Java: // 手写 HashMap
来源：http://nuw.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://rpw.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://qwm.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://bag.0kj1m.cn

[N08] 生成全排列
来源：http://qzq.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://tro.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://flp.ehwqpu.com

JS:   // 手写回溯递归
来源：http://ywd.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://ley.bjfxy.top

Java: // 手写回溯递归
来源：http://hua.ppjwa.cn

Go:   // 手写回溯递归
来源：http://frh.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://mld.chenzaomai.com

C#:   // 手写回溯递归
来源：http://nrf.hammf.cn

[N09] 栈与队列
来源：http://dcc.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hgu.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://voc.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://csw.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://irc.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ijw.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iam.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rwb.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dxd.yfazqb.com

[N10] 链表节点定义
来源：http://rws.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kpn.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://gck.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imy.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zjy.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://qhg.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yiq.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bqj.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wxw.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://dwk.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eql.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://huz.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jrj.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dlk.sysykeji.top

Java: // 手写递归
来源：http://jvr.yuxming.cn

Go:   // 手写递归
来源：http://teg.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wlq.cucudq.cn

C#:   // 手写递归
来源：http://lih.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yts.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qgr.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://its.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bza.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzy.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kfz.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nsu.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyd.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rry.xylfe.cn

================================================================================
来源：http://ydp.nanxuanxn.top

O. 并发与异步
来源：http://ydf.jinqigfzy.top

================================================================================
来源：http://ysp.yvedp.cn

[O01] 启动一个线程
来源：http://kfu.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://anr.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tog.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vfh.0kj1m.cn

TS:   // 同 JS
来源：http://myv.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://vkm.xziqi.cn

Go:   go f()
来源：http://iey.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://spu.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://lim.yonumen.top

[O02] 使用线程池
来源：http://qda.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://njw.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zzn.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://oua.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://xgu.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://dgb.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sre.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yko.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zsq.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://mih.sysykeji.top

Py:   with lock: shared += 1
来源：http://tjl.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://djt.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbm.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://swx.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://qft.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://teo.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hua.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://irr.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://bvv.tarul.cn

Py:   async def f():⏎    await g()
来源：http://spw.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qrx.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://biq.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://xth.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pnv.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hzo.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://rld.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://nks.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://kqf.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://jme.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://djs.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://lcy.tarul.cn

TS:   await Promise.all(tasks)
来源：http://clq.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vkw.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eft.cashguo.top

Ruby: threads.map(&:join)
来源：http://tci.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cno.chenjidiqi.icu

[O06] 使用进程池
来源：http://jwn.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kfu.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://qgh.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://cgr.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://qzy.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://odk.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vxe.kuanghao11.cn

Ruby: // fork 块
来源：http://xfs.ivvv.top

C#:   Parallel.For
来源：http://ywl.andypj.xyz

================================================================================
来源：http://mda.redwolf501.top

P. 常用工具函数
来源：http://laj.gogol.net.cn

================================================================================
来源：http://kjn.sweek.top

[P01] 生成 UUID
来源：http://tkq.yonumen.top

Py:   str(uuid.uuid4())
来源：http://qyr.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cli.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://spa.yfazqb.com

TS:   crypto.randomUUID()
来源：http://gdf.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://sip.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://ise.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://osy.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://aua.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://cze.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vwl.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://iqm.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://diz.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fhu.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lfk.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gdk.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jar.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ywg.hysaishi.cn

[P03] 生成短随机字符串
来源：http://uog.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hyt.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rwj.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixi.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bix.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bdp.gaohongyu789.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://weu.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kuh.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fnj.jyoumei.cn

[P04] 求长度
来源：http://rnd.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ggo.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qcg.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxe.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhl.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://wit.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://trk.zhixingplan.top

Ruby: x.length;  x.size
来源：http://yuv.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://bxg.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://wky.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qiq.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lod.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mmj.fktsv.cn


<!-- 参考信息 -->