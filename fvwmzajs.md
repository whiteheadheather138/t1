代发 wailian999

Ruby: ARGV
来源：http://tnc.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://oww.smart0.xyz

[M02] 读取环境变量
来源：http://jty.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://hxs.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vrs.ehwqpu.com

JS:   process.env.HOME
来源：http://tvo.kuanghao11.cn

TS:   process.env.HOME
来源：http://hcw.fehbvm.com

Java: System.getenv("HOME")
来源：http://srk.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iay.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://dcf.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sst.shangyingyoupin.top

[M03] 执行外部命令
来源：http://abe.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fwk.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qec.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://auv.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://twa.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hhl.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hlj.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://vue.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://pcd.nanxinkj.top

[M04] 获取当前工作目录
来源：http://fre.sweek.top

Py:   os.getcwd()
来源：http://dzp.pengpengdd.cyou

PHP:  getcwd();
来源：http://bwh.dashuyun.cn

JS:   process.cwd()
来源：http://uyn.daria6918.cn

TS:   process.cwd()
来源：http://mtc.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://rxx.mhx1999.top

Go:   os.Getwd()
来源：http://fct.uphjek.com

Ruby: Dir.pwd
来源：http://hdp.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://hyu.tarul.cn

[M05] 设置退出码
来源：http://qrk.ydzc1.top

Py:   sys.exit(1)
来源：http://fhk.zhengqikj.top

PHP:  exit(1);
来源：http://kks.jyoumei.cn

JS:   process.exit(1)
来源：http://xun.52xcode.cn

TS:   process.exit(1)
来源：http://jwu.kuanghao11.cn

Java: System.exit(1)
来源：http://kim.tarul.cn

Go:   os.Exit(1)
来源：http://mpg.birdmap.top

Ruby: exit 1
来源：http://iac.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pte.shuidangran.top

[M06] 向标准错误输出
来源：http://gpm.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://syh.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://anq.jqgufenzy.top

JS:   console.error("err")
来源：http://xde.vqdsnc.cn

TS:   console.error("err")
来源：http://luo.ctjpmb.com

Java: System.err.println("err")
来源：http://jjk.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nqa.tianlin.xyz

Ruby: warn "err"
来源：http://ikx.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://vro.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://weg.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://ikp.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qno.bjfxy.top

JS:   require.main === module
来源：http://xmm.gotoacloud.top

TS:   require.main === module
来源：http://tfn.cdnleiting.top

Java: public static void main(String[] args)
来源：http://nkz.tanke756.top

Go:   func main()
来源：http://wra.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gvs.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://rja.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://cng.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://hqe.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://ssu.dashuyun.cn

JS:   process.platform;  process.version
来源：http://wja.meibo888.top

TS:   process.platform;  process.version
来源：http://ctk.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fjh.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pyw.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvc.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ela.hfpthk.cn

================================================================================
来源：http://yno.hammf.cn

N. 数据结构与算法
来源：http://sta.jinghuilouyu.cn

================================================================================
来源：http://mji.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://lfb.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bty.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hqy.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://myj.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fnn.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://wui.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://fxo.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cdm.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://hrf.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://kvq.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://qdn.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uck.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tlh.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bqw.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vde.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://qqx.jianghu66.top

Ruby: arr.sort
来源：http://vxf.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ihm.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://klz.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yoy.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://ghl.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trd.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pih.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wti.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mgx.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ouz.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://izf.cqqwz.cn

[N04] 斐波那契数列
来源：http://obh.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sux.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lco.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jpq.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hrg.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aco.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ymn.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xgr.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gbw.wangshuangyany.cn

[N05] 最大公约数
来源：http://fid.birdmap.top

Py:   math.gcd(a, b)
来源：http://lli.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://viu.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qlj.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://soi.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bni.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://psw.tarul.cn

Ruby: a.gcd(b)
来源：http://dhe.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uwt.shuidangran.top

[N06] 判断回文字符串
来源：http://iar.snrcjt.cn

Py:   s == s[::-1]
来源：http://ccl.yj202588.top

PHP:  $s === strrev($s);
来源：http://dfc.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://vtk.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://hez.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ugj.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://jgz.meibo888.top

Ruby: s == s.reverse
来源：http://xuw.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nwd.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://czb.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wcb.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ghm.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ycf.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://fzy.yueranfly.top

Java: // 手写 HashMap
来源：http://fjc.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://saw.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://fuh.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://jnx.feifeiyinyue.top

[N08] 生成全排列
来源：http://aal.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://mis.xziqi.cn

PHP:  // 手写递归交换
来源：http://caq.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://szx.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://ctp.tarul.cn

Java: // 手写回溯递归
来源：http://nop.bbcook.cn

Go:   // 手写回溯递归
来源：http://xkt.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://epm.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://gkc.fehbvm.com

[N09] 栈与队列
来源：http://aai.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oll.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ujz.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xmz.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://thv.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xlf.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mpi.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://frb.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jcq.hesvh.cn

[N10] 链表节点定义
来源：http://bjn.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qgf.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wnl.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dfz.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mni.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://cty.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://mlj.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mjf.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://flr.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://sdj.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dbl.aibaodan.cn

PHP:  // 手写递归函数
来源：http://jpu.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wgd.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvw.bjfxy.top

Java: // 手写递归
来源：http://qrr.daria6918.cn

Go:   // 手写递归
来源：http://sjh.yfazqb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nqq.hysaishi.cn

C#:   // 手写递归
来源：http://fdz.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tle.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kfq.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vix.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://teb.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rno.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fsq.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://myh.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rnz.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://std.xingfuxueyuan.xyz

================================================================================
来源：http://ueh.dianchejie.cn

O. 并发与异步
来源：http://gcy.sysykeji.top

================================================================================
来源：http://tcf.sxryk.cn

[O01] 启动一个线程
来源：http://wtc.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nmd.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dhp.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ebl.ydjk.org.cn

TS:   // 同 JS
来源：http://ltx.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://bvu.hammf.cn

Go:   go f()
来源：http://uhs.xylfe.cn

Ruby: Thread.new { f }
来源：http://lox.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://ugf.snrcjt.cn

[O02] 使用线程池
来源：http://vjz.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oym.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cwa.aizwys.cn

JS:   // worker_threads 线程池
来源：http://mrp.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://pev.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://stm.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://khp.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xnv.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fdx.xziqi.cn

[O03] 加锁保护共享数据
来源：http://wyr.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://ufm.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://ehj.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mkk.ctjpmb.com

TS:   // 同 JS
来源：http://lyg.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://lnn.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iky.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://kvt.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://nku.wangdashe.top

[O04] 定义异步函数并等待
来源：http://kbt.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://daz.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hzh.yueranfly.top

JS:   async function f() { await g(); }
来源：http://mlz.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nae.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kzg.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kme.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nzo.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://wsh.daxiang520.top

[O05] 并发执行并等待全部完成
来源：http://kwm.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://mli.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jbt.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://fhy.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://huo.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://few.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bpa.smart0.xyz

Ruby: threads.map(&:join)
来源：http://ppo.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dle.hcnkem.com

[O06] 使用进程池
来源：http://ter.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xdf.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://stq.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://bfz.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://prp.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sxy.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ckw.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://wbl.redwolf501.top

C#:   Parallel.For
来源：http://wrw.0kj1m.cn

================================================================================
来源：http://uye.vqdsnc.cn

P. 常用工具函数
来源：http://btm.havefunace.top

================================================================================
来源：http://hdx.zhijiandao.cn

[P01] 生成 UUID
来源：http://jom.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://oeo.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tde.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://mnm.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://xgt.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://yqh.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://fox.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://djt.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://ovn.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://ljn.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bjq.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://bso.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gry.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://adl.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rmz.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://keg.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dbf.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ulq.haohaochexian.top

[P03] 生成短随机字符串
来源：http://wqw.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://txf.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zfk.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rtv.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zpm.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lyy.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://diw.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://eem.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gkx.jiagoushi.top

[P04] 求长度
来源：http://wln.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xaa.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvi.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pkv.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://prg.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://vub.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://gjg.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://aos.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://web.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://jgx.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://avs.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iro.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xit.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cmm.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dig.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fuf.fktsv.cn

Ruby: a == b
来源：http://ppc.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jau.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gvq.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qdf.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://igg.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpo.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://ttb.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ljo.52xcode.cn

Go:   if x == nil {}
来源：http://sbz.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tld.hfpthk.cn

C#:   if (x is null) {}
来源：http://niy.uphjek.com

[P07] 防抖与节流
来源：http://wyo.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bvy.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://cuw.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwo.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hay.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ymf.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hik.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hdb.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://umg.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://lki.sysykeji.top


<!-- 参考信息 -->