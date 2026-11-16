代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hoi.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://meb.sysykeji.top

================================================================================
来源：http://yxv.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://vez.zhijiandao.cn

================================================================================
来源：http://lux.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://pkx.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://zfo.hnqzz.top

PHP:  $argv;  $argc;
来源：http://poi.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://sts.hesvh.cn

TS:   process.argv.slice(2)
来源：http://vaw.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://adp.yonumen.top

Go:   os.Args[1:]
来源：http://vpd.mhx1999.top

Ruby: ARGV
来源：http://nmz.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://phd.dianchejie.cn

[M02] 读取环境变量
来源：http://bue.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://sff.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://unx.yj20258.top

JS:   process.env.HOME
来源：http://esv.sxryk.cn

TS:   process.env.HOME
来源：http://ite.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://qyp.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fhz.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://osu.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oek.snrcjt.cn

[M03] 执行外部命令
来源：http://fzp.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mva.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://igw.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fir.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sst.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eka.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xug.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kmt.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://ete.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://yqy.vehdjk.com

Py:   os.getcwd()
来源：http://hzh.zycfv.cn

PHP:  getcwd();
来源：http://rky.gaohongyu789.top

JS:   process.cwd()
来源：http://rgy.feifeiyinyue.top

TS:   process.cwd()
来源：http://apx.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://hol.zdbjq.cn

Go:   os.Getwd()
来源：http://utn.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://tbi.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fyq.yongpay.top

[M05] 设置退出码
来源：http://tpz.hcnkem.com

Py:   sys.exit(1)
来源：http://oha.uphjek.com

PHP:  exit(1);
来源：http://jqd.yanxiufei.cn

JS:   process.exit(1)
来源：http://gke.yuxming.cn

TS:   process.exit(1)
来源：http://vaz.yuxming.cn

Java: System.exit(1)
来源：http://ael.cashguo.top

Go:   os.Exit(1)
来源：http://awa.zdqjudy.top

Ruby: exit 1
来源：http://sgs.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hvy.aibaodan.cn

[M06] 向标准错误输出
来源：http://lob.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://emd.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uaw.hammf.cn

JS:   console.error("err")
来源：http://amk.tianlin.xyz

TS:   console.error("err")
来源：http://wpp.tianlin.xyz

Java: System.err.println("err")
来源：http://ljg.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rvk.jqgfzy.top

Ruby: warn "err"
来源：http://uup.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://ybk.yueranfly.top

[M07] 判断是否为主入口
来源：http://hhc.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://edp.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pyl.zhijiandao.cn

JS:   require.main === module
来源：http://sbb.hysaishi.cn

TS:   require.main === module
来源：http://gel.zhixingplan.top

Java: public static void main(String[] args)
来源：http://kqm.c1oappe.top

Go:   func main()
来源：http://ulg.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aog.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://yor.birdmap.top

[M08] 获取系统与运行时信息
来源：http://yev.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://fvq.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://bgd.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://pcl.cheryme.top

TS:   process.platform;  process.version
来源：http://erx.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iiq.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pos.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uiu.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vzv.jinghuilouyu.cn

================================================================================
来源：http://clv.gotoacloud.top

N. 数据结构与算法
来源：http://voj.epnwcf.com

================================================================================
来源：http://vuy.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://dcr.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://qef.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qkk.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://atx.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rcp.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://phw.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://dnt.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qzw.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://zwv.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://uqy.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://qsu.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wzv.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kop.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fga.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cfw.hnqzz.top

Go:   slices.Sort(arr)
来源：http://abw.gzhubu.top

Ruby: arr.sort
来源：http://iln.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hcj.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://xla.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nie.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://cgh.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyq.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jdl.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vxo.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://diy.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kfm.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://xtp.andypj.xyz

[N04] 斐波那契数列
来源：http://xpn.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxx.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ivh.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yeb.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pup.gogol.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zbl.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bsj.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://olf.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxz.aizwys.cn

[N05] 最大公约数
来源：http://lsz.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://ily.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xnz.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gpj.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xtz.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ivs.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kwk.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://yqu.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wef.jlsjyb.cn

[N06] 判断回文字符串
来源：http://dem.hcnkem.com

Py:   s == s[::-1]
来源：http://ydb.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://vfv.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://tqa.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://ibs.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cqa.gzhubu.top

Go:   // 双指针从两端比较
来源：http://woz.dashuyun.cn

Ruby: s == s.reverse
来源：http://uvv.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://baj.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://fdf.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://txs.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qch.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bsx.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://epn.haohaochexian.top

Java: // 手写 HashMap
来源：http://cks.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://gtu.dianchejie.cn

Ruby: // 手写 Hash
来源：http://sxd.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://pud.jinghuilouyu.cn

[N08] 生成全排列
来源：http://tzs.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://noz.bjfxy.top

PHP:  // 手写递归交换
来源：http://dge.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://rcm.xuanzx.com

TS:   // 手写回溯递归
来源：http://rgy.hnqzz.top

Java: // 手写回溯递归
来源：http://fwj.hywenlv.cn

Go:   // 手写回溯递归
来源：http://ert.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://wsd.birdmap.top

C#:   // 手写回溯递归
来源：http://wyg.kuanghao11.cn

[N09] 栈与队列
来源：http://qpe.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://voc.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kvm.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eut.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://alb.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bol.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dcm.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://otj.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://skk.birdmap.top

[N10] 链表节点定义
来源：http://taz.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vlx.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hzl.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xdn.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ecr.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://hhb.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://too.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pni.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dzj.nwbrower.top

[N11] 二叉树中序遍历
来源：http://gjc.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://weo.shzxlz.cn

PHP:  // 手写递归函数
来源：http://aah.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwh.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://utc.jinqigufen.top

Java: // 手写递归
来源：http://nay.316326.xyz

Go:   // 手写递归
来源：http://cnp.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lba.zhengqikj.top

C#:   // 手写递归
来源：http://rsf.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hwf.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wed.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fsd.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybu.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ogy.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pkm.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kte.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://suc.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yqg.guowangkeji.top

================================================================================
来源：http://mvx.vqdsnc.cn

O. 并发与异步
来源：http://hfd.yonumen.top

================================================================================
来源：http://fqe.tanke756.top

[O01] 启动一个线程
来源：http://ruj.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://atd.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://khz.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aao.chenlongwang.top

TS:   // 同 JS
来源：http://bmo.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://lkf.nwbrower.top

Go:   go f()
来源：http://yey.yangfankeji.com

Ruby: Thread.new { f }
来源：http://ipm.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://kqd.xinyue.icu

[O02] 使用线程池
来源：http://rtj.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pko.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pjq.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://kpb.tanke756.top

TS:   // worker_threads 线程池
来源：http://pgo.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://flo.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xld.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hig.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hzc.bbcook.cn

[O03] 加锁保护共享数据
来源：http://sym.chenzaomai.com

Py:   with lock: shared += 1
来源：http://fey.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://atj.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://may.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://tsh.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://sag.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aof.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ose.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://ifr.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://fzw.yongpay.top

Py:   async def f():⏎    await g()
来源：http://ckv.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://muh.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://dsi.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lbn.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tog.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vwp.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uae.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://tom.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://hrb.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://zew.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aaj.meibo888.top

JS:   await Promise.all(tasks)
来源：http://yow.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://wcs.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uqy.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rvg.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://txv.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://rzs.aibaodan.cn

[O06] 使用进程池
来源：http://yzj.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fbw.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ofa.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://gql.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://ysc.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nek.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://saw.cucudq.cn

Ruby: // fork 块
来源：http://jwn.hysaishi.cn

C#:   Parallel.For
来源：http://hfb.hywenlv.cn

================================================================================
来源：http://qmh.ppjwa.cn

P. 常用工具函数
来源：http://moz.nwbrower.top

================================================================================
来源：http://ugm.snrcjt.cn

[P01] 生成 UUID
来源：http://eeg.birdmap.top

Py:   str(uuid.uuid4())
来源：http://pru.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sfi.redwolf501.top

JS:   crypto.randomUUID()
来源：http://lwm.smart0.xyz

TS:   crypto.randomUUID()
来源：http://wts.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://vrt.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://waf.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://swu.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://jtf.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://rom.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uby.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tti.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aai.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mnu.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bns.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aws.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nxl.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fmu.jinqigufen.top

[P03] 生成短随机字符串
来源：http://yon.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tns.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iwk.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uva.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rhu.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://opr.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dwz.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tdf.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vqm.gogol.net.cn

[P04] 求长度
来源：http://qma.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ead.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://suv.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zgi.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ocr.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://hgq.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://fae.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://ugu.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ebg.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://umh.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tze.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tcd.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://acl.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ful.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kcy.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nnc.pycfn.com

Ruby: a == b
来源：http://thv.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hnm.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fae.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yrm.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://ljf.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://apx.jiagoushi.top

TS:   if (x == null) {}
来源：http://mpg.xuetiantiany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cdq.jiagoushi.top

Go:   if x == nil {}
来源：http://vct.pengpengdd.cyou


<!-- 参考信息 -->