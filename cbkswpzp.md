代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hyn.hfpthk.cn

[L08] 并发请求多个地址
来源：http://ymg.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://akk.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://puk.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ykj.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jcq.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xnh.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://and.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dwc.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eqj.daria6918.cn

================================================================================
来源：http://ulc.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://vih.zhijiandao.cn

================================================================================
来源：http://pyg.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://yni.cqqwz.cn

Py:   sys.argv[1:]
来源：http://tfv.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://rmk.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://nng.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://kym.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://inn.hysaishi.cn

Go:   os.Args[1:]
来源：http://ppo.quarkkingdee.top

Ruby: ARGV
来源：http://ugq.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://sis.yvedp.cn

[M02] 读取环境变量
来源：http://tkn.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://dpw.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yvg.guannengcc.top

JS:   process.env.HOME
来源：http://wzi.wangdashe.top

TS:   process.env.HOME
来源：http://ozg.svipenyu.cn

Java: System.getenv("HOME")
来源：http://lci.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ckx.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://cmr.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qfg.zdqjudy.top

[M03] 执行外部命令
来源：http://hmy.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zfw.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bjp.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pjr.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://igc.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hhl.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fnq.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://olh.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://axn.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://qwg.uphjek.com

Py:   os.getcwd()
来源：http://cvc.yj20258.top

PHP:  getcwd();
来源：http://kwj.jyoumei.cn

JS:   process.cwd()
来源：http://zox.shzxlz.cn

TS:   process.cwd()
来源：http://gel.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://qsv.yj20258.top

Go:   os.Getwd()
来源：http://mql.fzhhl.top

Ruby: Dir.pwd
来源：http://pqs.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://tee.yueranfly.top

[M05] 设置退出码
来源：http://bzc.shuidangran.top

Py:   sys.exit(1)
来源：http://nov.bjfxy.top

PHP:  exit(1);
来源：http://bvi.jinqigufen.top

JS:   process.exit(1)
来源：http://ffe.fehbvm.com

TS:   process.exit(1)
来源：http://zzk.hammf.cn

Java: System.exit(1)
来源：http://kiy.cdnleiting.top

Go:   os.Exit(1)
来源：http://dwt.mhx1999.top

Ruby: exit 1
来源：http://pcd.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ans.shzxlz.cn

[M06] 向标准错误输出
来源：http://vte.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://qnf.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jqe.9152youxi.cn

JS:   console.error("err")
来源：http://wst.havefunace.top

TS:   console.error("err")
来源：http://dwq.zdbjq.cn

Java: System.err.println("err")
来源：http://piy.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qrm.jinghuilouyu.cn

Ruby: warn "err"
来源：http://dck.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://epz.daria6918.cn

[M07] 判断是否为主入口
来源：http://nqg.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://ytl.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yuf.xziqi.cn

JS:   require.main === module
来源：http://ywo.cqqwz.cn

TS:   require.main === module
来源：http://yqy.guowangkeji.top

Java: public static void main(String[] args)
来源：http://bll.fzhhl.top

Go:   func main()
来源：http://ijx.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ksg.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://cek.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://cnb.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://tem.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://seg.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://ffy.birdmap.top

TS:   process.platform;  process.version
来源：http://iwp.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://knm.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://kul.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ity.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://eoe.yuxming.cn

================================================================================
来源：http://nzf.hongshengwenyu.top

N. 数据结构与算法
来源：http://jxr.nanxinkj.top

================================================================================
来源：http://mlt.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://aas.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kzh.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uta.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kqa.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dbf.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xoo.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://vsn.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://miz.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://amr.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://zzv.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://azz.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jlr.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sby.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cvg.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://twt.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://fuh.ivvv.top

Ruby: arr.sort
来源：http://gav.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nox.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://obz.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kao.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://rbc.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zjy.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sdt.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oxr.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bpz.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ewy.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kgq.52xcode.cn

[N04] 斐波那契数列
来源：http://tqg.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uzj.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yyb.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wyk.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rde.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nrc.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://icz.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ioo.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wyn.birdmap.top

[N05] 最大公约数
来源：http://kgg.sweek.top

Py:   math.gcd(a, b)
来源：http://jgm.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rhr.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlm.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tnw.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyi.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kmj.hfpthk.cn

Ruby: a.gcd(b)
来源：http://icu.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nmz.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://lmo.dianchejie.cn

Py:   s == s[::-1]
来源：http://sbl.ybcxt.top

PHP:  $s === strrev($s);
来源：http://jdh.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://aub.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://itn.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hmj.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://ejk.yj20258.top

Ruby: s == s.reverse
来源：http://qyn.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zar.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://ubs.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uyc.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sxu.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eed.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://kht.yfazqb.com

Java: // 手写 HashMap
来源：http://dgy.uphjek.com

Go:   // 手写 map[int]int
来源：http://kbj.chenzaomai.com

Ruby: // 手写 Hash
来源：http://acy.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mey.zhiwuduotai.top

[N08] 生成全排列
来源：http://hgw.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://tur.chenzaomai.com

PHP:  // 手写递归交换
来源：http://ekx.gzhubu.top

JS:   // 手写回溯递归
来源：http://xvr.nanxinkj.top

TS:   // 手写回溯递归
来源：http://epx.yj202588.top

Java: // 手写回溯递归
来源：http://bse.sxryk.cn

Go:   // 手写回溯递归
来源：http://zsp.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://pwt.ivvv.top

C#:   // 手写回溯递归
来源：http://vxd.cqqwz.cn

[N09] 栈与队列
来源：http://fne.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kwf.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://raq.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pxm.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hjh.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cdo.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mfs.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xgx.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qhr.xziqi.cn

[N10] 链表节点定义
来源：http://fyo.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lxb.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nni.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lmf.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cxy.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://nng.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://gbw.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://huc.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cin.gzhubu.top

[N11] 二叉树中序遍历
来源：http://krn.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://flj.shzxlz.cn

PHP:  // 手写递归函数
来源：http://uio.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://euj.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hlo.mhx1999.top

Java: // 手写递归
来源：http://zsg.aizwys.cn

Go:   // 手写递归
来源：http://avy.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cjv.fanxiaobao.xyz

C#:   // 手写递归
来源：http://ily.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ogf.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sxk.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pft.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://snj.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dow.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cfy.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://spy.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yvv.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lol.iojbl.cn

================================================================================
来源：http://tyw.shangyingyoupin.top

O. 并发与异步
来源：http://hle.ppjwa.cn

================================================================================
来源：http://luy.hnqzz.top

[O01] 启动一个线程
来源：http://vhz.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ghv.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qfe.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kpm.9152youxi.cn

TS:   // 同 JS
来源：http://ryd.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://bqa.yj20258.top

Go:   go f()
来源：http://xmj.haohaochexian.top

Ruby: Thread.new { f }
来源：http://rbl.meibo888.top

C#:   Task.Run(() => F());
来源：http://xjs.zdqjudy.top

[O02] 使用线程池
来源：http://xzz.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nsz.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mth.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://vgm.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://lzh.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://uwx.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xxe.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ump.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oqe.cucudq.cn

[O03] 加锁保护共享数据
来源：http://uil.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://svv.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://eor.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uhf.zdqjudy.top

TS:   // 同 JS
来源：http://sjz.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://krt.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ojy.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pux.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://zgi.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://ooc.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://jvz.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tav.sysykeji.top

JS:   async function f() { await g(); }
来源：http://ryz.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rod.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://efp.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhq.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://enq.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://jmu.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://ffw.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://qsk.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ifr.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://vyt.havefunace.top

TS:   await Promise.all(tasks)
来源：http://szz.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://imb.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ldr.redwolf501.top

Ruby: threads.map(&:join)
来源：http://jum.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xsl.andypj.xyz

[O06] 使用进程池
来源：http://ltb.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ukp.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mig.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://hys.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://ezz.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jzx.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hpu.feifeiyinyue.top

Ruby: // fork 块
来源：http://qjr.vqdsnc.cn

C#:   Parallel.For
来源：http://mlc.jqgufenzy.top

================================================================================
来源：http://ddy.chenlongwang.top

P. 常用工具函数
来源：http://pwp.jiagoushi.top

================================================================================
来源：http://dxg.zhixingplan.top

[P01] 生成 UUID
来源：http://yae.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://jog.ywan-chungtsiang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gpq.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://gts.hcnkem.com

TS:   crypto.randomUUID()
来源：http://xcf.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://afh.jianghu66.top

Go:   // 用 github.com/google/uuid
来源：http://qvn.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://kie.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://lyj.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://cte.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vdh.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bba.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rkb.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pyc.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zws.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://umr.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://myj.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jji.cheryme.top

[P03] 生成短随机字符串
来源：http://xko.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zwc.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yrq.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ius.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jdu.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kxk.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wgx.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lat.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lsd.wangdashe.top

[P04] 求长度
来源：http://ygk.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hvh.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdz.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://suf.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sow.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://tdn.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://uka.fktsv.cn

Ruby: x.length;  x.size
来源：http://kzu.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zbi.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://wsx.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ols.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gjs.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uzg.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cgj.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oia.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://qau.zdqjudy.top

Ruby: a == b
来源：http://idw.jinghuilouyu.cn


<!-- 参考信息 -->