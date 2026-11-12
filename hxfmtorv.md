代发 wailian999

JS:   process.argv.slice(2)
来源：http://tzi.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://mst.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://nuz.epnwcf.com

Go:   os.Args[1:]
来源：http://nfl.vehdjk.com

Ruby: ARGV
来源：http://iei.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://swj.sxryk.cn

[M02] 读取环境变量
来源：http://yvg.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://yud.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vhf.ybcxt.top

JS:   process.env.HOME
来源：http://ysi.52xcode.cn

TS:   process.env.HOME
来源：http://kgq.ivvv.top

Java: System.getenv("HOME")
来源：http://qnu.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jxy.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://sex.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ell.guannengcc.top

[M03] 执行外部命令
来源：http://ohm.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bks.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://exy.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://yyl.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxd.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jlc.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hqc.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uen.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://cbi.cucudq.cn

[M04] 获取当前工作目录
来源：http://wce.shzxlz.cn

Py:   os.getcwd()
来源：http://ifm.sysykeji.top

PHP:  getcwd();
来源：http://zkp.fzhhl.top

JS:   process.cwd()
来源：http://agv.tian-w.cn

TS:   process.cwd()
来源：http://qct.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://jvz.ydjk.org.cn

Go:   os.Getwd()
来源：http://leu.ybcxt.top

Ruby: Dir.pwd
来源：http://nul.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://rpx.fanxiaobao.xyz

[M05] 设置退出码
来源：http://jmq.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://pxq.vehdjk.com

PHP:  exit(1);
来源：http://sgd.haohaochexian.top

JS:   process.exit(1)
来源：http://qnb.jlsjyb.cn

TS:   process.exit(1)
来源：http://oiy.dianchejie.cn

Java: System.exit(1)
来源：http://fex.zdqjudy.top

Go:   os.Exit(1)
来源：http://xcg.hammf.cn

Ruby: exit 1
来源：http://oxl.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fdx.jianghu66.top

[M06] 向标准错误输出
来源：http://nty.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://ssm.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eii.0kj1m.cn

JS:   console.error("err")
来源：http://cix.havefunace.top

TS:   console.error("err")
来源：http://uvs.nanxinkj.top

Java: System.err.println("err")
来源：http://wms.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bkz.hnxiangtu.top

Ruby: warn "err"
来源：http://dhp.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://opl.meibo888.top

[M07] 判断是否为主入口
来源：http://sjw.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://qdb.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ppu.wangshuangyany.cn

JS:   require.main === module
来源：http://vmp.smart0.xyz

TS:   require.main === module
来源：http://kqh.chenlongwang.top

Java: public static void main(String[] args)
来源：http://cra.smart0.xyz

Go:   func main()
来源：http://gen.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pbw.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://saf.yonumen.top

[M08] 获取系统与运行时信息
来源：http://aad.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://hik.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://evq.ehwqpu.com

JS:   process.platform;  process.version
来源：http://irl.yfazqb.com

TS:   process.platform;  process.version
来源：http://tuu.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mxc.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aes.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aoo.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nak.quarkkingdee.top

================================================================================
来源：http://iqy.aizwys.cn

N. 数据结构与算法
来源：http://lkn.bjfxy.top

================================================================================
来源：http://qul.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://hep.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://bbl.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fvc.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lux.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yrg.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://nlo.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://jka.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iul.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://gea.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://bls.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://wpu.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ony.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eqa.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pun.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bds.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://acx.c1oappe.top

Ruby: arr.sort
来源：http://isu.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wpu.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://brm.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xqs.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://lpx.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gav.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://atl.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lld.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kng.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hyt.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://zsb.hysaishi.cn

[N04] 斐波那契数列
来源：http://ikh.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aff.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mex.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xqa.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djn.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yan.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zey.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://swq.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hmt.jyoumei.cn

[N05] 最大公约数
来源：http://rfk.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://xjq.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zhj.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wwf.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://irj.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qwr.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ghr.sweek.top

Ruby: a.gcd(b)
来源：http://acb.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sle.yongpay.top

[N06] 判断回文字符串
来源：http://lpt.vqdsnc.cn

Py:   s == s[::-1]
来源：http://ufu.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://bpz.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://ezy.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://txn.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rhz.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://gtc.xziqi.cn

Ruby: s == s.reverse
来源：http://thh.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uom.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://tjy.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kmz.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqr.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ari.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://avm.tarul.cn

Java: // 手写 HashMap
来源：http://kra.sweek.top

Go:   // 手写 map[int]int
来源：http://mtp.pycfn.com

Ruby: // 手写 Hash
来源：http://upz.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wfs.fktsv.cn

[N08] 生成全排列
来源：http://sxk.tanke756.top

Py:   itertools.permutations(arr)
来源：http://lsw.iojbl.cn

PHP:  // 手写递归交换
来源：http://vhe.yangfankeji.com

JS:   // 手写回溯递归
来源：http://nec.zhixingplan.top

TS:   // 手写回溯递归
来源：http://gvy.yanxiufei.cn

Java: // 手写回溯递归
来源：http://qow.yvedp.cn

Go:   // 手写回溯递归
来源：http://mjr.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://sdl.hesvh.cn

C#:   // 手写回溯递归
来源：http://qyy.bjfxy.top

[N09] 栈与队列
来源：http://smm.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://acf.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xgi.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eln.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vws.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xwc.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tat.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ybi.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jjk.ctjpmb.com

[N10] 链表节点定义
来源：http://hnx.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://scd.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fvz.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pok.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ddk.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://trq.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://wew.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://bjw.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://zgz.epnwcf.com

[N11] 二叉树中序遍历
来源：http://snd.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cnr.aibaodan.cn

PHP:  // 手写递归函数
来源：http://kqv.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://slt.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgf.yj202588.top

Java: // 手写递归
来源：http://qpw.xziqi.cn

Go:   // 手写递归
来源：http://bmh.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wtq.xziqi.cn

C#:   // 手写递归
来源：http://ccf.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ell.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kwx.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zfc.jqgfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ldj.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://odr.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qxg.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pbl.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hgm.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yho.yj20258888.top

================================================================================
来源：http://zjp.kuanghao11.cn

O. 并发与异步
来源：http://xwj.daxiang520.top

================================================================================
来源：http://xxa.fzhhl.top

[O01] 启动一个线程
来源：http://dyt.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xps.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jje.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cnn.jianghu66.top

TS:   // 同 JS
来源：http://hiz.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://jlc.xingfuxueyuan.xyz

Go:   go f()
来源：http://ola.jqgfzy.top

Ruby: Thread.new { f }
来源：http://rnh.ivvv.top

C#:   Task.Run(() => F());
来源：http://qti.birdmap.top

[O02] 使用线程池
来源：http://hwy.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wjk.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lbw.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://uho.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://lnr.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://xrr.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kho.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dwp.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kis.epnwcf.com

[O03] 加锁保护共享数据
来源：http://hyf.hcnkem.com

Py:   with lock: shared += 1
来源：http://eiu.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://dab.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lhf.ivvv.top

TS:   // 同 JS
来源：http://doz.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://oth.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://btx.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zht.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://gxg.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://xfk.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://egy.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyw.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://fzb.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fud.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hrd.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vvw.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://uky.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://rxs.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://ggv.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://fvk.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ora.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://ypy.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://otf.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xop.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mnt.fehbvm.com

Ruby: threads.map(&:join)
来源：http://trv.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vbs.shanyushiyangtech.top

[O06] 使用进程池
来源：http://tjk.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cot.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pxd.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://btr.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://vhi.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tpn.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zcm.shzxlz.cn

Ruby: // fork 块
来源：http://kbf.zhengqikj.top

C#:   Parallel.For
来源：http://pae.fehbvm.com

================================================================================
来源：http://hsn.chenzaomai.com

P. 常用工具函数
来源：http://soz.zhaomingkeji.xyz

================================================================================
来源：http://mtz.feifeiyinyue.top

[P01] 生成 UUID
来源：http://fnr.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://rsz.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tgj.daria6918.cn

JS:   crypto.randomUUID()
来源：http://zeb.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://wpz.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://qyn.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://gwm.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://vbl.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://qpz.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://qsb.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oax.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wbv.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nal.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ile.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tat.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tew.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kyq.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwu.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://cur.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://twu.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rfd.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://leh.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wxq.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gos.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dxr.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ifu.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gnr.xuetiantiany.cn

[P04] 求长度
来源：http://bkf.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gmn.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sty.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wyb.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wsf.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://nvu.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://sbs.ydzc1.top

Ruby: x.length;  x.size
来源：http://zjs.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iff.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://xdp.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ekg.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xek.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysp.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zwg.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://epu.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uef.sweek.top

Ruby: a == b
来源：http://wal.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xak.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cfk.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kki.316326.xyz

PHP:  if (empty($x)) {}
来源：http://ihp.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgb.yj20258888.top

TS:   if (x == null) {}
来源：http://bev.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kra.xylfe.cn

Go:   if x == nil {}
来源：http://ana.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iyq.yueranfly.top

C#:   if (x is null) {}
来源：http://ier.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://gqt.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duh.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://tsz.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swt.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vjw.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://apr.sxryk.cn


<!-- 参考信息 -->