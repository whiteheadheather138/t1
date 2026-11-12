代发 wailian999

JS:   process.argv.slice(2)
来源：http://jvv.bbcook.cn

TS:   process.argv.slice(2)
来源：http://zxb.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://geq.fktsv.cn

Go:   os.Args[1:]
来源：http://tky.nanxinkj.top

Ruby: ARGV
来源：http://zbm.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://smf.sufxvd.cn

[M02] 读取环境变量
来源：http://zhw.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://uop.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mbz.zycfv.cn

JS:   process.env.HOME
来源：http://nel.daxiang520.top

TS:   process.env.HOME
来源：http://zjb.zhixingplan.top

Java: System.getenv("HOME")
来源：http://dhy.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://too.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://iqs.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hqa.cdnleiting.top

[M03] 执行外部命令
来源：http://rzg.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gbk.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zuq.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lwr.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kpg.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rzk.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qgl.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://vji.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://gfh.yfazqb.com

[M04] 获取当前工作目录
来源：http://rsq.hammf.cn

Py:   os.getcwd()
来源：http://pmz.uphjek.com

PHP:  getcwd();
来源：http://pxt.hongshengwenyu.top

JS:   process.cwd()
来源：http://uew.shangyingyoupin.top

TS:   process.cwd()
来源：http://bbr.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://wha.chenlongwang.top

Go:   os.Getwd()
来源：http://nly.fktsv.cn

Ruby: Dir.pwd
来源：http://bfv.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://zrp.chenzaomai.com

[M05] 设置退出码
来源：http://qzq.shuidangran.top

Py:   sys.exit(1)
来源：http://esv.316326.xyz

PHP:  exit(1);
来源：http://fue.kuanghao11.cn

JS:   process.exit(1)
来源：http://byt.cqqwz.cn

TS:   process.exit(1)
来源：http://lmc.hesvh.cn

Java: System.exit(1)
来源：http://lpk.cdnleiting.top

Go:   os.Exit(1)
来源：http://hdp.dianchejie.cn

Ruby: exit 1
来源：http://nmz.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lqp.c1oappe.top

[M06] 向标准错误输出
来源：http://btl.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://akz.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bvh.gogol.net.cn

JS:   console.error("err")
来源：http://vap.ctjpmb.com

TS:   console.error("err")
来源：http://frb.ydjk.org.cn

Java: System.err.println("err")
来源：http://gwf.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://znv.jqgfzy.top

Ruby: warn "err"
来源：http://xur.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://jgs.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://hno.ivvv.top

Py:   if __name__ == "__main__":
来源：http://rwk.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ahc.ydjk.org.cn

JS:   require.main === module
来源：http://kni.sxryk.cn

TS:   require.main === module
来源：http://yyt.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://smw.zhixingplan.top

Go:   func main()
来源：http://rga.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jmi.sysykeji.top

C#:   static void Main(string[] args)
来源：http://hfz.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://aem.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://jmj.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://xac.yj202588.top

JS:   process.platform;  process.version
来源：http://otz.daxiang520.top

TS:   process.platform;  process.version
来源：http://ywv.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lfk.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kkv.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jfp.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://imi.sxryk.cn

================================================================================
来源：http://rew.xinyue.icu

N. 数据结构与算法
来源：http://ber.wangdashe.top

================================================================================
来源：http://oeg.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://wws.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://juu.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vkz.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fjm.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dag.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://rbl.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://jhj.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vch.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://irt.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://avh.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ktb.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bqf.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ptf.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tru.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://okk.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://niv.xziqi.cn

Ruby: arr.sort
来源：http://nvp.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iba.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://umr.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mnt.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://pjy.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvn.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aft.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qce.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nez.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qmr.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://baz.vqdsnc.cn

[N04] 斐波那契数列
来源：http://uzp.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://osu.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oka.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ltz.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxt.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uwe.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dud.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hld.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kts.guannengcc.top

[N05] 最大公约数
来源：http://nby.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://use.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tak.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lss.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfy.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sru.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wdt.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://ngs.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qwq.chenzaomai.com

[N06] 判断回文字符串
来源：http://aap.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://zwo.hammf.cn

PHP:  $s === strrev($s);
来源：http://xgg.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://okj.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://mbw.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://plr.sxryk.cn

Go:   // 双指针从两端比较
来源：http://yvg.shuidangran.top

Ruby: s == s.reverse
来源：http://wdd.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lsq.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://ktt.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xne.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xuj.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uwk.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://dps.jqgufenzy.top

Java: // 手写 HashMap
来源：http://mvg.mhx1999.top

Go:   // 手写 map[int]int
来源：http://zst.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://glo.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://oge.yueranfly.top

[N08] 生成全排列
来源：http://xbg.yonumen.top

Py:   itertools.permutations(arr)
来源：http://mrq.mhx1999.top

PHP:  // 手写递归交换
来源：http://wsl.sysykeji.top

JS:   // 手写回溯递归
来源：http://bsf.xinyue.icu

TS:   // 手写回溯递归
来源：http://ppd.xziqi.cn

Java: // 手写回溯递归
来源：http://jdg.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://uuj.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://juu.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://ddy.yueranfly.top

[N09] 栈与队列
来源：http://hzh.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kqa.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hwe.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://epi.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dca.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ybg.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qhy.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vgl.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zbs.shangyingyoupin.top

[N10] 链表节点定义
来源：http://aft.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://syz.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://guu.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cbp.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eei.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://crh.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://fsa.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kfk.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bjy.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://rsc.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ybv.cashguo.top

PHP:  // 手写递归函数
来源：http://pxt.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jmt.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vua.cdnleiting.top

Java: // 手写递归
来源：http://nvv.yuxming.cn

Go:   // 手写递归
来源：http://smp.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rzn.hammf.cn

C#:   // 手写递归
来源：http://oqb.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jeu.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ckw.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iur.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iol.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vki.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mak.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ctn.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pib.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hjt.aizwys.cn

================================================================================
来源：http://uwu.zhoulong.xyz

O. 并发与异步
来源：http://fep.zycfv.cn

================================================================================
来源：http://qcy.yvedp.cn

[O01] 启动一个线程
来源：http://iov.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ltf.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vec.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zzn.tian-w.cn

TS:   // 同 JS
来源：http://pqv.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://iwi.jinqigfzy.top

Go:   go f()
来源：http://dgv.hnqzz.top

Ruby: Thread.new { f }
来源：http://yis.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://vuw.xuetiantiany.cn

[O02] 使用线程池
来源：http://dul.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wst.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qjm.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://rys.xziqi.cn

TS:   // worker_threads 线程池
来源：http://jxv.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://egy.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ipe.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sdg.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hel.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://rap.tanke756.top

Py:   with lock: shared += 1
来源：http://vqs.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://kat.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fbi.yuxming.cn

TS:   // 同 JS
来源：http://iqd.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://kce.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://euw.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dtf.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://omh.pycfn.com

[O04] 定义异步函数并等待
来源：http://qds.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://mpl.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lew.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://axy.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://emy.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pnb.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pdc.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dhl.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://man.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://yan.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://sib.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bwb.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://kna.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://tfv.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sgv.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cmg.sxryk.cn

Ruby: threads.map(&:join)
来源：http://ksu.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uqe.vehdjk.com

[O06] 使用进程池
来源：http://pjm.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jzu.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fpi.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://xhh.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://mtn.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bdw.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://foc.chenzaomai.com

Ruby: // fork 块
来源：http://giw.xziqi.cn

C#:   Parallel.For
来源：http://kib.yongpay.top

================================================================================
来源：http://opo.jinyuanbaomall.cn

P. 常用工具函数
来源：http://olu.quarkkingdee.top

================================================================================
来源：http://cbf.0kj1m.cn

[P01] 生成 UUID
来源：http://hmf.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://bhr.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rek.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://omx.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://eux.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://zba.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://rnh.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://xcr.nanxinkj.top

C#:   Guid.NewGuid().ToString()
来源：http://gwo.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://ieq.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wvc.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mlh.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fmg.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sbq.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ipi.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oqh.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xvs.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dkj.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://tae.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nid.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xxd.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hrl.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hno.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gym.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qto.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pyb.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zhi.yfazqb.com

[P04] 求长度
来源：http://ibe.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lpp.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ceh.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zlc.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tio.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://jwu.daxiang520.top

Go:   len(arr);  len(m)
来源：http://rcm.redwolf501.top

Ruby: x.length;  x.size
来源：http://lyx.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://udf.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://wmn.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://npz.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://agx.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sej.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://asz.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tbk.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cgm.uphjek.com

Ruby: a == b
来源：http://uev.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fvu.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tyd.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jsz.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://jtk.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qhj.0kj1m.cn

TS:   if (x == null) {}
来源：http://cbp.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xva.chenlongwang.top

Go:   if x == nil {}
来源：http://dii.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nef.jiagoushi.top

C#:   if (x is null) {}
来源：http://gbt.zhixingplan.top

[P07] 防抖与节流
来源：http://qwr.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lds.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://iuf.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfp.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zld.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dgt.jqgufenzy.top


<!-- 参考信息 -->