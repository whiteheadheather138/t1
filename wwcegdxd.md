代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vzr.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkf.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lah.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ulg.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ygs.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ozs.gotoacloud.top

================================================================================
来源：http://rtw.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://xli.chenjidiqi.icu

================================================================================
来源：http://ltc.sjlbkw.cn

[M01] 读取命令行参数
来源：http://szu.bbcook.cn

Py:   sys.argv[1:]
来源：http://jou.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://nyg.316326.xyz

JS:   process.argv.slice(2)
来源：http://fqy.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://hom.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://ecc.zycfv.cn

Go:   os.Args[1:]
来源：http://efm.tarul.cn

Ruby: ARGV
来源：http://bfv.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://lko.jinqigufen.top

[M02] 读取环境变量
来源：http://nxn.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://ghw.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mmu.yfazqb.com

JS:   process.env.HOME
来源：http://edd.feifeiyinyue.top

TS:   process.env.HOME
来源：http://lxg.wangdashe.top

Java: System.getenv("HOME")
来源：http://hoe.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jzd.zhaomingkeji.xyz

Ruby: ENV["HOME"]
来源：http://sni.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ldo.jyoumei.cn

[M03] 执行外部命令
来源：http://grp.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tqz.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qum.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xtw.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mwm.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ada.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lhy.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ylk.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://qfl.sxryk.cn

[M04] 获取当前工作目录
来源：http://vdr.birdmap.top

Py:   os.getcwd()
来源：http://hkd.jqgfzy.top

PHP:  getcwd();
来源：http://mpt.redwolf501.top

JS:   process.cwd()
来源：http://uvt.xylfe.cn

TS:   process.cwd()
来源：http://ais.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://lrb.9152youxi.cn

Go:   os.Getwd()
来源：http://eka.sufxvd.cn

Ruby: Dir.pwd
来源：http://fsh.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ejk.xinyue.icu

[M05] 设置退出码
来源：http://vkj.nwbrower.top

Py:   sys.exit(1)
来源：http://toz.gotoacloud.top

PHP:  exit(1);
来源：http://vls.feifeiyinyue.top

JS:   process.exit(1)
来源：http://ngk.zhongyouzk.top

TS:   process.exit(1)
来源：http://uox.jqgfzy.top

Java: System.exit(1)
来源：http://ijm.sufxvd.cn

Go:   os.Exit(1)
来源：http://jok.hongshengwenyu.top

Ruby: exit 1
来源：http://ezt.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wnb.9152youxi.cn

[M06] 向标准错误输出
来源：http://ote.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://vzy.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nxn.nwbrower.top

JS:   console.error("err")
来源：http://rrh.gzhubu.top

TS:   console.error("err")
来源：http://lsg.zdbjq.cn

Java: System.err.println("err")
来源：http://saw.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kbg.kuanghao11.cn

Ruby: warn "err"
来源：http://hqy.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://ljm.dianchejie.cn

[M07] 判断是否为主入口
来源：http://vcb.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://jup.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nvx.shanyushiyangtech.top

JS:   require.main === module
来源：http://omy.zhaomingkeji.xyz

TS:   require.main === module
来源：http://ney.yuxming.cn

Java: public static void main(String[] args)
来源：http://kwg.zhiwuduotai.top

Go:   func main()
来源：http://gdc.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mac.fengsongda.top

C#:   static void Main(string[] args)
来源：http://vmr.havefunace.top

[M08] 获取系统与运行时信息
来源：http://sdk.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://sqv.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://jgy.snrcjt.cn

JS:   process.platform;  process.version
来源：http://ldl.aibaodan.cn

TS:   process.platform;  process.version
来源：http://rej.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gwo.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ysk.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yyr.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://trk.gzhubu.top

================================================================================
来源：http://bvn.ivvv.top

N. 数据结构与算法
来源：http://zuw.xylfe.cn

================================================================================
来源：http://dbh.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://lbu.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://msw.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://adb.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snb.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gei.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rto.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://vfd.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ztf.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://xcz.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://mud.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://agk.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nfm.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hug.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bis.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ido.xylfe.cn

Go:   slices.Sort(arr)
来源：http://ppr.snrcjt.cn

Ruby: arr.sort
来源：http://ohh.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xde.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://lbz.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kmz.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://wsl.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ilz.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gfu.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dru.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hed.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bbi.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://vbx.nanxinkj.top

[N04] 斐波那契数列
来源：http://bdp.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vnl.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jjb.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fga.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://egl.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pho.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nup.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owd.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fya.gzhubu.top

[N05] 最大公约数
来源：http://zfb.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://qao.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gep.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vkb.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://foy.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vxx.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ytp.sufxvd.cn

Ruby: a.gcd(b)
来源：http://uxy.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ljl.cheryme.top

[N06] 判断回文字符串
来源：http://qxi.tarul.cn

Py:   s == s[::-1]
来源：http://ups.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://qfu.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://fck.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://hbt.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rpj.guannengcc.top

Go:   // 双指针从两端比较
来源：http://qdi.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://jqj.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cvf.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://sjp.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gno.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kwo.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xri.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://okl.chenzaomai.com

Java: // 手写 HashMap
来源：http://wnc.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://nuv.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://cmu.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mlc.bjfxy.top

[N08] 生成全排列
来源：http://yfi.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://xcl.ctjpmb.com

PHP:  // 手写递归交换
来源：http://rcq.sxryk.cn

JS:   // 手写回溯递归
来源：http://adf.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://dwh.yj202588.top

Java: // 手写回溯递归
来源：http://off.yonumen.top

Go:   // 手写回溯递归
来源：http://obq.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://cjn.meibo888.top

C#:   // 手写回溯递归
来源：http://tre.tianlin.xyz

[N09] 栈与队列
来源：http://fas.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yha.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gtq.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jgs.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hnn.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ekk.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ssc.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ebv.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxl.zhijiandao.cn

[N10] 链表节点定义
来源：http://dld.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ejw.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://rwq.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hml.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ykx.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://our.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iam.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://uqy.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://whp.wangdashe.top

[N11] 二叉树中序遍历
来源：http://ueg.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dlo.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://xys.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zxa.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikf.jinyuanbaomall.cn

Java: // 手写递归
来源：http://one.yj20258.top

Go:   // 手写递归
来源：http://fvx.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ggr.chenzaomai.com

C#:   // 手写递归
来源：http://wzj.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sqt.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xqk.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lua.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kja.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbf.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yyz.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kuu.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://opc.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ofc.snrcjt.cn

================================================================================
来源：http://kje.uphjek.com

O. 并发与异步
来源：http://pob.hesvh.cn

================================================================================
来源：http://utr.snrcjt.cn

[O01] 启动一个线程
来源：http://dzj.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hkh.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lte.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zmb.aibaodan.cn

TS:   // 同 JS
来源：http://plu.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://qxk.vqdsnc.cn

Go:   go f()
来源：http://bht.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://mit.fengsongda.top

C#:   Task.Run(() => F());
来源：http://rdo.haohaochexian.top

[O02] 使用线程池
来源：http://tcx.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://txa.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sym.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://qkw.aizwys.cn

TS:   // worker_threads 线程池
来源：http://qkt.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://boc.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xvd.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qch.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fxa.yj20258888.top

[O03] 加锁保护共享数据
来源：http://snp.haohaochexian.top

Py:   with lock: shared += 1
来源：http://kcz.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://sof.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://glp.xylfe.cn

TS:   // 同 JS
来源：http://bie.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://ikh.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qlz.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pzr.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://mux.zhengqikj.top

[O04] 定义异步函数并等待
来源：http://swa.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://yrg.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tla.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://eyi.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vrm.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sbu.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cjm.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://qaa.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://bgw.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://nzx.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://imm.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://onw.yonumen.top

JS:   await Promise.all(tasks)
来源：http://dqo.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://ben.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mnk.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mec.andypj.xyz

Ruby: threads.map(&:join)
来源：http://voy.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wgu.316326.xyz

[O06] 使用进程池
来源：http://twp.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adn.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uez.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://nay.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://gcb.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ftw.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tkw.cashguo.top

Ruby: // fork 块
来源：http://pqp.wangdashe.top

C#:   Parallel.For
来源：http://fsu.mhx1999.top

================================================================================
来源：http://wyl.vqdsnc.cn

P. 常用工具函数
来源：http://zst.yuanzhike.top

================================================================================
来源：http://gcu.ydzc1.top

[P01] 生成 UUID
来源：http://mmz.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://mwm.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mfs.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://ksy.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://wnc.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://qox.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://rwl.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://iad.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://giv.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://myf.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xbs.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eed.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lqg.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://esv.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://owk.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pjk.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hnd.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fas.aizwys.cn

[P03] 生成短随机字符串
来源：http://zxm.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tor.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cug.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qdb.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zsv.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aax.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jkj.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wyq.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dpa.meibo888.top

[P04] 求长度
来源：http://fdx.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zhn.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lvp.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bvg.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://heg.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://fbd.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://wox.xuanzx.com

Ruby: x.length;  x.size
来源：http://psb.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://zms.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://ubk.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zdb.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nhv.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gtp.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dxc.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tst.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jyr.bbcook.cn

Ruby: a == b
来源：http://wmb.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rza.gogol.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sxz.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rhp.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://tbi.zhiwuduotai.top


<!-- 参考信息 -->