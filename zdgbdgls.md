代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dua.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jzi.nanxinkj.top

================================================================================
来源：http://qlo.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://aga.jianghu66.top

================================================================================
来源：http://ska.tanke756.top

[M01] 读取命令行参数
来源：http://utd.sweek.top

Py:   sys.argv[1:]
来源：http://gsv.uphjek.com

PHP:  $argv;  $argc;
来源：http://kfz.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://els.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://hyz.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://gdo.nanxuanxn.top

Go:   os.Args[1:]
来源：http://iet.jinqigufen.top

Ruby: ARGV
来源：http://cwn.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://uuq.jlsjyb.cn

[M02] 读取环境变量
来源：http://xwx.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://dau.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oyi.sjlbkw.cn

JS:   process.env.HOME
来源：http://rmv.bbcook.cn

TS:   process.env.HOME
来源：http://zgs.zycfv.cn

Java: System.getenv("HOME")
来源：http://rjc.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ocm.yvedp.cn

Ruby: ENV["HOME"]
来源：http://obh.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cqy.ybcxt.top

[M03] 执行外部命令
来源：http://uhu.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uep.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tbu.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ori.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vxo.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mly.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nvg.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://gea.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://asa.yangfankeji.com

[M04] 获取当前工作目录
来源：http://qfy.yvedp.cn

Py:   os.getcwd()
来源：http://cwl.uphjek.com

PHP:  getcwd();
来源：http://kqv.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://zta.feifeiyinyue.top

TS:   process.cwd()
来源：http://vyw.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://gvt.yueranfly.top

Go:   os.Getwd()
来源：http://kfx.c1oappe.top

Ruby: Dir.pwd
来源：http://zwx.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://upx.cdnleiting.top

[M05] 设置退出码
来源：http://vkq.bjfxy.top

Py:   sys.exit(1)
来源：http://uxx.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://fed.havefunace.top

JS:   process.exit(1)
来源：http://hmj.ivvv.top

TS:   process.exit(1)
来源：http://jux.ybcxt.top

Java: System.exit(1)
来源：http://kjl.svipenyu.cn

Go:   os.Exit(1)
来源：http://idz.fanxiaobao.xyz

Ruby: exit 1
来源：http://lkh.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tgj.quarkkingdee.top

[M06] 向标准错误输出
来源：http://pub.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://ltv.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dvf.nanxinkj.top

JS:   console.error("err")
来源：http://xqx.chenjidiqi.icu

TS:   console.error("err")
来源：http://iki.tianlin.xyz

Java: System.err.println("err")
来源：http://xzl.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kkn.hywenlv.cn

Ruby: warn "err"
来源：http://kqx.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://dwr.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://aux.gaohongyu789.top

Py:   if __name__ == "__main__":
来源：http://nmv.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hlj.mhx1999.top

JS:   require.main === module
来源：http://qzd.haohaochexian.top

TS:   require.main === module
来源：http://nvb.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://gyo.jinqigfzy.top

Go:   func main()
来源：http://lmo.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yib.ybcxt.top

C#:   static void Main(string[] args)
来源：http://mra.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://dqp.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://bww.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://oqf.fktsv.cn

JS:   process.platform;  process.version
来源：http://zco.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://xkr.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rnt.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qll.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dyd.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gsr.gotoacloud.top

================================================================================
来源：http://kuu.kuanghao11.cn

N. 数据结构与算法
来源：http://imu.zhoulong.xyz

================================================================================
来源：http://cvl.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://qgw.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://mmt.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mxe.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zuu.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ewa.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://dez.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://dvy.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dzr.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://ldj.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://hyt.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://kyn.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rwu.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mig.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://avc.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hyt.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://kfj.hywenlv.cn

Ruby: arr.sort
来源：http://gun.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ofr.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://lit.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wml.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://wbh.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gya.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppi.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rgz.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cug.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://joz.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tlc.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://rdf.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xlw.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ssw.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxw.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cdp.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bmd.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sfm.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jkk.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qqc.c1oappe.top

[N05] 最大公约数
来源：http://eys.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://osi.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xlp.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tft.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xol.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rnk.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nbi.pycfn.com

Ruby: a.gcd(b)
来源：http://vfm.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jra.tanke756.top

[N06] 判断回文字符串
来源：http://vfz.iojbl.cn

Py:   s == s[::-1]
来源：http://wii.ybcxt.top

PHP:  $s === strrev($s);
来源：http://byc.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://kbu.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://sts.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://agn.ivvv.top

Go:   // 双指针从两端比较
来源：http://wus.meibo888.top

Ruby: s == s.reverse
来源：http://qdw.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://pyu.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://edw.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://spa.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ace.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://spk.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://gsf.hnqzz.top

Java: // 手写 HashMap
来源：http://laq.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://nph.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://sfz.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://efx.redwolf501.top

[N08] 生成全排列
来源：http://dff.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://reo.andypj.xyz

PHP:  // 手写递归交换
来源：http://wha.yongpay.top

JS:   // 手写回溯递归
来源：http://rrw.snrcjt.cn

TS:   // 手写回溯递归
来源：http://hxv.ydjk.org.cn

Java: // 手写回溯递归
来源：http://gcj.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://hdq.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://osx.guowangkeji.top

C#:   // 手写回溯递归
来源：http://kmk.smart0.xyz

[N09] 栈与队列
来源：http://mlh.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jvu.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tpt.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://arh.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qqk.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aqr.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://acb.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dlw.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dbu.bjfxy.top

[N10] 链表节点定义
来源：http://oia.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iaj.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oii.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pvs.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://buu.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://ldy.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lme.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nbe.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ndt.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://ovr.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ddg.sweek.top

PHP:  // 手写递归函数
来源：http://vfd.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgm.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hbt.quarkkingdee.top

Java: // 手写递归
来源：http://cdl.sweek.top

Go:   // 手写递归
来源：http://yfi.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqv.dianchejie.cn

C#:   // 手写递归
来源：http://xwy.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eec.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://all.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mtt.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mgb.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sgu.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eox.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lvi.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://shy.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hft.cucudq.cn

================================================================================
来源：http://xxo.hnqzz.top

O. 并发与异步
来源：http://egs.shangyingyoupin.top

================================================================================
来源：http://bpf.kuanghao11.cn

[O01] 启动一个线程
来源：http://edl.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qml.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pcz.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ujw.sxryk.cn

TS:   // 同 JS
来源：http://xbp.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://pna.cucudq.cn

Go:   go f()
来源：http://slo.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://oqu.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://yoy.ctjpmb.com

[O02] 使用线程池
来源：http://daz.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ucq.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aem.yj202588.top

JS:   // worker_threads 线程池
来源：http://feu.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://exq.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://bhe.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://doo.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yjo.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ibq.andypj.xyz

[O03] 加锁保护共享数据
来源：http://xgp.yvedp.cn

Py:   with lock: shared += 1
来源：http://kpb.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://one.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jvl.zycfv.cn

TS:   // 同 JS
来源：http://afb.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://kga.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ujk.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sgh.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://tue.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://imr.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://nvy.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhb.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://tyc.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lzy.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fji.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bgx.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://cnr.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://xml.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://ejq.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://jrs.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mpp.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://cyq.sweek.top

TS:   await Promise.all(tasks)
来源：http://gup.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nnn.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kjd.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://pfh.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://wvl.quarkkingdee.top

[O06] 使用进程池
来源：http://buz.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rgq.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bou.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://raf.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://rrh.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://anc.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uht.ehwqpu.com

Ruby: // fork 块
来源：http://mht.shzxlz.cn

C#:   Parallel.For
来源：http://tbo.nanxuanxn.top

================================================================================
来源：http://qxa.sxryk.cn

P. 常用工具函数
来源：http://tgv.aizwys.cn

================================================================================
来源：http://mdr.hcnkem.com

[P01] 生成 UUID
来源：http://htt.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://qwa.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ugo.fengsongda.top

JS:   crypto.randomUUID()
来源：http://zrn.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://dsw.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://hmy.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://cfj.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://soh.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://ezd.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://fhj.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xga.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dgr.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jis.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pbw.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fxm.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bkn.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mus.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cth.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://fei.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mii.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://unr.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://riv.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pad.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blv.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jfl.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://doy.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gaa.jqgufenzy.top

[P04] 求长度
来源：http://qno.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zre.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://avm.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ivm.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oge.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://iev.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://vzi.guowangkeji.top

Ruby: x.length;  x.size
来源：http://lpb.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://yhr.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://pww.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wqd.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ova.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tmr.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vmm.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ezp.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fss.hnqzz.top

Ruby: a == b
来源：http://dlq.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://szv.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fen.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cjf.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://uvr.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wsh.vehdjk.com

TS:   if (x == null) {}
来源：http://gum.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://qep.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://xgg.yuxming.cn


<!-- 参考信息 -->