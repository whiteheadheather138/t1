代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pkx.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hud.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zgb.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lfp.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tsp.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mot.jianghu66.top

================================================================================
来源：http://awr.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://pup.tanke756.top

================================================================================
来源：http://qol.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://nmt.bbcook.cn

Py:   sys.argv[1:]
来源：http://svq.havefunace.top

PHP:  $argv;  $argc;
来源：http://ftg.xuanzx.com

JS:   process.argv.slice(2)
来源：http://xio.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://azz.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://uzd.nanxinkj.top

Go:   os.Args[1:]
来源：http://mmw.chenzaomai.com

Ruby: ARGV
来源：http://hlh.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://obs.gaohongyu789.top

[M02] 读取环境变量
来源：http://jgg.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://mrj.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xhm.yongpay.top

JS:   process.env.HOME
来源：http://ria.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://cht.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://hhw.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hma.xuanzx.com

Ruby: ENV["HOME"]
来源：http://uzq.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iaa.cheryme.top

[M03] 执行外部命令
来源：http://bgz.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vkf.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vng.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sse.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wml.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ggw.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pqb.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://sbq.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://igf.guowangkeji.top

[M04] 获取当前工作目录
来源：http://bka.yonumen.top

Py:   os.getcwd()
来源：http://flr.yonumen.top

PHP:  getcwd();
来源：http://kmv.quarkkingdee.top

JS:   process.cwd()
来源：http://ysf.yj20258888.top

TS:   process.cwd()
来源：http://xos.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://fvo.hfpthk.cn

Go:   os.Getwd()
来源：http://ryn.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://wyq.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://rjt.cheryme.top

[M05] 设置退出码
来源：http://qpy.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://dym.9152youxi.cn

PHP:  exit(1);
来源：http://owj.nanxinkj.top

JS:   process.exit(1)
来源：http://ikc.hnqzz.top

TS:   process.exit(1)
来源：http://klh.svipenyu.cn

Java: System.exit(1)
来源：http://luz.zdbjq.cn

Go:   os.Exit(1)
来源：http://eyd.meibo888.top

Ruby: exit 1
来源：http://tij.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://axj.redwolf501.top

[M06] 向标准错误输出
来源：http://nfp.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://qpo.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gdo.daxiang520.top

JS:   console.error("err")
来源：http://kah.jyoumei.cn

TS:   console.error("err")
来源：http://lcv.nanxinkj.top

Java: System.err.println("err")
来源：http://twz.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gcr.yonumen.top

Ruby: warn "err"
来源：http://kgw.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://pso.hysaishi.cn

[M07] 判断是否为主入口
来源：http://wqf.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://wmk.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cem.jinghuilouyu.cn

JS:   require.main === module
来源：http://yos.smart0.xyz

TS:   require.main === module
来源：http://vig.meibo888.top

Java: public static void main(String[] args)
来源：http://waz.shangyingyoupin.top

Go:   func main()
来源：http://lia.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bug.xylfe.cn

C#:   static void Main(string[] args)
来源：http://fos.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://kbv.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://uet.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://zuu.hfpthk.cn

JS:   process.platform;  process.version
来源：http://eto.hcnkem.com

TS:   process.platform;  process.version
来源：http://ebe.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://euw.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pnn.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tmg.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qzf.birdmap.top

================================================================================
来源：http://fhk.chenzaomai.com

N. 数据结构与算法
来源：http://smo.yj202588.top

================================================================================
来源：http://xrr.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://rnf.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fiq.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wrc.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvb.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgj.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mwz.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://tht.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qke.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sti.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://yez.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://clm.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xzi.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://npw.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://woh.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yjk.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://cfq.fengsongda.top

Ruby: arr.sort
来源：http://isg.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pra.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://vgy.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gnx.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://ozb.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pvq.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nmh.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://djc.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://klf.chenlongwang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gxi.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lbl.ydzc1.top

[N04] 斐波那契数列
来源：http://kty.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qit.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aog.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ieg.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tlh.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yer.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rtd.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxn.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ruw.gogol.net.cn

[N05] 最大公约数
来源：http://vyf.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://owo.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nyo.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqy.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dhp.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qty.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kep.andypj.xyz

Ruby: a.gcd(b)
来源：http://ele.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qcn.tarul.cn

[N06] 判断回文字符串
来源：http://pbf.jqgufenzy.top

Py:   s == s[::-1]
来源：http://sgc.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://uze.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://yae.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://pef.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fmn.xinyue.icu

Go:   // 双指针从两端比较
来源：http://asb.ybcxt.top

Ruby: s == s.reverse
来源：http://nsr.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oas.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://zol.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njr.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vlw.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rpx.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://iod.pycfn.com

Java: // 手写 HashMap
来源：http://dif.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://jdc.aibaodan.cn

Ruby: // 手写 Hash
来源：http://tir.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dlf.fanxiaobao.xyz

[N08] 生成全排列
来源：http://ruh.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://wyf.wangdashe.top

PHP:  // 手写递归交换
来源：http://ueb.ehwqpu.com

JS:   // 手写回溯递归
来源：http://gra.xuanzx.com

TS:   // 手写回溯递归
来源：http://crk.mhx1999.top

Java: // 手写回溯递归
来源：http://aqu.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://ssn.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://ink.nwbrower.top

C#:   // 手写回溯递归
来源：http://anb.guannengcc.top

[N09] 栈与队列
来源：http://zmc.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ujc.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ckb.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bdv.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ycf.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://diy.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vbu.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kzn.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bpv.yfazqb.com

[N10] 链表节点定义
来源：http://mgf.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bre.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pkz.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kfq.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tqj.ivvv.top

Java: class Node { int v; Node next; }
来源：http://mjc.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lzn.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://epm.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ral.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://nht.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oxd.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://nyk.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://veg.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wxs.pengpengdd.cyou

Java: // 手写递归
来源：http://khv.zdbjq.cn

Go:   // 手写递归
来源：http://ptx.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xys.gaohongyu789.top

C#:   // 手写递归
来源：http://jsd.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fpx.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vdt.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xzh.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jdm.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ubl.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hha.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hit.quarkkingdee.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bkl.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ttx.xuanzx.com

================================================================================
来源：http://otd.hywenlv.cn

O. 并发与异步
来源：http://sle.gotoacloud.top

================================================================================
来源：http://uly.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://lii.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://imh.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qop.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cxk.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://xes.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://grd.jianghu66.top

Go:   go f()
来源：http://kuc.nwbrower.top

Ruby: Thread.new { f }
来源：http://adg.aizwys.cn

C#:   Task.Run(() => F());
来源：http://yhy.zdbjq.cn

[O02] 使用线程池
来源：http://rvb.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ety.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://min.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://uhk.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://tkx.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://tbx.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ksy.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vri.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cja.tian-w.cn

[O03] 加锁保护共享数据
来源：http://txm.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://jqw.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://spx.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ysh.jqgufenzy.top

TS:   // 同 JS
来源：http://qxe.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://olg.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vxb.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fkk.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://rcy.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://rej.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://hqt.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jek.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://qzo.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eoj.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tyh.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hxr.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sej.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://ida.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://iad.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://gzy.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dno.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://yol.ivvv.top

TS:   await Promise.all(tasks)
来源：http://hap.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kkt.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uqb.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://jid.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tfn.jqgfzy.top

[O06] 使用进程池
来源：http://iyb.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oka.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qtw.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://czi.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://lrw.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pjm.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sne.fanxiaobao.xyz

Ruby: // fork 块
来源：http://ozg.havefunace.top

C#:   Parallel.For
来源：http://chb.fengsongda.top

================================================================================
来源：http://xll.52xcode.cn

P. 常用工具函数
来源：http://hqt.nanxinkj.top

================================================================================
来源：http://gel.gotoacloud.top

[P01] 生成 UUID
来源：http://sdo.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://mbn.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bsi.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://qah.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://cgn.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://liy.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://psa.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://msn.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://udt.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://muj.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jec.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mkp.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pkj.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dmh.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rdy.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ldz.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kmr.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tgq.hywenlv.cn

[P03] 生成短随机字符串
来源：http://wzx.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yzf.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jej.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkj.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vjr.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rxt.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://djv.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kek.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ugy.zdbjq.cn

[P04] 求长度
来源：http://sfc.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bjm.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eoy.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avn.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lcj.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://lqm.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://gvj.jinqigufen.top

Ruby: x.length;  x.size
来源：http://uoj.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xxf.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://kwv.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://abs.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kpt.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lfk.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ezm.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ufy.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://nen.tianlin.xyz

Ruby: a == b
来源：http://lns.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qeh.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wtu.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kej.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://ssp.tanke756.top


<!-- 参考信息 -->