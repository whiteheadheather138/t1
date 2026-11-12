代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rkm.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qxj.pengpengdd.cyou

================================================================================
来源：http://eep.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://bve.dianchejie.cn

================================================================================
来源：http://zik.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://uqb.yueranfly.top

Py:   sys.argv[1:]
来源：http://vwt.yj20258888.top

PHP:  $argv;  $argc;
来源：http://wrh.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://ewd.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://iyv.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://pix.ivvv.top

Go:   os.Args[1:]
来源：http://pzm.fehbvm.com

Ruby: ARGV
来源：http://zro.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://qlq.vqdsnc.cn

[M02] 读取环境变量
来源：http://oss.meibo888.top

Py:   os.environ.get("HOME")
来源：http://riq.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ryh.xziqi.cn

JS:   process.env.HOME
来源：http://zuu.jianghu66.top

TS:   process.env.HOME
来源：http://wbt.sxryk.cn

Java: System.getenv("HOME")
来源：http://oif.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cye.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://enj.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vug.gogol.net.cn

[M03] 执行外部命令
来源：http://zer.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://acr.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xlf.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jfd.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ean.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vac.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rwy.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://zdz.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://clp.dianchejie.cn

[M04] 获取当前工作目录
来源：http://fak.gotoacloud.top

Py:   os.getcwd()
来源：http://eaw.zhijiandao.cn

PHP:  getcwd();
来源：http://axn.hywenlv.cn

JS:   process.cwd()
来源：http://tsw.snrcjt.cn

TS:   process.cwd()
来源：http://dnj.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://gty.xylfe.cn

Go:   os.Getwd()
来源：http://mlo.dianchejie.cn

Ruby: Dir.pwd
来源：http://amq.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ynk.zhongyouzk.top

[M05] 设置退出码
来源：http://izo.gaohongyu789.top

Py:   sys.exit(1)
来源：http://ncp.cucudq.cn

PHP:  exit(1);
来源：http://wuh.yuanzhike.top

JS:   process.exit(1)
来源：http://rzv.hfpthk.cn

TS:   process.exit(1)
来源：http://qsk.jqgfzy.top

Java: System.exit(1)
来源：http://mof.xinyue.icu

Go:   os.Exit(1)
来源：http://quc.sufxvd.cn

Ruby: exit 1
来源：http://fby.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://csp.chenzaomai.com

[M06] 向标准错误输出
来源：http://yyk.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://cmc.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://brj.jlsjyb.cn

JS:   console.error("err")
来源：http://qep.chenlongwang.top

TS:   console.error("err")
来源：http://rlp.wangdashe.top

Java: System.err.println("err")
来源：http://tks.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jcs.uphjek.com

Ruby: warn "err"
来源：http://rtj.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://dyu.tanke756.top

[M07] 判断是否为主入口
来源：http://jsl.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://wnl.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gsk.ehwqpu.com

JS:   require.main === module
来源：http://wxx.ydjk.org.cn

TS:   require.main === module
来源：http://rcw.yongpay.top

Java: public static void main(String[] args)
来源：http://tce.tianlin.xyz

Go:   func main()
来源：http://wzz.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://avs.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://chf.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://ebd.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://wpz.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://ajw.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://uki.zycfv.cn

TS:   process.platform;  process.version
来源：http://sje.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dic.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eyr.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fup.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ejc.ivvv.top

================================================================================
来源：http://zzd.sxryk.cn

N. 数据结构与算法
来源：http://rlh.zhongyouzk.top

================================================================================
来源：http://ylf.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://ubq.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://qsr.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gqn.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jfk.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tas.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bzl.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://ysd.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://vms.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://kry.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://srb.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://egl.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tms.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jxy.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qlh.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zjk.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://bij.fehbvm.com

Ruby: arr.sort
来源：http://yrs.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://jyt.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://jdo.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cmy.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://fca.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcw.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdy.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ddm.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sne.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dlq.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ueg.0kj1m.cn

[N04] 斐波那契数列
来源：http://jze.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://auj.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nkb.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wua.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yor.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jmp.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bsi.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cze.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qto.snrcjt.cn

[N05] 最大公约数
来源：http://xnb.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://ywi.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://evy.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ehd.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvf.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tbo.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vpr.fzhhl.top

Ruby: a.gcd(b)
来源：http://lgd.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cjo.sufxvd.cn

[N06] 判断回文字符串
来源：http://fsw.52xcode.cn

Py:   s == s[::-1]
来源：http://lyd.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://und.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://rgq.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://ezk.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yhk.xziqi.cn

Go:   // 双指针从两端比较
来源：http://yzo.zhengqikj.top

Ruby: s == s.reverse
来源：http://uey.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jiz.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://xgw.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hza.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cbf.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ovi.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://aal.yangfankeji.com

Java: // 手写 HashMap
来源：http://njx.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://zlk.zhixingplan.top

Ruby: // 手写 Hash
来源：http://asp.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://wco.chenjidiqi.icu

[N08] 生成全排列
来源：http://lsw.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://kcs.snrcjt.cn

PHP:  // 手写递归交换
来源：http://vlj.chenzaomai.com

JS:   // 手写回溯递归
来源：http://kla.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://ssv.pycfn.com

Java: // 手写回溯递归
来源：http://osw.hfpthk.cn

Go:   // 手写回溯递归
来源：http://byp.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://jzb.sufxvd.cn

C#:   // 手写回溯递归
来源：http://xrt.fanxiaobao.xyz

[N09] 栈与队列
来源：http://hsk.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://myl.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cbz.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ksx.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jsm.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gxx.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hdp.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ifg.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gyh.ydjk.org.cn

[N10] 链表节点定义
来源：http://zxz.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://quz.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://utg.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tyg.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vzl.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://nig.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://tvu.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uje.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://ifo.smart0.xyz

[N11] 二叉树中序遍历
来源：http://aml.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyh.cheryme.top

PHP:  // 手写递归函数
来源：http://svh.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ldo.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czq.ywan-chungtsiang.top

Java: // 手写递归
来源：http://hvm.ivvv.top

Go:   // 手写递归
来源：http://qop.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fae.svipenyu.cn

C#:   // 手写递归
来源：http://vki.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://etk.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yiz.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xer.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rso.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bmk.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://huz.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xsr.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://smc.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iyp.fehbvm.com

================================================================================
来源：http://wga.ybcxt.top

O. 并发与异步
来源：http://ykq.fengsongda.top

================================================================================
来源：http://vjv.dashuyun.cn

[O01] 启动一个线程
来源：http://kjp.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://etn.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nmv.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wcm.xuetiantiany.cn

TS:   // 同 JS
来源：http://lhb.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://gcd.yfazqb.com

Go:   go f()
来源：http://mzw.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://lwm.bbcook.cn

C#:   Task.Run(() => F());
来源：http://pvq.9152youxi.cn

[O02] 使用线程池
来源：http://ksr.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bdm.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://otx.yonumen.top

JS:   // worker_threads 线程池
来源：http://usl.xuanzx.com

TS:   // worker_threads 线程池
来源：http://jts.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wcf.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://euu.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ndt.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xwn.nwbrower.top

[O03] 加锁保护共享数据
来源：http://tlb.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://gkq.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://umj.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qhn.chenzaomai.com

TS:   // 同 JS
来源：http://emf.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://vyc.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lsn.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uxb.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://hoa.tian-w.cn

[O04] 定义异步函数并等待
来源：http://brq.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://nlf.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bhe.bbcook.cn

JS:   async function f() { await g(); }
来源：http://oyg.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pbe.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yje.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yah.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://suh.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://yhq.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://tih.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://oli.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qnh.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://pqx.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://bpt.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vlf.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hhx.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://sam.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pwb.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://ojg.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ttd.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zka.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://tju.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://fee.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qhx.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://avc.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://qeg.andypj.xyz

C#:   Parallel.For
来源：http://ifs.bjfxy.top

================================================================================
来源：http://pnq.yueranfly.top

P. 常用工具函数
来源：http://wnz.yueranfly.top

================================================================================
来源：http://yjq.epnwcf.com

[P01] 生成 UUID
来源：http://urz.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://sno.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nnv.havefunace.top

JS:   crypto.randomUUID()
来源：http://ksu.cheryme.top

TS:   crypto.randomUUID()
来源：http://fna.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://psg.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://phc.cashguo.top

Ruby: SecureRandom.uuid
来源：http://oxp.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://sms.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://rdf.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zjx.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://yda.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xhb.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://usf.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://okm.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://psb.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hvl.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wir.aibaodan.cn

[P03] 生成短随机字符串
来源：http://fze.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yoj.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dny.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wqj.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uhk.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cru.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lea.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://grt.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ptt.zhijiandao.cn

[P04] 求长度
来源：http://kcw.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://teb.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gel.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xtd.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://box.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://xab.uphjek.com

Go:   len(arr);  len(m)
来源：http://czf.shzxlz.cn

Ruby: x.length;  x.size
来源：http://vwm.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cdb.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://juu.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hby.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fgx.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mqz.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zob.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uuu.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://mim.zhengqikj.top

Ruby: a == b
来源：http://orp.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zas.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xhc.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sgx.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://idu.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://snk.zhengqikj.top

TS:   if (x == null) {}
来源：http://abm.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iup.jiagoushi.top

Go:   if x == nil {}
来源：http://xbf.yvedp.cn


<!-- 参考信息 -->