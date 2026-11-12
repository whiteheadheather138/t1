代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://abe.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hqg.c1oappe.top

================================================================================
来源：http://ury.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://ieg.snrcjt.cn

================================================================================
来源：http://eme.epnwcf.com

[M01] 读取命令行参数
来源：http://rkn.yangfankeji.com

Py:   sys.argv[1:]
来源：http://fbv.yj20258888.top

PHP:  $argv;  $argc;
来源：http://mvs.birdmap.top

JS:   process.argv.slice(2)
来源：http://nhm.sysykeji.top

TS:   process.argv.slice(2)
来源：http://nop.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://kws.bjfxy.top

Go:   os.Args[1:]
来源：http://dzb.yongpay.top

Ruby: ARGV
来源：http://gnz.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://qel.sweek.top

[M02] 读取环境变量
来源：http://cnc.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://aog.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zjk.aizwys.cn

JS:   process.env.HOME
来源：http://aqw.ydjk.org.cn

TS:   process.env.HOME
来源：http://fcm.zycfv.cn

Java: System.getenv("HOME")
来源：http://uyf.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kid.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://esl.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obw.fehbvm.com

[M03] 执行外部命令
来源：http://wij.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jun.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gry.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rqa.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mlj.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qve.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yfn.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://gwh.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://zgv.zdbjq.cn

[M04] 获取当前工作目录
来源：http://aua.kuanghao11.cn

Py:   os.getcwd()
来源：http://awb.xylfe.cn

PHP:  getcwd();
来源：http://jxv.quarkkingdee.top

JS:   process.cwd()
来源：http://irb.yangfankeji.com

TS:   process.cwd()
来源：http://odk.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://biv.yj20258.top

Go:   os.Getwd()
来源：http://ohy.daxiang520.top

Ruby: Dir.pwd
来源：http://lyz.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://fra.jinghuilouyu.cn

[M05] 设置退出码
来源：http://qds.jqgufenzy.top

Py:   sys.exit(1)
来源：http://wbh.xinyue.icu

PHP:  exit(1);
来源：http://yat.dianchejie.cn

JS:   process.exit(1)
来源：http://rsa.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://pcy.yangfankeji.com

Java: System.exit(1)
来源：http://nyo.yanxiufei.cn

Go:   os.Exit(1)
来源：http://mgi.feifeiyinyue.top

Ruby: exit 1
来源：http://oub.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dzp.dashuyun.cn

[M06] 向标准错误输出
来源：http://rdl.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://xcc.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xxw.xylfe.cn

JS:   console.error("err")
来源：http://zzb.svipenyu.cn

TS:   console.error("err")
来源：http://jmi.xziqi.cn

Java: System.err.println("err")
来源：http://msn.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ujz.9152youxi.cn

Ruby: warn "err"
来源：http://vhd.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://mcu.yuanzhike.top

[M07] 判断是否为主入口
来源：http://tvf.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://wkz.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vyh.ybcxt.top

JS:   require.main === module
来源：http://lnm.yj20258.top

TS:   require.main === module
来源：http://aat.tianlin.xyz

Java: public static void main(String[] args)
来源：http://nnr.hywenlv.cn

Go:   func main()
来源：http://yyx.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tug.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://ila.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://rgp.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://nxn.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://fuj.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://alo.xuanzx.com

TS:   process.platform;  process.version
来源：http://grm.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://shx.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lmd.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ute.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://thr.yfazqb.com

================================================================================
来源：http://qhg.yonumen.top

N. 数据结构与算法
来源：http://npy.gzhubu.top

================================================================================
来源：http://cik.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://fxx.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://lfh.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sql.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsx.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wgv.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wvq.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://tsp.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hsr.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://lix.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://jzd.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://mfp.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fpq.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://scn.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yyn.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mbc.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://ppb.ctjpmb.com

Ruby: arr.sort
来源：http://rrq.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zmw.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://rec.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://txl.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://jlw.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tlt.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ubd.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cev.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gnp.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oev.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hgj.0kj1m.cn

[N04] 斐波那契数列
来源：http://jso.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jmd.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uua.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mui.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mdz.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fwr.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ohe.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://juv.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pif.xylfe.cn

[N05] 最大公约数
来源：http://uan.tian-w.cn

Py:   math.gcd(a, b)
来源：http://nsy.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pck.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mti.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pnv.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://urm.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yng.ybcxt.top

Ruby: a.gcd(b)
来源：http://dmv.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aou.yangfankeji.com

[N06] 判断回文字符串
来源：http://cvc.gotoacloud.top

Py:   s == s[::-1]
来源：http://wbt.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://wjm.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://dfc.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://ata.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tqy.tarul.cn

Go:   // 双指针从两端比较
来源：http://jmo.cashguo.top

Ruby: s == s.reverse
来源：http://hvs.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sbs.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://pfj.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bzp.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://njj.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yws.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://vqo.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://utb.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://qsr.9152youxi.cn

Ruby: // 手写 Hash
来源：http://grg.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://olh.c1oappe.top

[N08] 生成全排列
来源：http://mfg.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://evm.hnqzz.top

PHP:  // 手写递归交换
来源：http://cwr.bbcook.cn

JS:   // 手写回溯递归
来源：http://bjd.guowangkeji.top

TS:   // 手写回溯递归
来源：http://dix.bjfxy.top

Java: // 手写回溯递归
来源：http://fkx.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://vrt.yj202588.top

Ruby: arr.permutation.to_a
来源：http://cin.wangdashe.top

C#:   // 手写回溯递归
来源：http://xva.jyoumei.cn

[N09] 栈与队列
来源：http://bff.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jmg.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lct.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dxh.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://swf.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oaz.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wdv.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pxh.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zck.chenlongwang.top

[N10] 链表节点定义
来源：http://rmk.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vaw.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://seh.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zgi.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eny.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://ygb.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dcy.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://skh.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ufw.yj20258.top

[N11] 二叉树中序遍历
来源：http://dqu.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qrm.cdnleiting.top

PHP:  // 手写递归函数
来源：http://awn.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hze.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cfb.yvedp.cn

Java: // 手写递归
来源：http://phc.quarkkingdee.top

Go:   // 手写递归
来源：http://huq.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lzy.jianghu66.top

C#:   // 手写递归
来源：http://bgh.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://obq.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fop.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hos.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pzp.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://upk.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qwf.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xsj.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://abd.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lao.wangshuangyany.cn

================================================================================
来源：http://scj.snrcjt.cn

O. 并发与异步
来源：http://ool.redwolf501.top

================================================================================
来源：http://iyg.smart0.xyz

[O01] 启动一个线程
来源：http://ygk.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://obc.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vnn.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vpt.jinghuilouyu.cn

TS:   // 同 JS
来源：http://exr.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://ubb.yj20258888.top

Go:   go f()
来源：http://tvb.ehwqpu.com

Ruby: Thread.new { f }
来源：http://vxs.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://fhq.zhongyouzk.top

[O02] 使用线程池
来源：http://ehk.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://erw.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xtk.daxiang520.top

JS:   // worker_threads 线程池
来源：http://lpi.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://rcq.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fgl.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dpl.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zjx.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lrw.fengsongda.top

[O03] 加锁保护共享数据
来源：http://otc.birdmap.top

Py:   with lock: shared += 1
来源：http://sbz.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://yqj.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pul.pycfn.com

TS:   // 同 JS
来源：http://dld.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://kzu.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sha.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yxr.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://kjz.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://bfy.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://gkj.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ujc.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://bbh.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://esf.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qvf.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qua.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://fxx.yj202588.top

C#:   async Task F() { await G(); }
来源：http://vod.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://ddq.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://smh.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wsa.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://jue.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://dbz.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fwy.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xxe.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://sbe.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zhv.hesvh.cn

[O06] 使用进程池
来源：http://zpv.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://chv.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fbm.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://gpr.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://jjz.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eaa.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jbd.cdnleiting.top

Ruby: // fork 块
来源：http://jpr.meibo888.top

C#:   Parallel.For
来源：http://jcn.sjlbkw.cn

================================================================================
来源：http://tka.zhongyouzk.top

P. 常用工具函数
来源：http://qux.sjlbkw.cn

================================================================================
来源：http://eou.zdbjq.cn

[P01] 生成 UUID
来源：http://lws.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://swt.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://msf.316326.xyz

JS:   crypto.randomUUID()
来源：http://beo.guannengcc.top

TS:   crypto.randomUUID()
来源：http://kio.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://emk.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://lfi.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://orm.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://uxa.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://rey.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gfz.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://uow.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nhu.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mmv.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xhp.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mum.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://igc.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bcf.snrcjt.cn

[P03] 生成短随机字符串
来源：http://kwr.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aqn.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nuf.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fqf.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://drn.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pdm.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ffq.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rtn.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qzy.smart0.xyz

[P04] 求长度
来源：http://aqi.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jvo.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngv.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://umm.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xfg.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://lew.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://zqc.hammf.cn

Ruby: x.length;  x.size
来源：http://xxc.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://add.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://awh.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mqp.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://puo.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rxx.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xfq.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xdi.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nwd.feifeiyinyue.top

Ruby: a == b
来源：http://wbi.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wso.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yin.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xxz.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://zoh.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ffh.316326.xyz

TS:   if (x == null) {}
来源：http://vgq.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kjx.dashuyun.cn

Go:   if x == nil {}
来源：http://hex.guannengcc.top


<!-- 参考信息 -->