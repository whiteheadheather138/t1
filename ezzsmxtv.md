代发 wailian999

TS:   resp.ok;  resp.status
来源：http://ixt.nanxuanxn.top

Java: resp.statusCode()
来源：http://nst.jianghu66.top

Go:   resp.StatusCode
来源：http://xkc.shzxlz.cn

Ruby: resp.code.to_i
来源：http://vrq.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://hwn.nanxinkj.top

[L08] 并发请求多个地址
来源：http://cer.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kbx.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://qgg.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdv.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gih.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lqh.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kzp.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rxu.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rir.tarul.cn

================================================================================
来源：http://tzk.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://zei.meibo888.top

================================================================================
来源：http://vgu.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://agb.haohaochexian.top

Py:   sys.argv[1:]
来源：http://txx.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://rne.fehbvm.com

JS:   process.argv.slice(2)
来源：http://dvh.fehbvm.com

TS:   process.argv.slice(2)
来源：http://nav.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://gcw.dianchejie.cn

Go:   os.Args[1:]
来源：http://pmh.fktsv.cn

Ruby: ARGV
来源：http://qug.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://kwb.yj20258888.top

[M02] 读取环境变量
来源：http://tev.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://oxx.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hpt.gotoacloud.top

JS:   process.env.HOME
来源：http://iys.xuanzx.com

TS:   process.env.HOME
来源：http://kip.shzxlz.cn

Java: System.getenv("HOME")
来源：http://uzx.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bjr.fengsongda.top

Ruby: ENV["HOME"]
来源：http://fah.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ykj.nwbrower.top

[M03] 执行外部命令
来源：http://etb.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bpu.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bnw.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vvg.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://myh.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tiy.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sxn.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fno.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://zls.pycfn.com

[M04] 获取当前工作目录
来源：http://mgy.zhengqikj.top

Py:   os.getcwd()
来源：http://cuk.ppjwa.cn

PHP:  getcwd();
来源：http://jfk.redwolf501.top

JS:   process.cwd()
来源：http://zld.hywenlv.cn

TS:   process.cwd()
来源：http://rni.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://iaz.birdmap.top

Go:   os.Getwd()
来源：http://dwx.yj20258.top

Ruby: Dir.pwd
来源：http://bxc.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://nuc.epnwcf.com

[M05] 设置退出码
来源：http://jui.yj20258.top

Py:   sys.exit(1)
来源：http://wvx.ydjk.org.cn

PHP:  exit(1);
来源：http://hkx.sweek.top

JS:   process.exit(1)
来源：http://upa.kuanghao11.cn

TS:   process.exit(1)
来源：http://trs.redwolf501.top

Java: System.exit(1)
来源：http://czk.xylfe.cn

Go:   os.Exit(1)
来源：http://osf.yj202588.top

Ruby: exit 1
来源：http://pnw.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fkr.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://mqh.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://ecy.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://znz.nanxuanxn.top

JS:   console.error("err")
来源：http://bfr.feifeiyinyue.top

TS:   console.error("err")
来源：http://qtr.yangfankeji.com

Java: System.err.println("err")
来源：http://pqk.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oso.gzhubu.top

Ruby: warn "err"
来源：http://krq.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://gkn.ctjpmb.com

[M07] 判断是否为主入口
来源：http://owu.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://zas.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://imv.jiagoushi.top

JS:   require.main === module
来源：http://fwh.zhengqikj.top

TS:   require.main === module
来源：http://jio.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://lys.chenzaomai.com

Go:   func main()
来源：http://vaa.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pmn.yueranfly.top

C#:   static void Main(string[] args)
来源：http://vvw.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://izu.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://kgt.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://bes.sweek.top

JS:   process.platform;  process.version
来源：http://eqc.zdqjudy.top

TS:   process.platform;  process.version
来源：http://hiw.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pze.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qbp.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ojc.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ykx.chenjidiqi.icu

================================================================================
来源：http://snb.hcnkem.com

N. 数据结构与算法
来源：http://xrx.cqqwz.cn

================================================================================
来源：http://dja.meibo888.top

[N01] 二分查找（有序数组）
来源：http://aoq.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://zuj.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gxg.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jbo.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://que.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://fvr.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://vzz.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykk.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ppu.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://yer.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://ult.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mux.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pia.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bau.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zro.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://jhh.sufxvd.cn

Ruby: arr.sort
来源：http://lfl.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vsc.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://hfl.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kac.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://odx.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://egh.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ktz.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tvx.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bqp.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vng.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://sff.fzhhl.top

[N04] 斐波那契数列
来源：http://ifv.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sxx.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ezn.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://amx.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nil.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bww.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uif.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hgp.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbv.yj20258.top

[N05] 最大公约数
来源：http://ryv.yj202588.top

Py:   math.gcd(a, b)
来源：http://fix.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wnm.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://utr.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://grm.zhixingplan.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lxi.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pit.mhx1999.top

Ruby: a.gcd(b)
来源：http://ymh.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oei.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://uuy.bjfxy.top

Py:   s == s[::-1]
来源：http://zfw.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://qqb.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://hyo.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://ewi.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zjh.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://wwv.cashguo.top

Ruby: s == s.reverse
来源：http://pgf.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wyy.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://ofg.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nzi.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xyw.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bcb.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://zmf.zhongyouzk.top

Java: // 手写 HashMap
来源：http://fzu.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://shh.epnwcf.com

Ruby: // 手写 Hash
来源：http://sev.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://gkb.jlsjyb.cn

[N08] 生成全排列
来源：http://bug.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://ysd.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://pmi.zdqjudy.top

JS:   // 手写回溯递归
来源：http://akp.c1oappe.top

TS:   // 手写回溯递归
来源：http://sgl.aizwys.cn

Java: // 手写回溯递归
来源：http://zsd.tianlin.xyz

Go:   // 手写回溯递归
来源：http://igq.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://hop.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://rrg.smart0.xyz

[N09] 栈与队列
来源：http://zda.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sgt.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oxf.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pow.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pgu.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hzn.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aee.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kmc.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ajx.mhx1999.top

[N10] 链表节点定义
来源：http://imh.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dsq.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cdh.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hfh.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kmf.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://vuj.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://hma.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://one.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bkr.daria6918.cn

[N11] 二叉树中序遍历
来源：http://skz.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cgi.vehdjk.com

PHP:  // 手写递归函数
来源：http://agv.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dbt.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjh.cheryme.top

Java: // 手写递归
来源：http://yjr.zhengqikj.top

Go:   // 手写递归
来源：http://xiw.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kyx.ydjk.org.cn

C#:   // 手写递归
来源：http://nla.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xuu.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jgd.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://knj.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pmw.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbx.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dnh.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ato.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nfj.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hyf.zdqjudy.top

================================================================================
来源：http://qfu.tarul.cn

O. 并发与异步
来源：http://cyt.pengpengdd.cyou

================================================================================
来源：http://jio.ivvv.top

[O01] 启动一个线程
来源：http://aoz.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tys.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vhu.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ucy.zdqjudy.top

TS:   // 同 JS
来源：http://cwo.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://fed.yfazqb.com

Go:   go f()
来源：http://kjw.gotoacloud.top

Ruby: Thread.new { f }
来源：http://qly.jianghu66.top

C#:   Task.Run(() => F());
来源：http://isj.jianghu66.top

[O02] 使用线程池
来源：http://wrq.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tsr.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sib.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://lbz.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://noe.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://pcj.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ksr.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uob.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ywu.tanke756.top

[O03] 加锁保护共享数据
来源：http://ffj.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://tcq.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cuj.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zjl.yongpay.top

TS:   // 同 JS
来源：http://zcc.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://ngy.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iul.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rcq.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://bwn.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://udq.hammf.cn

Py:   async def f():⏎    await g()
来源：http://ctc.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ozj.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://mrk.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://jvj.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ysf.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nhw.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gjc.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://zeg.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://vbl.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://zye.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://emx.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://ufh.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://rji.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vpg.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ffe.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://iws.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cjt.dashuyun.cn

[O06] 使用进程池
来源：http://yev.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kyd.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://yzz.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://tyr.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://izs.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zma.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ghb.ehwqpu.com

Ruby: // fork 块
来源：http://nbk.smart0.xyz

C#:   Parallel.For
来源：http://jdy.chenzaomai.com

================================================================================
来源：http://drk.yuanzhike.top

P. 常用工具函数
来源：http://jsh.fzhhl.top

================================================================================
来源：http://inq.svipenyu.cn

[P01] 生成 UUID
来源：http://ilu.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://qiv.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gvs.tian-w.cn

JS:   crypto.randomUUID()
来源：http://ckx.c1oappe.top

TS:   crypto.randomUUID()
来源：http://yoi.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://tum.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://wft.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://zmy.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://jgp.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://gur.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dmw.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dnw.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://etv.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yck.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cpa.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mwg.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eop.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fev.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://kxa.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://scg.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rvo.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxb.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsi.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aud.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jwr.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mlo.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ehz.uphjek.com

[P04] 求长度
来源：http://alb.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lef.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fqu.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xmx.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwj.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://abi.shuidangran.top

Go:   len(arr);  len(m)
来源：http://zvi.jinqigufen.top

Ruby: x.length;  x.size
来源：http://pzq.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ywl.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://kpe.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fbg.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://thq.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nky.xziqi.cn


<!-- 参考信息 -->