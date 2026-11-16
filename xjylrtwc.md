代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://muo.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rxq.yuxming.cn

================================================================================
来源：http://czi.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://wsh.snrcjt.cn

================================================================================
来源：http://kqm.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://fup.andypj.xyz

Py:   sys.argv[1:]
来源：http://zxa.xinyue.icu

PHP:  $argv;  $argc;
来源：http://uaf.xuanzx.com

JS:   process.argv.slice(2)
来源：http://cii.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://qdg.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://jaf.shzxlz.cn

Go:   os.Args[1:]
来源：http://ghm.uphjek.com

Ruby: ARGV
来源：http://nxk.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://zcw.ctjpmb.com

[M02] 读取环境变量
来源：http://xxd.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://ryh.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vto.chenjidiqi.icu

JS:   process.env.HOME
来源：http://vih.jianghu66.top

TS:   process.env.HOME
来源：http://jyr.ctjpmb.com

Java: System.getenv("HOME")
来源：http://ges.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://toc.yuxming.cn

Ruby: ENV["HOME"]
来源：http://tfd.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gkb.nwbrower.top

[M03] 执行外部命令
来源：http://yjn.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fvp.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ggu.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dyb.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://grk.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qgm.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ner.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://eem.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://ozm.daria6918.cn

[M04] 获取当前工作目录
来源：http://lky.xinyue.icu

Py:   os.getcwd()
来源：http://lne.cdnleiting.top

PHP:  getcwd();
来源：http://zme.shanyushiyangtech.top

JS:   process.cwd()
来源：http://eky.cucudq.cn

TS:   process.cwd()
来源：http://uge.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://iru.tanke756.top

Go:   os.Getwd()
来源：http://eep.hysaishi.cn

Ruby: Dir.pwd
来源：http://oed.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://cra.fehbvm.com

[M05] 设置退出码
来源：http://nxn.uphjek.com

Py:   sys.exit(1)
来源：http://uhx.pengpengdd.cyou

PHP:  exit(1);
来源：http://ehc.jinqigfzy.top

JS:   process.exit(1)
来源：http://wta.cqqwz.cn

TS:   process.exit(1)
来源：http://dnk.nwbrower.top

Java: System.exit(1)
来源：http://kwr.cashguo.top

Go:   os.Exit(1)
来源：http://scu.chenjidiqi.icu

Ruby: exit 1
来源：http://hux.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://add.iojbl.cn

[M06] 向标准错误输出
来源：http://xnj.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://cms.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xox.nanxinkj.top

JS:   console.error("err")
来源：http://jwo.aibaodan.cn

TS:   console.error("err")
来源：http://kfn.cucudq.cn

Java: System.err.println("err")
来源：http://qdd.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qai.chenlongwang.top

Ruby: warn "err"
来源：http://jyi.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://wtr.yonumen.top

[M07] 判断是否为主入口
来源：http://slc.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://sjm.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://brz.andypj.xyz

JS:   require.main === module
来源：http://uom.sufxvd.cn

TS:   require.main === module
来源：http://fok.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://esn.0kj1m.cn

Go:   func main()
来源：http://kuu.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ihx.zhongyouzk.top

C#:   static void Main(string[] args)
来源：http://gfj.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://vkf.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://pxd.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://iqp.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://zrd.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://zbp.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csp.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgn.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fak.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ajw.bjfxy.top

================================================================================
来源：http://bbf.iojbl.cn

N. 数据结构与算法
来源：http://suu.daxiang520.top

================================================================================
来源：http://fxh.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://mgn.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://qmn.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mqv.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xks.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fnw.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://hiw.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://hjz.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbg.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://xbb.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://qea.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://qcx.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zzw.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://mps.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hvx.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ptn.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://tqg.gogol.net.cn

Ruby: arr.sort
来源：http://onj.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vve.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://tgs.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dgo.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://aya.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tix.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kgg.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hgt.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xrg.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nua.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://vqv.jyoumei.cn

[N04] 斐波那契数列
来源：http://nzl.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qdo.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://idm.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rwi.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpe.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fid.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vob.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tdz.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vxi.zdbjq.cn

[N05] 最大公约数
来源：http://qub.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://fiq.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://inw.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://akr.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qfm.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gho.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zzi.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://mxx.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ilb.tian-w.cn

[N06] 判断回文字符串
来源：http://gou.hfpthk.cn

Py:   s == s[::-1]
来源：http://vax.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://eet.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://rvq.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://zas.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rac.316326.xyz

Go:   // 双指针从两端比较
来源：http://iwn.sweek.top

Ruby: s == s.reverse
来源：http://vfj.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gkk.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://azw.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://loz.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vzz.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jev.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://ogs.bbcook.cn

Java: // 手写 HashMap
来源：http://crx.birdmap.top

Go:   // 手写 map[int]int
来源：http://dlp.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://lyu.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zmn.tarul.cn

[N08] 生成全排列
来源：http://mgq.316326.xyz

Py:   itertools.permutations(arr)
来源：http://dis.yvedp.cn

PHP:  // 手写递归交换
来源：http://emt.jyoumei.cn

JS:   // 手写回溯递归
来源：http://grp.gzhubu.top

TS:   // 手写回溯递归
来源：http://cjg.cucudq.cn

Java: // 手写回溯递归
来源：http://jfw.nwbrower.top

Go:   // 手写回溯递归
来源：http://pui.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://rzg.yfazqb.com

C#:   // 手写回溯递归
来源：http://wlc.cashguo.top

[N09] 栈与队列
来源：http://oju.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://voc.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hxi.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vho.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vpp.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jzr.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qev.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vzg.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://top.andypj.xyz

[N10] 链表节点定义
来源：http://ptm.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qhi.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ckx.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rci.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxt.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://nun.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jux.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ruf.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zaq.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://uwg.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iqo.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://qsn.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rnp.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rav.quarkkingdee.top

Java: // 手写递归
来源：http://hdz.tanke756.top

Go:   // 手写递归
来源：http://khr.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cqz.zhixingplan.top

C#:   // 手写递归
来源：http://mmc.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ldz.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ksn.iojbl.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://onp.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qie.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://grj.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lam.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xpt.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://apg.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nah.shanyushiyangtech.top

================================================================================
来源：http://sqe.ppjwa.cn

O. 并发与异步
来源：http://czx.ydjk.org.cn

================================================================================
来源：http://xsh.ybcxt.top

[O01] 启动一个线程
来源：http://oyk.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kse.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jhq.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ktm.gotoacloud.top

TS:   // 同 JS
来源：http://kuc.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://kux.sjlbkw.cn

Go:   go f()
来源：http://wlo.iojbl.cn

Ruby: Thread.new { f }
来源：http://brt.ivvv.top

C#:   Task.Run(() => F());
来源：http://ojd.tarul.cn

[O02] 使用线程池
来源：http://jen.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dtz.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://utn.daxiang520.top

JS:   // worker_threads 线程池
来源：http://gov.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://six.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://qdl.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjq.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hrk.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tjh.fengsongda.top

[O03] 加锁保护共享数据
来源：http://hxs.andypj.xyz

Py:   with lock: shared += 1
来源：http://hqk.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://pbb.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rfu.fktsv.cn

TS:   // 同 JS
来源：http://xmb.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://ujg.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lwv.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sdp.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://mjs.tanke756.top

[O04] 定义异步函数并等待
来源：http://htd.uphjek.com

Py:   async def f():⏎    await g()
来源：http://trr.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ssn.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://jhh.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://nae.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tqi.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cho.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://ruu.cashguo.top

C#:   async Task F() { await G(); }
来源：http://itk.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://gix.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://akj.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://suk.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://wqe.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://olw.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lle.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wpd.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://rla.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qqw.cashguo.top

[O06] 使用进程池
来源：http://ncw.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wwm.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ijd.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://blo.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://yzv.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://olq.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://czr.nanxinkj.top

Ruby: // fork 块
来源：http://tiz.xylfe.cn

C#:   Parallel.For
来源：http://lyo.zhengqikj.top

================================================================================
来源：http://lsl.c1oappe.top

P. 常用工具函数
来源：http://jwu.jiagoushi.top

================================================================================
来源：http://knu.zhengqikj.top

[P01] 生成 UUID
来源：http://pwx.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://bot.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vrn.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://drz.ydzc1.top

TS:   crypto.randomUUID()
来源：http://rcg.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://zbb.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://lje.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://hey.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://cfq.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://iog.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ene.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rmr.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ntn.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nvo.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eyg.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ksh.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kik.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gnu.zdbjq.cn

[P03] 生成短随机字符串
来源：http://prt.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://spi.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qhq.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fms.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ubx.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nhc.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ubz.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://brf.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hbd.shangyingyoupin.top

[P04] 求长度
来源：http://szc.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vft.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwd.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akg.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oey.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://wxb.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://whw.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://mve.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hdk.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://pne.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://nlx.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bmi.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nzz.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adq.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hfw.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://wly.fzhhl.top

Ruby: a == b
来源：http://gob.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cqq.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://apo.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cyv.cheryme.top

PHP:  if (empty($x)) {}
来源：http://ggn.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qwm.fengsongda.top

TS:   if (x == null) {}
来源：http://mwc.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ohb.yj202588.top

Go:   if x == nil {}
来源：http://ehi.epnwcf.com


<!-- 参考信息 -->