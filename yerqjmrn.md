代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://mrr.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cpp.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nye.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://qjr.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://tgh.yanxiufei.cn

Java: resp.statusCode()
来源：http://ecx.yuxming.cn

Go:   resp.StatusCode
来源：http://zik.dianchejie.cn

Ruby: resp.code.to_i
来源：http://wqi.havefunace.top

C#:   (int)resp.StatusCode
来源：http://nzq.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://zrp.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rhn.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://hwy.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qww.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://leu.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sbt.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nvt.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttm.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://guk.yvedp.cn

================================================================================
来源：http://kmg.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://jpo.cqqwz.cn

================================================================================
来源：http://bfo.redwolf501.top

[M01] 读取命令行参数
来源：http://wwf.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://kjh.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://wti.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://qgv.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://fnb.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://prt.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://gch.yj202588.top

Ruby: ARGV
来源：http://yfn.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://raf.fzhhl.top

[M02] 读取环境变量
来源：http://jvb.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://fno.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cnp.nanxinkj.top

JS:   process.env.HOME
来源：http://hes.wangdashe.top

TS:   process.env.HOME
来源：http://cth.hammf.cn

Java: System.getenv("HOME")
来源：http://uop.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lnl.vehdjk.com

Ruby: ENV["HOME"]
来源：http://fzn.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jjw.feifeiyinyue.top

[M03] 执行外部命令
来源：http://mxz.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uvm.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fjk.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ckm.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nok.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wkr.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://qyi.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mqy.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://nip.ehwqpu.com

[M04] 获取当前工作目录
来源：http://ulx.xziqi.cn

Py:   os.getcwd()
来源：http://qjw.zhixingplan.top

PHP:  getcwd();
来源：http://ghf.guowangkeji.top

JS:   process.cwd()
来源：http://utk.jyoumei.cn

TS:   process.cwd()
来源：http://zuv.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://aln.mhx1999.top

Go:   os.Getwd()
来源：http://wyg.fengsongda.top

Ruby: Dir.pwd
来源：http://dfg.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nxy.shanyushiyangtech.top

[M05] 设置退出码
来源：http://otd.xinyue.icu

Py:   sys.exit(1)
来源：http://ukj.nanxinkj.top

PHP:  exit(1);
来源：http://vyu.tanke756.top

JS:   process.exit(1)
来源：http://qqb.chenzaomai.com

TS:   process.exit(1)
来源：http://npz.zdbjq.cn

Java: System.exit(1)
来源：http://qwi.snrcjt.cn

Go:   os.Exit(1)
来源：http://nzm.jinqigufen.top

Ruby: exit 1
来源：http://mqy.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mzn.hammf.cn

[M06] 向标准错误输出
来源：http://tcb.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://app.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cjv.jinghuilouyu.cn

JS:   console.error("err")
来源：http://urp.zhixingplan.top

TS:   console.error("err")
来源：http://bfb.sjlbkw.cn

Java: System.err.println("err")
来源：http://lsr.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rcv.0kj1m.cn

Ruby: warn "err"
来源：http://zuz.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://hfw.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://oqz.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://ujc.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eby.shanyushiyangtech.top

JS:   require.main === module
来源：http://osx.chenzaomai.com

TS:   require.main === module
来源：http://pnt.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://iwk.fehbvm.com

Go:   func main()
来源：http://bzb.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tyu.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://mun.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://cwf.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://fqn.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://grb.yuxming.cn

JS:   process.platform;  process.version
来源：http://ygz.sxryk.cn

TS:   process.platform;  process.version
来源：http://hzi.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gcp.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fck.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iyx.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zyj.ydjk.org.cn

================================================================================
来源：http://zjn.zhongyouzk.top

N. 数据结构与算法
来源：http://krk.kuanghao11.cn

================================================================================
来源：http://wau.yj20258.top

[N01] 二分查找（有序数组）
来源：http://uhi.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://scs.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sgk.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fzi.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://osd.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lsz.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ghh.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://jfh.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://igw.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://hvh.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://ioe.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iin.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qye.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jfg.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wir.yuxming.cn

Go:   slices.Sort(arr)
来源：http://ywn.dashuyun.cn

Ruby: arr.sort
来源：http://xxz.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ezi.cashguo.top

[N03] 快速排序（分治示例）
来源：http://att.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cyw.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://rum.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pus.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qni.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fjk.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jbq.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mrm.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://cyi.yj20258888.top

[N04] 斐波那契数列
来源：http://ytu.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wbm.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qrk.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ogd.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uwg.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uhc.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rwv.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gyn.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mio.cucudq.cn

[N05] 最大公约数
来源：http://pub.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://rfy.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lil.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cxj.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cbj.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aid.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ulr.hammf.cn

Ruby: a.gcd(b)
来源：http://lsp.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cab.yuanzhike.top

[N06] 判断回文字符串
来源：http://bzf.yonumen.top

Py:   s == s[::-1]
来源：http://aam.aizwys.cn

PHP:  $s === strrev($s);
来源：http://inx.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://gym.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://hnw.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jce.cucudq.cn

Go:   // 双指针从两端比较
来源：http://fpx.fktsv.cn

Ruby: s == s.reverse
来源：http://iuy.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lvw.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://fys.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ros.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://chb.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nho.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://egq.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://lcb.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://paj.tianlin.xyz

Ruby: // 手写 Hash
来源：http://nfk.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://avi.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://gzk.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://qpv.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://cfv.shzxlz.cn

JS:   // 手写回溯递归
来源：http://khz.xziqi.cn

TS:   // 手写回溯递归
来源：http://itj.shzxlz.cn

Java: // 手写回溯递归
来源：http://msi.dashuyun.cn

Go:   // 手写回溯递归
来源：http://yev.uphjek.com

Ruby: arr.permutation.to_a
来源：http://mel.fktsv.cn

C#:   // 手写回溯递归
来源：http://ihz.tanke756.top

[N09] 栈与队列
来源：http://knx.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hut.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sbc.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pzd.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qel.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://duv.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xna.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zsr.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wld.sysykeji.top

[N10] 链表节点定义
来源：http://dsx.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xdj.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rfs.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fpu.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nxs.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://hwp.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://rxv.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ppb.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zpr.fzhhl.top

[N11] 二叉树中序遍历
来源：http://agd.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ysy.daxiang520.top

PHP:  // 手写递归函数
来源：http://zyl.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dbg.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fai.andypj.xyz

Java: // 手写递归
来源：http://noz.wangshuangyany.cn

Go:   // 手写递归
来源：http://dpe.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sja.guannengcc.top

C#:   // 手写递归
来源：http://rpy.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://err.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jzy.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vip.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://inn.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmp.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lta.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://alq.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tfs.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://czm.shangyingyoupin.top

================================================================================
来源：http://mxw.bjfxy.top

O. 并发与异步
来源：http://sdt.yonumen.top

================================================================================
来源：http://wcl.yj20258.top

[O01] 启动一个线程
来源：http://wvv.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://avr.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qvb.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://reu.chenzaomai.com

TS:   // 同 JS
来源：http://uzb.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://ivu.316326.xyz

Go:   go f()
来源：http://ygm.tian-w.cn

Ruby: Thread.new { f }
来源：http://hug.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://ivf.zhijiandao.cn

[O02] 使用线程池
来源：http://dmk.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pvz.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://azx.epnwcf.com

JS:   // worker_threads 线程池
来源：http://euk.epnwcf.com

TS:   // worker_threads 线程池
来源：http://xju.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fzi.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lwq.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uvd.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ncq.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://onk.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://srz.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://dhq.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrc.chenlongwang.top

TS:   // 同 JS
来源：http://idp.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://zyn.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://usl.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://deo.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://anv.sxryk.cn

[O04] 定义异步函数并等待
来源：http://skk.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://hvo.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bbf.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://xio.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tsl.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bfn.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yny.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pgb.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://uev.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://twl.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://hzc.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxy.yj202588.top

JS:   await Promise.all(tasks)
来源：http://aqp.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://irc.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dge.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyx.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://nph.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://una.hesvh.cn

[O06] 使用进程池
来源：http://ktl.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qdi.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fqj.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://xls.yonumen.top

TS:   // child_process / cluster 模块
来源：http://xdp.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbo.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ung.yongpay.top

Ruby: // fork 块
来源：http://xvf.fanxiaobao.xyz

C#:   Parallel.For
来源：http://cyo.cucudq.cn

================================================================================
来源：http://gzn.jinqigufen.top

P. 常用工具函数
来源：http://zuc.aizwys.cn

================================================================================
来源：http://raw.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://omm.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://rxj.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sod.c1oappe.top

JS:   crypto.randomUUID()
来源：http://ojz.aizwys.cn

TS:   crypto.randomUUID()
来源：http://nzs.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://gum.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://dgg.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://alo.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://luq.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://vrk.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qrb.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rsa.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wfb.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qfn.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bhl.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yoc.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tst.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ygi.chenlongwang.top

[P03] 生成短随机字符串
来源：http://gic.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rbn.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mzm.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://otc.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jqp.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lws.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://saj.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cic.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://chk.meibo888.top

[P04] 求长度
来源：http://tap.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ish.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lza.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xtq.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nwy.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://fqe.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://txw.xziqi.cn

Ruby: x.length;  x.size
来源：http://cdk.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dug.sysykeji.top


<!-- 参考信息 -->