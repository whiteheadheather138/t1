代发 wailian999

C#:   (int)resp.StatusCode
来源：http://zty.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://qqb.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oru.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://zjy.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nct.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bue.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ino.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pzr.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hrp.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sor.jlsjyb.cn

================================================================================
来源：http://kxh.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://awy.guannengcc.top

================================================================================
来源：http://krs.yanxiufei.cn

[M01] 读取命令行参数
来源：http://zzj.fehbvm.com

Py:   sys.argv[1:]
来源：http://iha.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://sav.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://qra.sweek.top

TS:   process.argv.slice(2)
来源：http://wmc.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://wtn.yvedp.cn

Go:   os.Args[1:]
来源：http://mnp.shanyushiyangkeji.top

Ruby: ARGV
来源：http://xrx.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://bjg.vehdjk.com

[M02] 读取环境变量
来源：http://gdu.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://bzb.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mat.uphjek.com

JS:   process.env.HOME
来源：http://tcj.jqgufenzy.top

TS:   process.env.HOME
来源：http://czr.cqqwz.cn

Java: System.getenv("HOME")
来源：http://hnk.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hmp.epnwcf.com

Ruby: ENV["HOME"]
来源：http://ard.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xeg.redwolf501.top

[M03] 执行外部命令
来源：http://agj.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mjn.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ntx.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jcj.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fqs.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hqh.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rhr.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ppb.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://jjh.hywenlv.cn

[M04] 获取当前工作目录
来源：http://vaw.gotoacloud.top

Py:   os.getcwd()
来源：http://rbs.vqdsnc.cn

PHP:  getcwd();
来源：http://cfx.yfazqb.com

JS:   process.cwd()
来源：http://gji.mhx1999.top

TS:   process.cwd()
来源：http://wjr.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://wpp.c1oappe.top

Go:   os.Getwd()
来源：http://nct.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://voy.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://lao.zdbjq.cn

[M05] 设置退出码
来源：http://kor.yfazqb.com

Py:   sys.exit(1)
来源：http://ase.yj202588.top

PHP:  exit(1);
来源：http://qvk.vqdsnc.cn

JS:   process.exit(1)
来源：http://xdl.52xcode.cn

TS:   process.exit(1)
来源：http://dlj.sweek.top

Java: System.exit(1)
来源：http://wvi.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://vhr.cqqwz.cn

Ruby: exit 1
来源：http://dkg.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dfy.jlsjyb.cn

[M06] 向标准错误输出
来源：http://pyq.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://hir.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ths.tanke756.top

JS:   console.error("err")
来源：http://zgg.cqqwz.cn

TS:   console.error("err")
来源：http://mwg.dashuyun.cn

Java: System.err.println("err")
来源：http://rms.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jtp.meibo888.top

Ruby: warn "err"
来源：http://kgu.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://reo.sxryk.cn

[M07] 判断是否为主入口
来源：http://fkd.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://wdj.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ifq.shzxlz.cn

JS:   require.main === module
来源：http://ofl.tianlin.xyz

TS:   require.main === module
来源：http://jne.epnwcf.com

Java: public static void main(String[] args)
来源：http://yzu.haohaochexian.top

Go:   func main()
来源：http://ehy.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zpv.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://cha.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://jzg.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://wuu.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://uzb.daxiang520.top

JS:   process.platform;  process.version
来源：http://zov.shzxlz.cn

TS:   process.platform;  process.version
来源：http://sko.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xty.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sji.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hrq.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ouj.vqdsnc.cn

================================================================================
来源：http://gtu.yfazqb.com

N. 数据结构与算法
来源：http://gaw.smart0.xyz

================================================================================
来源：http://kvp.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://thb.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://ugu.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://edh.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kil.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qfp.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gmb.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://qwe.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jtq.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://wur.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://teh.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://voj.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://chm.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lny.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gez.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fmz.sysykeji.top

Go:   slices.Sort(arr)
来源：http://vbu.smart0.xyz

Ruby: arr.sort
来源：http://mhp.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://umt.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://mjs.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://myc.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://bew.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdy.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://odf.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://awt.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://smt.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://isq.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://nkt.iojbl.cn

[N04] 斐波那契数列
来源：http://ahn.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xdl.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wtm.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kxz.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtt.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://brt.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sje.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jzg.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oux.aizwys.cn

[N05] 最大公约数
来源：http://mtu.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://vqx.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eyk.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bjg.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vsq.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zvj.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sab.jqgfzy.top

Ruby: a.gcd(b)
来源：http://kwe.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gof.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://ann.andypj.xyz

Py:   s == s[::-1]
来源：http://jer.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://ckn.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://uwc.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://ndd.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pif.tarul.cn

Go:   // 双指针从两端比较
来源：http://uah.tanke756.top

Ruby: s == s.reverse
来源：http://pal.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://bfx.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://aud.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wld.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tzx.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hoj.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://bqs.dianchejie.cn

Java: // 手写 HashMap
来源：http://arx.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://yuw.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://sll.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://cdi.yj20258888.top

[N08] 生成全排列
来源：http://tmw.hammf.cn

Py:   itertools.permutations(arr)
来源：http://qpf.vehdjk.com

PHP:  // 手写递归交换
来源：http://okj.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://zen.guannengcc.top

TS:   // 手写回溯递归
来源：http://jet.hesvh.cn

Java: // 手写回溯递归
来源：http://hcs.hesvh.cn

Go:   // 手写回溯递归
来源：http://gja.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://kek.cqqwz.cn

C#:   // 手写回溯递归
来源：http://bqv.chenlongwang.top

[N09] 栈与队列
来源：http://lpk.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yxb.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qwu.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sss.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ojo.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yrk.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nio.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ylc.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ldu.yanxiufei.cn

[N10] 链表节点定义
来源：http://kpl.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ifw.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eaz.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dso.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kvs.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://ozn.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://aar.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mew.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ojb.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://sbo.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sja.nanxinkj.top

PHP:  // 手写递归函数
来源：http://tff.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bfi.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jna.gotoacloud.top

Java: // 手写递归
来源：http://eqz.0kj1m.cn

Go:   // 手写递归
来源：http://lis.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dpq.nwbrower.top

C#:   // 手写递归
来源：http://lrb.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rfu.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qce.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://htm.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejp.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kis.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eyb.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bkq.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tpu.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qgc.c1oappe.top

================================================================================
来源：http://ioc.jiagoushi.top

O. 并发与异步
来源：http://lze.xingfuxueyuan.xyz

================================================================================
来源：http://xvi.sufxvd.cn

[O01] 启动一个线程
来源：http://pup.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bfc.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ybt.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jyb.feifeiyinyue.top

TS:   // 同 JS
来源：http://zwo.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://qfp.epnwcf.com

Go:   go f()
来源：http://now.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://vft.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://ejh.shzxlz.cn

[O02] 使用线程池
来源：http://rle.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gyt.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://psp.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://hzn.ivvv.top

TS:   // worker_threads 线程池
来源：http://juc.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lmt.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oie.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mbl.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bmx.tarul.cn

[O03] 加锁保护共享数据
来源：http://ddu.uphjek.com

Py:   with lock: shared += 1
来源：http://lnr.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://jqf.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zmt.meibo888.top

TS:   // 同 JS
来源：http://djt.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://hgt.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ykq.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xiu.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://huz.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://zgp.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://lvn.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xjh.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://kaz.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xqs.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://axu.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jgd.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://dzo.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://rrt.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://zng.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://dlq.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fss.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://vac.ivvv.top

TS:   await Promise.all(tasks)
来源：http://zaa.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vqp.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kdp.hcnkem.com

Ruby: threads.map(&:join)
来源：http://ltm.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ifp.pengpengdd.cyou

[O06] 使用进程池
来源：http://nbe.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tdt.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jtb.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://pbe.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://siq.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xcc.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qlb.guannengcc.top

Ruby: // fork 块
来源：http://ogb.316326.xyz

C#:   Parallel.For
来源：http://mgn.andypj.xyz

================================================================================
来源：http://dll.zhixingplan.top

P. 常用工具函数
来源：http://jsg.ywan-chungtsiang.top

================================================================================
来源：http://iog.xziqi.cn

[P01] 生成 UUID
来源：http://ibb.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://wxh.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lji.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://lyk.sysykeji.top

TS:   crypto.randomUUID()
来源：http://ufe.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://lfn.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://tou.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://elp.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://lls.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://ocn.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eta.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nke.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bxd.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fpr.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lgr.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xwj.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://thy.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qmm.zycfv.cn

[P03] 生成短随机字符串
来源：http://beh.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ilf.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nhd.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhp.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwm.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://brs.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ara.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ywb.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://duv.jinqigfzy.top

[P04] 求长度
来源：http://srz.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mbh.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://saf.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jpl.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jan.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://lhh.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://ngm.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://niu.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lef.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://nrh.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xjy.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mex.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rcg.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://efq.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dvd.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://dve.fengsongda.top

Ruby: a == b
来源：http://cue.c1oappe.top


<!-- 参考信息 -->