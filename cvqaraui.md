代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yor.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rnq.cashguo.top

================================================================================
来源：http://gmb.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://ris.shuidangran.top

================================================================================
来源：http://kda.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://sof.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://iwn.smart0.xyz

PHP:  $argv;  $argc;
来源：http://inf.xziqi.cn

JS:   process.argv.slice(2)
来源：http://wgj.yj20258888.top

TS:   process.argv.slice(2)
来源：http://mjq.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://egh.aibaodan.cn

Go:   os.Args[1:]
来源：http://pkh.zhoulong.xyz

Ruby: ARGV
来源：http://lje.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://yex.gotoacloud.top

[M02] 读取环境变量
来源：http://rjy.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://cuw.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://imq.tarul.cn

JS:   process.env.HOME
来源：http://odf.chenlongwang.top

TS:   process.env.HOME
来源：http://vii.chenzaomai.com

Java: System.getenv("HOME")
来源：http://zgr.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lze.yonumen.top

Ruby: ENV["HOME"]
来源：http://awl.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cfi.nanxinkj.top

[M03] 执行外部命令
来源：http://kov.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tnc.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oho.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cxa.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://iip.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hek.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://gtb.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xnh.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://hmw.gogol.net.cn

[M04] 获取当前工作目录
来源：http://etj.yanxiufei.cn

Py:   os.getcwd()
来源：http://dsw.chenjidiqi.icu

PHP:  getcwd();
来源：http://oav.tian-w.cn

JS:   process.cwd()
来源：http://cnx.xziqi.cn

TS:   process.cwd()
来源：http://zbc.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://vac.jqgfzy.top

Go:   os.Getwd()
来源：http://ofs.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://abl.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://rnd.andypj.xyz

[M05] 设置退出码
来源：http://itb.wangdashe.top

Py:   sys.exit(1)
来源：http://kdh.hcnkem.com

PHP:  exit(1);
来源：http://ajz.gogol.net.cn

JS:   process.exit(1)
来源：http://wxu.quarkkingdee.top

TS:   process.exit(1)
来源：http://xur.chenjidiqi.icu

Java: System.exit(1)
来源：http://wpk.pycfn.com

Go:   os.Exit(1)
来源：http://odn.ywan-chungtsiang.top

Ruby: exit 1
来源：http://wra.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uyj.jyoumei.cn

[M06] 向标准错误输出
来源：http://bam.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://slp.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ltz.tanke756.top

JS:   console.error("err")
来源：http://hch.svipenyu.cn

TS:   console.error("err")
来源：http://dhk.cashguo.top

Java: System.err.println("err")
来源：http://jyp.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cfx.pycfn.com

Ruby: warn "err"
来源：http://swz.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ski.zycfv.cn

[M07] 判断是否为主入口
来源：http://dwj.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://iez.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://efk.yj20258.top

JS:   require.main === module
来源：http://iom.jinqigfzy.top

TS:   require.main === module
来源：http://epr.nwbrower.top

Java: public static void main(String[] args)
来源：http://drz.yvedp.cn

Go:   func main()
来源：http://mid.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qef.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://sai.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://uyv.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://txz.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://ozk.tianlin.xyz

JS:   process.platform;  process.version
来源：http://tcv.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://hio.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nxq.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cvi.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvq.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://leq.tarul.cn

================================================================================
来源：http://ini.xziqi.cn

N. 数据结构与算法
来源：http://kih.hongshengwenyu.top

================================================================================
来源：http://pkq.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://dqr.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://lad.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bfg.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wnd.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgn.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://vqp.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://kka.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cfh.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://qof.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://nus.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://dbo.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wov.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rpo.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://slj.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://skg.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://kxw.yvedp.cn

Ruby: arr.sort
来源：http://zjt.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gsw.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://ooh.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://akp.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://rli.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fsz.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abp.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ojy.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qpp.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ubx.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://xie.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://kwr.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iuv.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gkq.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bls.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tox.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kto.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qls.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ztj.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wok.fanxiaobao.xyz

[N05] 最大公约数
来源：http://nmx.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://rhn.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lei.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eci.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vbp.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://brt.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brd.yj202588.top

Ruby: a.gcd(b)
来源：http://zfq.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sat.gotoacloud.top

[N06] 判断回文字符串
来源：http://yeq.svipenyu.cn

Py:   s == s[::-1]
来源：http://gro.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://yer.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://ubk.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://mom.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wgt.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://okr.yonumen.top

Ruby: s == s.reverse
来源：http://mxc.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vpg.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://rau.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://obt.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xjb.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zmj.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://gdv.52xcode.cn

Java: // 手写 HashMap
来源：http://xqz.yj20258888.top

Go:   // 手写 map[int]int
来源：http://lue.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://slk.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mei.yj202588.top

[N08] 生成全排列
来源：http://cim.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://ozf.hfpthk.cn

PHP:  // 手写递归交换
来源：http://xrb.dashuyun.cn

JS:   // 手写回溯递归
来源：http://vjf.cqqwz.cn

TS:   // 手写回溯递归
来源：http://tis.gogol.net.cn

Java: // 手写回溯递归
来源：http://pup.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://qej.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://bpr.iojbl.cn

C#:   // 手写回溯递归
来源：http://fye.hongshengwenyu.top

[N09] 栈与队列
来源：http://pbz.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cyp.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mnm.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lkp.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lbf.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qdw.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vcs.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fbi.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wxs.cqqwz.cn

[N10] 链表节点定义
来源：http://boj.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ris.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://syb.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fnu.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tzf.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://jun.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://bln.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rmw.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oby.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://wyu.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eau.jiagoushi.top

PHP:  // 手写递归函数
来源：http://ukh.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihr.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qfg.jinyuanbaomall.cn

Java: // 手写递归
来源：http://uqg.cheryme.top

Go:   // 手写递归
来源：http://ebx.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://der.pengpengdd.cyou

C#:   // 手写递归
来源：http://ynm.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tgd.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gos.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bor.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hmx.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tlh.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hyg.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dem.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mwj.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jpy.chenjidiqi.icu

================================================================================
来源：http://eje.cqqwz.cn

O. 并发与异步
来源：http://xzg.zhengqikj.top

================================================================================
来源：http://mal.nanxinkj.top

[O01] 启动一个线程
来源：http://kdk.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dtw.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://owk.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ifz.hywenlv.cn

TS:   // 同 JS
来源：http://lox.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://cnv.fehbvm.com

Go:   go f()
来源：http://str.cqqwz.cn

Ruby: Thread.new { f }
来源：http://koc.yj202588.top

C#:   Task.Run(() => F());
来源：http://cgr.daxiang520.top

[O02] 使用线程池
来源：http://oeg.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://itc.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iov.shuidangran.top

JS:   // worker_threads 线程池
来源：http://rgi.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://phm.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://frz.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://woz.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://umg.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tit.hammf.cn

[O03] 加锁保护共享数据
来源：http://etb.daria6918.cn

Py:   with lock: shared += 1
来源：http://zqz.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://gya.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ygz.hnxiangtu.top

TS:   // 同 JS
来源：http://nab.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://xda.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eov.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hbv.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://pax.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://hrl.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://wlp.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvd.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://rkg.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://agy.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://agc.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dtm.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uju.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://dkn.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://ldx.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://faz.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yal.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://inr.yongpay.top

TS:   await Promise.all(tasks)
来源：http://dii.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vlu.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vvp.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://nff.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://lfd.smart0.xyz

[O06] 使用进程池
来源：http://gdt.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qcs.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://agr.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://kyj.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://bax.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mbd.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://spg.ppjwa.cn

Ruby: // fork 块
来源：http://fbi.zdbjq.cn

C#:   Parallel.For
来源：http://ymx.xuanzx.com

================================================================================
来源：http://cms.yj20258.top

P. 常用工具函数
来源：http://xmt.chenjidiqi.icu

================================================================================
来源：http://osx.zhixingplan.top

[P01] 生成 UUID
来源：http://iim.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://xgm.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fjf.ydzc1.top

JS:   crypto.randomUUID()
来源：http://ara.zycfv.cn

TS:   crypto.randomUUID()
来源：http://hvr.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://cww.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://baf.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://ymf.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://ikl.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://ktf.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wpx.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bas.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ctf.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gur.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://slx.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rbj.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dgh.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vln.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://grm.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qiy.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yej.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wsa.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hap.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dmk.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kfz.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dnc.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://icu.shuidangran.top

[P04] 求长度
来源：http://qca.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uyl.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ckm.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tvg.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fli.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://jdp.sxryk.cn

Go:   len(arr);  len(m)
来源：http://uoy.xziqi.cn

Ruby: x.length;  x.size
来源：http://imb.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xka.fehbvm.com

[P05] 判断两个对象内容是否相等
来源：http://nei.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://scf.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blt.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pcm.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://okl.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://csq.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mit.hongshengwenyu.top

Ruby: a == b
来源：http://qph.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tvq.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lqi.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fgq.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://rqx.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://quu.vehdjk.com

TS:   if (x == null) {}
来源：http://wir.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://exz.ydjk.org.cn

Go:   if x == nil {}
来源：http://zjz.sjlbkw.cn


<!-- 参考信息 -->