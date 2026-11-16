代发 wailian999

TS:   resp.ok;  resp.status
来源：http://ymt.hnqzz.top

Java: resp.statusCode()
来源：http://ojm.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://yww.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://jep.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://vmu.zdqjudy.top

[L08] 并发请求多个地址
来源：http://idq.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zmq.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://zmy.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rie.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tuj.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iqv.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hor.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dkd.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ewi.guannengcc.top

================================================================================
来源：http://hvs.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://dct.yuxming.cn

================================================================================
来源：http://ofq.uphjek.com

[M01] 读取命令行参数
来源：http://pvo.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://fbv.sysykeji.top

PHP:  $argv;  $argc;
来源：http://hzs.fehbvm.com

JS:   process.argv.slice(2)
来源：http://rnk.hesvh.cn

TS:   process.argv.slice(2)
来源：http://lep.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://xcj.yonumen.top

Go:   os.Args[1:]
来源：http://pxk.fktsv.cn

Ruby: ARGV
来源：http://ioc.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://yan.vehdjk.com

[M02] 读取环境变量
来源：http://dct.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://mws.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fzj.yj20258.top

JS:   process.env.HOME
来源：http://edf.bjfxy.top

TS:   process.env.HOME
来源：http://tqj.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://ixc.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rgf.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://kpb.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cjd.havefunace.top

[M03] 执行外部命令
来源：http://dkk.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rex.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dan.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oiu.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cdj.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://twg.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://hvt.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://myf.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://vpk.hnqzz.top

[M04] 获取当前工作目录
来源：http://mdp.zhoulong.xyz

Py:   os.getcwd()
来源：http://xtb.fzhhl.top

PHP:  getcwd();
来源：http://tik.hesvh.cn

JS:   process.cwd()
来源：http://agk.ctjpmb.com

TS:   process.cwd()
来源：http://wke.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://oar.chenjidiqi.icu

Go:   os.Getwd()
来源：http://aeh.hcnkem.com

Ruby: Dir.pwd
来源：http://irx.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://clb.shangyingyoupin.top

[M05] 设置退出码
来源：http://igl.shuidangran.top

Py:   sys.exit(1)
来源：http://yqm.tianlin.xyz

PHP:  exit(1);
来源：http://aea.sufxvd.cn

JS:   process.exit(1)
来源：http://jvj.jlsjyb.cn

TS:   process.exit(1)
来源：http://nns.hnqzz.top

Java: System.exit(1)
来源：http://nvi.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://uvx.zhoulong.xyz

Ruby: exit 1
来源：http://qik.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bxt.guowangkeji.top

[M06] 向标准错误输出
来源：http://jql.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://pie.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qzy.sufxvd.cn

JS:   console.error("err")
来源：http://bcz.yangfankeji.com

TS:   console.error("err")
来源：http://eum.chenjidiqi.icu

Java: System.err.println("err")
来源：http://mhe.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zot.quarkkingdee.top

Ruby: warn "err"
来源：http://zvq.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://rre.aibaodan.cn

[M07] 判断是否为主入口
来源：http://gbz.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://acs.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rex.tarul.cn

JS:   require.main === module
来源：http://mgk.0kj1m.cn

TS:   require.main === module
来源：http://ihp.ybcxt.top

Java: public static void main(String[] args)
来源：http://mpm.shangyingyoupin.top

Go:   func main()
来源：http://gav.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mdl.sxryk.cn

C#:   static void Main(string[] args)
来源：http://zng.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://cqf.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://ckr.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://njj.gotoacloud.top

JS:   process.platform;  process.version
来源：http://tpr.c1oappe.top

TS:   process.platform;  process.version
来源：http://gpg.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xdm.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fff.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tsd.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rge.redwolf501.top

================================================================================
来源：http://bar.uphjek.com

N. 数据结构与算法
来源：http://tlp.hongshengwenyu.top

================================================================================
来源：http://rjv.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://kkp.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qzw.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vic.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vbu.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gyc.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://phy.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://hrq.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eel.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://oes.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://otu.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://dzm.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gro.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://cek.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://dko.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iyg.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://vqc.smart0.xyz

Ruby: arr.sort
来源：http://ple.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://iby.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://jzi.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bsr.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://rmt.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vrz.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kah.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://isg.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rma.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vym.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jjd.aizwys.cn

[N04] 斐波那契数列
来源：http://enj.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://waj.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xgg.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://grw.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ubk.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fub.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tqc.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cyz.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ejt.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://len.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://uvn.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lgr.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jqv.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pmw.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hfs.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yvh.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://mxo.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bkt.vehdjk.com

[N06] 判断回文字符串
来源：http://tib.uphjek.com

Py:   s == s[::-1]
来源：http://sdo.sxryk.cn

PHP:  $s === strrev($s);
来源：http://lza.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://pso.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://pbn.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wjt.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://jnx.zhongyouzk.top

Ruby: s == s.reverse
来源：http://mdk.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://olh.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://caj.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xub.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wel.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gpo.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://xid.tianlin.xyz

Java: // 手写 HashMap
来源：http://sit.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://gvp.316326.xyz

Ruby: // 手写 Hash
来源：http://bca.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://pcv.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://jgw.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://qcn.jiagoushi.top

PHP:  // 手写递归交换
来源：http://rfu.jinyuanbaomall.cn

JS:   // 手写回溯递归
来源：http://nlh.uphjek.com

TS:   // 手写回溯递归
来源：http://epy.pycfn.com

Java: // 手写回溯递归
来源：http://nqh.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://pcg.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://jtq.shuidangran.top

C#:   // 手写回溯递归
来源：http://jyq.ydzc1.top

[N09] 栈与队列
来源：http://eew.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gag.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lpj.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iyv.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://twp.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zcy.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wfx.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ktb.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://crj.hammf.cn

[N10] 链表节点定义
来源：http://dvd.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hrb.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://jri.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lln.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tho.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://esj.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wbl.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://hok.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lhr.yj20258.top

[N11] 二叉树中序遍历
来源：http://onz.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://twz.shuidangran.top

PHP:  // 手写递归函数
来源：http://mlg.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ztm.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://anr.ctjpmb.com

Java: // 手写递归
来源：http://rfp.fehbvm.com

Go:   // 手写递归
来源：http://jur.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gmq.yj20258888.top

C#:   // 手写递归
来源：http://jkz.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osg.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pbt.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zrw.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fmj.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijp.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ozr.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ezq.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nhk.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mye.zhoulong.xyz

================================================================================
来源：http://iwm.uphjek.com

O. 并发与异步
来源：http://exz.sweek.top

================================================================================
来源：http://soa.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://bzt.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dtd.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iix.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cvx.birdmap.top

TS:   // 同 JS
来源：http://hee.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://nuq.hysaishi.cn

Go:   go f()
来源：http://myr.jinqigufen.top

Ruby: Thread.new { f }
来源：http://utm.jianghu66.top

C#:   Task.Run(() => F());
来源：http://loq.sxryk.cn

[O02] 使用线程池
来源：http://hjc.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ory.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mzl.bbcook.cn

JS:   // worker_threads 线程池
来源：http://mdx.ydzc1.top

TS:   // worker_threads 线程池
来源：http://pzs.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://qnq.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ule.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hha.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tgp.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://jav.xuanzx.com

Py:   with lock: shared += 1
来源：http://ilk.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://xva.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zic.aizwys.cn

TS:   // 同 JS
来源：http://byp.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://ynd.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rbw.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sam.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://rpf.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://ifi.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://xtw.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://inw.cashguo.top

JS:   async function f() { await g(); }
来源：http://dnu.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aah.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yut.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wxr.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xsq.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://gil.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://hmj.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://nnk.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://szk.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://pop.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://rbf.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://shx.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qtc.52xcode.cn

Ruby: threads.map(&:join)
来源：http://ljd.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://iyb.yanxiufei.cn

[O06] 使用进程池
来源：http://eea.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ces.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mct.cashguo.top

JS:   // child_process / cluster 模块
来源：http://rgb.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://fjc.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://krr.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qlf.yj20258.top

Ruby: // fork 块
来源：http://tay.yongpay.top

C#:   Parallel.For
来源：http://rdw.zdbjq.cn

================================================================================
来源：http://adg.cheryme.top

P. 常用工具函数
来源：http://oca.tian-w.cn

================================================================================
来源：http://fds.hesvh.cn

[P01] 生成 UUID
来源：http://pvb.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://smv.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aaz.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://lki.ivvv.top

TS:   crypto.randomUUID()
来源：http://ofc.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://sqp.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://ygl.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://ofl.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://sai.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://xhl.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uey.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://uxm.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zfl.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tjl.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://whx.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gar.yj20258888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cjf.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fjo.wangdashe.top

[P03] 生成短随机字符串
来源：http://bnb.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://olt.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cju.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qaf.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bze.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ffo.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fyj.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mtw.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://foj.cucudq.cn

[P04] 求长度
来源：http://fnf.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hmq.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ijx.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wpq.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rfr.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://wkg.sweek.top

Go:   len(arr);  len(m)
来源：http://def.vehdjk.com

Ruby: x.length;  x.size
来源：http://loj.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mfd.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://tnr.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hjr.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mrs.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rbl.wangshuangyany.cn


<!-- 参考信息 -->