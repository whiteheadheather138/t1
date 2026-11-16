代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://rao.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dmv.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://axa.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://xqd.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://ijt.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://pav.jqgufenzy.top

Go:   resp.StatusCode
来源：http://tco.dashuyun.cn

Ruby: resp.code.to_i
来源：http://pbw.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://grh.guowangkeji.top

[L08] 并发请求多个地址
来源：http://pff.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oka.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://wvc.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xlf.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sbo.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yzq.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hmf.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ssp.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qbh.cheryme.top

================================================================================
来源：http://sej.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://cbc.chenzaomai.com

================================================================================
来源：http://gsy.xuanzx.com

[M01] 读取命令行参数
来源：http://jqk.nwbrower.top

Py:   sys.argv[1:]
来源：http://aal.316326.xyz

PHP:  $argv;  $argc;
来源：http://rbn.bbcook.cn

JS:   process.argv.slice(2)
来源：http://bkb.jianghu66.top

TS:   process.argv.slice(2)
来源：http://stt.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://dsg.zycfv.cn

Go:   os.Args[1:]
来源：http://uzg.pengpengdd.cyou

Ruby: ARGV
来源：http://gqi.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://lqv.zdbjq.cn

[M02] 读取环境变量
来源：http://tof.cashguo.top

Py:   os.environ.get("HOME")
来源：http://ecq.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uvq.yj20258888.top

JS:   process.env.HOME
来源：http://dwa.shuidangran.top

TS:   process.env.HOME
来源：http://mml.guowangkeji.top

Java: System.getenv("HOME")
来源：http://htd.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wmc.316326.xyz

Ruby: ENV["HOME"]
来源：http://grz.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nrc.hcnkem.com

[M03] 执行外部命令
来源：http://sni.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggz.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cpp.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ifd.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://klz.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://clt.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dwt.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://zbl.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://nar.xuanzx.com

[M04] 获取当前工作目录
来源：http://ira.vehdjk.com

Py:   os.getcwd()
来源：http://rio.chenlongwang.top

PHP:  getcwd();
来源：http://per.fanxiaobao.xyz

JS:   process.cwd()
来源：http://gdl.meibo888.top

TS:   process.cwd()
来源：http://bbl.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://qxy.bjfxy.top

Go:   os.Getwd()
来源：http://yga.zhijiandao.cn

Ruby: Dir.pwd
来源：http://lhx.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://khr.zhoulong.xyz

[M05] 设置退出码
来源：http://fuj.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://rsa.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://xvs.vqdsnc.cn

JS:   process.exit(1)
来源：http://leu.chenjidiqi.icu

TS:   process.exit(1)
来源：http://hus.cucudq.cn

Java: System.exit(1)
来源：http://tcw.yonumen.top

Go:   os.Exit(1)
来源：http://gme.nanxinkj.top

Ruby: exit 1
来源：http://dcj.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mvt.shzxlz.cn

[M06] 向标准错误输出
来源：http://vmi.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://vma.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bep.wangdashe.top

JS:   console.error("err")
来源：http://eft.ybcxt.top

TS:   console.error("err")
来源：http://yhb.uphjek.com

Java: System.err.println("err")
来源：http://nub.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nsw.nwbrower.top

Ruby: warn "err"
来源：http://kct.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://sne.bjfxy.top

[M07] 判断是否为主入口
来源：http://bge.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://jml.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nwx.shuidangran.top

JS:   require.main === module
来源：http://xgf.gaohongyu789.top

TS:   require.main === module
来源：http://rcr.yangfankeji.com

Java: public static void main(String[] args)
来源：http://tyr.andypj.xyz

Go:   func main()
来源：http://oqh.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://khy.fengsongda.top

C#:   static void Main(string[] args)
来源：http://rii.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://xvv.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://bbt.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://nzv.hysaishi.cn

JS:   process.platform;  process.version
来源：http://rhv.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://aic.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wpe.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dnc.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mpm.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ygz.sweek.top

================================================================================
来源：http://qmg.havefunace.top

N. 数据结构与算法
来源：http://piz.zhaomingkeji.xyz

================================================================================
来源：http://ypw.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://oyr.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://usz.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wki.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rja.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hrg.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qcy.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://omd.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iew.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://bgo.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://jbi.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://sdk.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kof.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://kii.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ypc.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vgv.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://flz.wangshuangyany.cn

Ruby: arr.sort
来源：http://uwe.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ner.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://llh.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cyw.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://vrn.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsz.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dpb.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://now.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sfk.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ldv.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://fqy.316326.xyz

[N04] 斐波那契数列
来源：http://rum.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ycp.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wbm.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mab.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://atq.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ylb.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sur.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wrt.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lob.nwbrower.top

[N05] 最大公约数
来源：http://yze.vehdjk.com

Py:   math.gcd(a, b)
来源：http://iyh.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uzm.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wed.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dks.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nsw.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ckr.xinyue.icu

Ruby: a.gcd(b)
来源：http://qyk.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fpv.hesvh.cn

[N06] 判断回文字符串
来源：http://vbs.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://ios.yonumen.top

PHP:  $s === strrev($s);
来源：http://rma.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://fql.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://kcb.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mtc.yueranfly.top

Go:   // 双指针从两端比较
来源：http://jpx.meibo888.top

Ruby: s == s.reverse
来源：http://djs.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://zep.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://pqr.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hli.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ayh.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://icm.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://kvg.c1oappe.top

Java: // 手写 HashMap
来源：http://rja.hnqzz.top

Go:   // 手写 map[int]int
来源：http://rjt.aibaodan.cn

Ruby: // 手写 Hash
来源：http://mqd.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xzw.gaohongyu789.top

[N08] 生成全排列
来源：http://ehv.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://ucg.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://lgu.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://wzd.cucudq.cn

TS:   // 手写回溯递归
来源：http://wna.0kj1m.cn

Java: // 手写回溯递归
来源：http://iso.iojbl.cn

Go:   // 手写回溯递归
来源：http://mhh.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://ttu.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://lqf.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://rpv.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vfb.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://phw.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ucs.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fnw.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cin.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://itt.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rez.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mty.sysykeji.top

[N10] 链表节点定义
来源：http://fjv.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nbb.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ivg.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yab.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hmk.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://fyd.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://bqk.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zjc.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hgo.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://hxf.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rca.meibo888.top

PHP:  // 手写递归函数
来源：http://noc.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zwh.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fqc.hongshengwenyu.top

Java: // 手写递归
来源：http://ohw.iojbl.cn

Go:   // 手写递归
来源：http://que.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ybg.yj20258888.top

C#:   // 手写递归
来源：http://jic.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pac.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kgy.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ynq.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://loh.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrw.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vxq.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://utz.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wxw.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bie.zhoulong.xyz

================================================================================
来源：http://eux.hongshengwenyu.top

O. 并发与异步
来源：http://rgo.andypj.xyz

================================================================================
来源：http://dwn.xuetiantiany.cn

[O01] 启动一个线程
来源：http://frw.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lqn.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://duc.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://phy.hcnkem.com

TS:   // 同 JS
来源：http://xxm.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://aab.uphjek.com

Go:   go f()
来源：http://vng.fktsv.cn

Ruby: Thread.new { f }
来源：http://xxu.fktsv.cn

C#:   Task.Run(() => F());
来源：http://exy.gotoacloud.top

[O02] 使用线程池
来源：http://dqy.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://czp.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://npx.yfazqb.com

JS:   // worker_threads 线程池
来源：http://set.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://eww.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://eoj.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dop.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mdd.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://toi.xinyue.icu

[O03] 加锁保护共享数据
来源：http://eul.ydzc1.top

Py:   with lock: shared += 1
来源：http://zix.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://ldq.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qjb.xinyue.icu

TS:   // 同 JS
来源：http://nmt.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://mlv.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rnj.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://phu.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://ifs.52xcode.cn

[O04] 定义异步函数并等待
来源：http://bmb.yj20258.top

Py:   async def f():⏎    await g()
来源：http://eon.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nca.nwbrower.top

JS:   async function f() { await g(); }
来源：http://gwe.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zfn.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cqj.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qha.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://fad.yonumen.top

C#:   async Task F() { await G(); }
来源：http://hex.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://uzc.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://cun.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eep.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://awf.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://sld.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://afj.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rcf.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://qun.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jka.cdnleiting.top

[O06] 使用进程池
来源：http://gfe.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://boj.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jon.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://zev.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://nwn.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lfz.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jzs.jinqigfzy.top

Ruby: // fork 块
来源：http://eqw.daria6918.cn

C#:   Parallel.For
来源：http://ktp.xziqi.cn

================================================================================
来源：http://kgf.ppjwa.cn

P. 常用工具函数
来源：http://iod.daria6918.cn

================================================================================
来源：http://rrj.feifeiyinyue.top

[P01] 生成 UUID
来源：http://ljx.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://mxa.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cut.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://pmm.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://hgc.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://vno.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://uyg.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://jeg.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://wuk.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://qly.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ksl.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sui.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://are.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fmh.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mnr.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iyo.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iwd.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yjm.redwolf501.top

[P03] 生成短随机字符串
来源：http://rph.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dfp.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gri.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fut.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://knv.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ewx.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vxp.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lrh.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://llg.yonumen.top

[P04] 求长度
来源：http://hwc.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zlg.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dbq.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qbi.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://btd.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://lau.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://neg.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://awv.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://wio.yonumen.top


<!-- 参考信息 -->