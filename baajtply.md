代发 wailian999

JS:   process.argv.slice(2)
来源：http://csj.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://yow.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://xgp.fengsongda.top

Go:   os.Args[1:]
来源：http://xuf.xuanzx.com

Ruby: ARGV
来源：http://iyb.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://mzb.redwolf501.top

[M02] 读取环境变量
来源：http://lbl.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://eii.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mzy.zdbjq.cn

JS:   process.env.HOME
来源：http://zpt.fzhhl.top

TS:   process.env.HOME
来源：http://csx.uphjek.com

Java: System.getenv("HOME")
来源：http://kce.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vnj.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://qwd.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vce.hongshengwenyu.top

[M03] 执行外部命令
来源：http://txs.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ynb.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yoa.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://msp.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rbn.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wot.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wzj.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://upx.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://nyb.yj202588.top

[M04] 获取当前工作目录
来源：http://ibj.tarul.cn

Py:   os.getcwd()
来源：http://rua.hfpthk.cn

PHP:  getcwd();
来源：http://fgh.hongshengwenyu.top

JS:   process.cwd()
来源：http://bma.tianlin.xyz

TS:   process.cwd()
来源：http://ccv.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://ltc.hnxiangtu.top

Go:   os.Getwd()
来源：http://msq.tian-w.cn

Ruby: Dir.pwd
来源：http://pdz.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://yfx.vehdjk.com

[M05] 设置退出码
来源：http://iwh.bbcook.cn

Py:   sys.exit(1)
来源：http://rwe.ybcxt.top

PHP:  exit(1);
来源：http://itm.jinqigfzy.top

JS:   process.exit(1)
来源：http://gzr.yangfankeji.com

TS:   process.exit(1)
来源：http://feo.shzxlz.cn

Java: System.exit(1)
来源：http://wjt.yfazqb.com

Go:   os.Exit(1)
来源：http://cmu.aibaodan.cn

Ruby: exit 1
来源：http://snn.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fwx.smart0.xyz

[M06] 向标准错误输出
来源：http://rth.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://igj.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jcq.xylfe.cn

JS:   console.error("err")
来源：http://wtk.yj20258.top

TS:   console.error("err")
来源：http://aid.fehbvm.com

Java: System.err.println("err")
来源：http://odm.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xoj.fehbvm.com

Ruby: warn "err"
来源：http://fqu.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://zvk.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://kjj.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://zfc.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cnn.hfpthk.cn

JS:   require.main === module
来源：http://yqh.xuetiantiany.cn

TS:   require.main === module
来源：http://hjl.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://vmd.zhixingplan.top

Go:   func main()
来源：http://mhc.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oje.epnwcf.com

C#:   static void Main(string[] args)
来源：http://cpn.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://igh.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://wjq.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://pbf.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://jsg.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://kvf.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tvp.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gsk.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jhh.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pkk.xuanzx.com

================================================================================
来源：http://khp.xuanzx.com

N. 数据结构与算法
来源：http://ntp.gaohongyu789.top

================================================================================
来源：http://tsc.hammf.cn

[N01] 二分查找（有序数组）
来源：http://ptu.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://ihn.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hsf.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ntz.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dpq.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yhr.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://mft.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://coh.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hvr.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://ldy.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://fuk.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nag.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://vam.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ctq.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ajq.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://rik.haohaochexian.top

Ruby: arr.sort
来源：http://fcl.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tbe.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://xru.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrj.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://clc.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://weo.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zah.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xcs.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wbu.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sml.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ggz.sjlbkw.cn

[N04] 斐波那契数列
来源：http://kuk.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ixj.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mvo.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pra.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://grm.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cnh.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nvb.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://snl.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://buc.chenzaomai.com

[N05] 最大公约数
来源：http://bls.yj202588.top

Py:   math.gcd(a, b)
来源：http://xin.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://edx.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mwz.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dsr.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yjf.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uxd.aibaodan.cn

Ruby: a.gcd(b)
来源：http://aej.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lhp.daxiang520.top

[N06] 判断回文字符串
来源：http://grt.xuanzx.com

Py:   s == s[::-1]
来源：http://cml.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://smn.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://qqj.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://mxc.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nss.havefunace.top

Go:   // 双指针从两端比较
来源：http://ujy.meibo888.top

Ruby: s == s.reverse
来源：http://bou.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jax.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://pxj.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bbi.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lgs.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kqh.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://kqo.yj20258.top

Java: // 手写 HashMap
来源：http://tcy.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://fec.fktsv.cn

Ruby: // 手写 Hash
来源：http://dkd.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://rch.sjlbkw.cn

[N08] 生成全排列
来源：http://kje.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://tnv.zdqjudy.top

PHP:  // 手写递归交换
来源：http://xyp.hnqzz.top

JS:   // 手写回溯递归
来源：http://aaw.nwbrower.top

TS:   // 手写回溯递归
来源：http://vfa.jinqigfzy.top

Java: // 手写回溯递归
来源：http://vws.yueranfly.top

Go:   // 手写回溯递归
来源：http://xby.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://pjv.tianlin.xyz

C#:   // 手写回溯递归
来源：http://crs.fktsv.cn

[N09] 栈与队列
来源：http://trm.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mdl.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdq.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wpq.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eao.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://coi.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wuj.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zkr.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yag.c1oappe.top

[N10] 链表节点定义
来源：http://njp.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zma.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kdj.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bcb.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://omd.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://mxt.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://aws.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mrh.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mul.birdmap.top

[N11] 二叉树中序遍历
来源：http://xjb.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jqm.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://dhp.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgk.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dbi.zhijiandao.cn

Java: // 手写递归
来源：http://mqr.mhx1999.top

Go:   // 手写递归
来源：http://xcb.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tyo.sjlbkw.cn

C#:   // 手写递归
来源：http://hil.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dku.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rdr.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ntw.xylfe.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://avy.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fxa.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://luv.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nch.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://knt.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rlq.yuxming.cn

================================================================================
来源：http://aqm.nanxinkj.top

O. 并发与异步
来源：http://irt.meibo888.top

================================================================================
来源：http://uzy.cashguo.top

[O01] 启动一个线程
来源：http://mmz.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://seq.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ydp.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vub.316326.xyz

TS:   // 同 JS
来源：http://tbw.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://uzz.wangshuangyany.cn

Go:   go f()
来源：http://egs.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://yyh.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://mnb.xylfe.cn

[O02] 使用线程池
来源：http://san.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ysv.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yay.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://plx.ybcxt.top

TS:   // worker_threads 线程池
来源：http://xjz.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gbf.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kgw.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wua.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xaw.ybcxt.top

[O03] 加锁保护共享数据
来源：http://txw.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://zsm.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://xlu.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tob.wangdashe.top

TS:   // 同 JS
来源：http://jyj.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://mwu.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kxj.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tyy.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://iql.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://wdc.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://ukb.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rku.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://rpj.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://sjc.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kek.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bos.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://lhn.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://xlr.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://qea.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://juu.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nxi.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://xdj.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://nax.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jki.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pfl.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://xlq.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ssl.sysykeji.top

[O06] 使用进程池
来源：http://oba.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wjx.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oiz.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://fkw.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://ypc.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ezo.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sto.ydjk.org.cn

Ruby: // fork 块
来源：http://ngx.gzhubu.top

C#:   Parallel.For
来源：http://uso.jqgufenzy.top

================================================================================
来源：http://idw.chenlongwang.top

P. 常用工具函数
来源：http://hlx.jyoumei.cn

================================================================================
来源：http://vxm.redwolf501.top

[P01] 生成 UUID
来源：http://hdu.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://deb.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mwu.52xcode.cn

JS:   crypto.randomUUID()
来源：http://yzc.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://rpe.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://plk.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://rht.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://ded.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://njg.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://tli.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wbf.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dek.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hse.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xez.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hzj.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yqy.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ukj.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nmm.zhixingplan.top

[P03] 生成短随机字符串
来源：http://mwz.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pdl.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://znj.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kts.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ncr.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bxc.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sov.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://amm.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kvc.hesvh.cn

[P04] 求长度
来源：http://rvu.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pmf.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qlr.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pax.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dpe.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://enf.sysykeji.top

Go:   len(arr);  len(m)
来源：http://dny.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://axd.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ypa.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://zbx.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gnl.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qen.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wjf.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://akq.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xyb.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wan.bjfxy.top

Ruby: a == b
来源：http://hsc.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ida.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rsu.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zij.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://afc.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qnk.tanke756.top

TS:   if (x == null) {}
来源：http://zxg.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jxl.jqgfzy.top

Go:   if x == nil {}
来源：http://myq.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ltk.hysaishi.cn

C#:   if (x is null) {}
来源：http://lxd.tanke756.top

[P07] 防抖与节流
来源：http://rrh.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://idg.cheryme.top

PHP:  // 手写时间戳比较
来源：http://lka.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dki.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzn.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bav.zhiwuduotai.top


<!-- 参考信息 -->