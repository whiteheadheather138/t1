代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pjw.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xmq.shanyushiyangtech.top

================================================================================
来源：http://bjn.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://umo.jinqigufen.top

================================================================================
来源：http://ktv.quarkkingdee.top

[M01] 读取命令行参数
来源：http://uag.c1oappe.top

Py:   sys.argv[1:]
来源：http://tkb.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://jct.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://izg.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://sbd.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://rqi.zhongyouzk.top

Go:   os.Args[1:]
来源：http://kkc.316326.xyz

Ruby: ARGV
来源：http://cif.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://fee.andypj.xyz

[M02] 读取环境变量
来源：http://fav.uphjek.com

Py:   os.environ.get("HOME")
来源：http://zss.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbm.fzhhl.top

JS:   process.env.HOME
来源：http://dka.hfpthk.cn

TS:   process.env.HOME
来源：http://rzl.zdqjudy.top

Java: System.getenv("HOME")
来源：http://uvk.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nvy.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://zdv.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ohc.haohaochexian.top

[M03] 执行外部命令
来源：http://xda.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vam.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hxc.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://uzn.bjfxy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qzb.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vdg.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yoh.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qeb.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://ztj.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://jvt.jinqigufen.top

Py:   os.getcwd()
来源：http://wds.0kj1m.cn

PHP:  getcwd();
来源：http://nxn.hywenlv.cn

JS:   process.cwd()
来源：http://mht.aibaodan.cn

TS:   process.cwd()
来源：http://fcv.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://bcf.nanxinkj.top

Go:   os.Getwd()
来源：http://whx.snrcjt.cn

Ruby: Dir.pwd
来源：http://yjy.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://kqh.tanke756.top

[M05] 设置退出码
来源：http://gev.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://lhe.jinqigufen.top

PHP:  exit(1);
来源：http://qcl.hesvh.cn

JS:   process.exit(1)
来源：http://ixo.meibo888.top

TS:   process.exit(1)
来源：http://pka.iojbl.cn

Java: System.exit(1)
来源：http://cip.cashguo.top

Go:   os.Exit(1)
来源：http://wax.gotoacloud.top

Ruby: exit 1
来源：http://ito.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://edl.zdqjudy.top

[M06] 向标准错误输出
来源：http://yqw.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://hcc.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wvi.chenzaomai.com

JS:   console.error("err")
来源：http://exa.meibo888.top

TS:   console.error("err")
来源：http://kyn.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://yxf.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://azi.316326.xyz

Ruby: warn "err"
来源：http://oaf.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://inq.xinyue.icu

[M07] 判断是否为主入口
来源：http://kcq.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://qsl.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://owo.zhaomingkeji.xyz

JS:   require.main === module
来源：http://vgm.cdnleiting.top

TS:   require.main === module
来源：http://mky.sufxvd.cn

Java: public static void main(String[] args)
来源：http://cbz.sweek.top

Go:   func main()
来源：http://rab.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fkt.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://wgp.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://ruq.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://hji.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://scp.gotoacloud.top

JS:   process.platform;  process.version
来源：http://owh.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://mbz.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jrv.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xwy.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ldj.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hrh.jianghu66.top

================================================================================
来源：http://why.shangyingyoupin.top

N. 数据结构与算法
来源：http://ncp.zhixingplan.top

================================================================================
来源：http://mmp.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://bym.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://mrb.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mtp.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uka.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nwo.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://ivr.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://aeh.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gvp.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://ajo.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://kjy.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ndv.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iip.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://gaz.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kxy.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://goz.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://oce.havefunace.top

Ruby: arr.sort
来源：http://boh.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpz.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://tpm.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pog.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://utg.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cfs.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fsu.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ndy.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eyb.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mfq.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://dwx.zycfv.cn

[N04] 斐波那契数列
来源：http://mmr.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://okg.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tht.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbb.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mdm.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rxm.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zxr.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hmx.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ipe.cqqwz.cn

[N05] 最大公约数
来源：http://kxx.andypj.xyz

Py:   math.gcd(a, b)
来源：http://gfe.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ptw.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zrm.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqg.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wna.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hlj.daxiang520.top

Ruby: a.gcd(b)
来源：http://vwt.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sjd.aizwys.cn

[N06] 判断回文字符串
来源：http://oij.bjfxy.top

Py:   s == s[::-1]
来源：http://bsh.yueranfly.top

PHP:  $s === strrev($s);
来源：http://hke.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://nwn.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://sgi.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lvv.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://emy.0kj1m.cn

Ruby: s == s.reverse
来源：http://cpo.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zsl.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://cpg.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xbq.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nuy.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sgf.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://dba.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://zec.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://fjs.aizwys.cn

Ruby: // 手写 Hash
来源：http://umh.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://bea.tanke756.top

[N08] 生成全排列
来源：http://mxh.yj20258.top

Py:   itertools.permutations(arr)
来源：http://yfi.epnwcf.com

PHP:  // 手写递归交换
来源：http://rpk.nwbrower.top

JS:   // 手写回溯递归
来源：http://ega.mhx1999.top

TS:   // 手写回溯递归
来源：http://chr.0kj1m.cn

Java: // 手写回溯递归
来源：http://gvl.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://vrv.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://vdl.xziqi.cn

C#:   // 手写回溯递归
来源：http://jfd.hnqzz.top

[N09] 栈与队列
来源：http://tzz.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kxf.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rjs.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ahj.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zps.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gkq.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qkm.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xbi.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://szg.fengsongda.top

[N10] 链表节点定义
来源：http://srg.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vum.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tnu.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mtm.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wxr.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://vks.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://xyp.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kvf.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://npy.yongpay.top

[N11] 二叉树中序遍历
来源：http://ajy.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://llg.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://iww.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pco.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovm.zhiwuduotai.top

Java: // 手写递归
来源：http://voz.jianghu66.top

Go:   // 手写递归
来源：http://wpt.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mmq.guowangkeji.top

C#:   // 手写递归
来源：http://ubq.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dmp.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iwp.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhv.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tiz.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cki.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ywj.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fey.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uwa.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lnr.xziqi.cn

================================================================================
来源：http://bqc.xingfuxueyuan.xyz

O. 并发与异步
来源：http://vkc.zhoulong.xyz

================================================================================
来源：http://hel.yvedp.cn

[O01] 启动一个线程
来源：http://ltw.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xle.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yqg.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kru.havefunace.top

TS:   // 同 JS
来源：http://bdf.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://ryr.xinyue.icu

Go:   go f()
来源：http://oth.vehdjk.com

Ruby: Thread.new { f }
来源：http://pji.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://wdi.c1oappe.top

[O02] 使用线程池
来源：http://naj.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kzg.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://izx.sxryk.cn

JS:   // worker_threads 线程池
来源：http://wyf.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://ecz.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://waw.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zwe.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rkn.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mlo.fengsongda.top

[O03] 加锁保护共享数据
来源：http://xjf.cashguo.top

Py:   with lock: shared += 1
来源：http://drt.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://scm.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zgu.ehwqpu.com

TS:   // 同 JS
来源：http://tbb.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://vid.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kag.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fji.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://nan.jianghu66.top

[O04] 定义异步函数并等待
来源：http://hvz.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://jtt.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhj.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://rxt.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dnn.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fvy.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kts.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://hew.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://wei.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://ebv.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://zqs.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xue.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://abs.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://lbu.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pmh.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jhb.andypj.xyz

Ruby: threads.map(&:join)
来源：http://oel.gogol.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jfv.chenjidiqi.icu

[O06] 使用进程池
来源：http://tko.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eym.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wly.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://sgx.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://hww.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gib.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hnv.feifeiyinyue.top

Ruby: // fork 块
来源：http://scu.sxryk.cn

C#:   Parallel.For
来源：http://qgm.uphjek.com

================================================================================
来源：http://opc.zhongyouzk.top

P. 常用工具函数
来源：http://mfo.sjlbkw.cn

================================================================================
来源：http://awu.gaohongyu789.top

[P01] 生成 UUID
来源：http://jgg.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://rdl.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wrv.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://oeg.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://oeg.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://lkt.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://juy.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://exw.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://nve.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://lfg.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mis.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://yqu.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://swb.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oor.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://shr.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vzw.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hyv.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tye.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://cdp.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qlv.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ows.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uya.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqw.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rpt.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xed.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jsa.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gdx.ppjwa.cn

[P04] 求长度
来源：http://yuk.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tnp.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lym.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vpa.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cbe.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://qqy.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://rda.zhengqikj.top

Ruby: x.length;  x.size
来源：http://yfo.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bmm.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://wwg.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://sdm.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kni.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nkz.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gcr.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://evu.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://bvh.meibo888.top

Ruby: a == b
来源：http://zbo.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tij.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kmf.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yxm.yj20258.top

PHP:  if (empty($x)) {}
来源：http://nwz.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tfp.zhongyouzk.top

TS:   if (x == null) {}
来源：http://wld.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://bgh.zdbjq.cn

Go:   if x == nil {}
来源：http://ome.tanke756.top


<!-- 参考信息 -->