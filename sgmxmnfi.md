代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfy.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://guo.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rwt.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kfd.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ezy.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qkb.meibo888.top

================================================================================
来源：http://lfc.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://efa.c1oappe.top

================================================================================
来源：http://drq.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://kpt.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://iho.sweek.top

PHP:  $argv;  $argc;
来源：http://sfj.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://trs.daxiang520.top

TS:   process.argv.slice(2)
来源：http://nsy.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://gtk.wangdashe.top

Go:   os.Args[1:]
来源：http://syr.jianghu66.top

Ruby: ARGV
来源：http://pmw.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://ymm.yueranfly.top

[M02] 读取环境变量
来源：http://nyf.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://zph.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://brj.zhixingplan.top

JS:   process.env.HOME
来源：http://kax.gaohongyu789.top

TS:   process.env.HOME
来源：http://lqq.dashuyun.cn

Java: System.getenv("HOME")
来源：http://ugx.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dwj.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://tia.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vcj.guowangkeji.top

[M03] 执行外部命令
来源：http://sii.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bvd.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jwb.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://efp.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://kmr.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bjb.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ibw.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://rjw.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://cki.ppjwa.cn

[M04] 获取当前工作目录
来源：http://dtv.aibaodan.cn

Py:   os.getcwd()
来源：http://oap.shangyingyoupin.top

PHP:  getcwd();
来源：http://ujt.uphjek.com

JS:   process.cwd()
来源：http://qcx.ydzc1.top

TS:   process.cwd()
来源：http://lms.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://fes.jlsjyb.cn

Go:   os.Getwd()
来源：http://gsk.bbcook.cn

Ruby: Dir.pwd
来源：http://ynp.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vft.jianghu66.top

[M05] 设置退出码
来源：http://icc.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://ogx.9152youxi.cn

PHP:  exit(1);
来源：http://wkx.nanxinkj.top

JS:   process.exit(1)
来源：http://lev.zhoulong.xyz

TS:   process.exit(1)
来源：http://uql.haohaochexian.top

Java: System.exit(1)
来源：http://oku.bjfxy.top

Go:   os.Exit(1)
来源：http://rki.iojbl.cn

Ruby: exit 1
来源：http://vei.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kcc.fzhhl.top

[M06] 向标准错误输出
来源：http://wzb.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://kbx.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jal.chenlongwang.top

JS:   console.error("err")
来源：http://vzy.kuanghao11.cn

TS:   console.error("err")
来源：http://ten.fktsv.cn

Java: System.err.println("err")
来源：http://ksm.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://szh.fanxiaobao.xyz

Ruby: warn "err"
来源：http://qmt.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://plj.redwolf501.top

[M07] 判断是否为主入口
来源：http://fqj.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://bja.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vlk.svipenyu.cn

JS:   require.main === module
来源：http://ncm.zdqjudy.top

TS:   require.main === module
来源：http://ovt.cheryme.top

Java: public static void main(String[] args)
来源：http://xrp.daxiang520.top

Go:   func main()
来源：http://uzh.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yxe.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://ref.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://nxb.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://bsc.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://net.jianghu66.top

JS:   process.platform;  process.version
来源：http://msw.vehdjk.com

TS:   process.platform;  process.version
来源：http://ckr.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fzw.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://opr.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zig.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iok.sufxvd.cn

================================================================================
来源：http://dtd.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://ors.kuanghao11.cn

================================================================================
来源：http://lgo.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://rwb.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://tsg.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kik.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zpd.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bge.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://poa.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://fur.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vst.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://qvi.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://lbh.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://rmj.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lkq.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ids.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zcu.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bfh.xuanzx.com

Go:   slices.Sort(arr)
来源：http://rmh.shuidangran.top

Ruby: arr.sort
来源：http://aqo.ydzc1.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hpe.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://tuo.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://njv.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://ucn.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eor.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mzu.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ozb.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wtc.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ons.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://tpc.shzxlz.cn

[N04] 斐波那契数列
来源：http://zup.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fcy.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yvy.ydzc1.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ykq.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oul.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hpi.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eqr.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mek.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ozk.uphjek.com

[N05] 最大公约数
来源：http://ozy.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://gue.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://evv.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxu.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://emw.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tyx.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qfm.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://tru.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ggz.shzxlz.cn

[N06] 判断回文字符串
来源：http://etw.fehbvm.com

Py:   s == s[::-1]
来源：http://kma.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://uwf.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://gst.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://tyb.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://owa.hnqzz.top

Go:   // 双指针从两端比较
来源：http://nts.jinqigufen.top

Ruby: s == s.reverse
来源：http://xnc.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cxk.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://iyr.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eil.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uso.daxiang520.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uxv.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://vvt.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://pay.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://ntu.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://nwc.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://idn.9152youxi.cn

[N08] 生成全排列
来源：http://wzg.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://zoh.sufxvd.cn

PHP:  // 手写递归交换
来源：http://eiu.yueranfly.top

JS:   // 手写回溯递归
来源：http://vva.yj20258888.top

TS:   // 手写回溯递归
来源：http://tyf.gzhubu.top

Java: // 手写回溯递归
来源：http://fvx.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://gmd.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://mry.gotoacloud.top

C#:   // 手写回溯递归
来源：http://ecu.ehwqpu.com

[N09] 栈与队列
来源：http://hfr.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ylv.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yzg.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nln.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yoe.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rks.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xkm.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lvs.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ser.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://xqs.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rxr.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cha.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mji.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eou.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://gzh.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://xkz.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sxo.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kdh.cucudq.cn

[N11] 二叉树中序遍历
来源：http://eyq.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://npa.yueranfly.top

PHP:  // 手写递归函数
来源：http://fxu.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sjk.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lqk.jianghu66.top

Java: // 手写递归
来源：http://yow.jinghuilouyu.cn

Go:   // 手写递归
来源：http://edc.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://utx.yvedp.cn

C#:   // 手写递归
来源：http://eoo.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iyy.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qiq.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cws.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wug.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgp.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hjg.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://prw.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kjp.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qwi.dashuyun.cn

================================================================================
来源：http://wcu.cucudq.cn

O. 并发与异步
来源：http://nvj.cucudq.cn

================================================================================
来源：http://tyv.chenlongwang.top

[O01] 启动一个线程
来源：http://rsz.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dkx.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vve.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vjl.cashguo.top

TS:   // 同 JS
来源：http://cmb.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://luu.yueranfly.top

Go:   go f()
来源：http://sch.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://jba.aizwys.cn

C#:   Task.Run(() => F());
来源：http://hml.gotoacloud.top

[O02] 使用线程池
来源：http://vsy.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oek.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://noi.guannengcc.top

JS:   // worker_threads 线程池
来源：http://equ.c1oappe.top

TS:   // worker_threads 线程池
来源：http://atg.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://sov.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjk.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://khr.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rhg.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://xtt.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://fiy.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://ijx.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mrd.dashuyun.cn

TS:   // 同 JS
来源：http://rwk.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://wac.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rqz.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xdb.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://ptf.fzhhl.top

[O04] 定义异步函数并等待
来源：http://kkr.cashguo.top

Py:   async def f():⏎    await g()
来源：http://gww.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vqc.tanke756.top

JS:   async function f() { await g(); }
来源：http://ohq.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nsc.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zei.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hhp.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jma.yongpay.top

C#:   async Task F() { await G(); }
来源：http://dnq.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://wtg.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://fos.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qth.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://ynv.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://sdy.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://muj.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tmn.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://gjk.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jsb.9152youxi.cn

[O06] 使用进程池
来源：http://fpq.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kbj.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tcv.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://efi.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://vpi.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rok.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sqa.9152youxi.cn

Ruby: // fork 块
来源：http://tzr.yuxming.cn

C#:   Parallel.For
来源：http://wjz.yuxming.cn

================================================================================
来源：http://rpq.dashuyun.cn

P. 常用工具函数
来源：http://sys.316326.xyz

================================================================================
来源：http://uka.wangshuangyany.cn

[P01] 生成 UUID
来源：http://lgx.tarul.cn

Py:   str(uuid.uuid4())
来源：http://zut.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mwn.xinyue.icu

JS:   crypto.randomUUID()
来源：http://wvi.fktsv.cn

TS:   crypto.randomUUID()
来源：http://grk.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://win.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://oqs.hammf.cn

Ruby: SecureRandom.uuid
来源：http://owm.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://inr.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://qak.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rdg.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xcx.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ype.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://clt.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pmo.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jdh.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jfs.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fqq.nwbrower.top

[P03] 生成短随机字符串
来源：http://mek.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qtt.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qvx.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eeb.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ubj.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qri.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ggx.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://hdj.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wtc.zhiwuduotai.top

[P04] 求长度
来源：http://zen.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://knf.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://egc.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vaz.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nhw.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://cun.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://yhv.cqqwz.cn

Ruby: x.length;  x.size
来源：http://tyk.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mfp.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://kul.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qft.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vtn.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://izz.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dwe.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xvf.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tns.epnwcf.com

Ruby: a == b
来源：http://qgy.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vml.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vfn.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uya.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://rby.shzxlz.cn


<!-- 参考信息 -->