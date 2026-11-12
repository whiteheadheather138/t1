代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wih.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://czc.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hdt.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fll.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kzx.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://knk.uphjek.com

================================================================================
来源：http://ozi.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://pdt.yj202588.top

================================================================================
来源：http://hrz.meibo888.top

[M01] 读取命令行参数
来源：http://slx.shzxlz.cn

Py:   sys.argv[1:]
来源：http://fkw.yfazqb.com

PHP:  $argv;  $argc;
来源：http://qcc.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://qoo.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://nno.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://stb.daria6918.cn

Go:   os.Args[1:]
来源：http://tun.daria6918.cn

Ruby: ARGV
来源：http://utl.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://tqe.birdmap.top

[M02] 读取环境变量
来源：http://vjn.pycfn.com

Py:   os.environ.get("HOME")
来源：http://knp.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fvr.hywenlv.cn

JS:   process.env.HOME
来源：http://lqf.guannengcc.top

TS:   process.env.HOME
来源：http://izo.xuanzx.com

Java: System.getenv("HOME")
来源：http://zdt.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ega.smart0.xyz

Ruby: ENV["HOME"]
来源：http://ymd.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ppi.guowangkeji.top

[M03] 执行外部命令
来源：http://ygq.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zkb.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mym.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://upp.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wog.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qxd.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hbo.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yxf.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://ggh.52xcode.cn

[M04] 获取当前工作目录
来源：http://cgn.nwbrower.top

Py:   os.getcwd()
来源：http://wuy.yj20258888.top

PHP:  getcwd();
来源：http://ibw.jinqigfzy.top

JS:   process.cwd()
来源：http://pcq.hywenlv.cn

TS:   process.cwd()
来源：http://jcn.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://vlq.iojbl.cn

Go:   os.Getwd()
来源：http://ppt.zhongyouzk.top

Ruby: Dir.pwd
来源：http://say.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xse.aizwys.cn

[M05] 设置退出码
来源：http://zfd.iojbl.cn

Py:   sys.exit(1)
来源：http://ruv.mhx1999.top

PHP:  exit(1);
来源：http://rau.nanxinkj.top

JS:   process.exit(1)
来源：http://hhy.zhengqikj.top

TS:   process.exit(1)
来源：http://prk.ybcxt.top

Java: System.exit(1)
来源：http://tgv.jqgufenzy.top

Go:   os.Exit(1)
来源：http://wxq.yj20258.top

Ruby: exit 1
来源：http://jyb.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://itl.zhijiandao.cn

[M06] 向标准错误输出
来源：http://bos.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://eqy.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gqy.cashguo.top

JS:   console.error("err")
来源：http://exo.sxryk.cn

TS:   console.error("err")
来源：http://wbn.yvedp.cn

Java: System.err.println("err")
来源：http://rrz.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qxu.wangshuangyany.cn

Ruby: warn "err"
来源：http://eua.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://cyk.daxiang520.top

[M07] 判断是否为主入口
来源：http://gri.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://pze.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ccw.yangfankeji.com

JS:   require.main === module
来源：http://qaa.hywenlv.cn

TS:   require.main === module
来源：http://oty.sysykeji.top

Java: public static void main(String[] args)
来源：http://sdm.tian-w.cn

Go:   func main()
来源：http://dwb.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xwb.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://fsh.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://awf.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://pkz.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://yde.daxiang520.top

JS:   process.platform;  process.version
来源：http://xdv.jianghu66.top

TS:   process.platform;  process.version
来源：http://oeb.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tec.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://oiq.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uyb.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mkw.shanyushiyangtech.top

================================================================================
来源：http://bvx.hysaishi.cn

N. 数据结构与算法
来源：http://zyh.hywenlv.cn

================================================================================
来源：http://ixe.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://xis.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qhs.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://icx.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hcb.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rgx.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://iks.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://ghm.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cic.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://qlj.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://bob.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://vhp.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://agu.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bha.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vil.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eax.yj20258888.top

Go:   slices.Sort(arr)
来源：http://xzm.jqgufenzy.top

Ruby: arr.sort
来源：http://fat.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xcc.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://vjp.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://obi.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://emb.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rsx.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wwa.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dko.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xyj.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ibf.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://zsm.ydjk.org.cn

[N04] 斐波那契数列
来源：http://nuo.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tpb.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zgl.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mrk.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhy.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zrb.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ann.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wrd.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ffm.yj20258.top

[N05] 最大公约数
来源：http://fho.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://pxk.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ysw.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ouz.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wbt.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zdl.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://llo.dianchejie.cn

Ruby: a.gcd(b)
来源：http://ijx.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uno.bbcook.cn

[N06] 判断回文字符串
来源：http://brt.jiagoushi.top

Py:   s == s[::-1]
来源：http://vmg.fengsongda.top

PHP:  $s === strrev($s);
来源：http://jqs.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://eml.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://nvf.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zaz.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://qqa.ehwqpu.com

Ruby: s == s.reverse
来源：http://rln.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cvo.meibo888.top

[N07] 两数之和（返回下标）
来源：http://gte.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://usd.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jcb.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ztb.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://hci.xylfe.cn

Java: // 手写 HashMap
来源：http://ixa.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://krz.jinqigufen.top

Ruby: // 手写 Hash
来源：http://mhd.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kfa.jinghuilouyu.cn

[N08] 生成全排列
来源：http://joa.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://sqh.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://isq.cucudq.cn

JS:   // 手写回溯递归
来源：http://tit.sxryk.cn

TS:   // 手写回溯递归
来源：http://beq.0kj1m.cn

Java: // 手写回溯递归
来源：http://zuk.svipenyu.cn

Go:   // 手写回溯递归
来源：http://jdd.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://ziw.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://lck.zdqjudy.top

[N09] 栈与队列
来源：http://lzi.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kmt.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ntj.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lvb.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aws.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hbn.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rnf.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ury.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://grk.316326.xyz

[N10] 链表节点定义
来源：http://cgk.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sls.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ybu.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vzw.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gqy.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://oyh.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gej.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rfb.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xlu.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://mgm.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://igv.ehwqpu.com

PHP:  // 手写递归函数
来源：http://tfk.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tsx.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ubr.yueranfly.top

Java: // 手写递归
来源：http://sjf.9152youxi.cn

Go:   // 手写递归
来源：http://uaf.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tsj.tarul.cn

C#:   // 手写递归
来源：http://rgk.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cyh.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://acf.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://frj.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mil.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mrg.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://obw.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xcc.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ilu.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zbe.ivvv.top

================================================================================
来源：http://rgm.bbcook.cn

O. 并发与异步
来源：http://gur.xinyue.icu

================================================================================
来源：http://bqq.smart0.xyz

[O01] 启动一个线程
来源：http://xws.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dnj.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xuj.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vpi.c1oappe.top

TS:   // 同 JS
来源：http://mtk.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://umz.xziqi.cn

Go:   go f()
来源：http://mhl.pycfn.com

Ruby: Thread.new { f }
来源：http://iis.ybcxt.top

C#:   Task.Run(() => F());
来源：http://wkd.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://agn.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vui.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vxl.sxryk.cn

JS:   // worker_threads 线程池
来源：http://nid.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://jve.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://vmw.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uhi.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bcm.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vnj.yvedp.cn

[O03] 加锁保护共享数据
来源：http://dyu.yvedp.cn

Py:   with lock: shared += 1
来源：http://tcs.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://aua.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gjn.zhiwuduotai.top

TS:   // 同 JS
来源：http://kxj.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://ipx.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mqv.yonumen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://csv.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://nai.mhx1999.top

[O04] 定义异步函数并等待
来源：http://pfa.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://jvq.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yfk.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://hmi.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jbx.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bmq.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://udd.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://nuq.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://zyy.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://cas.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://xjl.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxu.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://ebc.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://hdw.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://diu.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://imr.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://gwk.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zli.hnxiangtu.top

[O06] 使用进程池
来源：http://byq.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zhq.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://psy.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://mat.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://nfr.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://taz.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vgs.redwolf501.top

Ruby: // fork 块
来源：http://dcs.xuanzx.com

C#:   Parallel.For
来源：http://jan.andypj.xyz

================================================================================
来源：http://fji.xziqi.cn

P. 常用工具函数
来源：http://qgp.52xcode.cn

================================================================================
来源：http://mvt.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://jag.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://skf.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kci.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://fys.yongpay.top

TS:   crypto.randomUUID()
来源：http://yex.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://uvk.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://caa.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://ajj.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://nua.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://rno.hcnkem.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vlx.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zgq.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sba.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://anp.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iar.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://agd.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uxu.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mwy.havefunace.top

[P03] 生成短随机字符串
来源：http://ujh.xingfuxueyuan.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xav.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tam.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tdt.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://how.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://txw.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pvt.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ewk.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bvl.bbcook.cn

[P04] 求长度
来源：http://ohb.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lpn.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sbq.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://axi.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uwx.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://pid.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://sxa.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://oqt.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gba.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://wxq.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yxz.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cjp.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zxw.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hro.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://buf.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jqg.yuanzhike.top

Ruby: a == b
来源：http://obu.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zsd.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kpu.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://olh.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://mef.52xcode.cn


<!-- 参考信息 -->