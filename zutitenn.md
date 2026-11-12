代发 wailian999

================================================================================
来源：http://vvy.yj20258888.top

[M01] 读取命令行参数
来源：http://hju.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://ywb.cheryme.top

PHP:  $argv;  $argc;
来源：http://ymw.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://xuj.havefunace.top

TS:   process.argv.slice(2)
来源：http://lew.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://qqy.jianghu66.top

Go:   os.Args[1:]
来源：http://wnn.fanxiaobao.xyz

Ruby: ARGV
来源：http://yhh.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://bqf.chenjidiqi.icu

[M02] 读取环境变量
来源：http://zry.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://hhk.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yya.hcnkem.com

JS:   process.env.HOME
来源：http://frh.gogol.net.cn

TS:   process.env.HOME
来源：http://ivb.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://eui.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ikl.yonumen.top

Ruby: ENV["HOME"]
来源：http://wqf.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vnm.hongshengwenyu.top

[M03] 执行外部命令
来源：http://qwe.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lzg.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yjz.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://evc.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rlc.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yag.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oiv.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://omv.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://iqk.yj20258888.top

[M04] 获取当前工作目录
来源：http://gqx.yvedp.cn

Py:   os.getcwd()
来源：http://uzv.gzhubu.top

PHP:  getcwd();
来源：http://ndg.nanxuanxn.top

JS:   process.cwd()
来源：http://ayw.ppjwa.cn

TS:   process.cwd()
来源：http://yjk.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://uvq.sxryk.cn

Go:   os.Getwd()
来源：http://uyi.zycfv.cn

Ruby: Dir.pwd
来源：http://ufr.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://nkv.aibaodan.cn

[M05] 设置退出码
来源：http://lxe.fehbvm.com

Py:   sys.exit(1)
来源：http://crq.nanxinkj.top

PHP:  exit(1);
来源：http://rfs.yuxming.cn

JS:   process.exit(1)
来源：http://qpg.vehdjk.com

TS:   process.exit(1)
来源：http://otz.c1oappe.top

Java: System.exit(1)
来源：http://wep.haohaochexian.top

Go:   os.Exit(1)
来源：http://xub.fanxiaobao.xyz

Ruby: exit 1
来源：http://opr.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bzh.zhongyouzk.top

[M06] 向标准错误输出
来源：http://gis.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://vli.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vpn.dianchejie.cn

JS:   console.error("err")
来源：http://trd.hfpthk.cn

TS:   console.error("err")
来源：http://xfm.havefunace.top

Java: System.err.println("err")
来源：http://xpr.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bxe.hnxiangtu.top

Ruby: warn "err"
来源：http://llq.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://xzz.yuanzhike.top

[M07] 判断是否为主入口
来源：http://vaw.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://sbu.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://opc.zhaomingkeji.xyz

JS:   require.main === module
来源：http://aki.kuanghao11.cn

TS:   require.main === module
来源：http://vyg.gotoacloud.top

Java: public static void main(String[] args)
来源：http://fvt.quarkkingdee.top

Go:   func main()
来源：http://mii.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lfq.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://yzx.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://kzm.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://ijv.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://qit.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://gjv.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://otg.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vhp.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qpa.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kqi.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kiu.mhx1999.top

================================================================================
来源：http://rta.zdbjq.cn

N. 数据结构与算法
来源：http://wrl.yfazqb.com

================================================================================
来源：http://cmu.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://gax.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://yel.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ddw.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bwm.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qqg.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wld.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://hhl.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jwy.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bmb.fzhhl.top

[N02] 排序（工程实践用内置实现）
来源：http://xqz.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://tbl.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nuu.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zlz.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pty.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fxm.yonumen.top

Go:   slices.Sort(arr)
来源：http://ega.zhengqikj.top

Ruby: arr.sort
来源：http://lat.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://jyl.pycfn.com

[N03] 快速排序（分治示例）
来源：http://lau.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nst.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://bbl.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lkn.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lmq.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wnu.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kpb.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hxm.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://pmf.fengsongda.top

[N04] 斐波那契数列
来源：http://kcq.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://piz.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lpb.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://feh.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mae.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ygf.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://edj.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ipv.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uyn.mhx1999.top

[N05] 最大公约数
来源：http://ylc.hesvh.cn

Py:   math.gcd(a, b)
来源：http://uto.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rtc.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://els.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ksk.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gil.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xfw.316326.xyz

Ruby: a.gcd(b)
来源：http://usg.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ufk.yuanzhike.top

[N06] 判断回文字符串
来源：http://qog.tarul.cn

Py:   s == s[::-1]
来源：http://phb.wangdashe.top

PHP:  $s === strrev($s);
来源：http://pli.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://bjv.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://siv.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://luy.uphjek.com

Go:   // 双指针从两端比较
来源：http://zbu.uphjek.com

Ruby: s == s.reverse
来源：http://cmf.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://smt.yj202588.top

[N07] 两数之和（返回下标）
来源：http://fad.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydm.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bqf.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xrl.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://yxa.zdqjudy.top

Java: // 手写 HashMap
来源：http://wox.sysykeji.top

Go:   // 手写 map[int]int
来源：http://itp.birdmap.top

Ruby: // 手写 Hash
来源：http://ulx.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hwc.fktsv.cn

[N08] 生成全排列
来源：http://ott.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://uqw.nanxinkj.top

PHP:  // 手写递归交换
来源：http://ltp.fehbvm.com

JS:   // 手写回溯递归
来源：http://tsy.xylfe.cn

TS:   // 手写回溯递归
来源：http://cpa.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://ndh.sweek.top

Go:   // 手写回溯递归
来源：http://vdb.pycfn.com

Ruby: arr.permutation.to_a
来源：http://uac.zhengqikj.top

C#:   // 手写回溯递归
来源：http://hlj.yj20258888.top

[N09] 栈与队列
来源：http://fvb.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nrm.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nch.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://siw.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qbs.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wyz.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lyi.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wna.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ker.cdnleiting.top

[N10] 链表节点定义
来源：http://rrv.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ifs.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://phv.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vta.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yfu.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://ojv.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ewb.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://win.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ryn.yvedp.cn

[N11] 二叉树中序遍历
来源：http://azz.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wau.fengsongda.top

PHP:  // 手写递归函数
来源：http://cvr.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nni.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xln.hnxiangtu.top

Java: // 手写递归
来源：http://wrv.hfpthk.cn

Go:   // 手写递归
来源：http://cjs.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pfh.uphjek.com

C#:   // 手写递归
来源：http://wzd.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yfi.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bxv.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lgh.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kma.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gmv.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gkr.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://idh.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pbq.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hkc.xinyue.icu

================================================================================
来源：http://fte.guowangkeji.top

O. 并发与异步
来源：http://oxf.shanyushiyangtech.top

================================================================================
来源：http://tyu.zhongyouzk.top

[O01] 启动一个线程
来源：http://nzn.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dtj.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wwb.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zki.gzhubu.top

TS:   // 同 JS
来源：http://uyt.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://omc.shzxlz.cn

Go:   go f()
来源：http://jve.yongpay.top

Ruby: Thread.new { f }
来源：http://goe.fzhhl.top

C#:   Task.Run(() => F());
来源：http://ysg.xylfe.cn

[O02] 使用线程池
来源：http://uvs.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://urz.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://crd.daxiang520.top

JS:   // worker_threads 线程池
来源：http://rdc.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://stc.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://ycm.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gmk.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ehg.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://crc.wangdashe.top

[O03] 加锁保护共享数据
来源：http://gqm.cucudq.cn

Py:   with lock: shared += 1
来源：http://dgy.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://coo.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ouy.zhoulong.xyz

TS:   // 同 JS
来源：http://lfd.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://usq.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wzs.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://etd.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://ntx.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://yij.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://luj.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://owv.andypj.xyz

JS:   async function f() { await g(); }
来源：http://aex.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wbv.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zih.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zsl.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://raj.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://ppi.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://hqm.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://jra.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nym.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://pue.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://mdf.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwh.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tue.cashguo.top

Ruby: threads.map(&:join)
来源：http://xzi.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sts.aizwys.cn

[O06] 使用进程池
来源：http://okv.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mcj.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cqv.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://lov.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://ozb.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tob.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sjm.ydzc1.top

Ruby: // fork 块
来源：http://ebr.cqqwz.cn

C#:   Parallel.For
来源：http://agj.tanke756.top

================================================================================
来源：http://cfs.fzhhl.top

P. 常用工具函数
来源：http://xax.bjfxy.top

================================================================================
来源：http://fbn.dianchejie.cn

[P01] 生成 UUID
来源：http://pth.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://jfs.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qle.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://jgu.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://wyv.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://kgc.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://huy.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://ihl.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://eup.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://cbh.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qjj.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oyu.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mmt.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hhc.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eqe.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kdf.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lwu.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gdx.andypj.xyz

[P03] 生成短随机字符串
来源：http://wrq.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bsm.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rfa.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ube.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pms.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://utz.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iol.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iiv.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nxc.zhixingplan.top

[P04] 求长度
来源：http://htn.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwn.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yog.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://roz.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jum.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://kiv.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://sdy.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://oyl.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://txs.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://bmu.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wlv.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://olq.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://udu.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ojd.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uvy.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://kii.zhijiandao.cn

Ruby: a == b
来源：http://ixa.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://orz.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qoc.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lia.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://aid.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://npe.fktsv.cn

TS:   if (x == null) {}
来源：http://jjn.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tdw.chenlongwang.top

Go:   if x == nil {}
来源：http://ydk.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://adb.jinqigfzy.top

C#:   if (x is null) {}
来源：http://cuc.jinqigufen.top

[P07] 防抖与节流
来源：http://tdj.ydjk.org.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tng.guowangkeji.top


<!-- 参考信息 -->