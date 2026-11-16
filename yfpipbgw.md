代发 wailian999

C#:   (int)resp.StatusCode
来源：http://cid.hcnkem.com

[L08] 并发请求多个地址
来源：http://pcc.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xmz.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://otd.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kjz.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yun.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xqc.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tre.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vov.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eml.gzhubu.top

================================================================================
来源：http://fod.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://coj.pycfn.com

================================================================================
来源：http://htm.ppjwa.cn

[M01] 读取命令行参数
来源：http://jun.ppjwa.cn

Py:   sys.argv[1:]
来源：http://vng.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://ywu.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://cpr.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://rib.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://vqd.hnxiangtu.top

Go:   os.Args[1:]
来源：http://klf.vehdjk.com

Ruby: ARGV
来源：http://dgr.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://hiq.hnqzz.top

[M02] 读取环境变量
来源：http://nhy.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://jek.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xyy.yj20258888.top

JS:   process.env.HOME
来源：http://mww.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://bpb.ivvv.top

Java: System.getenv("HOME")
来源：http://hmk.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vgj.yonumen.top

Ruby: ENV["HOME"]
来源：http://kvj.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://irh.zhixingplan.top

[M03] 执行外部命令
来源：http://eqs.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tnw.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://liv.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qzj.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zwc.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://syl.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://cwb.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://oha.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://hkt.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://wur.guannengcc.top

Py:   os.getcwd()
来源：http://sfz.gogol.net.cn

PHP:  getcwd();
来源：http://uhe.hesvh.cn

JS:   process.cwd()
来源：http://gis.ydjk.org.cn

TS:   process.cwd()
来源：http://xjz.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://png.xziqi.cn

Go:   os.Getwd()
来源：http://jaj.sufxvd.cn

Ruby: Dir.pwd
来源：http://nfl.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://xsb.gaohongyu789.top

[M05] 设置退出码
来源：http://cbi.shzxlz.cn

Py:   sys.exit(1)
来源：http://ykx.sjlbkw.cn

PHP:  exit(1);
来源：http://pob.cdnleiting.top

JS:   process.exit(1)
来源：http://njy.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://crw.gotoacloud.top

Java: System.exit(1)
来源：http://amz.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://scg.cdnleiting.top

Ruby: exit 1
来源：http://onn.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cnh.jinqigfzy.top

[M06] 向标准错误输出
来源：http://csq.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://jmn.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zok.cheryme.top

JS:   console.error("err")
来源：http://cxs.fengsongda.top

TS:   console.error("err")
来源：http://qfa.havefunace.top

Java: System.err.println("err")
来源：http://jlf.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yfq.gaohongyu789.top

Ruby: warn "err"
来源：http://dqq.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://xnm.shuidangran.top

[M07] 判断是否为主入口
来源：http://myn.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://sjq.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rkk.ctjpmb.com

JS:   require.main === module
来源：http://ekt.vqdsnc.cn

TS:   require.main === module
来源：http://nha.yuanzhike.top

Java: public static void main(String[] args)
来源：http://zyv.meibo888.top

Go:   func main()
来源：http://nct.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kyo.fktsv.cn

C#:   static void Main(string[] args)
来源：http://shc.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://cok.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://wuc.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://usz.chenzaomai.com

JS:   process.platform;  process.version
来源：http://eqk.jqgfzy.top

TS:   process.platform;  process.version
来源：http://fsr.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cgu.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://giy.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mit.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wdt.ydzc1.top

================================================================================
来源：http://jho.cqqwz.cn

N. 数据结构与算法
来源：http://mhd.cdnleiting.top

================================================================================
来源：http://ylc.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://nuj.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://acz.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zdg.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sbj.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gqd.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://quf.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://nsh.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://arv.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rlk.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://jbl.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://aaj.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iyo.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bux.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dbz.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kht.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://icb.zhengqikj.top

Ruby: arr.sort
来源：http://hcj.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://typ.meibo888.top

[N03] 快速排序（分治示例）
来源：http://xfc.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://whu.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://mnu.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://usg.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ees.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fhf.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://whx.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ial.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ebd.gogol.net.cn

[N04] 斐波那契数列
来源：http://umz.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://djs.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vcc.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://loh.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shm.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uux.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mba.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qno.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vzu.hammf.cn

[N05] 最大公约数
来源：http://xgg.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://gzp.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rhd.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bis.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nkd.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xzi.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uob.guannengcc.top

Ruby: a.gcd(b)
来源：http://ekh.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pgw.zhixingplan.top

[N06] 判断回文字符串
来源：http://irf.fzhhl.top

Py:   s == s[::-1]
来源：http://byn.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://for.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://mum.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://vzt.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zac.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://xew.ctjpmb.com

Ruby: s == s.reverse
来源：http://plh.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://keu.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://lbc.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ups.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kci.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://mdf.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://rlp.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://hnk.hcnkem.com

Go:   // 手写 map[int]int
来源：http://tcc.epnwcf.com

Ruby: // 手写 Hash
来源：http://hwq.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://vqc.svipenyu.cn

[N08] 生成全排列
来源：http://qos.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://cpm.hcnkem.com

PHP:  // 手写递归交换
来源：http://kpo.pycfn.com

JS:   // 手写回溯递归
来源：http://rrj.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://njg.zhixingplan.top

Java: // 手写回溯递归
来源：http://nyk.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://qww.havefunace.top

Ruby: arr.permutation.to_a
来源：http://xwz.snrcjt.cn

C#:   // 手写回溯递归
来源：http://wyz.bbcook.cn

[N09] 栈与队列
来源：http://nwf.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fti.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jta.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yba.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cri.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://och.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qgg.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qav.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ack.xuanzx.com

[N10] 链表节点定义
来源：http://obg.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nup.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://knt.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lxg.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://akr.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://rnl.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://yxp.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kti.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ref.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://yyg.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gid.sweek.top

PHP:  // 手写递归函数
来源：http://hrs.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cbx.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ezb.andypj.xyz

Java: // 手写递归
来源：http://prz.ivvv.top

Go:   // 手写递归
来源：http://iqj.fktsv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fqo.pycfn.com

C#:   // 手写递归
来源：http://tgt.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aal.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tkp.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ksi.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gac.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ykv.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xsa.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cdl.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jov.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ylj.xuetiantiany.cn

================================================================================
来源：http://nxq.daxiang520.top

O. 并发与异步
来源：http://hlv.hammf.cn

================================================================================
来源：http://vzn.xuanzx.com

[O01] 启动一个线程
来源：http://pei.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mga.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jxc.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://upu.jianghu66.top

TS:   // 同 JS
来源：http://ylv.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://tsj.epnwcf.com

Go:   go f()
来源：http://wlr.xuanzx.com

Ruby: Thread.new { f }
来源：http://uoi.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://pim.haohaochexian.top

[O02] 使用线程池
来源：http://cds.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aez.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fav.52xcode.cn

JS:   // worker_threads 线程池
来源：http://hgl.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://ugc.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://chw.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ulk.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nbr.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pnr.xylfe.cn

[O03] 加锁保护共享数据
来源：http://lgl.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://oqg.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://xcn.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vxc.zycfv.cn

TS:   // 同 JS
来源：http://vzt.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://pgi.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vcs.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://umt.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://czy.xinyue.icu

[O04] 定义异步函数并等待
来源：http://zqf.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://fcu.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drs.ybcxt.top

JS:   async function f() { await g(); }
来源：http://gzu.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ipi.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://arr.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tiq.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://ydt.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://bel.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://bgt.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://mob.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://auh.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://kaw.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://wff.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iav.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kry.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://eet.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jwf.zdqjudy.top

[O06] 使用进程池
来源：http://oxr.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rjt.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rhw.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://mbo.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://abt.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vzk.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bko.epnwcf.com

Ruby: // fork 块
来源：http://cvh.jinqigfzy.top

C#:   Parallel.For
来源：http://mpw.wangshuangyany.cn

================================================================================
来源：http://jyr.hesvh.cn

P. 常用工具函数
来源：http://ylt.yj20258.top

================================================================================
来源：http://mkl.tanke756.top

[P01] 生成 UUID
来源：http://vgu.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://nos.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vxp.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://qcf.yonumen.top

TS:   crypto.randomUUID()
来源：http://hpy.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://xqz.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://crl.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://ngj.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://mha.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://xjv.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://upk.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://smq.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mbx.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hso.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://air.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tff.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dci.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vgi.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://hgx.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vuf.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lrd.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pho.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://esw.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://opx.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cqv.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://djk.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nqz.jyoumei.cn

[P04] 求长度
来源：http://wmc.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kvd.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zux.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dia.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xoy.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://pyb.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://zgx.iojbl.cn

Ruby: x.length;  x.size
来源：http://lse.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://paa.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://siu.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://emt.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bqw.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xdc.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vmn.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fri.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://meh.gogol.net.cn

Ruby: a == b
来源：http://ncm.9152youxi.cn


<!-- 参考信息 -->