代发 wailian999

JS:   process.argv.slice(2)
来源：http://adz.yonumen.top

TS:   process.argv.slice(2)
来源：http://nua.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://meb.epnwcf.com

Go:   os.Args[1:]
来源：http://yjk.iojbl.cn

Ruby: ARGV
来源：http://foo.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://wkj.chenzaomai.com

[M02] 读取环境变量
来源：http://ozp.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://vtx.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jgw.svipenyu.cn

JS:   process.env.HOME
来源：http://gbp.jinqigufen.top

TS:   process.env.HOME
来源：http://grr.gogol.net.cn

Java: System.getenv("HOME")
来源：http://stf.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jen.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://ajx.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ugs.snrcjt.cn

[M03] 执行外部命令
来源：http://hav.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ndg.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jeu.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aku.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yju.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cjc.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pyl.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://uyq.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://igf.daxiang520.top

[M04] 获取当前工作目录
来源：http://qbg.zdqjudy.top

Py:   os.getcwd()
来源：http://fgr.cashguo.top

PHP:  getcwd();
来源：http://xhb.chenjidiqi.icu

JS:   process.cwd()
来源：http://gxi.aibaodan.cn

TS:   process.cwd()
来源：http://icr.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://uql.yj202588.top

Go:   os.Getwd()
来源：http://pkk.mhx1999.top

Ruby: Dir.pwd
来源：http://heu.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://dtb.wangshuangyany.cn

[M05] 设置退出码
来源：http://lwk.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://gvo.gotoacloud.top

PHP:  exit(1);
来源：http://pae.wangdashe.top

JS:   process.exit(1)
来源：http://jcu.tianlin.xyz

TS:   process.exit(1)
来源：http://hil.hesvh.cn

Java: System.exit(1)
来源：http://lpp.hammf.cn

Go:   os.Exit(1)
来源：http://fwg.ybcxt.top

Ruby: exit 1
来源：http://haf.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://enr.0kj1m.cn

[M06] 向标准错误输出
来源：http://iqz.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://rks.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ban.daxiang520.top

JS:   console.error("err")
来源：http://ngd.gzhubu.top

TS:   console.error("err")
来源：http://vcn.chenlongwang.top

Java: System.err.println("err")
来源：http://exn.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pmc.vqdsnc.cn

Ruby: warn "err"
来源：http://lnk.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://avx.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://rrz.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://jge.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eeu.jqgfzy.top

JS:   require.main === module
来源：http://por.hfpthk.cn

TS:   require.main === module
来源：http://flj.xinyue.icu

Java: public static void main(String[] args)
来源：http://ddf.xingfuxueyuan.xyz

Go:   func main()
来源：http://aqc.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://for.sysykeji.top

C#:   static void Main(string[] args)
来源：http://joi.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://gky.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://uqg.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://qkp.fehbvm.com

JS:   process.platform;  process.version
来源：http://lhm.iojbl.cn

TS:   process.platform;  process.version
来源：http://tdv.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oec.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://trt.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zpl.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dvb.haohaochexian.top

================================================================================
来源：http://yjf.tarul.cn

N. 数据结构与算法
来源：http://cqi.yuxming.cn

================================================================================
来源：http://gng.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://uxx.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qen.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yut.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://psp.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bjn.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://opd.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://ptt.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://nsp.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vhf.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://xwl.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://asy.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pou.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://waz.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bjp.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vfy.andypj.xyz

Go:   slices.Sort(arr)
来源：http://hhi.dianchejie.cn

Ruby: arr.sort
来源：http://dtx.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://juo.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://khw.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dik.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://mjn.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xry.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nvo.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vsy.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://toq.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xqv.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://duc.hywenlv.cn

[N04] 斐波那契数列
来源：http://htt.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lvt.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://klq.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opw.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://psl.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qid.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fff.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cin.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tqt.tianlin.xyz

[N05] 最大公约数
来源：http://mfo.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://xjm.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iop.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jqr.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wqc.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://adc.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qrx.jianghu66.top

Ruby: a.gcd(b)
来源：http://hxm.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oli.ctjpmb.com

[N06] 判断回文字符串
来源：http://xow.yfazqb.com

Py:   s == s[::-1]
来源：http://njp.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://gxo.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://fjf.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://sdv.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jgb.xylfe.cn

Go:   // 双指针从两端比较
来源：http://yas.gotoacloud.top

Ruby: s == s.reverse
来源：http://awv.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rqm.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://psf.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tri.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gdx.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://onl.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://wym.yj20258888.top

Java: // 手写 HashMap
来源：http://aug.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://psf.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://jdf.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hyd.cheryme.top

[N08] 生成全排列
来源：http://ejc.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://swh.yuxming.cn

PHP:  // 手写递归交换
来源：http://ybz.yj20258888.top

JS:   // 手写回溯递归
来源：http://ryn.yonumen.top

TS:   // 手写回溯递归
来源：http://giv.pycfn.com

Java: // 手写回溯递归
来源：http://dni.ehwqpu.com

Go:   // 手写回溯递归
来源：http://qzd.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://xxa.ybcxt.top

C#:   // 手写回溯递归
来源：http://ypd.daxiang520.top

[N09] 栈与队列
来源：http://pyo.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yuy.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baf.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aki.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rbq.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fgk.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wnq.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://czy.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aop.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://lbw.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tgz.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nsp.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vsr.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://djx.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://uhq.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://wxx.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://myf.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ixv.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://djq.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kjl.c1oappe.top

PHP:  // 手写递归函数
来源：http://qfv.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tcm.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dsx.iojbl.cn

Java: // 手写递归
来源：http://vch.sjlbkw.cn

Go:   // 手写递归
来源：http://wsk.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mvy.zhongyouzk.top

C#:   // 手写递归
来源：http://jqc.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://thz.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wfv.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dop.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fna.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tpi.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://loq.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zrr.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dua.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ztg.birdmap.top

================================================================================
来源：http://yhv.jinqigufen.top

O. 并发与异步
来源：http://wrk.nwbrower.top

================================================================================
来源：http://uvu.xziqi.cn

[O01] 启动一个线程
来源：http://fgi.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zdg.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bml.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pxd.wangdashe.top

TS:   // 同 JS
来源：http://pvs.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://cyf.cashguo.top

Go:   go f()
来源：http://oqs.ydzc1.top

Ruby: Thread.new { f }
来源：http://ccc.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://csz.redwolf501.top

[O02] 使用线程池
来源：http://pra.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xqx.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cde.pycfn.com

JS:   // worker_threads 线程池
来源：http://iye.ydzc1.top

TS:   // worker_threads 线程池
来源：http://jfl.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dsu.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://khk.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://llz.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://czz.sweek.top

[O03] 加锁保护共享数据
来源：http://jpw.bjfxy.top

Py:   with lock: shared += 1
来源：http://hpn.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://aej.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zeh.havefunace.top

TS:   // 同 JS
来源：http://ics.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://fjl.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sct.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gjy.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://chy.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://jvz.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://lcc.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sla.meibo888.top

JS:   async function f() { await g(); }
来源：http://qxs.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://khy.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hvf.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pft.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jwl.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://mwq.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://hgw.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://ila.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vqm.uphjek.com

JS:   await Promise.all(tasks)
来源：http://ilk.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://tsj.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wlv.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mna.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://cxx.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gtp.jinqigfzy.top

[O06] 使用进程池
来源：http://fmf.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yme.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mnn.hammf.cn

JS:   // child_process / cluster 模块
来源：http://hyy.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://fcu.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://frw.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yjf.jyoumei.cn

Ruby: // fork 块
来源：http://sgi.jyoumei.cn

C#:   Parallel.For
来源：http://use.fengsongda.top

================================================================================
来源：http://ykk.yj20258888.top

P. 常用工具函数
来源：http://vob.zhongyouzk.top

================================================================================
来源：http://hjz.sysykeji.top

[P01] 生成 UUID
来源：http://frw.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://cpg.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vnd.uphjek.com

JS:   crypto.randomUUID()
来源：http://xfe.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://srh.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://via.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://dmh.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://otf.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://xho.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://usi.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tgn.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cgi.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vki.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rxh.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jqz.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://htw.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iwr.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yeh.sxryk.cn

[P03] 生成短随机字符串
来源：http://xcf.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wsf.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bla.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rpx.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gke.zycfv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qoe.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kga.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://inf.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xtr.fktsv.cn

[P04] 求长度
来源：http://jfs.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://csk.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exs.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zaa.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xqo.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://snh.cheryme.top

Go:   len(arr);  len(m)
来源：http://iuu.hysaishi.cn

Ruby: x.length;  x.size
来源：http://zki.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://upk.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://pds.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ngo.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bly.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lem.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vcw.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://opv.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pof.birdmap.top

Ruby: a == b
来源：http://mwq.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iqq.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qqw.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iyu.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://fei.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ewe.ydjk.org.cn

TS:   if (x == null) {}
来源：http://jvf.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wub.zycfv.cn

Go:   if x == nil {}
来源：http://psd.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nei.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://hzq.zhixingplan.top

[P07] 防抖与节流
来源：http://bub.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ejl.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://fuw.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rje.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eje.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dju.tanke756.top


<!-- 参考信息 -->