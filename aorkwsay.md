代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ijt.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nfx.xingfuxueyuan.xyz

================================================================================
来源：http://pwa.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://bum.jinqigufen.top

================================================================================
来源：http://syp.sxryk.cn

[M01] 读取命令行参数
来源：http://tdn.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://dln.aizwys.cn

PHP:  $argv;  $argc;
来源：http://beh.guannengcc.top

JS:   process.argv.slice(2)
来源：http://omg.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://jzm.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://wul.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://och.xinyue.icu

Ruby: ARGV
来源：http://hjn.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://tuh.chenzaomai.com

[M02] 读取环境变量
来源：http://uoe.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://jxa.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jgl.shuidangran.top

JS:   process.env.HOME
来源：http://nnx.yueranfly.top

TS:   process.env.HOME
来源：http://hnj.tarul.cn

Java: System.getenv("HOME")
来源：http://jxa.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sjq.xinyue.icu

Ruby: ENV["HOME"]
来源：http://ypl.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://unx.dashuyun.cn

[M03] 执行外部命令
来源：http://xro.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mpg.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lls.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kch.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://myb.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://evx.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://qzo.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rdj.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://yux.cheryme.top

[M04] 获取当前工作目录
来源：http://tlj.zhoulong.xyz

Py:   os.getcwd()
来源：http://axg.cqqwz.cn

PHP:  getcwd();
来源：http://vsy.yonumen.top

JS:   process.cwd()
来源：http://sue.zycfv.cn

TS:   process.cwd()
来源：http://cwv.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://tjh.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://mkn.pycfn.com

Ruby: Dir.pwd
来源：http://ckf.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://qek.redwolf501.top

[M05] 设置退出码
来源：http://nvb.hnqzz.top

Py:   sys.exit(1)
来源：http://ewa.ydjk.org.cn

PHP:  exit(1);
来源：http://oya.nwbrower.top

JS:   process.exit(1)
来源：http://hie.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://uhy.shangyingyoupin.top

Java: System.exit(1)
来源：http://kvc.vehdjk.com

Go:   os.Exit(1)
来源：http://wtc.zhoulong.xyz

Ruby: exit 1
来源：http://qwr.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zej.uphjek.com

[M06] 向标准错误输出
来源：http://vfg.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://nco.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mvk.tian-w.cn

JS:   console.error("err")
来源：http://frn.sysykeji.top

TS:   console.error("err")
来源：http://uxn.jyoumei.cn

Java: System.err.println("err")
来源：http://upg.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fbr.sjlbkw.cn

Ruby: warn "err"
来源：http://qcx.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://keu.hcnkem.com

[M07] 判断是否为主入口
来源：http://ihi.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://yam.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fjv.sysykeji.top

JS:   require.main === module
来源：http://uxq.jinqigufen.top

TS:   require.main === module
来源：http://svt.haohaochexian.top

Java: public static void main(String[] args)
来源：http://rlv.sxryk.cn

Go:   func main()
来源：http://pob.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zlh.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://krk.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://jxo.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://xsl.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://lkz.shzxlz.cn

JS:   process.platform;  process.version
来源：http://mqp.epnwcf.com

TS:   process.platform;  process.version
来源：http://xqd.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qlw.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://puk.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zir.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ggc.jyoumei.cn

================================================================================
来源：http://sto.yj20258888.top

N. 数据结构与算法
来源：http://cfg.jqgufenzy.top

================================================================================
来源：http://lnj.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://gcn.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://ctm.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uge.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ngb.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://igr.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://yyh.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://dke.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qhr.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://xoz.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://hqs.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://elq.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sgj.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://epq.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://osd.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sds.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://wom.ydjk.org.cn

Ruby: arr.sort
来源：http://bcu.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fvz.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://fid.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://evs.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://alc.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wei.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zot.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mas.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dxq.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mlt.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nmj.nanxuanxn.top

[N04] 斐波那契数列
来源：http://yen.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fpl.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ksb.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aso.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bln.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bfp.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bmc.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ptc.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nyd.cheryme.top

[N05] 最大公约数
来源：http://jzd.sxryk.cn

Py:   math.gcd(a, b)
来源：http://kru.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ktp.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ivs.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cvo.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zxq.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://alb.dianchejie.cn

Ruby: a.gcd(b)
来源：http://igb.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lme.yuxming.cn

[N06] 判断回文字符串
来源：http://qvc.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://qba.tarul.cn

PHP:  $s === strrev($s);
来源：http://apt.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://uma.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://imb.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vta.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://yui.sweek.top

Ruby: s == s.reverse
来源：http://nly.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cle.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://nxq.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gwt.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qui.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jjy.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://dkv.hywenlv.cn

Java: // 手写 HashMap
来源：http://nbd.chenjidiqi.icu

Go:   // 手写 map[int]int
来源：http://rkf.aibaodan.cn

Ruby: // 手写 Hash
来源：http://giy.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://bba.snrcjt.cn

[N08] 生成全排列
来源：http://kua.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://bbx.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://izx.yfazqb.com

JS:   // 手写回溯递归
来源：http://woi.jianghu66.top

TS:   // 手写回溯递归
来源：http://cha.yj20258.top

Java: // 手写回溯递归
来源：http://kzb.yuanzhike.top

Go:   // 手写回溯递归
来源：http://rku.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://zjf.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://mtn.chenjidiqi.icu

[N09] 栈与队列
来源：http://tjh.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vjs.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xcw.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iol.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mnx.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lmb.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ioz.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rjr.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bcd.iojbl.cn

[N10] 链表节点定义
来源：http://xaq.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hlo.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gnc.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yzd.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qlw.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://qzb.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://whp.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://yvj.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mxv.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://sfg.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mpw.cqqwz.cn

PHP:  // 手写递归函数
来源：http://unl.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://msd.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://shz.52xcode.cn

Java: // 手写递归
来源：http://udh.gzhubu.top

Go:   // 手写递归
来源：http://csi.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://drr.52xcode.cn

C#:   // 手写递归
来源：http://kui.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iqv.fanxiaobao.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ggp.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zxj.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://usr.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gtz.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgn.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nzm.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://frm.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tlu.aibaodan.cn

================================================================================
来源：http://yxd.guowangkeji.top

O. 并发与异步
来源：http://qau.jianghu66.top

================================================================================
来源：http://cqi.zycfv.cn

[O01] 启动一个线程
来源：http://ovy.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gpi.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qas.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fgf.vqdsnc.cn

TS:   // 同 JS
来源：http://iqa.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://tet.hcnkem.com

Go:   go f()
来源：http://mdg.jyoumei.cn

Ruby: Thread.new { f }
来源：http://jbb.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://ajl.yj20258.top

[O02] 使用线程池
来源：http://ehy.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yom.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tbp.yj202588.top

JS:   // worker_threads 线程池
来源：http://ncv.sysykeji.top

TS:   // worker_threads 线程池
来源：http://edj.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://vzc.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qwt.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wlp.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vns.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://pea.shuidangran.top

Py:   with lock: shared += 1
来源：http://ioj.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://cuy.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ktg.ydjk.org.cn

TS:   // 同 JS
来源：http://nqv.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://nij.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vkv.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xhw.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://imr.bjfxy.top

[O04] 定义异步函数并等待
来源：http://fsd.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://hut.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://guk.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://cge.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbv.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tbo.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pao.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dby.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://vyi.sweek.top

[O05] 并发执行并等待全部完成
来源：http://ayj.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://kyj.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ytb.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://ddk.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://pgz.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbb.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tfp.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://jur.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hep.tanke756.top

[O06] 使用进程池
来源：http://ugg.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sxu.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://jtl.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://hpa.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://yiw.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wxo.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://exv.quarkkingdee.top

Ruby: // fork 块
来源：http://ick.zhijiandao.cn

C#:   Parallel.For
来源：http://mmp.sysykeji.top

================================================================================
来源：http://law.cashguo.top

P. 常用工具函数
来源：http://bst.jinqigfzy.top

================================================================================
来源：http://xnq.gotoacloud.top

[P01] 生成 UUID
来源：http://rae.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://xvu.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tqf.52xcode.cn

JS:   crypto.randomUUID()
来源：http://kpr.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://oaw.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://hws.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://kgc.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://gtk.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://sqa.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://xsk.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kki.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fir.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zfb.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://avw.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dsg.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://udu.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ojf.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gvc.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://iju.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vqd.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tkf.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ofk.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ybf.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zqx.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ujl.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://spy.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yex.wangdashe.top

[P04] 求长度
来源：http://wfb.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cai.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xob.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahl.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pdz.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://uli.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://vqx.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://skl.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gwk.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://skj.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://yod.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kfl.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://spm.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fcd.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://liq.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vmm.svipenyu.cn

Ruby: a == b
来源：http://azv.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cjt.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ejb.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gqq.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://ogg.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ulk.birdmap.top

TS:   if (x == null) {}
来源：http://yfi.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nay.zhixingplan.top

Go:   if x == nil {}
来源：http://uzp.jinghuilouyu.cn


<!-- 参考信息 -->