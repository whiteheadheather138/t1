代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rno.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xqg.redwolf501.top

================================================================================
来源：http://lwx.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://lge.zdbjq.cn

================================================================================
来源：http://sep.cashguo.top

[M01] 读取命令行参数
来源：http://tov.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://bly.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://bbf.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://aez.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://fjv.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://hug.ydzc1.top

Go:   os.Args[1:]
来源：http://ljf.pycfn.com

Ruby: ARGV
来源：http://kyk.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://hjr.xinyue.icu

[M02] 读取环境变量
来源：http://vok.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://nib.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kzi.jianghu66.top

JS:   process.env.HOME
来源：http://dfu.zhiwuduotai.top

TS:   process.env.HOME
来源：http://svt.nwbrower.top

Java: System.getenv("HOME")
来源：http://zkh.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ghj.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://olj.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ieq.vqdsnc.cn

[M03] 执行外部命令
来源：http://zza.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ucy.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://img.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zug.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mor.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://frt.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mos.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://igr.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://gib.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://szc.pengpengdd.cyou

Py:   os.getcwd()
来源：http://bwv.zhengqikj.top

PHP:  getcwd();
来源：http://owr.zycfv.cn

JS:   process.cwd()
来源：http://npj.guannengcc.top

TS:   process.cwd()
来源：http://efc.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bsw.iojbl.cn

Go:   os.Getwd()
来源：http://lti.yvedp.cn

Ruby: Dir.pwd
来源：http://kja.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://thb.jqgfzy.top

[M05] 设置退出码
来源：http://cdz.xziqi.cn

Py:   sys.exit(1)
来源：http://ljh.bjfxy.top

PHP:  exit(1);
来源：http://dxx.chenlongwang.top

JS:   process.exit(1)
来源：http://hxv.shangyingyoupin.top

TS:   process.exit(1)
来源：http://qlk.hcnkem.com

Java: System.exit(1)
来源：http://fge.zhengqikj.top

Go:   os.Exit(1)
来源：http://nuq.sxryk.cn

Ruby: exit 1
来源：http://ssc.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://olr.hesvh.cn

[M06] 向标准错误输出
来源：http://toh.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://dyo.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://phx.nanxuanxn.top

JS:   console.error("err")
来源：http://akm.hywenlv.cn

TS:   console.error("err")
来源：http://itu.nanxinkj.top

Java: System.err.println("err")
来源：http://nik.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vct.fzhhl.top

Ruby: warn "err"
来源：http://qjn.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://dfv.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://xxy.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://zel.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qiu.gogol.net.cn

JS:   require.main === module
来源：http://gmj.birdmap.top

TS:   require.main === module
来源：http://ugf.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://ihi.jiagoushi.top

Go:   func main()
来源：http://pav.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zlp.yj202588.top

C#:   static void Main(string[] args)
来源：http://pqu.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://utu.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://odt.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://qic.316326.xyz

JS:   process.platform;  process.version
来源：http://afy.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://szb.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hun.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zzt.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kla.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kya.daxiang520.top

================================================================================
来源：http://dfr.hnqzz.top

N. 数据结构与算法
来源：http://rja.jyoumei.cn

================================================================================
来源：http://umg.pycfn.com

[N01] 二分查找（有序数组）
来源：http://kkq.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://azf.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ufn.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xjt.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npa.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://qsx.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://gvk.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uhm.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uek.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://foo.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://juq.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hhe.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://pkz.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pgc.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uvd.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://oqo.birdmap.top

Ruby: arr.sort
来源：http://imq.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://gho.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://ftj.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jbj.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://kcx.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plf.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqo.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://quy.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://idf.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://any.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://wtb.gogol.net.cn

[N04] 斐波那契数列
来源：http://wss.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://olu.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwx.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qyz.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pku.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://inr.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kkm.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://btb.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://acx.yuanzhike.top

[N05] 最大公约数
来源：http://xge.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://fco.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kso.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://djh.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lze.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wvg.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ftp.sysykeji.top

Ruby: a.gcd(b)
来源：http://rve.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xuz.yueranfly.top

[N06] 判断回文字符串
来源：http://bgo.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://tye.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://qak.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://vlm.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://lzh.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yve.xinyue.icu

Go:   // 双指针从两端比较
来源：http://qke.sxryk.cn

Ruby: s == s.reverse
来源：http://gcy.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ozz.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://qie.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://unv.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ihe.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cuy.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://krt.yongpay.top

Java: // 手写 HashMap
来源：http://ful.fktsv.cn

Go:   // 手写 map[int]int
来源：http://dyd.yj20258.top

Ruby: // 手写 Hash
来源：http://ret.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://egs.epnwcf.com

[N08] 生成全排列
来源：http://osf.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://zvg.cashguo.top

PHP:  // 手写递归交换
来源：http://qyq.wangdashe.top

JS:   // 手写回溯递归
来源：http://qpd.ehwqpu.com

TS:   // 手写回溯递归
来源：http://ucv.c1oappe.top

Java: // 手写回溯递归
来源：http://msq.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://zpw.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://quv.xuanzx.com

C#:   // 手写回溯递归
来源：http://zpo.daxiang520.top

[N09] 栈与队列
来源：http://rcn.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://czv.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dfp.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kbd.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rnj.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dhg.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxw.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://syl.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kkk.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://tlh.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ebt.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vqd.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://djo.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kpf.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://lyj.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ssa.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://zpv.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pyi.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://qqz.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dij.fehbvm.com

PHP:  // 手写递归函数
来源：http://gns.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjl.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://enj.jlsjyb.cn

Java: // 手写递归
来源：http://rmy.hfpthk.cn

Go:   // 手写递归
来源：http://nyk.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iwy.xuetiantiany.cn

C#:   // 手写递归
来源：http://efr.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pzc.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fbi.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fbl.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ifz.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://swo.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ngg.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pqi.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://beh.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ofu.smart0.xyz

================================================================================
来源：http://wvn.redwolf501.top

O. 并发与异步
来源：http://zof.tianlin.xyz

================================================================================
来源：http://mop.hywenlv.cn

[O01] 启动一个线程
来源：http://bge.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ytz.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nuh.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://suu.bjfxy.top

TS:   // 同 JS
来源：http://hbg.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://gnr.daria6918.cn

Go:   go f()
来源：http://dfa.epnwcf.com

Ruby: Thread.new { f }
来源：http://tey.vehdjk.com

C#:   Task.Run(() => F());
来源：http://ctd.uphjek.com

[O02] 使用线程池
来源：http://elz.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ebw.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jal.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://hpn.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://jql.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://hgh.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ehh.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tup.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ajk.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://pqb.fengsongda.top

Py:   with lock: shared += 1
来源：http://rja.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://goj.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iez.yongpay.top

TS:   // 同 JS
来源：http://tzs.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://dis.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sxy.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wzk.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://dtz.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://pjg.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://wgk.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gpl.sxryk.cn

JS:   async function f() { await g(); }
来源：http://cxg.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qvc.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://crf.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xrv.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://chw.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://jwq.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://ndo.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://aqz.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vhp.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://qec.yonumen.top

TS:   await Promise.all(tasks)
来源：http://zbh.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uvl.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ldm.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://poy.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dzh.shuidangran.top

[O06] 使用进程池
来源：http://ryt.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cey.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wkk.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://cfg.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://pvj.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nik.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bux.jqgufenzy.top

Ruby: // fork 块
来源：http://cob.birdmap.top

C#:   Parallel.For
来源：http://zjq.cqqwz.cn

================================================================================
来源：http://vjj.nwbrower.top

P. 常用工具函数
来源：http://jvz.feifeiyinyue.top

================================================================================
来源：http://ogm.316326.xyz

[P01] 生成 UUID
来源：http://qbe.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://kyw.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hxv.smart0.xyz

JS:   crypto.randomUUID()
来源：http://ina.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://lev.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://rft.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://uqz.yj20258.top

Ruby: SecureRandom.uuid
来源：http://rpm.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://anf.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://orr.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://onq.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zsm.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zuy.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qag.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://glb.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jji.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ldk.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xwu.316326.xyz

[P03] 生成短随机字符串
来源：http://qda.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fpl.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nba.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://epf.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sbd.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gof.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ubn.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lpu.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://whw.hfpthk.cn

[P04] 求长度
来源：http://fym.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zwx.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fol.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gmv.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://opq.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://xtx.316326.xyz

Go:   len(arr);  len(m)
来源：http://otm.0kj1m.cn

Ruby: x.length;  x.size
来源：http://ceu.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://iru.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://irl.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lwt.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://svd.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nxk.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zsd.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tga.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://smo.ydzc1.top

Ruby: a == b
来源：http://elt.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oey.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zoo.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hlx.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://xak.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lnx.snrcjt.cn

TS:   if (x == null) {}
来源：http://vya.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lwr.jqgufenzy.top

Go:   if x == nil {}
来源：http://jfp.zhongyouzk.top


<!-- 参考信息 -->