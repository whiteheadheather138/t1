代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bbf.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oyd.gaohongyu789.top

================================================================================
来源：http://ziw.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://xfa.c1oappe.top

================================================================================
来源：http://qpd.cdnleiting.top

[M01] 读取命令行参数
来源：http://ibu.hammf.cn

Py:   sys.argv[1:]
来源：http://xqs.sysykeji.top

PHP:  $argv;  $argc;
来源：http://mjj.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://udi.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://tyo.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://nua.ctjpmb.com

Go:   os.Args[1:]
来源：http://acm.cashguo.top

Ruby: ARGV
来源：http://qbr.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://jvo.52xcode.cn

[M02] 读取环境变量
来源：http://aoj.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://vme.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xzo.9152youxi.cn

JS:   process.env.HOME
来源：http://gpw.zhengqikj.top

TS:   process.env.HOME
来源：http://dlv.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://qjd.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kst.iojbl.cn

Ruby: ENV["HOME"]
来源：http://ial.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fik.daxiang520.top

[M03] 执行外部命令
来源：http://ndb.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fbx.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bre.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ily.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tln.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xjs.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wkf.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kkf.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://hqq.jianghu66.top

[M04] 获取当前工作目录
来源：http://ewd.xuanzx.com

Py:   os.getcwd()
来源：http://ghm.zycfv.cn

PHP:  getcwd();
来源：http://gnh.hysaishi.cn

JS:   process.cwd()
来源：http://bdq.xuetiantiany.cn

TS:   process.cwd()
来源：http://bhf.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://ulc.daria6918.cn

Go:   os.Getwd()
来源：http://xvr.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://fyd.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vqy.zdqjudy.top

[M05] 设置退出码
来源：http://iwv.bjfxy.top

Py:   sys.exit(1)
来源：http://exr.meibo888.top

PHP:  exit(1);
来源：http://tol.zhixingplan.top

JS:   process.exit(1)
来源：http://qav.xuanzx.com

TS:   process.exit(1)
来源：http://koa.yvedp.cn

Java: System.exit(1)
来源：http://uaj.aizwys.cn

Go:   os.Exit(1)
来源：http://suf.yuxming.cn

Ruby: exit 1
来源：http://peq.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rjm.jinqigufen.top

[M06] 向标准错误输出
来源：http://ihj.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://nqq.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://byq.gogol.net.cn

JS:   console.error("err")
来源：http://qmv.yuanzhike.top

TS:   console.error("err")
来源：http://tdp.ppjwa.cn

Java: System.err.println("err")
来源：http://xzb.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rzi.hfpthk.cn

Ruby: warn "err"
来源：http://yfz.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://scp.xziqi.cn

[M07] 判断是否为主入口
来源：http://cgc.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://ntw.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xar.snrcjt.cn

JS:   require.main === module
来源：http://fff.cqqwz.cn

TS:   require.main === module
来源：http://dho.daria6918.cn

Java: public static void main(String[] args)
来源：http://tva.xingfuxueyuan.xyz

Go:   func main()
来源：http://hnj.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zak.hesvh.cn

C#:   static void Main(string[] args)
来源：http://paw.yj20258.top

[M08] 获取系统与运行时信息
来源：http://bax.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://lnp.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://ojl.meibo888.top

JS:   process.platform;  process.version
来源：http://uof.dashuyun.cn

TS:   process.platform;  process.version
来源：http://sdw.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ydb.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://kzw.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://unn.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zvx.bjfxy.top

================================================================================
来源：http://gpb.shangyingyoupin.top

N. 数据结构与算法
来源：http://klv.hesvh.cn

================================================================================
来源：http://gpu.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://fkl.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://loy.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gij.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wxp.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://txz.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://wpu.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://pfl.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zbo.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://fbs.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://azq.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://thq.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mns.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://xqq.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ypc.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jkm.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://bdj.fzhhl.top

Ruby: arr.sort
来源：http://wye.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gfo.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://wdt.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xcm.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://lhd.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iiz.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pse.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://myk.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ves.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mkd.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://ubk.yj20258.top

[N04] 斐波那契数列
来源：http://ffy.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jjb.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nts.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fqp.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xvq.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vmi.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://llq.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sfr.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rgc.ydzc1.top

[N05] 最大公约数
来源：http://nsi.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://qlm.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://moz.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rdu.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vmf.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wzd.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cgn.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://pgk.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mkr.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://gqu.redwolf501.top

Py:   s == s[::-1]
来源：http://apx.yonumen.top

PHP:  $s === strrev($s);
来源：http://dov.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://huz.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://gmg.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvg.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://dfn.sufxvd.cn

Ruby: s == s.reverse
来源：http://thi.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zec.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://dad.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mfi.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kql.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cms.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://bcv.sjlbkw.cn

Java: // 手写 HashMap
来源：http://sai.nwbrower.top

Go:   // 手写 map[int]int
来源：http://nkr.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://orz.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://ssv.xinyue.icu

[N08] 生成全排列
来源：http://igx.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://mff.epnwcf.com

PHP:  // 手写递归交换
来源：http://rkk.ehwqpu.com

JS:   // 手写回溯递归
来源：http://pin.dashuyun.cn

TS:   // 手写回溯递归
来源：http://aag.meibo888.top

Java: // 手写回溯递归
来源：http://jph.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://tei.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://aoe.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://qmr.wangdashe.top

[N09] 栈与队列
来源：http://div.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ukn.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://drb.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bwp.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tmo.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fzy.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gld.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://idz.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vqi.bbcook.cn

[N10] 链表节点定义
来源：http://fyi.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://noi.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xtx.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vsw.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pdh.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://nhd.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://jej.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kco.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zro.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://pmh.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ihl.jqgfzy.top

PHP:  // 手写递归函数
来源：http://hei.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://goj.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vay.ppjwa.cn

Java: // 手写递归
来源：http://dep.ppjwa.cn

Go:   // 手写递归
来源：http://ech.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://phr.hfpthk.cn

C#:   // 手写递归
来源：http://fic.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mwd.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://axo.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jym.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofp.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jzb.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qlw.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uby.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wsk.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cvq.xuanzx.com

================================================================================
来源：http://kuz.zhaomingkeji.xyz

O. 并发与异步
来源：http://jcv.yueranfly.top

================================================================================
来源：http://ohh.cdnleiting.top

[O01] 启动一个线程
来源：http://iax.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pub.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ptg.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iah.wangdashe.top

TS:   // 同 JS
来源：http://pkb.zhongyouzk.top

Java: new Thread(() -> f()).start()
来源：http://hpn.tarul.cn

Go:   go f()
来源：http://zfe.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://jkh.xziqi.cn

C#:   Task.Run(() => F());
来源：http://gcq.smart0.xyz

[O02] 使用线程池
来源：http://pvv.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kex.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yep.yueranfly.top

JS:   // worker_threads 线程池
来源：http://jii.yvedp.cn

TS:   // worker_threads 线程池
来源：http://oid.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pbt.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjc.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bxx.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hfs.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://tsv.svipenyu.cn

Py:   with lock: shared += 1
来源：http://hsp.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://cpi.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hgv.gogol.net.cn

TS:   // 同 JS
来源：http://ppx.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://wvy.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ufs.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xcb.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://lmm.yonumen.top

[O04] 定义异步函数并等待
来源：http://jxt.yongpay.top

Py:   async def f():⏎    await g()
来源：http://rei.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pqt.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://vmw.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xop.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oel.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lkv.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xtk.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://rnb.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://iku.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://rvn.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mpc.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://awi.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://una.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://avm.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lou.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://vog.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ywv.sxryk.cn

[O06] 使用进程池
来源：http://zwg.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dnn.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lik.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://wvz.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://fwv.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://phd.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qmn.hcnkem.com

Ruby: // fork 块
来源：http://xht.aizwys.cn

C#:   Parallel.For
来源：http://phr.snrcjt.cn

================================================================================
来源：http://uxy.daria6918.cn

P. 常用工具函数
来源：http://ahv.aibaodan.cn

================================================================================
来源：http://rxb.yonumen.top

[P01] 生成 UUID
来源：http://ekv.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://uyu.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wti.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://wkf.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://htx.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://qkc.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://lmw.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://uhd.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://jnr.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://dgo.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aub.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qgb.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ekp.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jww.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pkt.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lka.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bjs.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ubp.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://cen.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhc.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nuj.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ita.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aez.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://elj.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://crs.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zxy.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jiw.sysykeji.top

[P04] 求长度
来源：http://ngw.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qan.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cdb.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://afm.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxy.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://exa.316326.xyz

Go:   len(arr);  len(m)
来源：http://lso.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://ewc.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qef.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://jyv.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pao.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fyd.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xof.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gbh.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lik.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://wkf.vehdjk.com

Ruby: a == b
来源：http://mat.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xru.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nov.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xdw.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://jwx.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xyt.havefunace.top

TS:   if (x == null) {}
来源：http://knm.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bpv.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://grv.sjlbkw.cn


<!-- 参考信息 -->