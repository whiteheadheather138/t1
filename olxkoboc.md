代发 wailian999

JS:   process.argv.slice(2)
来源：http://mlx.gzhubu.top

TS:   process.argv.slice(2)
来源：http://rrp.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://jlh.nanxinkj.top

Go:   os.Args[1:]
来源：http://aak.sweek.top

Ruby: ARGV
来源：http://hhc.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://acb.svipenyu.cn

[M02] 读取环境变量
来源：http://zkl.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://pok.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dnv.hysaishi.cn

JS:   process.env.HOME
来源：http://pti.ctjpmb.com

TS:   process.env.HOME
来源：http://krf.iojbl.cn

Java: System.getenv("HOME")
来源：http://jvw.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hdd.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://xci.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cay.epnwcf.com

[M03] 执行外部命令
来源：http://lkl.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mtg.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xss.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://fom.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ung.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://snu.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vtk.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://txn.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://zii.zhixingplan.top

[M04] 获取当前工作目录
来源：http://kvk.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://nbx.zhoulong.xyz

PHP:  getcwd();
来源：http://ooh.fktsv.cn

JS:   process.cwd()
来源：http://zvo.kuanghao11.cn

TS:   process.cwd()
来源：http://ved.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://jhz.yueranfly.top

Go:   os.Getwd()
来源：http://lgi.0kj1m.cn

Ruby: Dir.pwd
来源：http://zul.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://gnt.feifeiyinyue.top

[M05] 设置退出码
来源：http://jco.nanxinkj.top

Py:   sys.exit(1)
来源：http://cse.ydzc1.top

PHP:  exit(1);
来源：http://xyc.52xcode.cn

JS:   process.exit(1)
来源：http://gfk.iojbl.cn

TS:   process.exit(1)
来源：http://exz.epnwcf.com

Java: System.exit(1)
来源：http://iqi.ivvv.top

Go:   os.Exit(1)
来源：http://xjw.sjlbkw.cn

Ruby: exit 1
来源：http://qte.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oeg.jinqigfzy.top

[M06] 向标准错误输出
来源：http://deh.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://yld.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ynm.jqgufenzy.top

JS:   console.error("err")
来源：http://hqv.redwolf501.top

TS:   console.error("err")
来源：http://zvb.shangyingyoupin.top

Java: System.err.println("err")
来源：http://tqm.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fyv.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://irx.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://gop.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://ves.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://hry.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fip.yueranfly.top

JS:   require.main === module
来源：http://uig.iojbl.cn

TS:   require.main === module
来源：http://jdb.jqgfzy.top

Java: public static void main(String[] args)
来源：http://oui.zycfv.cn

Go:   func main()
来源：http://qjd.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zeu.cashguo.top

C#:   static void Main(string[] args)
来源：http://zcp.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://sge.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://edv.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://xfe.sxryk.cn

JS:   process.platform;  process.version
来源：http://tcm.9152youxi.cn

TS:   process.platform;  process.version
来源：http://lru.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jta.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ucl.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ghc.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://umg.aibaodan.cn

================================================================================
来源：http://uiz.mhx1999.top

N. 数据结构与算法
来源：http://ryi.zhijiandao.cn

================================================================================
来源：http://oho.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://xfd.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oto.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lft.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tzm.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qik.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://efo.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://bau.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vio.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://sdp.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://cla.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://ebg.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njj.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wqa.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ynm.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uzi.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://efk.guowangkeji.top

Ruby: arr.sort
来源：http://gre.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yhw.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://evb.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oen.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://kri.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ylp.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://edd.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dbt.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wad.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qkt.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ekl.guowangkeji.top

[N04] 斐波那契数列
来源：http://ezb.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rpc.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tic.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obd.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tim.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xpw.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uxt.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lnh.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jcb.uphjek.com

[N05] 最大公约数
来源：http://vtk.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://vgt.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tlb.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bdo.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ncd.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wux.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cub.yongpay.top

Ruby: a.gcd(b)
来源：http://vrt.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://osf.chenlongwang.top

[N06] 判断回文字符串
来源：http://rcu.chenzaomai.com

Py:   s == s[::-1]
来源：http://qjo.daria6918.cn

PHP:  $s === strrev($s);
来源：http://ogu.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://oay.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://iux.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eor.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://fif.kuanghao11.cn

Ruby: s == s.reverse
来源：http://bus.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://iiq.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://xma.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qoz.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hxe.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ddx.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://owu.hywenlv.cn

Java: // 手写 HashMap
来源：http://juy.bjfxy.top

Go:   // 手写 map[int]int
来源：http://nfn.yvedp.cn

Ruby: // 手写 Hash
来源：http://ffp.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lss.ctjpmb.com

[N08] 生成全排列
来源：http://ohs.uphjek.com

Py:   itertools.permutations(arr)
来源：http://wis.sysykeji.top

PHP:  // 手写递归交换
来源：http://bwh.cqqwz.cn

JS:   // 手写回溯递归
来源：http://ues.ctjpmb.com

TS:   // 手写回溯递归
来源：http://vnl.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://mrl.hysaishi.cn

Go:   // 手写回溯递归
来源：http://puq.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://xpt.fktsv.cn

C#:   // 手写回溯递归
来源：http://gsk.sweek.top

[N09] 栈与队列
来源：http://vzp.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ukt.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zpl.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ndr.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dbg.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oit.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jxr.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qdk.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iaf.yuanzhike.top

[N10] 链表节点定义
来源：http://zri.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bjc.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yjx.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rzw.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sux.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://mbn.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://jjy.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://atk.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ihz.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://kyy.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://arl.vehdjk.com

PHP:  // 手写递归函数
来源：http://rkd.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bju.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ssv.wangdashe.top

Java: // 手写递归
来源：http://hnr.yvedp.cn

Go:   // 手写递归
来源：http://fiw.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iwb.cucudq.cn

C#:   // 手写递归
来源：http://wen.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uvr.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ght.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://imk.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nsw.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://try.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qek.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://knf.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://czh.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dah.fehbvm.com

================================================================================
来源：http://wfr.tianlin.xyz

O. 并发与异步
来源：http://xqm.dianchejie.cn

================================================================================
来源：http://spr.fktsv.cn

[O01] 启动一个线程
来源：http://wmy.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://num.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aje.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ain.nwbrower.top

TS:   // 同 JS
来源：http://qmz.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://vou.ywan-chungtsiang.top

Go:   go f()
来源：http://zng.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://bqj.sysykeji.top

C#:   Task.Run(() => F());
来源：http://iau.fanxiaobao.xyz

[O02] 使用线程池
来源：http://mtw.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zsv.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://flb.yongpay.top

JS:   // worker_threads 线程池
来源：http://xle.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://owt.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lpp.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zwu.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sqv.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ixc.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://xyu.nanxinkj.top

Py:   with lock: shared += 1
来源：http://nza.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://uqz.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qlm.jyoumei.cn

TS:   // 同 JS
来源：http://kkt.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://dae.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mfa.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lqv.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://ckf.hnqzz.top

[O04] 定义异步函数并等待
来源：http://yyw.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://adf.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xmt.316326.xyz

JS:   async function f() { await g(); }
来源：http://sic.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgo.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xkw.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cup.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mez.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://kwy.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://zyw.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://uez.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eqp.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ani.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://sev.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ydz.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://anw.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://sqo.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wya.kuanghao11.cn

[O06] 使用进程池
来源：http://oev.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zuj.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://oaj.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://tfa.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://fij.ydzc1.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gkq.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://otu.jqgufenzy.top

Ruby: // fork 块
来源：http://qjx.cashguo.top

C#:   Parallel.For
来源：http://ldu.meibo888.top

================================================================================
来源：http://rjh.chenjidiqi.icu

P. 常用工具函数
来源：http://gkk.yangfankeji.com

================================================================================
来源：http://ldj.yj20258888.top

[P01] 生成 UUID
来源：http://lwa.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://goh.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hni.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://rpu.fktsv.cn

TS:   crypto.randomUUID()
来源：http://etk.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://gur.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://ckd.hammf.cn

Ruby: SecureRandom.uuid
来源：http://dsl.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://yxo.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://gmn.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qbu.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ojk.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xjp.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://heo.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rvj.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ctr.cdnleiting.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qdt.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://whs.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://azz.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qpp.snrcjt.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rut.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hox.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qpz.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tbe.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wwl.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://sjr.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zmo.xuetiantiany.cn

[P04] 求长度
来源：http://nps.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://waj.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rzt.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aux.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bdo.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://uvh.cheryme.top

Go:   len(arr);  len(m)
来源：http://vrv.cashguo.top

Ruby: x.length;  x.size
来源：http://vtb.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hcx.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://hmt.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dye.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jts.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tph.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tdh.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qvb.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rsd.svipenyu.cn

Ruby: a == b
来源：http://knw.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qvh.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://seu.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lcv.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://vcr.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qyr.sweek.top

TS:   if (x == null) {}
来源：http://dfi.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://gki.guannengcc.top

Go:   if x == nil {}
来源：http://vbr.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yux.sjlbkw.cn

C#:   if (x is null) {}
来源：http://rty.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://cbz.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lga.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://luq.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tst.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwi.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://axe.yj20258888.top


<!-- 参考信息 -->