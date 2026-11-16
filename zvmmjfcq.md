代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mzs.epnwcf.com

Java: resp.statusCode()
来源：http://ajx.shuidangran.top

Go:   resp.StatusCode
来源：http://bde.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://tax.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://xlw.tarul.cn

[L08] 并发请求多个地址
来源：http://rzn.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://avb.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://gbe.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ksk.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://myt.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iai.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xlc.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://egg.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vqt.sjlbkw.cn

================================================================================
来源：http://ash.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://oup.zhengqikj.top

================================================================================
来源：http://aip.hcnkem.com

[M01] 读取命令行参数
来源：http://gya.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://kdn.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://tzc.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://xpl.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://kuv.hammf.cn

Java: args 数组（main 方法参数）
来源：http://phw.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://cjz.52xcode.cn

Ruby: ARGV
来源：http://upi.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://zcq.gzhubu.top

[M02] 读取环境变量
来源：http://vud.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://hpa.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://chi.daxiang520.top

JS:   process.env.HOME
来源：http://dwo.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://yko.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://ydb.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gkl.guannengcc.top

Ruby: ENV["HOME"]
来源：http://aby.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kre.yj202588.top

[M03] 执行外部命令
来源：http://qju.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yxo.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vxa.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xjl.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pfu.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zza.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xlx.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://esc.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://mvi.chenzaomai.com

[M04] 获取当前工作目录
来源：http://bah.shzxlz.cn

Py:   os.getcwd()
来源：http://mis.svipenyu.cn

PHP:  getcwd();
来源：http://lpl.ydjk.org.cn

JS:   process.cwd()
来源：http://isq.nwbrower.top

TS:   process.cwd()
来源：http://ogi.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://oug.hesvh.cn

Go:   os.Getwd()
来源：http://sav.sweek.top

Ruby: Dir.pwd
来源：http://lfe.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rhe.0kj1m.cn

[M05] 设置退出码
来源：http://teh.sjlbkw.cn

Py:   sys.exit(1)
来源：http://ivx.yuxming.cn

PHP:  exit(1);
来源：http://xbv.shuidangran.top

JS:   process.exit(1)
来源：http://qru.bbcook.cn

TS:   process.exit(1)
来源：http://enp.daria6918.cn

Java: System.exit(1)
来源：http://yec.yonumen.top

Go:   os.Exit(1)
来源：http://yjx.c1oappe.top

Ruby: exit 1
来源：http://evq.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nik.daria6918.cn

[M06] 向标准错误输出
来源：http://sku.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://tpy.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mos.havefunace.top

JS:   console.error("err")
来源：http://qof.c1oappe.top

TS:   console.error("err")
来源：http://sob.nwbrower.top

Java: System.err.println("err")
来源：http://pty.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fhi.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://ain.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ocr.guowangkeji.top

[M07] 判断是否为主入口
来源：http://bdf.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://iuo.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fqs.jianghu66.top

JS:   require.main === module
来源：http://eov.aibaodan.cn

TS:   require.main === module
来源：http://bze.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://bmj.snrcjt.cn

Go:   func main()
来源：http://bme.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ctk.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://jiy.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://bli.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://put.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://jfh.birdmap.top

JS:   process.platform;  process.version
来源：http://dxz.snrcjt.cn

TS:   process.platform;  process.version
来源：http://tha.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zac.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xco.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kah.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cgn.ywan-chungtsiang.top

================================================================================
来源：http://ffb.tianlin.xyz

N. 数据结构与算法
来源：http://adg.nanxinkj.top

================================================================================
来源：http://zpe.uphjek.com

[N01] 二分查找（有序数组）
来源：http://tgf.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ffk.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eer.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zzu.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfz.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://glw.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://ilh.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hgh.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ove.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://ndq.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://yta.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wde.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kuf.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zif.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yzt.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://zzx.jyoumei.cn

Ruby: arr.sort
来源：http://wpy.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ety.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://jyw.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oaq.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://glw.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dte.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hqo.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hoa.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uwj.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fca.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://kwz.jinqigfzy.top

[N04] 斐波那契数列
来源：http://arp.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ycy.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://msi.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fcn.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsl.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fbs.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uxl.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tpm.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mgt.fengsongda.top

[N05] 最大公约数
来源：http://dwj.xylfe.cn

Py:   math.gcd(a, b)
来源：http://qot.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqh.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vsc.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pjc.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oml.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yss.dianchejie.cn

Ruby: a.gcd(b)
来源：http://sbq.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fci.guannengcc.top

[N06] 判断回文字符串
来源：http://zcq.hcnkem.com

Py:   s == s[::-1]
来源：http://grz.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://tys.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://yir.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://hec.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ddv.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://bue.havefunace.top

Ruby: s == s.reverse
来源：http://rzc.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xuu.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://vyl.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bxk.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jlo.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://voa.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://lha.sysykeji.top

Java: // 手写 HashMap
来源：http://njo.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://ybe.zhengqikj.top

Ruby: // 手写 Hash
来源：http://rqn.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://woa.guowangkeji.top

[N08] 生成全排列
来源：http://yaw.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://wry.hywenlv.cn

PHP:  // 手写递归交换
来源：http://awr.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://ogm.hcnkem.com

TS:   // 手写回溯递归
来源：http://cis.havefunace.top

Java: // 手写回溯递归
来源：http://bgl.smart0.xyz

Go:   // 手写回溯递归
来源：http://yai.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://uib.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://wgl.gogol.net.cn

[N09] 栈与队列
来源：http://qer.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qii.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dfx.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://npx.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://run.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://anf.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kps.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pam.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bwf.gzhubu.top

[N10] 链表节点定义
来源：http://ass.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iby.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rgs.redwolf501.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cqc.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://alo.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://ota.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wgn.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rbt.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mxk.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://fxk.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zjg.tarul.cn

PHP:  // 手写递归函数
来源：http://amn.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ren.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jgo.sjlbkw.cn

Java: // 手写递归
来源：http://uip.fzhhl.top

Go:   // 手写递归
来源：http://fjp.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xps.pycfn.com

C#:   // 手写递归
来源：http://rlm.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wro.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ojz.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vav.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bow.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sbq.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://upb.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ffp.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mpd.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qvj.sjlbkw.cn

================================================================================
来源：http://dmy.sjlbkw.cn

O. 并发与异步
来源：http://ahr.hesvh.cn

================================================================================
来源：http://pav.gotoacloud.top

[O01] 启动一个线程
来源：http://mvr.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tdu.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://srg.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fgl.hysaishi.cn

TS:   // 同 JS
来源：http://kjh.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://fwm.sjlbkw.cn

Go:   go f()
来源：http://ujl.nanxinkj.top

Ruby: Thread.new { f }
来源：http://exo.fzhhl.top

C#:   Task.Run(() => F());
来源：http://ams.9152youxi.cn

[O02] 使用线程池
来源：http://roc.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://obv.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://adj.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://grd.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://pms.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://qvi.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gfi.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://skn.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://apg.hammf.cn

[O03] 加锁保护共享数据
来源：http://wsr.sxryk.cn

Py:   with lock: shared += 1
来源：http://xmv.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://bbz.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jci.hywenlv.cn

TS:   // 同 JS
来源：http://ynt.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://miu.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mhh.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jwf.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://cxf.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://snj.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://ypv.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vvx.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://bwk.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hts.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ztp.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://beo.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://con.yj20258.top

C#:   async Task F() { await G(); }
来源：http://kqx.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://cxo.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://xgm.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iew.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://uju.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://svh.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bqv.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tgi.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://pzb.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qag.bjfxy.top

[O06] 使用进程池
来源：http://bxt.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lho.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://aec.hammf.cn

JS:   // child_process / cluster 模块
来源：http://oyi.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://fpf.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mgu.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qgh.smart0.xyz

Ruby: // fork 块
来源：http://asi.jianghu66.top

C#:   Parallel.For
来源：http://dfb.shangyingyoupin.top

================================================================================
来源：http://tes.aibaodan.cn

P. 常用工具函数
来源：http://khg.yvedp.cn

================================================================================
来源：http://ndh.xylfe.cn

[P01] 生成 UUID
来源：http://ohj.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://dhg.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mht.birdmap.top

JS:   crypto.randomUUID()
来源：http://ghc.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://hyp.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://kig.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://bkn.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://vkm.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://rxm.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://iqv.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fbn.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://sdb.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yrs.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pcj.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kxm.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sev.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nqp.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jxu.zhixingplan.top

[P03] 生成短随机字符串
来源：http://oiw.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pma.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ocn.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkj.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wbg.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jlr.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cby.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://raa.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fgt.svipenyu.cn

[P04] 求长度
来源：http://ont.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://roy.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://phh.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kfp.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvj.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://jfe.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://ukn.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://kyo.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ubj.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://gxl.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cvq.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jyb.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sbq.birdmap.top


<!-- 参考信息 -->