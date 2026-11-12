代发 wailian999

TS:   resp.ok;  resp.status
来源：http://qqq.cqqwz.cn

Java: resp.statusCode()
来源：http://dma.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://kly.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://psm.yj202588.top

C#:   (int)resp.StatusCode
来源：http://ldo.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://lii.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://avm.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://ijl.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qqa.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lup.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://llz.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://elp.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dvm.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sxe.shangyingyoupin.top

================================================================================
来源：http://vfa.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://ehj.wangshuangyany.cn

================================================================================
来源：http://cbl.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://urh.hywenlv.cn

Py:   sys.argv[1:]
来源：http://esq.jianghu66.top

PHP:  $argv;  $argc;
来源：http://ruf.fengsongda.top

JS:   process.argv.slice(2)
来源：http://jkx.316326.xyz

TS:   process.argv.slice(2)
来源：http://knm.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://pxm.316326.xyz

Go:   os.Args[1:]
来源：http://aat.zhongyouzk.top

Ruby: ARGV
来源：http://qvz.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://rmg.fktsv.cn

[M02] 读取环境变量
来源：http://lua.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://ooz.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tfy.yanxiufei.cn

JS:   process.env.HOME
来源：http://iwz.zhijiandao.cn

TS:   process.env.HOME
来源：http://yel.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://zai.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zxd.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://nrd.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gde.ppjwa.cn

[M03] 执行外部命令
来源：http://jmh.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzw.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lzb.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ghs.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oiy.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hod.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ynt.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ouk.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://wnx.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://wtj.yj202588.top

Py:   os.getcwd()
来源：http://nxi.daxiang520.top

PHP:  getcwd();
来源：http://tep.yueranfly.top

JS:   process.cwd()
来源：http://suo.sjlbkw.cn

TS:   process.cwd()
来源：http://sla.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://dqy.cqqwz.cn

Go:   os.Getwd()
来源：http://lmi.zhongyouzk.top

Ruby: Dir.pwd
来源：http://wdk.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://svr.tanke756.top

[M05] 设置退出码
来源：http://loe.jinqigfzy.top

Py:   sys.exit(1)
来源：http://rfc.shzxlz.cn

PHP:  exit(1);
来源：http://lty.svipenyu.cn

JS:   process.exit(1)
来源：http://dxw.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://svy.kuanghao11.cn

Java: System.exit(1)
来源：http://jho.tanke756.top

Go:   os.Exit(1)
来源：http://kfi.aibaodan.cn

Ruby: exit 1
来源：http://wep.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mel.ctjpmb.com

[M06] 向标准错误输出
来源：http://zmv.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://iuv.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://art.ydjk.org.cn

JS:   console.error("err")
来源：http://mnk.ctjpmb.com

TS:   console.error("err")
来源：http://kex.jyoumei.cn

Java: System.err.println("err")
来源：http://ezo.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://moi.chenzaomai.com

Ruby: warn "err"
来源：http://shp.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://itu.uphjek.com

[M07] 判断是否为主入口
来源：http://vnb.yongpay.top

Py:   if __name__ == "__main__":
来源：http://chw.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nxu.316326.xyz

JS:   require.main === module
来源：http://njs.ywan-chungtsiang.top

TS:   require.main === module
来源：http://lmv.zdqjudy.top

Java: public static void main(String[] args)
来源：http://ihy.xuanzx.com

Go:   func main()
来源：http://npw.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kez.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://vox.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://bww.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://wbe.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://ado.uphjek.com

JS:   process.platform;  process.version
来源：http://jeu.aibaodan.cn

TS:   process.platform;  process.version
来源：http://tij.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qsb.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://sln.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ijt.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vuo.shzxlz.cn

================================================================================
来源：http://vol.chenlongwang.top

N. 数据结构与算法
来源：http://ocl.hcnkem.com

================================================================================
来源：http://lxt.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://grp.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ntx.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uvi.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mfz.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvq.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://ovo.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://swl.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ajw.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://bvb.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://krq.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ozm.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://whg.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sae.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qse.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ihs.birdmap.top

Go:   slices.Sort(arr)
来源：http://pam.sjlbkw.cn

Ruby: arr.sort
来源：http://nwy.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://ksm.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://oeu.zhixingplan.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wka.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://qba.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vlf.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ivt.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pon.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://shl.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hdt.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rar.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://pqy.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fyi.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://faq.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gdm.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlj.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ugm.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://prd.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hkv.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pwl.zhijiandao.cn

[N05] 最大公约数
来源：http://hqv.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://hiy.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tun.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://okl.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mpj.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ozk.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zbb.fktsv.cn

Ruby: a.gcd(b)
来源：http://ltn.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vju.hesvh.cn

[N06] 判断回文字符串
来源：http://gyr.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://wqy.tanke756.top

PHP:  $s === strrev($s);
来源：http://hsr.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://ivy.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://zri.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uio.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://ywg.chenlongwang.top

Ruby: s == s.reverse
来源：http://maw.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://omp.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://smi.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zrh.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://civ.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zym.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://eni.fzhhl.top

Java: // 手写 HashMap
来源：http://yba.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://eoo.9152youxi.cn

Ruby: // 手写 Hash
来源：http://nlr.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://isc.shangyingyoupin.top

[N08] 生成全排列
来源：http://mmk.hammf.cn

Py:   itertools.permutations(arr)
来源：http://eui.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://efo.9152youxi.cn

JS:   // 手写回溯递归
来源：http://qlb.jianghu66.top

TS:   // 手写回溯递归
来源：http://wam.yuxming.cn

Java: // 手写回溯递归
来源：http://inb.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://esk.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://yre.smart0.xyz

C#:   // 手写回溯递归
来源：http://bzk.sxryk.cn

[N09] 栈与队列
来源：http://afr.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fvy.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gex.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lsq.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qtm.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hus.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://azh.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vuz.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdz.ehwqpu.com

[N10] 链表节点定义
来源：http://qnv.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://onz.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yio.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ajz.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmh.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://mby.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://yto.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bbm.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uih.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://lwr.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vsr.316326.xyz

PHP:  // 手写递归函数
来源：http://fsk.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fbr.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nxq.gaohongyu789.top

Java: // 手写递归
来源：http://eno.guannengcc.top

Go:   // 手写递归
来源：http://jcy.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pet.chenlongwang.top

C#:   // 手写递归
来源：http://iso.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eam.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qxl.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nmu.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gmu.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gdn.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xlg.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pta.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uwr.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dmb.ctjpmb.com

================================================================================
来源：http://huc.redwolf501.top

O. 并发与异步
来源：http://krd.zhongyouzk.top

================================================================================
来源：http://lrh.andypj.xyz

[O01] 启动一个线程
来源：http://mry.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ucv.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dee.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mpf.zhengqikj.top

TS:   // 同 JS
来源：http://csz.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://wno.ybcxt.top

Go:   go f()
来源：http://ltx.uphjek.com

Ruby: Thread.new { f }
来源：http://ckd.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://veh.yj20258888.top

[O02] 使用线程池
来源：http://zfp.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fbd.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rnh.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://txo.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://jzd.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://wwe.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://slf.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbv.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iav.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://lwk.wangdashe.top

Py:   with lock: shared += 1
来源：http://tti.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://kqm.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mdo.hesvh.cn

TS:   // 同 JS
来源：http://jiq.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://izh.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://esv.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cth.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://azl.shuidangran.top

[O04] 定义异步函数并等待
来源：http://rmg.yongpay.top

Py:   async def f():⏎    await g()
来源：http://tfn.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oud.xylfe.cn

JS:   async function f() { await g(); }
来源：http://ztd.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://slm.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fhg.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mgm.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://jey.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://tta.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://afe.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://cbg.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://usj.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://owt.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://bhr.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ggr.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gdb.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://guo.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://upb.aizwys.cn

[O06] 使用进程池
来源：http://xhz.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nts.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gtw.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://nvs.uphjek.com

TS:   // child_process / cluster 模块
来源：http://klj.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ndq.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cao.nwbrower.top

Ruby: // fork 块
来源：http://xfi.tianlin.xyz

C#:   Parallel.For
来源：http://iwy.yonumen.top

================================================================================
来源：http://ycq.sysykeji.top

P. 常用工具函数
来源：http://wrw.gotoacloud.top

================================================================================
来源：http://kpu.yanxiufei.cn

[P01] 生成 UUID
来源：http://nex.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://cqe.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nya.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://dna.yfazqb.com

TS:   crypto.randomUUID()
来源：http://dzv.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://hvl.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://rrq.yj202588.top

Ruby: SecureRandom.uuid
来源：http://imz.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://jay.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://fcw.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygj.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://bqm.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dxm.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ehp.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gnr.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xge.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://khi.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wia.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://kyz.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wng.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yld.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://soy.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://why.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ong.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uep.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://aoj.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jvu.hcnkem.com

[P04] 求长度
来源：http://ovh.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gsv.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbc.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zxs.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vkn.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://xlo.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://swl.daria6918.cn

Ruby: x.length;  x.size
来源：http://whh.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sff.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://jrs.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oas.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://swv.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xvx.zhixingplan.top


<!-- 参考信息 -->