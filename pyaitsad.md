代发 wailian999

JS:   process.argv.slice(2)
来源：http://qtg.mhx1999.top

TS:   process.argv.slice(2)
来源：http://zyb.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://qen.hysaishi.cn

Go:   os.Args[1:]
来源：http://sci.yj20258888.top

Ruby: ARGV
来源：http://lca.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://mjn.tian-w.cn

[M02] 读取环境变量
来源：http://blm.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://xso.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ulr.daria6918.cn

JS:   process.env.HOME
来源：http://myd.zycfv.cn

TS:   process.env.HOME
来源：http://xtj.sweek.top

Java: System.getenv("HOME")
来源：http://gsv.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sww.yfazqb.com

Ruby: ENV["HOME"]
来源：http://aal.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qeh.316326.xyz

[M03] 执行外部命令
来源：http://rti.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://myj.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tqp.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jjl.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://zmg.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kco.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://syu.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://htf.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://rep.mhx1999.top

[M04] 获取当前工作目录
来源：http://cto.zhiwuduotai.top

Py:   os.getcwd()
来源：http://uxy.daria6918.cn

PHP:  getcwd();
来源：http://ywu.aizwys.cn

JS:   process.cwd()
来源：http://iuz.gaohongyu789.top

TS:   process.cwd()
来源：http://reb.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://zfk.ivvv.top

Go:   os.Getwd()
来源：http://ryl.yueranfly.top

Ruby: Dir.pwd
来源：http://awc.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iyv.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://ibd.ctjpmb.com

Py:   sys.exit(1)
来源：http://hxl.yuxming.cn

PHP:  exit(1);
来源：http://lln.yj20258888.top

JS:   process.exit(1)
来源：http://qky.zhijiandao.cn

TS:   process.exit(1)
来源：http://njl.meibo888.top

Java: System.exit(1)
来源：http://egb.zhijiandao.cn

Go:   os.Exit(1)
来源：http://awx.9152youxi.cn

Ruby: exit 1
来源：http://azv.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://doh.hfpthk.cn

[M06] 向标准错误输出
来源：http://xti.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://hfb.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vvk.hywenlv.cn

JS:   console.error("err")
来源：http://koc.0kj1m.cn

TS:   console.error("err")
来源：http://tqj.iojbl.cn

Java: System.err.println("err")
来源：http://pqw.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvq.xinyue.icu

Ruby: warn "err"
来源：http://ghj.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://fmo.0kj1m.cn

[M07] 判断是否为主入口
来源：http://mdl.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://ogh.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://thh.snrcjt.cn

JS:   require.main === module
来源：http://bol.jyoumei.cn

TS:   require.main === module
来源：http://mpa.sxryk.cn

Java: public static void main(String[] args)
来源：http://eii.xuetiantiany.cn

Go:   func main()
来源：http://uxv.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ggn.pycfn.com

C#:   static void Main(string[] args)
来源：http://xxb.cheryme.top

[M08] 获取系统与运行时信息
来源：http://tms.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://cbl.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://fja.dashuyun.cn

JS:   process.platform;  process.version
来源：http://ayn.fzhhl.top

TS:   process.platform;  process.version
来源：http://uis.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dge.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vwk.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://maz.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xot.yueranfly.top

================================================================================
来源：http://vvn.cdnleiting.top

N. 数据结构与算法
来源：http://zgn.epnwcf.com

================================================================================
来源：http://tbt.316326.xyz

[N01] 二分查找（有序数组）
来源：http://kvb.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bes.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tyo.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dce.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmu.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://imm.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://bxn.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rfk.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qfp.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://syj.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ums.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sir.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vop.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uhs.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dau.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://vga.cashguo.top

Ruby: arr.sort
来源：http://mkh.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dam.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://new.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrj.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://xwe.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yey.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dxk.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ccd.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ohz.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://htk.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://xwk.shzxlz.cn

[N04] 斐波那契数列
来源：http://vxc.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cgj.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://svz.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://syz.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uuy.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iix.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://psd.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oef.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://anh.snrcjt.cn

[N05] 最大公约数
来源：http://qvs.mhx1999.top

Py:   math.gcd(a, b)
来源：http://tvj.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdy.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pol.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfu.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xzv.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hyv.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://xqj.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://efd.kuanghao11.cn

[N06] 判断回文字符串
来源：http://fmy.sysykeji.top

Py:   s == s[::-1]
来源：http://jgq.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://gho.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://phi.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://yhb.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mop.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://vli.dashuyun.cn

Ruby: s == s.reverse
来源：http://rrg.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nbw.havefunace.top

[N07] 两数之和（返回下标）
来源：http://typ.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qgn.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wjn.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://tei.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://whh.jyoumei.cn

Java: // 手写 HashMap
来源：http://viy.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://dca.sxryk.cn

Ruby: // 手写 Hash
来源：http://poq.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://amf.xylfe.cn

[N08] 生成全排列
来源：http://qaq.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://sad.gotoacloud.top

PHP:  // 手写递归交换
来源：http://eso.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://qcf.cashguo.top

TS:   // 手写回溯递归
来源：http://kxt.yuxming.cn

Java: // 手写回溯递归
来源：http://zfz.hysaishi.cn

Go:   // 手写回溯递归
来源：http://abx.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://nls.jiagoushi.top

C#:   // 手写回溯递归
来源：http://sho.cqqwz.cn

[N09] 栈与队列
来源：http://sbg.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ozk.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mpn.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qqd.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tjz.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kug.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zzc.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ojx.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wav.smart0.xyz

[N10] 链表节点定义
来源：http://ara.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kus.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tny.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cbl.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dlc.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://kim.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://kbj.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wkn.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://zzf.tarul.cn

[N11] 二叉树中序遍历
来源：http://cxv.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rua.tianlin.xyz

PHP:  // 手写递归函数
来源：http://sar.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fyg.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ump.hnqzz.top

Java: // 手写递归
来源：http://hcr.tian-w.cn

Go:   // 手写递归
来源：http://nmc.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://avj.chenzaomai.com

C#:   // 手写递归
来源：http://rue.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rtb.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hwg.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oqx.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sto.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ccf.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://erw.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dzy.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ota.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://snl.shangyingyoupin.top

================================================================================
来源：http://ryo.ctjpmb.com

O. 并发与异步
来源：http://aab.zhaomingkeji.xyz

================================================================================
来源：http://vft.gotoacloud.top

[O01] 启动一个线程
来源：http://xbq.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xmp.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zvl.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wdr.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://ehe.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://zds.vehdjk.com

Go:   go f()
来源：http://vhw.shuidangran.top

Ruby: Thread.new { f }
来源：http://kod.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://dtx.yuxming.cn

[O02] 使用线程池
来源：http://wbp.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pym.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lhl.ivvv.top

JS:   // worker_threads 线程池
来源：http://yeh.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://iuw.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zop.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jtx.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eqe.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qzo.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://trm.daria6918.cn

Py:   with lock: shared += 1
来源：http://ssp.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://qdr.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gxj.gaohongyu789.top

TS:   // 同 JS
来源：http://xpj.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://dcg.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://azu.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://esy.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://xvi.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://qua.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://wtl.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rcv.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://fbr.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbl.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yiw.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lnu.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://amj.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://lde.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://nce.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://thk.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://odb.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://ccu.yj202588.top

TS:   await Promise.all(tasks)
来源：http://ubf.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cys.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://owk.bjfxy.top

Ruby: threads.map(&:join)
来源：http://vcp.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://btx.fanxiaobao.xyz

[O06] 使用进程池
来源：http://gor.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://leb.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ncu.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://eoh.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://poz.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ywr.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://swh.jiagoushi.top

Ruby: // fork 块
来源：http://cpg.jqgfzy.top

C#:   Parallel.For
来源：http://cxc.yj20258888.top

================================================================================
来源：http://pis.smart0.xyz

P. 常用工具函数
来源：http://unx.redwolf501.top

================================================================================
来源：http://gud.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://uag.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://kdg.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xty.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://rkt.sweek.top

TS:   crypto.randomUUID()
来源：http://cor.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://lyi.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://irm.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://nif.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://uts.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://act.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rkq.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lnt.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iiw.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fke.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://umr.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wfv.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ktb.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bon.chenzaomai.com

[P03] 生成短随机字符串
来源：http://tcq.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dya.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xlu.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vsk.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oys.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qrw.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ejo.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xod.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rsl.tian-w.cn

[P04] 求长度
来源：http://ikz.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lhr.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mww.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlu.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xkj.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://mfl.zycfv.cn

Go:   len(arr);  len(m)
来源：http://hmn.iojbl.cn

Ruby: x.length;  x.size
来源：http://pgt.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hba.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://itw.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pbr.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ilg.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ggd.xziqi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nrn.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qsh.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vbz.pycfn.com

Ruby: a == b
来源：http://rnx.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqp.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cie.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ybs.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://znu.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yus.cucudq.cn

TS:   if (x == null) {}
来源：http://srk.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fji.cheryme.top

Go:   if x == nil {}
来源：http://dki.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hzm.hnxiangtu.top

C#:   if (x is null) {}
来源：http://lhu.iojbl.cn

[P07] 防抖与节流
来源：http://hqi.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ijv.316326.xyz

PHP:  // 手写时间戳比较
来源：http://mae.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zsu.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gji.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zoj.tanke756.top


<!-- 参考信息 -->