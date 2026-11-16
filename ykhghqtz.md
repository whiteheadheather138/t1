代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vaz.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jwz.yj20258888.top

================================================================================
来源：http://lae.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://uik.aibaodan.cn

================================================================================
来源：http://kto.cucudq.cn

[M01] 读取命令行参数
来源：http://qpx.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://mxg.cashguo.top

PHP:  $argv;  $argc;
来源：http://nca.cheryme.top

JS:   process.argv.slice(2)
来源：http://gwa.uphjek.com

TS:   process.argv.slice(2)
来源：http://edg.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://oek.c1oappe.top

Go:   os.Args[1:]
来源：http://kvx.yueranfly.top

Ruby: ARGV
来源：http://qzn.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://bqf.yonumen.top

[M02] 读取环境变量
来源：http://okw.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://xpx.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qle.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://win.xuetiantiany.cn

TS:   process.env.HOME
来源：http://kfo.nwbrower.top

Java: System.getenv("HOME")
来源：http://ivs.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gcr.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://pdu.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xsp.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://ara.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://adp.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://emv.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ecx.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://drl.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qau.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://maw.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://ckh.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://vwo.daria6918.cn

[M04] 获取当前工作目录
来源：http://xpx.dianchejie.cn

Py:   os.getcwd()
来源：http://rhw.jinqigfzy.top

PHP:  getcwd();
来源：http://tfq.jinqigufen.top

JS:   process.cwd()
来源：http://brb.xuetiantiany.cn

TS:   process.cwd()
来源：http://ene.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://ees.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://mrb.quarkkingdee.top

Ruby: Dir.pwd
来源：http://wko.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://pst.ybcxt.top

[M05] 设置退出码
来源：http://smz.xziqi.cn

Py:   sys.exit(1)
来源：http://wdp.fzhhl.top

PHP:  exit(1);
来源：http://rqo.yj202588.top

JS:   process.exit(1)
来源：http://akw.tarul.cn

TS:   process.exit(1)
来源：http://qmp.xuetiantiany.cn

Java: System.exit(1)
来源：http://jxs.gotoacloud.top

Go:   os.Exit(1)
来源：http://gnj.gaohongyu789.top

Ruby: exit 1
来源：http://qjj.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://edh.hesvh.cn

[M06] 向标准错误输出
来源：http://qda.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://jia.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iix.hfpthk.cn

JS:   console.error("err")
来源：http://bbi.nwbrower.top

TS:   console.error("err")
来源：http://uhc.birdmap.top

Java: System.err.println("err")
来源：http://pcf.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mkz.andypj.xyz

Ruby: warn "err"
来源：http://pdm.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://rfu.dashuyun.cn

[M07] 判断是否为主入口
来源：http://njc.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://dlk.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://edu.ybcxt.top

JS:   require.main === module
来源：http://xqr.0kj1m.cn

TS:   require.main === module
来源：http://qrl.meibo888.top

Java: public static void main(String[] args)
来源：http://uwu.ctjpmb.com

Go:   func main()
来源：http://sns.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cvw.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://kcc.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://nie.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://fak.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://juc.shzxlz.cn

JS:   process.platform;  process.version
来源：http://fas.jinqigufen.top

TS:   process.platform;  process.version
来源：http://xci.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ipo.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://urn.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lum.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pgi.quarkkingdee.top

================================================================================
来源：http://bht.xziqi.cn

N. 数据结构与算法
来源：http://uib.ctjpmb.com

================================================================================
来源：http://tpc.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://ktf.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lge.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ave.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tpm.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idz.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://qhp.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://izt.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sur.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://dbv.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://pvc.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://ekn.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xgb.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://evk.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xrz.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tck.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://ebn.pycfn.com

Ruby: arr.sort
来源：http://rrf.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nsy.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://ock.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xio.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://yvp.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hjy.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtd.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://whh.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://moj.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ldd.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://cmr.chenzaomai.com

[N04] 斐波那契数列
来源：http://gum.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://int.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kdw.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nde.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cdm.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://toz.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zvo.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rio.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vuz.quarkkingdee.top

[N05] 最大公约数
来源：http://qxl.tian-w.cn

Py:   math.gcd(a, b)
来源：http://oku.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://igv.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xpy.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tek.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bkq.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bjb.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://iwc.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://udc.gogol.net.cn

[N06] 判断回文字符串
来源：http://tdj.daxiang520.top

Py:   s == s[::-1]
来源：http://hpt.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://qig.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://jlp.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://iiu.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qdk.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://ziz.jinqigufen.top

Ruby: s == s.reverse
来源：http://isn.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kft.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://pzl.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ayc.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gcl.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rai.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://rpi.zdbjq.cn

Java: // 手写 HashMap
来源：http://mov.shuidangran.top

Go:   // 手写 map[int]int
来源：http://hba.jianghu66.top

Ruby: // 手写 Hash
来源：http://sod.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://nfd.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://nwc.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://vej.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://rbe.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://uia.aibaodan.cn

TS:   // 手写回溯递归
来源：http://wax.wangdashe.top

Java: // 手写回溯递归
来源：http://zlg.hesvh.cn

Go:   // 手写回溯递归
来源：http://bjy.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://gwk.bjfxy.top

C#:   // 手写回溯递归
来源：http://gcw.jianghu66.top

[N09] 栈与队列
来源：http://fqy.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://srn.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gac.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dpc.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qhc.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nuc.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iwd.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hwz.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://htv.andypj.xyz

[N10] 链表节点定义
来源：http://gmi.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fey.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tde.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jcp.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fpr.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://zed.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pcz.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ylc.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://buh.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://tdn.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ntl.xinyue.icu

PHP:  // 手写递归函数
来源：http://nyb.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dzc.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bgl.gogol.net.cn

Java: // 手写递归
来源：http://tyb.redwolf501.top

Go:   // 手写递归
来源：http://uew.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gbw.9152youxi.cn

C#:   // 手写递归
来源：http://eqw.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fej.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kak.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mqc.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zyr.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nkf.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ixa.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://esq.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kyl.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xxa.haohaochexian.top

================================================================================
来源：http://wbc.jyoumei.cn

O. 并发与异步
来源：http://kwo.tarul.cn

================================================================================
来源：http://jkz.zdbjq.cn

[O01] 启动一个线程
来源：http://awy.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://imb.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wkd.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ctu.52xcode.cn

TS:   // 同 JS
来源：http://wsg.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://ylz.xuetiantiany.cn

Go:   go f()
来源：http://aja.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://lio.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://xit.quarkkingdee.top

[O02] 使用线程池
来源：http://vta.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ocs.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tcx.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://khv.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://oxx.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://hcc.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nqn.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://raa.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sdc.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://mpc.xziqi.cn

Py:   with lock: shared += 1
来源：http://bux.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cka.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://spb.ehwqpu.com

TS:   // 同 JS
来源：http://uvk.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://jph.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://osl.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bni.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://ahj.yueranfly.top

[O04] 定义异步函数并等待
来源：http://dxt.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://uva.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dyg.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://lnh.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgc.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mpc.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hwi.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dwy.havefunace.top

C#:   async Task F() { await G(); }
来源：http://oqr.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://piv.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://itp.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://usp.yj202588.top

JS:   await Promise.all(tasks)
来源：http://liq.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://dad.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tfn.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kuc.tian-w.cn

Ruby: threads.map(&:join)
来源：http://nmw.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hqc.yuanzhike.top

[O06] 使用进程池
来源：http://ydp.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kid.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qxu.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://msp.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://jmz.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vij.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hwp.zhijiandao.cn

Ruby: // fork 块
来源：http://fsy.daxiang520.top

C#:   Parallel.For
来源：http://riw.dashuyun.cn

================================================================================
来源：http://doa.fzhhl.top

P. 常用工具函数
来源：http://qdc.fanxiaobao.xyz

================================================================================
来源：http://fih.wangdashe.top

[P01] 生成 UUID
来源：http://xac.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://xul.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://flg.cashguo.top

JS:   crypto.randomUUID()
来源：http://ewi.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://tyd.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://dun.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://sbm.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://dxg.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://mnv.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://uld.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bmx.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zsv.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://msi.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://glh.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kev.gzhubu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vwv.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sxa.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uhk.aibaodan.cn

[P03] 生成短随机字符串
来源：http://whp.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dup.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wal.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://csr.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dvb.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ilm.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iti.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://eat.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://klc.xingfuxueyuan.xyz

[P04] 求长度
来源：http://hjb.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ayt.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pcg.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ehr.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://upj.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://txj.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://sba.316326.xyz

Ruby: x.length;  x.size
来源：http://pus.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jig.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://kiu.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zpl.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jcx.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://csk.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gnn.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fdn.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://rxd.quarkkingdee.top

Ruby: a == b
来源：http://cqs.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vom.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sse.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iyl.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://dss.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jzw.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://tsj.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://jen.snrcjt.cn

Go:   if x == nil {}
来源：http://thz.jqgfzy.top


<!-- 参考信息 -->