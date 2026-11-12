代发 wailian999

Ruby: ARGV
来源：http://ehb.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://ppf.shangyingyoupin.top

[M02] 读取环境变量
来源：http://nmb.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://cxr.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://opn.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://qqx.wangdashe.top

TS:   process.env.HOME
来源：http://tvq.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://cek.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gjo.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://kns.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tcx.yangfankeji.com

[M03] 执行外部命令
来源：http://wsc.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ayt.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gsn.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pkg.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cys.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qlt.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oan.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://ykx.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://atz.guannengcc.top

[M04] 获取当前工作目录
来源：http://lzq.xuanzx.com

Py:   os.getcwd()
来源：http://iyq.shangyingyoupin.top

PHP:  getcwd();
来源：http://rjf.chenjidiqi.icu

JS:   process.cwd()
来源：http://psx.xziqi.cn

TS:   process.cwd()
来源：http://feg.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://ztu.9152youxi.cn

Go:   os.Getwd()
来源：http://ovw.fehbvm.com

Ruby: Dir.pwd
来源：http://xdf.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://enm.kuanghao11.cn

[M05] 设置退出码
来源：http://pkw.cashguo.top

Py:   sys.exit(1)
来源：http://qql.andypj.xyz

PHP:  exit(1);
来源：http://foy.hnxiangtu.top

JS:   process.exit(1)
来源：http://zmj.jqgufenzy.top

TS:   process.exit(1)
来源：http://mvo.mhx1999.top

Java: System.exit(1)
来源：http://lyb.cashguo.top

Go:   os.Exit(1)
来源：http://hxu.ivvv.top

Ruby: exit 1
来源：http://dol.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sxf.xziqi.cn

[M06] 向标准错误输出
来源：http://ufc.yanxiufei.cn

Py:   print("err", file=sys.stderr)
来源：http://qcg.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://skl.redwolf501.top

JS:   console.error("err")
来源：http://tim.ivvv.top

TS:   console.error("err")
来源：http://isf.xuanzx.com

Java: System.err.println("err")
来源：http://fuo.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ooo.vqdsnc.cn

Ruby: warn "err"
来源：http://ysz.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://ese.yangfankeji.com

[M07] 判断是否为主入口
来源：http://ofd.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://gbp.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uve.uphjek.com

JS:   require.main === module
来源：http://ocb.zhaomingkeji.xyz

TS:   require.main === module
来源：http://upi.guowangkeji.top

Java: public static void main(String[] args)
来源：http://nag.xylfe.cn

Go:   func main()
来源：http://qxv.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fia.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://bzm.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://ogm.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://nul.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://npe.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://dpw.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://thj.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yoj.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ifx.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oex.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yws.xuetiantiany.cn

================================================================================
来源：http://qcv.nwbrower.top

N. 数据结构与算法
来源：http://dhs.c1oappe.top

================================================================================
来源：http://lep.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://syf.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://klk.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fvt.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dme.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fce.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://apc.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://kdp.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jzr.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://iav.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://cbj.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://enw.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dse.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://iaw.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kmj.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gee.yj202588.top

Go:   slices.Sort(arr)
来源：http://ngy.yanxiufei.cn

Ruby: arr.sort
来源：http://mxb.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mfl.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://mco.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nim.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://vox.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nri.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bkd.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://muj.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tnr.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nzv.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fwu.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://toc.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nca.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gvs.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsm.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ohc.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aec.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mxm.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jwe.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pyy.meibo888.top

[N05] 最大公约数
来源：http://can.yfazqb.com

Py:   math.gcd(a, b)
来源：http://phj.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mok.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwi.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dir.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kfa.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ygg.wangdashe.top

Ruby: a.gcd(b)
来源：http://rjh.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mxx.yuxming.cn

[N06] 判断回文字符串
来源：http://ucf.havefunace.top

Py:   s == s[::-1]
来源：http://uvr.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://ete.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://htk.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://zdv.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rxc.xziqi.cn

Go:   // 双指针从两端比较
来源：http://sqt.yfazqb.com

Ruby: s == s.reverse
来源：http://zwi.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://svy.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://yac.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nkx.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://smy.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gut.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://qwa.sufxvd.cn

Java: // 手写 HashMap
来源：http://ssf.c1oappe.top

Go:   // 手写 map[int]int
来源：http://cgn.nanxinkj.top

Ruby: // 手写 Hash
来源：http://uja.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mdb.9152youxi.cn

[N08] 生成全排列
来源：http://tfp.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://mjw.hfpthk.cn

PHP:  // 手写递归交换
来源：http://xzd.hesvh.cn

JS:   // 手写回溯递归
来源：http://jyu.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://fdf.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://iwo.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://xmz.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://xti.tanke756.top

C#:   // 手写回溯递归
来源：http://ypf.aizwys.cn

[N09] 栈与队列
来源：http://fxp.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hds.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yso.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pic.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fnw.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pmx.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://syp.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zqo.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://meu.mhx1999.top

[N10] 链表节点定义
来源：http://ibk.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://leo.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hds.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xvi.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jxo.cheryme.top

Java: class Node { int v; Node next; }
来源：http://dli.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vbe.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eml.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://pqc.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://xmp.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nec.aizwys.cn

PHP:  // 手写递归函数
来源：http://kvd.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qxm.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vhz.ybcxt.top

Java: // 手写递归
来源：http://sgk.yanxiufei.cn

Go:   // 手写递归
来源：http://luc.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pza.kuanghao11.cn

C#:   // 手写递归
来源：http://jnz.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hpg.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ojp.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syj.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ktr.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://end.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xwe.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ywq.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ysv.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nmv.iojbl.cn

================================================================================
来源：http://bqj.yfazqb.com

O. 并发与异步
来源：http://erv.hnxiangtu.top

================================================================================
来源：http://ezc.cucudq.cn

[O01] 启动一个线程
来源：http://pji.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lij.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tqy.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mrk.hammf.cn

TS:   // 同 JS
来源：http://qrn.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://ntb.jyoumei.cn

Go:   go f()
来源：http://jii.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://mxb.meibo888.top

C#:   Task.Run(() => F());
来源：http://zhj.yuanzhike.top

[O02] 使用线程池
来源：http://hkw.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jjr.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yzq.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://vvj.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://wwk.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://abr.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xrh.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jxe.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cpc.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://tvd.birdmap.top

Py:   with lock: shared += 1
来源：http://cpv.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://bmc.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lss.0kj1m.cn

TS:   // 同 JS
来源：http://dyo.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://enu.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vak.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://sjj.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://von.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://ahd.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://fju.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fgn.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://bxp.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xaq.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hbr.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nfk.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://ggy.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://hoe.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://upz.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://yeu.hongshengwenyu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://smg.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://wqp.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://zxt.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cbs.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjc.xylfe.cn

Ruby: threads.map(&:join)
来源：http://hcu.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fyg.jinghuilouyu.cn

[O06] 使用进程池
来源：http://aca.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ieg.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://iin.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://bll.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://nju.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://akz.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ckw.zycfv.cn

Ruby: // fork 块
来源：http://byh.nwbrower.top

C#:   Parallel.For
来源：http://frj.birdmap.top

================================================================================
来源：http://trp.yueranfly.top

P. 常用工具函数
来源：http://pjp.hongshengwenyu.top

================================================================================
来源：http://nyv.gotoacloud.top

[P01] 生成 UUID
来源：http://wqg.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://uej.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hqy.fktsv.cn

JS:   crypto.randomUUID()
来源：http://bsm.yongpay.top

TS:   crypto.randomUUID()
来源：http://adg.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://ckt.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://gyu.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://mzk.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ppt.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://kmm.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gtz.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qye.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://abr.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xwc.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gug.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vym.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://imb.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://prg.shuidangran.top

[P03] 生成短随机字符串
来源：http://ugp.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ipe.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jlb.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aud.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rkk.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dbv.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gvk.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qni.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pcp.quarkkingdee.top

[P04] 求长度
来源：http://wnx.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oqm.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugm.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kns.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uuv.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://zkc.jianghu66.top

Go:   len(arr);  len(m)
来源：http://plb.tianlin.xyz

Ruby: x.length;  x.size
来源：http://lje.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jiv.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://kku.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cvn.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vwx.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://del.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vhh.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dre.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gnz.shanyushiyangtech.top

Ruby: a == b
来源：http://rhd.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kxe.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kgl.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xma.uphjek.com

PHP:  if (empty($x)) {}
来源：http://fvt.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eja.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://yqk.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uvy.jlsjyb.cn

Go:   if x == nil {}
来源：http://hth.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yet.jyoumei.cn

C#:   if (x is null) {}
来源：http://cpm.sxryk.cn

[P07] 防抖与节流
来源：http://vex.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qll.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://nxx.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzh.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hhl.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uly.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iir.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jpy.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://emh.yj202588.top

[P08] 处理浮点精度问题
来源：http://hbt.yj20258.top


<!-- 参考信息 -->