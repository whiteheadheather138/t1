代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yll.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhj.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ffi.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wnq.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://puw.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ruc.daria6918.cn

================================================================================
来源：http://yvi.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://ptu.52xcode.cn

================================================================================
来源：http://fhq.hysaishi.cn

[M01] 读取命令行参数
来源：http://dfm.svipenyu.cn

Py:   sys.argv[1:]
来源：http://uyg.ivvv.top

PHP:  $argv;  $argc;
来源：http://rby.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://kkj.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://pog.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://gdf.uphjek.com

Go:   os.Args[1:]
来源：http://csv.hongshengwenyu.top

Ruby: ARGV
来源：http://znj.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://xzi.yj202588.top

[M02] 读取环境变量
来源：http://kun.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://cnp.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oov.quarkkingdee.top

JS:   process.env.HOME
来源：http://fcc.zhiwuduotai.top

TS:   process.env.HOME
来源：http://iou.yangfankeji.com

Java: System.getenv("HOME")
来源：http://dcj.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ija.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://une.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vla.shuidangran.top

[M03] 执行外部命令
来源：http://aqr.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ngj.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lxq.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tux.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vcg.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://loh.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yrn.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://buk.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://xis.hysaishi.cn

[M04] 获取当前工作目录
来源：http://bcu.xylfe.cn

Py:   os.getcwd()
来源：http://dmy.yfazqb.com

PHP:  getcwd();
来源：http://dcs.hnqzz.top

JS:   process.cwd()
来源：http://nuo.meibo888.top

TS:   process.cwd()
来源：http://oec.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://ael.xinyue.icu

Go:   os.Getwd()
来源：http://hzw.ybcxt.top

Ruby: Dir.pwd
来源：http://cpm.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://evt.hfpthk.cn

[M05] 设置退出码
来源：http://xwu.zhengqikj.top

Py:   sys.exit(1)
来源：http://flu.svipenyu.cn

PHP:  exit(1);
来源：http://vqh.zhongyouzk.top

JS:   process.exit(1)
来源：http://rkt.shzxlz.cn

TS:   process.exit(1)
来源：http://une.hysaishi.cn

Java: System.exit(1)
来源：http://soy.tarul.cn

Go:   os.Exit(1)
来源：http://fqx.bjfxy.top

Ruby: exit 1
来源：http://mdm.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kaw.tanke756.top

[M06] 向标准错误输出
来源：http://yow.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://aep.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://plh.fengsongda.top

JS:   console.error("err")
来源：http://lsm.hongshengwenyu.top

TS:   console.error("err")
来源：http://ebk.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://ocb.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jgl.nanxinkj.top

Ruby: warn "err"
来源：http://mew.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://bfo.hysaishi.cn

[M07] 判断是否为主入口
来源：http://fuc.birdmap.top

Py:   if __name__ == "__main__":
来源：http://evi.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://igl.hysaishi.cn

JS:   require.main === module
来源：http://nbp.tarul.cn

TS:   require.main === module
来源：http://ett.epnwcf.com

Java: public static void main(String[] args)
来源：http://xkg.ivvv.top

Go:   func main()
来源：http://uax.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cih.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://uay.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://xhi.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://dta.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://pgo.havefunace.top

JS:   process.platform;  process.version
来源：http://iih.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://kve.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hnf.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://uiq.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pfn.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xjk.nanxuanxn.top

================================================================================
来源：http://xku.chenzaomai.com

N. 数据结构与算法
来源：http://yke.ctjpmb.com

================================================================================
来源：http://nij.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://dml.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://isc.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lpm.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yvn.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pty.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://xhh.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://cqo.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vjh.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://yvn.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://msz.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://pdh.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kqi.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pnw.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xuq.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zkg.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://ovf.zhixingplan.top

Ruby: arr.sort
来源：http://twz.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mgu.tarul.cn

[N03] 快速排序（分治示例）
来源：http://sqd.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qdx.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://gys.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lzz.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sud.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kdg.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gge.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tmh.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://aaw.0kj1m.cn

[N04] 斐波那契数列
来源：http://dqo.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kwq.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rpu.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jul.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvy.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bsm.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://imp.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ray.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://frh.cdnleiting.top

[N05] 最大公约数
来源：http://srd.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://yyv.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cjk.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eff.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jwl.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fjr.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://whn.nwbrower.top

Ruby: a.gcd(b)
来源：http://esp.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ogk.yongpay.top

[N06] 判断回文字符串
来源：http://qtl.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://oyl.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://mny.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://ugs.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://hqg.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nei.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://jkx.xuanzx.com

Ruby: s == s.reverse
来源：http://axm.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dfs.tanke756.top

[N07] 两数之和（返回下标）
来源：http://eje.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nxh.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eyo.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mcm.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://bdf.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://daq.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://wzm.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://xlu.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://guf.guowangkeji.top

[N08] 生成全排列
来源：http://fja.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://hgh.haohaochexian.top

PHP:  // 手写递归交换
来源：http://yvm.ctjpmb.com

JS:   // 手写回溯递归
来源：http://zxk.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://vhn.ivvv.top

Java: // 手写回溯递归
来源：http://zen.yj20258888.top

Go:   // 手写回溯递归
来源：http://soq.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://xgn.ehwqpu.com

C#:   // 手写回溯递归
来源：http://dup.redwolf501.top

[N09] 栈与队列
来源：http://jcv.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aft.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fbu.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fgy.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pfp.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://khc.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sqm.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zel.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vfa.zdbjq.cn

[N10] 链表节点定义
来源：http://nsd.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vlr.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gge.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bkn.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cjj.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://wdw.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://nay.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yio.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eix.guannengcc.top

[N11] 二叉树中序遍历
来源：http://vxc.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rqr.zhengqikj.top

PHP:  // 手写递归函数
来源：http://yig.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ruu.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fig.fehbvm.com

Java: // 手写递归
来源：http://cak.yj20258.top

Go:   // 手写递归
来源：http://wtk.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://srr.sxryk.cn

C#:   // 手写递归
来源：http://qvt.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mgc.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fld.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://szh.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sao.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nqo.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ttt.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uvj.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vjh.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ngv.ehwqpu.com

================================================================================
来源：http://xcu.cashguo.top

O. 并发与异步
来源：http://etr.zdqjudy.top

================================================================================
来源：http://zei.daxiang520.top

[O01] 启动一个线程
来源：http://dwg.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ybi.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hpf.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sdf.yangfankeji.com

TS:   // 同 JS
来源：http://adz.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://gff.fktsv.cn

Go:   go f()
来源：http://hzx.yongpay.top

Ruby: Thread.new { f }
来源：http://doi.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://buk.nanxuanxn.top

[O02] 使用线程池
来源：http://fvr.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bdh.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ngp.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://ehw.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://txz.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://ylv.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ras.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wuy.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jvy.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://jth.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://fmq.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://bvg.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://opk.yfazqb.com

TS:   // 同 JS
来源：http://lvn.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://bwr.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cbi.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://upz.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://sex.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://rjz.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://eys.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pmr.ydzc1.top

JS:   async function f() { await g(); }
来源：http://jxa.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aht.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lhy.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ryt.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lln.pycfn.com

C#:   async Task F() { await G(); }
来源：http://jug.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://odf.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://msa.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hab.yongpay.top

JS:   await Promise.all(tasks)
来源：http://ddr.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://wpz.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iqa.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qzr.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://unr.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qbm.smart0.xyz

[O06] 使用进程池
来源：http://kjj.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ixf.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://svt.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://rze.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://hsi.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pix.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ibb.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://sxa.meibo888.top

C#:   Parallel.For
来源：http://zuw.snrcjt.cn

================================================================================
来源：http://dvn.cashguo.top

P. 常用工具函数
来源：http://rok.hongshengwenyu.top

================================================================================
来源：http://xcx.zhoulong.xyz

[P01] 生成 UUID
来源：http://kid.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://dee.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fns.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://fan.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://ioa.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://fed.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://hjr.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://ajb.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://wlh.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://dea.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bvl.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://znd.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nhc.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wzz.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dyl.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lqe.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mlh.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nyl.yongpay.top

[P03] 生成短随机字符串
来源：http://bav.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wsc.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ufz.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jxo.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eom.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://frv.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upi.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bkl.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kwd.sweek.top

[P04] 求长度
来源：http://fhf.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sjy.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcn.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://doo.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ktp.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://ydq.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://vsn.fengsongda.top

Ruby: x.length;  x.size
来源：http://bix.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bql.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://beo.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tth.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aeb.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cnk.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://von.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dwa.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://ynl.jiagoushi.top

Ruby: a == b
来源：http://yvu.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yee.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://moy.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://htg.birdmap.top

PHP:  if (empty($x)) {}
来源：http://aki.quarkkingdee.top


<!-- 参考信息 -->