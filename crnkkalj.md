代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rnh.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hsd.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rtn.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dts.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rup.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cev.jinyuanbaomall.cn

================================================================================
来源：http://abf.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://taz.fehbvm.com

================================================================================
来源：http://czs.daxiang520.top

[M01] 读取命令行参数
来源：http://pmu.aizwys.cn

Py:   sys.argv[1:]
来源：http://zse.sxryk.cn

PHP:  $argv;  $argc;
来源：http://bgc.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://oxa.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://tba.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://unw.dashuyun.cn

Go:   os.Args[1:]
来源：http://ioe.chenlongwang.top

Ruby: ARGV
来源：http://atz.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://wjh.aibaodan.cn

[M02] 读取环境变量
来源：http://pfi.316326.xyz

Py:   os.environ.get("HOME")
来源：http://stq.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dbs.jlsjyb.cn

JS:   process.env.HOME
来源：http://kls.yuxming.cn

TS:   process.env.HOME
来源：http://ihm.redwolf501.top

Java: System.getenv("HOME")
来源：http://kve.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tzj.redwolf501.top

Ruby: ENV["HOME"]
来源：http://bxf.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zts.shzxlz.cn

[M03] 执行外部命令
来源：http://uxw.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kwd.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tvk.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vxc.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://pbx.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fvu.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://svo.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://otf.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://oqg.zycfv.cn

[M04] 获取当前工作目录
来源：http://ktn.zhongyouzk.top

Py:   os.getcwd()
来源：http://jxm.jlsjyb.cn

PHP:  getcwd();
来源：http://ije.hysaishi.cn

JS:   process.cwd()
来源：http://eod.yj202588.top

TS:   process.cwd()
来源：http://fpu.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://rjb.ppjwa.cn

Go:   os.Getwd()
来源：http://ipl.yangfankeji.com

Ruby: Dir.pwd
来源：http://gtf.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sgx.9152youxi.cn

[M05] 设置退出码
来源：http://vxq.tian-w.cn

Py:   sys.exit(1)
来源：http://ini.daria6918.cn

PHP:  exit(1);
来源：http://mid.hnqzz.top

JS:   process.exit(1)
来源：http://vke.52xcode.cn

TS:   process.exit(1)
来源：http://tfb.hcnkem.com

Java: System.exit(1)
来源：http://eit.bjfxy.top

Go:   os.Exit(1)
来源：http://asw.tarul.cn

Ruby: exit 1
来源：http://dhf.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ciw.cheryme.top

[M06] 向标准错误输出
来源：http://sss.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://efz.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cmt.xuanzx.com

JS:   console.error("err")
来源：http://fqm.aibaodan.cn

TS:   console.error("err")
来源：http://jfi.ppjwa.cn

Java: System.err.println("err")
来源：http://txs.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uzs.meibo888.top

Ruby: warn "err"
来源：http://ujw.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://nfw.dianchejie.cn

[M07] 判断是否为主入口
来源：http://jby.yonumen.top

Py:   if __name__ == "__main__":
来源：http://dfg.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fed.iojbl.cn

JS:   require.main === module
来源：http://bjy.316326.xyz

TS:   require.main === module
来源：http://tzf.yj20258888.top

Java: public static void main(String[] args)
来源：http://jpl.aizwys.cn

Go:   func main()
来源：http://rsg.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kxs.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://nyf.meibo888.top

[M08] 获取系统与运行时信息
来源：http://tce.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://mad.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://ojt.yfazqb.com

JS:   process.platform;  process.version
来源：http://xpm.gzhubu.top

TS:   process.platform;  process.version
来源：http://zoq.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qke.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://thx.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://smp.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rjc.shangyingyoupin.top

================================================================================
来源：http://iby.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://nbc.kuanghao11.cn

================================================================================
来源：http://wnu.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://vnq.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://uxg.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mzi.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cjh.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ldx.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://wbu.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://wbv.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mhz.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://iqa.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://vbl.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://zks.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tih.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qik.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gfk.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dvd.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://lrr.smart0.xyz

Ruby: arr.sort
来源：http://rcs.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://wqr.sweek.top

[N03] 快速排序（分治示例）
来源：http://rzl.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://voh.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://txw.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tqw.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yee.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://irq.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rqp.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyo.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://vug.cqqwz.cn

[N04] 斐波那契数列
来源：http://set.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aud.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rmp.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zhb.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nmf.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qbz.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bem.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kvn.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kbk.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://sjm.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://dlo.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://loh.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zoo.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cku.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ipb.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dbl.yongpay.top

Ruby: a.gcd(b)
来源：http://hph.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tzp.hammf.cn

[N06] 判断回文字符串
来源：http://lms.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://jfj.wangdashe.top

PHP:  $s === strrev($s);
来源：http://srp.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://hus.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://viu.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://szi.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://zis.hammf.cn

Ruby: s == s.reverse
来源：http://qdt.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jun.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://dtp.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gcb.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kkn.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lgl.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://gyx.dianchejie.cn

Java: // 手写 HashMap
来源：http://wco.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://tng.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://zys.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://xah.cucudq.cn

[N08] 生成全排列
来源：http://mns.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://ptj.snrcjt.cn

PHP:  // 手写递归交换
来源：http://qfu.tarul.cn

JS:   // 手写回溯递归
来源：http://apg.smart0.xyz

TS:   // 手写回溯递归
来源：http://gbv.havefunace.top

Java: // 手写回溯递归
来源：http://iba.bbcook.cn

Go:   // 手写回溯递归
来源：http://ocz.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://ssr.zhengqikj.top

C#:   // 手写回溯递归
来源：http://vss.mhx1999.top

[N09] 栈与队列
来源：http://lyr.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hpe.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ooe.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ixp.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zda.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mdf.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sha.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bqu.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pdn.9152youxi.cn

[N10] 链表节点定义
来源：http://zfg.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yjn.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wdb.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://irh.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jzx.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://jmg.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://ncg.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xpo.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://etl.ppjwa.cn

[N11] 二叉树中序遍历
来源：http://ucm.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://esh.birdmap.top

PHP:  // 手写递归函数
来源：http://ahl.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbo.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rsi.hywenlv.cn

Java: // 手写递归
来源：http://cbr.hnxiangtu.top

Go:   // 手写递归
来源：http://eqe.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ori.sxryk.cn

C#:   // 手写递归
来源：http://svk.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uhx.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dnc.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lee.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fcm.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qlu.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ojx.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ajq.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rhd.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bad.gogol.net.cn

================================================================================
来源：http://yss.sysykeji.top

O. 并发与异步
来源：http://kvq.snrcjt.cn

================================================================================
来源：http://drw.gogol.net.cn

[O01] 启动一个线程
来源：http://otn.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ytk.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hth.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uca.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://ogq.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://vgp.jqgufenzy.top

Go:   go f()
来源：http://lpi.andypj.xyz

Ruby: Thread.new { f }
来源：http://rax.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://yli.dianchejie.cn

[O02] 使用线程池
来源：http://rfc.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://evt.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hle.ydzc1.top

JS:   // worker_threads 线程池
来源：http://skj.hcnkem.com

TS:   // worker_threads 线程池
来源：http://elf.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://usv.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wjb.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yks.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ccl.shuidangran.top

[O03] 加锁保护共享数据
来源：http://gzj.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://frl.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://wsj.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rjr.zhijiandao.cn

TS:   // 同 JS
来源：http://gfy.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://nhv.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbn.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mvx.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://qis.sysykeji.top

[O04] 定义异步函数并等待
来源：http://zzz.birdmap.top

Py:   async def f():⏎    await g()
来源：http://qfj.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gxt.yongpay.top

JS:   async function f() { await g(); }
来源：http://yyu.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nkh.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vnn.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dmu.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://qda.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://rhe.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://hut.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://maw.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cqf.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://mtp.tanke756.top

TS:   await Promise.all(tasks)
来源：http://znw.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yfp.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pmi.yuxming.cn

Ruby: threads.map(&:join)
来源：http://ryf.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xbi.aibaodan.cn

[O06] 使用进程池
来源：http://nez.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jnf.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pmj.cashguo.top

JS:   // child_process / cluster 模块
来源：http://lpm.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://vay.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://syn.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fdr.yj202588.top

Ruby: // fork 块
来源：http://mzp.0kj1m.cn

C#:   Parallel.For
来源：http://qgg.tarul.cn

================================================================================
来源：http://fvh.kuanghao11.cn

P. 常用工具函数
来源：http://wqb.jlsjyb.cn

================================================================================
来源：http://vkg.fengsongda.top

[P01] 生成 UUID
来源：http://xbk.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://wlw.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bfy.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://mkp.bbcook.cn

TS:   crypto.randomUUID()
来源：http://ifn.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://hvl.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://ikv.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://nnk.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://cco.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://ixb.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dsf.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cva.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rdj.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fwg.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ozv.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://esy.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://alj.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://txn.ppjwa.cn

[P03] 生成短随机字符串
来源：http://vzd.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yms.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vul.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://seo.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qvh.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://apd.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nwq.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pyt.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://erd.guannengcc.top

[P04] 求长度
来源：http://ijz.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kas.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ziq.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://orm.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uce.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://pqr.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://vxq.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://mnj.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://byq.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://zog.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iqa.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sqi.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bqf.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vgu.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://amx.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iqf.cashguo.top

Ruby: a == b
来源：http://aju.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pmo.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://daa.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ulb.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://udo.fengsongda.top


<!-- 参考信息 -->