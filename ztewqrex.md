代发 wailian999

JS:   process.argv.slice(2)
来源：http://dhy.c1oappe.top

TS:   process.argv.slice(2)
来源：http://hei.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://stu.yj202588.top

Go:   os.Args[1:]
来源：http://uqi.dashuyun.cn

Ruby: ARGV
来源：http://rkn.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://zao.jiagoushi.top

[M02] 读取环境变量
来源：http://anf.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://poj.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wdd.xinyue.icu

JS:   process.env.HOME
来源：http://bzs.chenzaomai.com

TS:   process.env.HOME
来源：http://pbi.gotoacloud.top

Java: System.getenv("HOME")
来源：http://ylw.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qgx.yongpay.top

Ruby: ENV["HOME"]
来源：http://pbx.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://icx.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://grt.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tro.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://itz.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bxf.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ejm.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zrt.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://thk.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jfl.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://hus.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://xmj.jqgfzy.top

Py:   os.getcwd()
来源：http://qhe.sweek.top

PHP:  getcwd();
来源：http://uxy.fktsv.cn

JS:   process.cwd()
来源：http://ems.fktsv.cn

TS:   process.cwd()
来源：http://aib.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://gld.jqgfzy.top

Go:   os.Getwd()
来源：http://ouh.fengsongda.top

Ruby: Dir.pwd
来源：http://faq.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://tro.zhongyouzk.top

[M05] 设置退出码
来源：http://jvf.hfpthk.cn

Py:   sys.exit(1)
来源：http://svw.dianchejie.cn

PHP:  exit(1);
来源：http://bwm.birdmap.top

JS:   process.exit(1)
来源：http://run.shangyingyoupin.top

TS:   process.exit(1)
来源：http://yec.shangyingyoupin.top

Java: System.exit(1)
来源：http://wng.tianlin.xyz

Go:   os.Exit(1)
来源：http://qop.jqgufenzy.top

Ruby: exit 1
来源：http://nat.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iok.pycfn.com

[M06] 向标准错误输出
来源：http://jiy.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://vvg.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://web.hywenlv.cn

JS:   console.error("err")
来源：http://hub.zhengqikj.top

TS:   console.error("err")
来源：http://vac.jqgfzy.top

Java: System.err.println("err")
来源：http://upu.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xgf.xuanzx.com

Ruby: warn "err"
来源：http://bza.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://oub.yueranfly.top

[M07] 判断是否为主入口
来源：http://cui.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://utb.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mlb.ybcxt.top

JS:   require.main === module
来源：http://shj.zhixingplan.top

TS:   require.main === module
来源：http://rtb.ivvv.top

Java: public static void main(String[] args)
来源：http://mwb.shzxlz.cn

Go:   func main()
来源：http://tch.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mcc.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://nch.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://ppz.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://svf.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://eyv.ivvv.top

JS:   process.platform;  process.version
来源：http://whm.yangfankeji.com

TS:   process.platform;  process.version
来源：http://gck.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wex.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pyf.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ynl.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xmc.cdnleiting.top

================================================================================
来源：http://xmc.yfazqb.com

N. 数据结构与算法
来源：http://cki.ywan-chungtsiang.top

================================================================================
来源：http://rnw.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://lvv.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bnw.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ckd.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ckc.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ezv.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://ohh.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://ngp.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wqq.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tsg.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://cjk.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://vmh.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kki.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uap.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rwu.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wij.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://wdk.c1oappe.top

Ruby: arr.sort
来源：http://wlg.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vqg.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://fup.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bey.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://klr.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfh.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ukr.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uoe.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jfg.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nou.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://edf.ctjpmb.com

[N04] 斐波那契数列
来源：http://mxz.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fjg.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nwf.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nbf.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rbz.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yfi.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ycb.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://akz.hammf.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qaf.guowangkeji.top

[N05] 最大公约数
来源：http://ntj.tarul.cn

Py:   math.gcd(a, b)
来源：http://msb.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jvy.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cdf.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xft.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wxh.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://afu.jianghu66.top

Ruby: a.gcd(b)
来源：http://nmp.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jhx.yuanzhike.top

[N06] 判断回文字符串
来源：http://cpy.gogol.net.cn

Py:   s == s[::-1]
来源：http://pqv.epnwcf.com

PHP:  $s === strrev($s);
来源：http://mcv.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://bcz.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://chv.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eik.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://vqk.sjlbkw.cn

Ruby: s == s.reverse
来源：http://jib.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lhk.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://swh.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ruh.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tbf.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ynf.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://ykc.tarul.cn

Java: // 手写 HashMap
来源：http://ufw.uphjek.com

Go:   // 手写 map[int]int
来源：http://shq.xinyue.icu

Ruby: // 手写 Hash
来源：http://cvi.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://jpo.yj202588.top

[N08] 生成全排列
来源：http://kuv.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://prn.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://fot.fengsongda.top

JS:   // 手写回溯递归
来源：http://aej.zhengqikj.top

TS:   // 手写回溯递归
来源：http://wby.jlsjyb.cn

Java: // 手写回溯递归
来源：http://wqs.ppjwa.cn

Go:   // 手写回溯递归
来源：http://jbz.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://tsg.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://xsw.andypj.xyz

[N09] 栈与队列
来源：http://bzs.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vrw.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://szl.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wuf.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ceu.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kju.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yex.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pnk.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ucg.yongpay.top

[N10] 链表节点定义
来源：http://qgv.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eyl.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vcj.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bgb.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmm.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://fll.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ktl.shuidangran.top

Ruby: Node = Struct.new(:v, :next)
来源：http://eso.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jat.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://zbb.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jbv.zhengqikj.top

PHP:  // 手写递归函数
来源：http://ldy.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eby.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccd.yj20258.top

Java: // 手写递归
来源：http://ggg.hnxiangtu.top

Go:   // 手写递归
来源：http://uzo.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://chh.hywenlv.cn

C#:   // 手写递归
来源：http://uqb.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uyc.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yiq.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nvy.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lxe.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbl.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cdh.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kbf.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xpj.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://apz.cucudq.cn

================================================================================
来源：http://xtn.shanyushiyangkeji.top

O. 并发与异步
来源：http://hfe.shanyushiyangtech.top

================================================================================
来源：http://ppd.tanke756.top

[O01] 启动一个线程
来源：http://vgd.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zkb.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://std.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xom.vqdsnc.cn

TS:   // 同 JS
来源：http://wai.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://ohd.sysykeji.top

Go:   go f()
来源：http://rix.haohaochexian.top

Ruby: Thread.new { f }
来源：http://znl.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://dln.iojbl.cn

[O02] 使用线程池
来源：http://cyv.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cmk.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kap.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://xlj.xylfe.cn

TS:   // worker_threads 线程池
来源：http://mmv.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://yll.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cmy.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://akr.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://asq.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://hwi.chenzaomai.com

Py:   with lock: shared += 1
来源：http://swy.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://fcz.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nie.sxryk.cn

TS:   // 同 JS
来源：http://umy.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://nhd.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://haw.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fsu.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://gne.smart0.xyz

[O04] 定义异步函数并等待
来源：http://kda.ivvv.top

Py:   async def f():⏎    await g()
来源：http://wpw.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bkc.nwbrower.top

JS:   async function f() { await g(); }
来源：http://ugh.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://emk.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tso.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xxo.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://quy.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://hzs.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://fev.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://eyq.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://clz.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://ywh.birdmap.top

TS:   await Promise.all(tasks)
来源：http://rfg.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uxz.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ytb.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://hdv.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ccd.birdmap.top

[O06] 使用进程池
来源：http://vdo.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eyr.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yoh.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://gfz.uphjek.com

TS:   // child_process / cluster 模块
来源：http://yaf.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sok.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dxs.gotoacloud.top

Ruby: // fork 块
来源：http://tth.feifeiyinyue.top

C#:   Parallel.For
来源：http://had.shanyushiyangkeji.top

================================================================================
来源：http://apd.yj20258888.top

P. 常用工具函数
来源：http://bok.vqdsnc.cn

================================================================================
来源：http://zwm.wangshuangyany.cn

[P01] 生成 UUID
来源：http://yoa.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://hxl.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rqe.bbcook.cn

JS:   crypto.randomUUID()
来源：http://djv.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://rji.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://gbj.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://elk.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://uux.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://yfy.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://zxm.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wwv.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://sjq.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kni.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yll.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yrj.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://euz.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mlp.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://udp.aibaodan.cn

[P03] 生成短随机字符串
来源：http://axt.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blj.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rus.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klk.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bli.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zfd.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ozl.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fmh.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ouy.sufxvd.cn

[P04] 求长度
来源：http://lum.yongpay.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://clv.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xsc.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fpi.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lrt.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://wkj.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://afx.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://jkk.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kdc.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://zif.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qld.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nip.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jvj.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cit.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mzb.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://fgw.c1oappe.top

Ruby: a == b
来源：http://jhu.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fxv.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nfz.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pei.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://yos.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ifx.gzhubu.top

TS:   if (x == null) {}
来源：http://lfb.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ted.zhoulong.xyz

Go:   if x == nil {}
来源：http://uvc.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mcp.zhengqikj.top

C#:   if (x is null) {}
来源：http://rly.zycfv.cn

[P07] 防抖与节流
来源：http://pbh.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bmc.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://xvz.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwz.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsy.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://azy.guowangkeji.top


<!-- 参考信息 -->