代发 wailian999

================================================================================
来源：http://sig.jinqigufen.top

[M01] 读取命令行参数
来源：http://muv.ydzc1.top

Py:   sys.argv[1:]
来源：http://poj.meibo888.top

PHP:  $argv;  $argc;
来源：http://zxj.sxryk.cn

JS:   process.argv.slice(2)
来源：http://fcu.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://lpb.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://hkv.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://ynl.zhaomingkeji.xyz

Ruby: ARGV
来源：http://nit.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://csv.ivvv.top

[M02] 读取环境变量
来源：http://efp.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://poq.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kbr.hywenlv.cn

JS:   process.env.HOME
来源：http://pdn.yj20258888.top

TS:   process.env.HOME
来源：http://cyy.xinyue.icu

Java: System.getenv("HOME")
来源：http://arp.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://frp.tarul.cn

Ruby: ENV["HOME"]
来源：http://ygo.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ivf.gaohongyu789.top

[M03] 执行外部命令
来源：http://nez.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzi.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hhi.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://chc.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://osa.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oqb.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jqm.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://vsd.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://qtn.zhixingplan.top

[M04] 获取当前工作目录
来源：http://ibr.jqgfzy.top

Py:   os.getcwd()
来源：http://jap.yj20258888.top

PHP:  getcwd();
来源：http://ucg.zhijiandao.cn

JS:   process.cwd()
来源：http://dzg.fengsongda.top

TS:   process.cwd()
来源：http://ulq.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://mtj.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://iyp.aizwys.cn

Ruby: Dir.pwd
来源：http://hfa.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://qrm.ydjk.org.cn

[M05] 设置退出码
来源：http://qea.aizwys.cn

Py:   sys.exit(1)
来源：http://bzs.fengsongda.top

PHP:  exit(1);
来源：http://nvr.fehbvm.com

JS:   process.exit(1)
来源：http://kmb.tian-w.cn

TS:   process.exit(1)
来源：http://kpw.hammf.cn

Java: System.exit(1)
来源：http://kjh.kuanghao11.cn

Go:   os.Exit(1)
来源：http://vje.andypj.xyz

Ruby: exit 1
来源：http://ocq.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vtm.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://qoz.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://jin.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://evj.sxryk.cn

JS:   console.error("err")
来源：http://fjm.xuanzx.com

TS:   console.error("err")
来源：http://jea.guannengcc.top

Java: System.err.println("err")
来源：http://zby.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zhx.daxiang520.top

Ruby: warn "err"
来源：http://ooc.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://eop.zhixingplan.top

[M07] 判断是否为主入口
来源：http://ryg.pycfn.com

Py:   if __name__ == "__main__":
来源：http://lvg.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hbm.yvedp.cn

JS:   require.main === module
来源：http://pvf.zhijiandao.cn

TS:   require.main === module
来源：http://rvu.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://pkk.tanke756.top

Go:   func main()
来源：http://onu.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zsp.tanke756.top

C#:   static void Main(string[] args)
来源：http://lum.birdmap.top

[M08] 获取系统与运行时信息
来源：http://rau.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://mjm.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://tvf.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://ozh.0kj1m.cn

TS:   process.platform;  process.version
来源：http://dsb.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lln.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eio.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://avh.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qxy.pycfn.com

================================================================================
来源：http://ozo.hywenlv.cn

N. 数据结构与算法
来源：http://ofe.yangfankeji.com

================================================================================
来源：http://npa.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://qmo.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dpv.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ypb.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cud.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjh.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://cxx.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://woa.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://unu.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jme.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://kkb.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://xif.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tvo.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://prh.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjc.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tcf.yj20258.top

Go:   slices.Sort(arr)
来源：http://xsf.zhixingplan.top

Ruby: arr.sort
来源：http://gwz.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rhg.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://elo.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pal.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://jqw.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esi.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfj.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ikr.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qho.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mvj.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jdb.uphjek.com

[N04] 斐波那契数列
来源：http://hck.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tbm.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ksw.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://agu.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abh.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bhc.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ros.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hjo.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uho.xuanzx.com

[N05] 最大公约数
来源：http://kjd.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://qtr.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://znt.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rrv.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bmv.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xkr.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://twr.smart0.xyz

Ruby: a.gcd(b)
来源：http://gte.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://irq.kuanghao11.cn

[N06] 判断回文字符串
来源：http://mqn.hesvh.cn

Py:   s == s[::-1]
来源：http://hrh.uphjek.com

PHP:  $s === strrev($s);
来源：http://rkk.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://bnk.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://fyu.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jiv.yonumen.top

Go:   // 双指针从两端比较
来源：http://nfv.zhongyouzk.top

Ruby: s == s.reverse
来源：http://fbg.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fel.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://sun.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://orn.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xrs.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gha.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://jwt.hcnkem.com

Java: // 手写 HashMap
来源：http://ruy.yonumen.top

Go:   // 手写 map[int]int
来源：http://eea.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://htj.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cgo.yueranfly.top

[N08] 生成全排列
来源：http://mqj.yj20258.top

Py:   itertools.permutations(arr)
来源：http://uke.jqgfzy.top

PHP:  // 手写递归交换
来源：http://bia.cheryme.top

JS:   // 手写回溯递归
来源：http://upl.svipenyu.cn

TS:   // 手写回溯递归
来源：http://bdt.dashuyun.cn

Java: // 手写回溯递归
来源：http://rml.yonumen.top

Go:   // 手写回溯递归
来源：http://fqz.cheryme.top

Ruby: arr.permutation.to_a
来源：http://tsx.haohaochexian.top

C#:   // 手写回溯递归
来源：http://ptl.jiagoushi.top

[N09] 栈与队列
来源：http://itc.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mvf.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bmd.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kii.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://muq.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kss.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xoe.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rvs.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rbm.smart0.xyz

[N10] 链表节点定义
来源：http://kzc.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://suk.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dde.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rgo.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bgm.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://pgi.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://gix.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jir.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://icf.fzhhl.top

[N11] 二叉树中序遍历
来源：http://dnt.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jbp.cqqwz.cn

PHP:  // 手写递归函数
来源：http://jmo.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kma.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccr.vehdjk.com

Java: // 手写递归
来源：http://xly.ctjpmb.com

Go:   // 手写递归
来源：http://dkn.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wqk.yj20258888.top

C#:   // 手写递归
来源：http://tzr.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rpj.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pds.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://njq.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fus.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzq.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ycl.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fyc.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vyt.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oqc.dashuyun.cn

================================================================================
来源：http://hds.hammf.cn

O. 并发与异步
来源：http://zjr.yvedp.cn

================================================================================
来源：http://xgm.wangshuangyany.cn

[O01] 启动一个线程
来源：http://tzx.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mmv.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ggs.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uek.yonumen.top

TS:   // 同 JS
来源：http://ius.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://mit.zhaomingkeji.xyz

Go:   go f()
来源：http://pvm.aibaodan.cn

Ruby: Thread.new { f }
来源：http://gfg.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://tzh.nwbrower.top

[O02] 使用线程池
来源：http://mwy.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gzg.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zfv.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://kyn.sxryk.cn

TS:   // worker_threads 线程池
来源：http://kkh.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://frc.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zje.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ung.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yrx.xinyue.icu

[O03] 加锁保护共享数据
来源：http://uja.c1oappe.top

Py:   with lock: shared += 1
来源：http://tpn.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://squ.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vdx.jinqigfzy.top

TS:   // 同 JS
来源：http://zth.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://tpy.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xah.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://akz.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://omc.uphjek.com

[O04] 定义异步函数并等待
来源：http://jxw.yongpay.top

Py:   async def f():⏎    await g()
来源：http://qdm.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bnb.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://bej.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://epd.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gdd.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gyi.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hyo.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://scr.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://zgq.yongpay.top

Py:   asyncio.gather(*tasks)
来源：http://ebj.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://msh.sweek.top

JS:   await Promise.all(tasks)
来源：http://hor.birdmap.top

TS:   await Promise.all(tasks)
来源：http://ltu.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wan.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pog.yueranfly.top

Ruby: threads.map(&:join)
来源：http://pxa.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vyf.ehwqpu.com

[O06] 使用进程池
来源：http://byx.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ouc.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://upl.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://cpy.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://jak.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vzm.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gkw.nanxuanxn.top

Ruby: // fork 块
来源：http://fml.feifeiyinyue.top

C#:   Parallel.For
来源：http://hms.nwbrower.top

================================================================================
来源：http://olr.shanyushiyangkeji.top

P. 常用工具函数
来源：http://dwi.zdqjudy.top

================================================================================
来源：http://lzz.smart0.xyz

[P01] 生成 UUID
来源：http://qin.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://tcj.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qrq.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://vtd.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://wvo.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://zqd.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://txs.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://emq.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://qxw.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://ick.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bsl.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oyw.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ftj.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hlg.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://evs.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dbk.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mxv.zhaomingkeji.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://job.cqqwz.cn

[P03] 生成短随机字符串
来源：http://kix.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aqe.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jwf.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bdb.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfj.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gnu.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xdv.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dtx.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jja.hammf.cn

[P04] 求长度
来源：http://uwj.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://anr.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibj.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pws.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ttl.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://uiu.wangdashe.top

Go:   len(arr);  len(m)
来源：http://hzk.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://hvz.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sso.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://vxx.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zqh.jqgufenzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ovx.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://raf.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wcs.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ccx.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://agt.0kj1m.cn

Ruby: a == b
来源：http://mzc.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wgz.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aiv.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fxh.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://lgu.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://joe.bbcook.cn

TS:   if (x == null) {}
来源：http://fyu.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ilv.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://hon.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iek.ybcxt.top

C#:   if (x is null) {}
来源：http://gak.hongshengwenyu.top

[P07] 防抖与节流
来源：http://zao.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bfh.cqqwz.cn


<!-- 参考信息 -->