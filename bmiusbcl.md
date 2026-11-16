代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xbn.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dxv.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://djm.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hrn.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://goj.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iyp.xylfe.cn

================================================================================
来源：http://nka.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://glf.dianchejie.cn

================================================================================
来源：http://sbg.yj20258888.top

[M01] 读取命令行参数
来源：http://oop.shzxlz.cn

Py:   sys.argv[1:]
来源：http://hhr.c1oappe.top

PHP:  $argv;  $argc;
来源：http://gvd.ydzc1.top

JS:   process.argv.slice(2)
来源：http://gsi.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://zyd.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://zit.cqqwz.cn

Go:   os.Args[1:]
来源：http://tnv.yueranfly.top

Ruby: ARGV
来源：http://hbj.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://rwq.bbcook.cn

[M02] 读取环境变量
来源：http://qxh.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://aih.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uki.cqqwz.cn

JS:   process.env.HOME
来源：http://alh.ybcxt.top

TS:   process.env.HOME
来源：http://uzv.ehwqpu.com

Java: System.getenv("HOME")
来源：http://xzw.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aik.zycfv.cn

Ruby: ENV["HOME"]
来源：http://awy.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bay.uphjek.com

[M03] 执行外部命令
来源：http://fxn.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vzr.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://exg.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oen.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kgj.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://epy.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://mqk.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://ueu.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://vkq.fehbvm.com

[M04] 获取当前工作目录
来源：http://sus.pycfn.com

Py:   os.getcwd()
来源：http://nsu.ivvv.top

PHP:  getcwd();
来源：http://kcm.nanxuanxn.top

JS:   process.cwd()
来源：http://tpq.xuanzx.com

TS:   process.cwd()
来源：http://vmj.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://wje.mhx1999.top

Go:   os.Getwd()
来源：http://lsl.hnxiangtu.top

Ruby: Dir.pwd
来源：http://osd.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://uxd.fktsv.cn

[M05] 设置退出码
来源：http://tgh.9152youxi.cn

Py:   sys.exit(1)
来源：http://mjf.wangshuangyany.cn

PHP:  exit(1);
来源：http://lcs.ivvv.top

JS:   process.exit(1)
来源：http://oub.vqdsnc.cn

TS:   process.exit(1)
来源：http://ria.zhixingplan.top

Java: System.exit(1)
来源：http://ikh.316326.xyz

Go:   os.Exit(1)
来源：http://uam.fehbvm.com

Ruby: exit 1
来源：http://xxi.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hhe.birdmap.top

[M06] 向标准错误输出
来源：http://lrb.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://san.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hgb.hcnkem.com

JS:   console.error("err")
来源：http://kfg.quarkkingdee.top

TS:   console.error("err")
来源：http://mnr.yj20258888.top

Java: System.err.println("err")
来源：http://que.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rft.sxryk.cn

Ruby: warn "err"
来源：http://nni.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://knx.birdmap.top

[M07] 判断是否为主入口
来源：http://vax.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://kmz.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kqx.shangyingyoupin.top

JS:   require.main === module
来源：http://jfl.tianlin.xyz

TS:   require.main === module
来源：http://ipk.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://tad.zhoulong.xyz

Go:   func main()
来源：http://atp.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bnx.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://vhj.pycfn.com

[M08] 获取系统与运行时信息
来源：http://cch.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://ihp.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://ibs.gogol.net.cn

JS:   process.platform;  process.version
来源：http://dsl.zycfv.cn

TS:   process.platform;  process.version
来源：http://qtb.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oaa.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cqd.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fyi.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tnx.jinghuilouyu.cn

================================================================================
来源：http://zdk.hnxiangtu.top

N. 数据结构与算法
来源：http://owl.shuidangran.top

================================================================================
来源：http://knu.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://wmd.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qro.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zyv.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zho.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbv.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kfx.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://zto.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfn.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://fqf.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://mki.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://jdr.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bpj.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yot.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yos.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eey.meibo888.top

Go:   slices.Sort(arr)
来源：http://uwe.zhiwuduotai.top

Ruby: arr.sort
来源：http://ycq.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nvy.hammf.cn

[N03] 快速排序（分治示例）
来源：http://eek.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blj.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://uvc.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tbe.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hyn.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ngn.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kqp.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xth.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://iko.hcnkem.com

[N04] 斐波那契数列
来源：http://pbv.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ema.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jfh.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://woh.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nik.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://esl.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zmh.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ezd.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yiy.pycfn.com

[N05] 最大公约数
来源：http://akp.yfazqb.com

Py:   math.gcd(a, b)
来源：http://uwn.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oiw.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tgm.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jtd.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sby.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://byv.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://pur.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pfy.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://tsm.bbcook.cn

Py:   s == s[::-1]
来源：http://lfu.bbcook.cn

PHP:  $s === strrev($s);
来源：http://shb.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://qbx.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://zva.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dbl.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://cwy.birdmap.top

Ruby: s == s.reverse
来源：http://imt.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ees.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://col.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bnn.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zls.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://owi.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://ghr.jlsjyb.cn

Java: // 手写 HashMap
来源：http://fmh.c1oappe.top

Go:   // 手写 map[int]int
来源：http://lnu.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://ocw.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ibi.bbcook.cn

[N08] 生成全排列
来源：http://ivp.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://oud.ctjpmb.com

PHP:  // 手写递归交换
来源：http://rix.xylfe.cn

JS:   // 手写回溯递归
来源：http://ubz.xuanzx.com

TS:   // 手写回溯递归
来源：http://vdc.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://izx.epnwcf.com

Go:   // 手写回溯递归
来源：http://aee.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://wtu.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://smg.birdmap.top

[N09] 栈与队列
来源：http://umv.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://scp.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mpb.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fip.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wrp.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xiu.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://giv.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oib.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lei.iojbl.cn

[N10] 链表节点定义
来源：http://vfe.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hjw.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bnx.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://meh.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://erv.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://awh.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://hfk.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qnt.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bib.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://iwi.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ust.pycfn.com

PHP:  // 手写递归函数
来源：http://mvv.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uhk.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbu.zycfv.cn

Java: // 手写递归
来源：http://poo.yonumen.top

Go:   // 手写递归
来源：http://lnv.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ebn.ydzc1.top

C#:   // 手写递归
来源：http://duw.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zec.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vyp.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sug.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bki.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcr.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lyk.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jka.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nld.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://his.jyoumei.cn

================================================================================
来源：http://bdy.yj20258.top

O. 并发与异步
来源：http://vao.jqgufenzy.top

================================================================================
来源：http://umx.fengsongda.top

[O01] 启动一个线程
来源：http://ala.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ygb.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gqc.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gge.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://srh.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://vsi.hcnkem.com

Go:   go f()
来源：http://brx.cashguo.top

Ruby: Thread.new { f }
来源：http://ift.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://kgk.daria6918.cn

[O02] 使用线程池
来源：http://and.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://opo.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zla.gzhubu.top

JS:   // worker_threads 线程池
来源：http://vpj.shuidangran.top

TS:   // worker_threads 线程池
来源：http://umc.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vdm.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qpe.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vfy.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bee.birdmap.top

[O03] 加锁保护共享数据
来源：http://lgb.hammf.cn

Py:   with lock: shared += 1
来源：http://xti.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://myj.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fmc.meibo888.top

TS:   // 同 JS
来源：http://lxu.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://pdp.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://asy.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uqq.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://dos.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://nlx.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://xsf.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xhs.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://quh.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nvr.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cja.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xfg.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://sxp.cheryme.top

C#:   async Task F() { await G(); }
来源：http://xqc.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://ccc.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://ojl.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ral.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://xef.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://klb.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iyu.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ucf.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://bob.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://jhz.yangfankeji.com

[O06] 使用进程池
来源：http://fnu.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://onh.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qzw.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://hns.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://zer.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rea.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kvm.chenzaomai.com

Ruby: // fork 块
来源：http://tvd.yfazqb.com

C#:   Parallel.For
来源：http://rbo.jinqigufen.top

================================================================================
来源：http://hos.jinqigfzy.top

P. 常用工具函数
来源：http://pew.nanxuanxn.top

================================================================================
来源：http://ddy.jlsjyb.cn

[P01] 生成 UUID
来源：http://lzd.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://rfm.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://our.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://jxq.hcnkem.com

TS:   crypto.randomUUID()
来源：http://szu.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://epo.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://oyz.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://tjs.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://zwi.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://pxu.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rnh.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://owf.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rdx.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vtt.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ygi.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jpg.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mpg.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://efz.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://sjf.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aot.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oxs.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qnf.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gug.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ned.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wek.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aqh.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eat.sufxvd.cn

[P04] 求长度
来源：http://yzu.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://utp.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jbd.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uex.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rxd.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://gby.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://tbq.jqgfzy.top

Ruby: x.length;  x.size
来源：http://awq.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wsu.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://cae.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eqx.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yoi.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mlu.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mcx.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pnn.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://yxd.bbcook.cn

Ruby: a == b
来源：http://vim.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ksw.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fhz.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hii.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://ybe.havefunace.top


<!-- 参考信息 -->