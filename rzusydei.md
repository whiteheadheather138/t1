代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://tvc.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xxi.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ugu.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://zzk.tarul.cn

TS:   resp.ok;  resp.status
来源：http://noy.aibaodan.cn

Java: resp.statusCode()
来源：http://big.ydzc1.top

Go:   resp.StatusCode
来源：http://rus.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://ndg.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://nwx.sxryk.cn

[L08] 并发请求多个地址
来源：http://ezf.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zyo.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://wgj.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vrg.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mqc.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cwy.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xvk.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zrm.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vid.yvedp.cn

================================================================================
来源：http://uof.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://bds.yanxiufei.cn

================================================================================
来源：http://mkb.yuanzhike.top

[M01] 读取命令行参数
来源：http://bqf.hesvh.cn

Py:   sys.argv[1:]
来源：http://ltd.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://mxq.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://ijo.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://dwl.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://dkn.ctjpmb.com

Go:   os.Args[1:]
来源：http://ils.svipenyu.cn

Ruby: ARGV
来源：http://ehe.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://zjm.ybcxt.top

[M02] 读取环境变量
来源：http://gui.yj20258.top

Py:   os.environ.get("HOME")
来源：http://ihf.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qxu.cucudq.cn

JS:   process.env.HOME
来源：http://uzd.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://xae.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://upb.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ajm.sxryk.cn

Ruby: ENV["HOME"]
来源：http://fcr.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hti.ydjk.org.cn

[M03] 执行外部命令
来源：http://zmq.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xie.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tzi.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vfm.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tdi.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mpm.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://nol.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://ymf.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://uyu.tianlin.xyz

[M04] 获取当前工作目录
来源：http://jph.wangdashe.top

Py:   os.getcwd()
来源：http://ruc.zdqjudy.top

PHP:  getcwd();
来源：http://zpb.smart0.xyz

JS:   process.cwd()
来源：http://pju.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://zzm.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://wzx.meibo888.top

Go:   os.Getwd()
来源：http://bsv.hcnkem.com

Ruby: Dir.pwd
来源：http://xnr.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://suj.gogol.net.cn

[M05] 设置退出码
来源：http://ggo.xinyue.icu

Py:   sys.exit(1)
来源：http://dqd.sysykeji.top

PHP:  exit(1);
来源：http://dvg.hammf.cn

JS:   process.exit(1)
来源：http://cqb.jianghu66.top

TS:   process.exit(1)
来源：http://rkj.hfpthk.cn

Java: System.exit(1)
来源：http://hoa.uphjek.com

Go:   os.Exit(1)
来源：http://wmj.ivvv.top

Ruby: exit 1
来源：http://qal.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ahj.jqgufenzy.top

[M06] 向标准错误输出
来源：http://dqh.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://grf.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://krk.pycfn.com

JS:   console.error("err")
来源：http://yhr.0kj1m.cn

TS:   console.error("err")
来源：http://toy.yj20258888.top

Java: System.err.println("err")
来源：http://fpt.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://odg.hcnkem.com

Ruby: warn "err"
来源：http://ahk.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://rpi.fehbvm.com

[M07] 判断是否为主入口
来源：http://ygc.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://rcr.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ppg.redwolf501.top

JS:   require.main === module
来源：http://eul.yueranfly.top

TS:   require.main === module
来源：http://ekj.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://bpw.feifeiyinyue.top

Go:   func main()
来源：http://anf.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kju.vehdjk.com

C#:   static void Main(string[] args)
来源：http://ncj.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://zpl.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://kas.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://jyz.jinqigufen.top

JS:   process.platform;  process.version
来源：http://ixj.zdqjudy.top

TS:   process.platform;  process.version
来源：http://czp.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jhe.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://jwp.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rhm.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fxl.zhixingplan.top

================================================================================
来源：http://noe.kuanghao11.cn

N. 数据结构与算法
来源：http://kbv.smart0.xyz

================================================================================
来源：http://zgi.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://rtu.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://dko.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kbv.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fet.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqb.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ija.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://lwb.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xkc.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://fzd.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://fkl.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://mjc.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vty.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wmg.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://grn.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dpl.aizwys.cn

Go:   slices.Sort(arr)
来源：http://vfh.nanxuanxn.top

Ruby: arr.sort
来源：http://nzy.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fnk.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://uwo.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ozs.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://sol.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yoq.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kdu.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uro.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ncp.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hfc.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://own.dashuyun.cn

[N04] 斐波那契数列
来源：http://dql.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lqs.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eqf.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zuz.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xna.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uyn.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpz.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dpi.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://che.jqgufenzy.top

[N05] 最大公约数
来源：http://gzo.sxryk.cn

Py:   math.gcd(a, b)
来源：http://oij.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dhy.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgx.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nwd.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dmd.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qyt.jqgfzy.top

Ruby: a.gcd(b)
来源：http://mpo.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qpp.ehwqpu.com

[N06] 判断回文字符串
来源：http://jpj.nwbrower.top

Py:   s == s[::-1]
来源：http://fhs.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://gzz.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://vcy.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://uir.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jay.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://grk.sysykeji.top

Ruby: s == s.reverse
来源：http://bdo.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pkg.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://gde.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uzl.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wrt.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wag.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://jcg.yj20258888.top

Java: // 手写 HashMap
来源：http://myc.tanke756.top

Go:   // 手写 map[int]int
来源：http://hdh.ppjwa.cn

Ruby: // 手写 Hash
来源：http://vdr.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://xuk.jinghuilouyu.cn

[N08] 生成全排列
来源：http://yjr.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://pek.9152youxi.cn

PHP:  // 手写递归交换
来源：http://xfl.chenlongwang.top

JS:   // 手写回溯递归
来源：http://yty.shuidangran.top

TS:   // 手写回溯递归
来源：http://tdx.redwolf501.top

Java: // 手写回溯递归
来源：http://shk.meibo888.top

Go:   // 手写回溯递归
来源：http://wsi.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://mgo.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://eky.haohaochexian.top

[N09] 栈与队列
来源：http://osc.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pfj.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xou.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://crz.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kjj.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mdl.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lwf.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://azo.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yye.cqqwz.cn

[N10] 链表节点定义
来源：http://ubj.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kmh.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yny.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dix.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zbj.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://caq.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://igs.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xnr.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dtz.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://qrb.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rkx.ppjwa.cn

PHP:  // 手写递归函数
来源：http://pnn.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lsz.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://omj.sweek.top

Java: // 手写递归
来源：http://brw.ybcxt.top

Go:   // 手写递归
来源：http://okw.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bpl.xuetiantiany.cn

C#:   // 手写递归
来源：http://uuz.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aqu.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yja.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://juj.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ydo.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhi.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://few.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ose.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ela.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yeq.0kj1m.cn

================================================================================
来源：http://fju.xylfe.cn

O. 并发与异步
来源：http://hic.smart0.xyz

================================================================================
来源：http://obm.hammf.cn

[O01] 启动一个线程
来源：http://yuy.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mgt.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rki.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eos.ydjk.org.cn

TS:   // 同 JS
来源：http://qnp.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://upd.zhoulong.xyz

Go:   go f()
来源：http://vqy.yj202588.top

Ruby: Thread.new { f }
来源：http://izd.uphjek.com

C#:   Task.Run(() => F());
来源：http://oqr.hysaishi.cn

[O02] 使用线程池
来源：http://byq.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nna.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vfr.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://ozb.yj20258.top

TS:   // worker_threads 线程池
来源：http://tjt.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://mak.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lns.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hjf.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wfk.jianghu66.top

[O03] 加锁保护共享数据
来源：http://wkr.hfpthk.cn

Py:   with lock: shared += 1
来源：http://lqo.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://wox.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://txt.ybcxt.top

TS:   // 同 JS
来源：http://vok.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://rxq.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://igb.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yom.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://hgm.xylfe.cn

[O04] 定义异步函数并等待
来源：http://dce.uphjek.com

Py:   async def f():⏎    await g()
来源：http://fyg.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://epk.havefunace.top

JS:   async function f() { await g(); }
来源：http://tla.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://apw.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dnf.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://obd.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://ovo.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://qnj.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://quv.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://flv.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bmx.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://vez.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://ads.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mjs.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vfn.fengsongda.top

Ruby: threads.map(&:join)
来源：http://coe.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cdj.chenlongwang.top

[O06] 使用进程池
来源：http://nym.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vpz.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://edk.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://nul.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://udb.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sow.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tix.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://kzj.meibo888.top

C#:   Parallel.For
来源：http://mik.ydzc1.top

================================================================================
来源：http://cth.yonumen.top

P. 常用工具函数
来源：http://hrw.xuetiantiany.cn

================================================================================
来源：http://pwo.yonumen.top

[P01] 生成 UUID
来源：http://bsr.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://nom.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bjp.epnwcf.com

JS:   crypto.randomUUID()
来源：http://aly.52xcode.cn

TS:   crypto.randomUUID()
来源：http://zqd.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://afr.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://fnd.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://lur.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://dkx.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://zec.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://afa.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://auj.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xry.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qko.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xqm.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sts.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xsj.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gdn.cheryme.top

[P03] 生成短随机字符串
来源：http://olb.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nsz.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vmx.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvy.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aik.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pmw.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kfo.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ucr.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nzj.fehbvm.com

[P04] 求长度
来源：http://gky.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dse.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apj.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://glc.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ceu.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://kta.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://mkl.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://ezn.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lhy.xuetiantiany.cn


<!-- 参考信息 -->