代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmg.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rss.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vkb.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wvm.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mwh.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bsk.zhoulong.xyz

================================================================================
来源：http://cdw.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://xbm.vehdjk.com

================================================================================
来源：http://jwr.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://tlu.xziqi.cn

Py:   sys.argv[1:]
来源：http://dwq.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://oul.ydzc1.top

JS:   process.argv.slice(2)
来源：http://fet.fktsv.cn

TS:   process.argv.slice(2)
来源：http://zre.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://guk.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://kyq.guowangkeji.top

Ruby: ARGV
来源：http://ltd.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://jns.yfazqb.com

[M02] 读取环境变量
来源：http://hpb.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://ldk.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rpj.zhongyouzk.top

JS:   process.env.HOME
来源：http://noa.chenzaomai.com

TS:   process.env.HOME
来源：http://duq.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://vym.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qqs.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://mag.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sfb.havefunace.top

[M03] 执行外部命令
来源：http://zuo.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dfs.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ufb.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://xbw.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wad.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ihx.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tsz.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://vpb.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://wve.hywenlv.cn

[M04] 获取当前工作目录
来源：http://eyv.guowangkeji.top

Py:   os.getcwd()
来源：http://eka.zycfv.cn

PHP:  getcwd();
来源：http://yof.snrcjt.cn

JS:   process.cwd()
来源：http://zco.gaohongyu789.top

TS:   process.cwd()
来源：http://gfe.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://zww.fktsv.cn

Go:   os.Getwd()
来源：http://ejs.cheryme.top

Ruby: Dir.pwd
来源：http://era.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mob.xuetiantiany.cn

[M05] 设置退出码
来源：http://qrs.yongpay.top

Py:   sys.exit(1)
来源：http://dyd.jyoumei.cn

PHP:  exit(1);
来源：http://tyh.pengpengdd.cyou

JS:   process.exit(1)
来源：http://mgo.ydzc1.top

TS:   process.exit(1)
来源：http://brp.meibo888.top

Java: System.exit(1)
来源：http://gln.fzhhl.top

Go:   os.Exit(1)
来源：http://vga.zhijiandao.cn

Ruby: exit 1
来源：http://tcb.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cqm.pycfn.com

[M06] 向标准错误输出
来源：http://nui.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://bgb.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://oyi.svipenyu.cn

JS:   console.error("err")
来源：http://msw.vehdjk.com

TS:   console.error("err")
来源：http://iam.wangshuangyany.cn

Java: System.err.println("err")
来源：http://gaf.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ruw.ydzc1.top

Ruby: warn "err"
来源：http://ckf.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://xcv.sxryk.cn

[M07] 判断是否为主入口
来源：http://awl.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://egm.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iab.dashuyun.cn

JS:   require.main === module
来源：http://dty.zdbjq.cn

TS:   require.main === module
来源：http://tlz.0kj1m.cn

Java: public static void main(String[] args)
来源：http://dqc.snrcjt.cn

Go:   func main()
来源：http://yug.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nqz.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://dzm.tarul.cn

[M08] 获取系统与运行时信息
来源：http://izs.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://qsn.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://wdh.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://akm.nwbrower.top

TS:   process.platform;  process.version
来源：http://clx.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wma.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yps.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ktv.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ieh.dashuyun.cn

================================================================================
来源：http://jrn.aizwys.cn

N. 数据结构与算法
来源：http://hon.hywenlv.cn

================================================================================
来源：http://dhj.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://olx.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://lqo.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://exi.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jnx.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gxp.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://wvp.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://zth.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rcx.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://xwz.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://nhd.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://viy.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hqp.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ppv.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dso.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rwc.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://pxb.andypj.xyz

Ruby: arr.sort
来源：http://dhm.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nnj.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://rmy.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qmd.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://yfr.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hil.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbw.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ajy.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aah.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rlp.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://tiv.cqqwz.cn

[N04] 斐波那契数列
来源：http://vej.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pnk.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xuv.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pkm.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpm.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://clg.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sgr.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ayf.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bmo.xylfe.cn

[N05] 最大公约数
来源：http://pfk.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://pyu.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://isy.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://waz.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixv.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hat.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://whb.xinyue.icu

Ruby: a.gcd(b)
来源：http://ych.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gks.fzhhl.top

[N06] 判断回文字符串
来源：http://txv.fktsv.cn

Py:   s == s[::-1]
来源：http://hzp.yj20258888.top

PHP:  $s === strrev($s);
来源：http://lvp.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://tuy.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://fwk.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://phb.xylfe.cn

Go:   // 双指针从两端比较
来源：http://dgn.zycfv.cn

Ruby: s == s.reverse
来源：http://fus.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jiu.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://czx.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://haq.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pbj.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lwm.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://zia.ydzc1.top

Java: // 手写 HashMap
来源：http://vng.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://zkr.sysykeji.top

Ruby: // 手写 Hash
来源：http://iyr.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://rma.daria6918.cn

[N08] 生成全排列
来源：http://lyy.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://jfo.tanke756.top

PHP:  // 手写递归交换
来源：http://hqh.cdnleiting.top

JS:   // 手写回溯递归
来源：http://nmh.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://eop.52xcode.cn

Java: // 手写回溯递归
来源：http://kpm.ybcxt.top

Go:   // 手写回溯递归
来源：http://byw.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://trn.zycfv.cn

C#:   // 手写回溯递归
来源：http://uuy.daria6918.cn

[N09] 栈与队列
来源：http://sbx.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ktk.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hms.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://srv.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bmv.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gcz.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yva.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zwn.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fze.bbcook.cn

[N10] 链表节点定义
来源：http://flv.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ras.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hrp.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eax.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ien.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://itn.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://kpz.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sjs.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iat.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://bym.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://irk.guannengcc.top

PHP:  // 手写递归函数
来源：http://eqp.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lil.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqu.hnqzz.top

Java: // 手写递归
来源：http://xli.xuetiantiany.cn

Go:   // 手写递归
来源：http://lqd.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fll.c1oappe.top

C#:   // 手写递归
来源：http://vte.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mda.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bdx.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pay.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wrt.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lhy.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nbs.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://plv.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fyu.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qxa.yj20258.top

================================================================================
来源：http://ksq.xuanzx.com

O. 并发与异步
来源：http://quo.birdmap.top

================================================================================
来源：http://xwp.zhoulong.xyz

[O01] 启动一个线程
来源：http://cek.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bkm.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oqk.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mne.9152youxi.cn

TS:   // 同 JS
来源：http://ysl.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://zrr.ppjwa.cn

Go:   go f()
来源：http://cer.iojbl.cn

Ruby: Thread.new { f }
来源：http://jno.yvedp.cn

C#:   Task.Run(() => F());
来源：http://tuq.0kj1m.cn

[O02] 使用线程池
来源：http://osu.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://efe.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ffe.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://ryw.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://qvv.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://hze.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rne.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iro.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fto.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://def.svipenyu.cn

Py:   with lock: shared += 1
来源：http://zbc.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://vvk.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qlf.jlsjyb.cn

TS:   // 同 JS
来源：http://sgh.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://jco.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wxp.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qys.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://dsn.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://qng.meibo888.top

Py:   async def f():⏎    await g()
来源：http://lxc.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ien.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://mjp.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jty.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebt.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kqg.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://vji.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://sek.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://ijj.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://sfb.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://btk.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://sen.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://tzf.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mck.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://szr.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://vnl.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qxh.c1oappe.top

[O06] 使用进程池
来源：http://tkz.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bmj.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tpm.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://wmg.meibo888.top

TS:   // child_process / cluster 模块
来源：http://jfh.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cvg.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eff.nanxinkj.top

Ruby: // fork 块
来源：http://let.yonumen.top

C#:   Parallel.For
来源：http://bcs.chenzaomai.com

================================================================================
来源：http://wti.jlsjyb.cn

P. 常用工具函数
来源：http://syi.jyoumei.cn

================================================================================
来源：http://mzu.daxiang520.top

[P01] 生成 UUID
来源：http://dne.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://kuj.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eip.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://izi.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://enc.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://zoq.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://oho.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://nux.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://jmu.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://jrq.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://glb.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iht.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ptg.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ist.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tci.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sse.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tcl.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tah.yfazqb.com

[P03] 生成短随机字符串
来源：http://dfd.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rou.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://giq.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pbj.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ikb.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wyj.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uck.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://kkk.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sub.hesvh.cn

[P04] 求长度
来源：http://omk.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vzi.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://irs.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bjx.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jyp.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://asv.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://wjl.sufxvd.cn

Ruby: x.length;  x.size
来源：http://nsq.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qss.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://pyg.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://igd.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rmk.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dby.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fxk.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iqa.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rgw.chenzaomai.com

Ruby: a == b
来源：http://xzh.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aae.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zlx.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vbo.316326.xyz

PHP:  if (empty($x)) {}
来源：http://dgb.birdmap.top


<!-- 参考信息 -->