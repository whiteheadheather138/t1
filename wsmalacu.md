代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwl.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zau.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zhb.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://riz.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hri.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dkd.tanke756.top

================================================================================
来源：http://dtg.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://xdt.cheryme.top

================================================================================
来源：http://nus.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://nbf.haohaochexian.top

Py:   sys.argv[1:]
来源：http://quj.yj20258888.top

PHP:  $argv;  $argc;
来源：http://qtr.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://ukh.xuanzx.com

TS:   process.argv.slice(2)
来源：http://mnj.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://akx.fehbvm.com

Go:   os.Args[1:]
来源：http://zhl.gaohongyu789.top

Ruby: ARGV
来源：http://mtd.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://ldi.epnwcf.com

[M02] 读取环境变量
来源：http://ppa.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://xis.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zat.redwolf501.top

JS:   process.env.HOME
来源：http://sqn.chenzaomai.com

TS:   process.env.HOME
来源：http://ham.hesvh.cn

Java: System.getenv("HOME")
来源：http://oac.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zys.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://cud.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://khc.zdbjq.cn

[M03] 执行外部命令
来源：http://bim.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ajj.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tkb.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lly.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cuq.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zed.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gow.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://tnc.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://gcj.hcnkem.com

[M04] 获取当前工作目录
来源：http://tkf.9152youxi.cn

Py:   os.getcwd()
来源：http://pyf.jinqigfzy.top

PHP:  getcwd();
来源：http://dzu.aibaodan.cn

JS:   process.cwd()
来源：http://ibf.kuanghao11.cn

TS:   process.cwd()
来源：http://caq.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://wss.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://lkz.xinyue.icu

Ruby: Dir.pwd
来源：http://ddf.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yvv.cucudq.cn

[M05] 设置退出码
来源：http://rbh.tianlin.xyz

Py:   sys.exit(1)
来源：http://vud.ivvv.top

PHP:  exit(1);
来源：http://sbo.jianghu66.top

JS:   process.exit(1)
来源：http://tob.cucudq.cn

TS:   process.exit(1)
来源：http://aec.ehwqpu.com

Java: System.exit(1)
来源：http://bmr.nanxinkj.top

Go:   os.Exit(1)
来源：http://tzg.mhx1999.top

Ruby: exit 1
来源：http://qfz.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lwd.yonumen.top

[M06] 向标准错误输出
来源：http://ugf.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://dpa.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vsz.epnwcf.com

JS:   console.error("err")
来源：http://inu.gogol.net.cn

TS:   console.error("err")
来源：http://mvj.mhx1999.top

Java: System.err.println("err")
来源：http://ama.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pmr.sweek.top

Ruby: warn "err"
来源：http://skj.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://tqh.fehbvm.com

[M07] 判断是否为主入口
来源：http://kzg.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://eku.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://asi.zycfv.cn

JS:   require.main === module
来源：http://jjs.zdqjudy.top

TS:   require.main === module
来源：http://dxa.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://hix.zhixingplan.top

Go:   func main()
来源：http://djv.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://woz.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://jlx.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://lhc.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://coj.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://xbr.hesvh.cn

JS:   process.platform;  process.version
来源：http://cil.fehbvm.com

TS:   process.platform;  process.version
来源：http://vqg.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zyj.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rnq.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gos.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fjc.guowangkeji.top

================================================================================
来源：http://mnu.chenzaomai.com

N. 数据结构与算法
来源：http://gdt.yj20258.top

================================================================================
来源：http://tha.ivvv.top

[N01] 二分查找（有序数组）
来源：http://zjd.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://hlo.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fhj.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jrp.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ill.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://efq.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://szj.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://hfb.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gzb.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://qdv.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://ioz.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zwr.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jmg.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tmm.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://esl.yuxming.cn

Go:   slices.Sort(arr)
来源：http://dpo.zhoulong.xyz

Ruby: arr.sort
来源：http://rbk.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kro.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://qwx.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tgt.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://ops.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmy.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fpt.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wgm.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bfm.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://piu.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://bcf.xylfe.cn

[N04] 斐波那契数列
来源：http://ddm.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ltq.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cqh.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://voi.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wld.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tvs.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qeg.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://twv.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://szk.feifeiyinyue.top

[N05] 最大公约数
来源：http://alb.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://slg.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bfi.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iox.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbl.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gip.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jas.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://gfv.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cqo.dashuyun.cn

[N06] 判断回文字符串
来源：http://tjj.cucudq.cn

Py:   s == s[::-1]
来源：http://nnm.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://fis.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://rab.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://dol.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sdx.wangdashe.top

Go:   // 双指针从两端比较
来源：http://jvh.zdqjudy.top

Ruby: s == s.reverse
来源：http://ufw.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lbw.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://rjs.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gdu.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqo.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://btr.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://abw.cqqwz.cn

Java: // 手写 HashMap
来源：http://xyk.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://tpu.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://pdi.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://qvw.xuanzx.com

[N08] 生成全排列
来源：http://lpu.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://rwx.yj20258.top

PHP:  // 手写递归交换
来源：http://gvf.ybcxt.top

JS:   // 手写回溯递归
来源：http://tic.shuidangran.top

TS:   // 手写回溯递归
来源：http://hst.cucudq.cn

Java: // 手写回溯递归
来源：http://uor.guowangkeji.top

Go:   // 手写回溯递归
来源：http://ctc.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://udq.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://xwf.ydjk.org.cn

[N09] 栈与队列
来源：http://jhl.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rie.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zku.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://drp.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yfh.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iys.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eux.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xon.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tei.shzxlz.cn

[N10] 链表节点定义
来源：http://tju.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ogj.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iwn.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ayf.zhongyouzk.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rtu.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://ljd.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://bev.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uga.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sjo.fehbvm.com

[N11] 二叉树中序遍历
来源：http://wfw.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ams.xylfe.cn

PHP:  // 手写递归函数
来源：http://nmp.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wgh.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vdb.mhx1999.top

Java: // 手写递归
来源：http://rti.daxiang520.top

Go:   // 手写递归
来源：http://gjh.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xoi.zhixingplan.top

C#:   // 手写递归
来源：http://nqn.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uqy.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zds.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xbc.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vje.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bsc.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yvw.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gdl.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dur.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kzh.ydzc1.top

================================================================================
来源：http://fnf.sxryk.cn

O. 并发与异步
来源：http://yfz.fengsongda.top

================================================================================
来源：http://bzw.aibaodan.cn

[O01] 启动一个线程
来源：http://wjm.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gsm.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mmq.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://egy.gogol.net.cn

TS:   // 同 JS
来源：http://eda.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://gcn.xuetiantiany.cn

Go:   go f()
来源：http://sip.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://xbs.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://nkh.chenzaomai.com

[O02] 使用线程池
来源：http://utq.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yxm.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rid.daria6918.cn

JS:   // worker_threads 线程池
来源：http://qft.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://ogb.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://brj.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tzy.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fwo.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rir.aizwys.cn

[O03] 加锁保护共享数据
来源：http://oyx.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://ecz.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://njl.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kip.zhongyouzk.top

TS:   // 同 JS
来源：http://leq.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://dig.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dbv.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://asn.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://qon.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://nyf.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://jbl.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://doh.iojbl.cn

JS:   async function f() { await g(); }
来源：http://vps.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://tqj.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://abb.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rlt.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://jni.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://qpm.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://oen.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://ios.xinyue.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tao.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://qmj.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://tie.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://exm.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mxx.sxryk.cn

Ruby: threads.map(&:join)
来源：http://onx.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dvv.yj202588.top

[O06] 使用进程池
来源：http://wdg.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dpl.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uam.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://sjd.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://lxg.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lrr.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jox.mhx1999.top

Ruby: // fork 块
来源：http://mxy.shzxlz.cn

C#:   Parallel.For
来源：http://qdn.zhaomingkeji.xyz

================================================================================
来源：http://awu.ppjwa.cn

P. 常用工具函数
来源：http://bwd.52xcode.cn

================================================================================
来源：http://dor.uphjek.com

[P01] 生成 UUID
来源：http://bxo.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://tem.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kao.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://psx.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://ntl.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://qew.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://vpg.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://bue.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://bjo.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://jhh.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://myk.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://btp.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mfq.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://spf.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qsk.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ufz.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mgt.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://djr.xylfe.cn

[P03] 生成短随机字符串
来源：http://bxn.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tmt.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bcq.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mle.yvedp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gpj.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qkf.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vru.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kqn.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tyr.shanyushiyangkeji.top

[P04] 求长度
来源：http://bsm.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zdd.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hqi.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uee.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqd.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://umh.xinyue.icu

Go:   len(arr);  len(m)
来源：http://ffp.cashguo.top

Ruby: x.length;  x.size
来源：http://wol.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zkk.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://pqh.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yqh.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fls.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://osx.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hyi.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://spb.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ygr.gaohongyu789.top

Ruby: a == b
来源：http://auf.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rgi.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kyo.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wwb.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://jxt.shangyingyoupin.top


<!-- 参考信息 -->