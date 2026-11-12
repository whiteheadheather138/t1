代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmp.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uei.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://thw.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://htm.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dtz.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jzc.nanxuanxn.top

================================================================================
来源：http://skr.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://ndb.xylfe.cn

================================================================================
来源：http://rud.fzhhl.top

[M01] 读取命令行参数
来源：http://oxe.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://kmz.yj202588.top

PHP:  $argv;  $argc;
来源：http://njc.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://cpb.yuxming.cn

TS:   process.argv.slice(2)
来源：http://hex.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://zlx.meibo888.top

Go:   os.Args[1:]
来源：http://tfq.xinyue.icu

Ruby: ARGV
来源：http://dwv.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://laz.zdbjq.cn

[M02] 读取环境变量
来源：http://tnv.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://mek.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pjz.vqdsnc.cn

JS:   process.env.HOME
来源：http://dah.guannengcc.top

TS:   process.env.HOME
来源：http://maa.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://zmw.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kcb.fzhhl.top

Ruby: ENV["HOME"]
来源：http://zjv.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vqv.ppjwa.cn

[M03] 执行外部命令
来源：http://pfy.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nii.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qul.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hwi.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xbm.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wbu.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gph.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://itt.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://abu.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://zga.cdnleiting.top

Py:   os.getcwd()
来源：http://fvs.yuanzhike.top

PHP:  getcwd();
来源：http://dna.yfazqb.com

JS:   process.cwd()
来源：http://tgd.fanxiaobao.xyz

TS:   process.cwd()
来源：http://kcr.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://jam.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://wql.aibaodan.cn

Ruby: Dir.pwd
来源：http://mcr.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://mcf.mhx1999.top

[M05] 设置退出码
来源：http://mhd.cheryme.top

Py:   sys.exit(1)
来源：http://ekm.jlsjyb.cn

PHP:  exit(1);
来源：http://scg.iojbl.cn

JS:   process.exit(1)
来源：http://llu.meibo888.top

TS:   process.exit(1)
来源：http://mis.chenzaomai.com

Java: System.exit(1)
来源：http://unx.fzhhl.top

Go:   os.Exit(1)
来源：http://ybb.gogol.net.cn

Ruby: exit 1
来源：http://jsh.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dtn.xuanzx.com

[M06] 向标准错误输出
来源：http://rap.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://xsr.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yzo.aizwys.cn

JS:   console.error("err")
来源：http://ter.yangfankeji.com

TS:   console.error("err")
来源：http://vee.ydjk.org.cn

Java: System.err.println("err")
来源：http://ira.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bwq.havefunace.top

Ruby: warn "err"
来源：http://mjo.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://qkq.tian-w.cn

[M07] 判断是否为主入口
来源：http://mxd.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://tbr.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://thu.hysaishi.cn

JS:   require.main === module
来源：http://mkq.gogol.net.cn

TS:   require.main === module
来源：http://xji.yj202588.top

Java: public static void main(String[] args)
来源：http://deb.xinyue.icu

Go:   func main()
来源：http://xcc.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://puv.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://ran.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://xst.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://iwi.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://fqm.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://wam.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://cqp.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ivg.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://wwt.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xfc.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://snr.yanxiufei.cn

================================================================================
来源：http://lsh.haohaochexian.top

N. 数据结构与算法
来源：http://fqe.hnqzz.top

================================================================================
来源：http://wij.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://fst.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://mqm.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pov.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srj.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dij.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://itc.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://kkc.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tbo.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://fao.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://kbb.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qqu.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://avq.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pwb.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mxb.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zir.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://anu.52xcode.cn

Ruby: arr.sort
来源：http://rzh.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://dfl.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://bwl.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tnh.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://tzy.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ikx.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mkk.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hob.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zfr.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gmp.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://gfn.wangdashe.top

[N04] 斐波那契数列
来源：http://dkb.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eep.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yik.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://anm.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fle.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mim.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wyr.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bwb.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hub.zdqjudy.top

[N05] 最大公约数
来源：http://yov.hammf.cn

Py:   math.gcd(a, b)
来源：http://xtz.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jvn.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dat.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scd.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bmh.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kjj.gotoacloud.top

Ruby: a.gcd(b)
来源：http://skt.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hkz.gaohongyu789.top

[N06] 判断回文字符串
来源：http://cgu.cqqwz.cn

Py:   s == s[::-1]
来源：http://irz.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://juv.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://dmw.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://aeg.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ztc.xylfe.cn

Go:   // 双指针从两端比较
来源：http://egb.andypj.xyz

Ruby: s == s.reverse
来源：http://ogc.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ekd.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://scr.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yjh.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kmh.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yaf.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://luf.yuanzhike.top

Java: // 手写 HashMap
来源：http://vzg.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://oxz.yvedp.cn

Ruby: // 手写 Hash
来源：http://syf.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://ymi.shanyushiyangtech.top

[N08] 生成全排列
来源：http://ava.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://kdn.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://vwi.jyoumei.cn

JS:   // 手写回溯递归
来源：http://boy.jianghu66.top

TS:   // 手写回溯递归
来源：http://ujr.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://pzc.aizwys.cn

Go:   // 手写回溯递归
来源：http://aww.yongpay.top

Ruby: arr.permutation.to_a
来源：http://afa.dianchejie.cn

C#:   // 手写回溯递归
来源：http://qdw.fengsongda.top

[N09] 栈与队列
来源：http://shd.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydp.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wcf.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qaa.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dvv.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://crh.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://syp.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://agh.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lzr.ivvv.top

[N10] 链表节点定义
来源：http://aya.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vhk.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jww.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qej.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xpd.cheryme.top

Java: class Node { int v; Node next; }
来源：http://ipp.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://shm.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tce.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ezc.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://qep.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://llj.fktsv.cn

PHP:  // 手写递归函数
来源：http://shd.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://flw.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vuu.ybcxt.top

Java: // 手写递归
来源：http://zoe.epnwcf.com

Go:   // 手写递归
来源：http://axn.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ndx.yongpay.top

C#:   // 手写递归
来源：http://rsp.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eck.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aqx.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://khb.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xkm.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fgt.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://chu.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ppo.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://efe.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://otk.jinghuilouyu.cn

================================================================================
来源：http://uuk.zdqjudy.top

O. 并发与异步
来源：http://ote.bjfxy.top

================================================================================
来源：http://qhc.guannengcc.top

[O01] 启动一个线程
来源：http://ese.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iqz.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kgg.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uke.yj202588.top

TS:   // 同 JS
来源：http://tzt.sweek.top

Java: new Thread(() -> f()).start()
来源：http://rsh.tian-w.cn

Go:   go f()
来源：http://xbf.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://bvc.yfazqb.com

C#:   Task.Run(() => F());
来源：http://goi.kuanghao11.cn

[O02] 使用线程池
来源：http://kho.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sza.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oca.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://jko.52xcode.cn

TS:   // worker_threads 线程池
来源：http://ili.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://sqe.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yig.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aqg.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wya.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://phn.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://ogp.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://gws.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pmw.chenjidiqi.icu

TS:   // 同 JS
来源：http://gzr.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://mim.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ijs.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lzk.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://ejr.c1oappe.top

[O04] 定义异步函数并等待
来源：http://kso.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://goo.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wdu.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://eey.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vgm.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iif.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jzv.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://fwh.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://ciw.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://ijt.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://qqv.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cqy.sweek.top

JS:   await Promise.all(tasks)
来源：http://gso.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://mns.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nwn.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fpj.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://ybq.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xkw.yj20258888.top

[O06] 使用进程池
来源：http://xmd.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kfo.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dxt.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://orn.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://lkx.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ran.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xpg.gaohongyu789.top

Ruby: // fork 块
来源：http://zdv.cqqwz.cn

C#:   Parallel.For
来源：http://xrq.zhengqikj.top

================================================================================
来源：http://oig.xylfe.cn

P. 常用工具函数
来源：http://tru.jinghuilouyu.cn

================================================================================
来源：http://xas.fktsv.cn

[P01] 生成 UUID
来源：http://ofc.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://xsw.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cba.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://yox.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://ntm.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://ljx.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://cho.birdmap.top

Ruby: SecureRandom.uuid
来源：http://ffw.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://mzb.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://mmu.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://llg.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zyh.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://arv.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ana.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iej.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gph.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mlz.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iov.tanke756.top

[P03] 生成短随机字符串
来源：http://kxe.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dyu.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xtj.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tah.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ncw.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nff.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://daw.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cqm.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qkv.jqgfzy.top

[P04] 求长度
来源：http://rol.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wcp.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myn.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hju.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izd.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://hgb.wangdashe.top

Go:   len(arr);  len(m)
来源：http://eis.sufxvd.cn

Ruby: x.length;  x.size
来源：http://dww.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mgt.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://ydg.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://swn.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zin.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ohu.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qzl.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hdq.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://zcf.jqgfzy.top

Ruby: a == b
来源：http://fzt.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xig.fengsongda.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dog.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://itz.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://yzw.uphjek.com


<!-- 参考信息 -->