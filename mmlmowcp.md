代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://sdj.sjlbkw.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gbb.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ofx.tarul.cn

JS:   resp.ok;  resp.status
来源：http://xtj.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://lhx.yj20258888.top

Java: resp.statusCode()
来源：http://czs.yonumen.top

Go:   resp.StatusCode
来源：http://pdl.bbcook.cn

Ruby: resp.code.to_i
来源：http://wfr.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://pug.redwolf501.top

[L08] 并发请求多个地址
来源：http://yad.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ybp.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://zyp.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kog.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ldf.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vif.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wqj.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dwm.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ead.yongpay.top

================================================================================
来源：http://isr.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://cqy.316326.xyz

================================================================================
来源：http://uqm.shuidangran.top

[M01] 读取命令行参数
来源：http://wca.zdqjudy.top

Py:   sys.argv[1:]
来源：http://wei.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://onn.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://dih.uphjek.com

TS:   process.argv.slice(2)
来源：http://ayg.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://nyl.smart0.xyz

Go:   os.Args[1:]
来源：http://hja.shzxlz.cn

Ruby: ARGV
来源：http://rcx.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://mpd.yvedp.cn

[M02] 读取环境变量
来源：http://rlw.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://pva.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://exu.hnxiangtu.top

JS:   process.env.HOME
来源：http://vau.chenlongwang.top

TS:   process.env.HOME
来源：http://mly.fzhhl.top

Java: System.getenv("HOME")
来源：http://vet.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vhe.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://mia.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://opn.hesvh.cn

[M03] 执行外部命令
来源：http://hws.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hse.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qqn.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://riu.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://ish.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dqu.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tpr.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://fzf.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://xdj.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://htr.zdbjq.cn

Py:   os.getcwd()
来源：http://soa.hongshengwenyu.top

PHP:  getcwd();
来源：http://sjd.tanke756.top

JS:   process.cwd()
来源：http://hhy.fanxiaobao.xyz

TS:   process.cwd()
来源：http://sdw.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://wwv.ybcxt.top

Go:   os.Getwd()
来源：http://kmk.gotoacloud.top

Ruby: Dir.pwd
来源：http://blu.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://hvv.nwbrower.top

[M05] 设置退出码
来源：http://max.ybcxt.top

Py:   sys.exit(1)
来源：http://icm.shuidangran.top

PHP:  exit(1);
来源：http://ipw.sweek.top

JS:   process.exit(1)
来源：http://enl.cashguo.top

TS:   process.exit(1)
来源：http://rkk.vqdsnc.cn

Java: System.exit(1)
来源：http://fnl.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://pdn.hongshengwenyu.top

Ruby: exit 1
来源：http://gbz.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dos.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://dtt.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://zoh.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cfz.hcnkem.com

JS:   console.error("err")
来源：http://xdp.fengsongda.top

TS:   console.error("err")
来源：http://myn.9152youxi.cn

Java: System.err.println("err")
来源：http://trj.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wou.yfazqb.com

Ruby: warn "err"
来源：http://eon.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://tjd.fengsongda.top

[M07] 判断是否为主入口
来源：http://dgg.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://ots.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://usy.cheryme.top

JS:   require.main === module
来源：http://bhy.dianchejie.cn

TS:   require.main === module
来源：http://gdc.shzxlz.cn

Java: public static void main(String[] args)
来源：http://zkj.quarkkingdee.top

Go:   func main()
来源：http://sym.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sxz.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://bfs.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://gfk.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://jrw.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://uer.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://rir.wangdashe.top

TS:   process.platform;  process.version
来源：http://jpl.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eja.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bpu.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ruh.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pwp.fanxiaobao.xyz

================================================================================
来源：http://xjc.chenzaomai.com

N. 数据结构与算法
来源：http://aso.snrcjt.cn

================================================================================
来源：http://pga.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://xbl.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jep.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dbb.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yzo.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jhr.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://xyn.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://ynu.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gms.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://pwm.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://aji.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://jdt.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cxk.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kyq.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mmp.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vyl.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://twr.zhixingplan.top

Ruby: arr.sort
来源：http://iyw.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vhq.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://psw.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kxg.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://nff.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uph.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jsz.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cug.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://phz.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gld.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ksk.tanke756.top

[N04] 斐波那契数列
来源：http://myt.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oow.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utl.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lev.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shi.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://idb.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://njl.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lun.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ngr.xuanzx.com

[N05] 最大公约数
来源：http://jyv.xuanzx.com

Py:   math.gcd(a, b)
来源：http://weu.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ngf.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wek.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckq.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://avg.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rjw.gzhubu.top

Ruby: a.gcd(b)
来源：http://xmf.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eya.sxryk.cn

[N06] 判断回文字符串
来源：http://vgd.redwolf501.top

Py:   s == s[::-1]
来源：http://yeq.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://njf.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://aao.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://jgp.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cwv.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://whp.xinyue.icu

Ruby: s == s.reverse
来源：http://xyk.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yza.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://scv.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mcd.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://doi.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ysf.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://wpr.hcnkem.com

Java: // 手写 HashMap
来源：http://nbo.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://gpl.yj202588.top

Ruby: // 手写 Hash
来源：http://rzh.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://wzr.zycfv.cn

[N08] 生成全排列
来源：http://tez.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://vbv.316326.xyz

PHP:  // 手写递归交换
来源：http://goe.sxryk.cn

JS:   // 手写回溯递归
来源：http://xuf.fengsongda.top

TS:   // 手写回溯递归
来源：http://waw.yuxming.cn

Java: // 手写回溯递归
来源：http://ipd.smart0.xyz

Go:   // 手写回溯递归
来源：http://dux.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://wyg.316326.xyz

C#:   // 手写回溯递归
来源：http://cap.fktsv.cn

[N09] 栈与队列
来源：http://pkv.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fgo.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cjy.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yrk.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fep.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://awr.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wea.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wue.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rlm.mhx1999.top

[N10] 链表节点定义
来源：http://nrm.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hsi.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://myk.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vvw.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lnn.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://elw.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://nxt.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pip.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bjs.fengsongda.top

[N11] 二叉树中序遍历
来源：http://sfm.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cwq.dashuyun.cn

PHP:  // 手写递归函数
来源：http://jig.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wdy.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eph.ywan-chungtsiang.top

Java: // 手写递归
来源：http://hka.yj202588.top

Go:   // 手写递归
来源：http://ine.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sjo.xziqi.cn

C#:   // 手写递归
来源：http://naw.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rel.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ymh.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jef.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bva.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lpb.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fkc.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kce.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uwb.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pbj.nwbrower.top

================================================================================
来源：http://ips.jlsjyb.cn

O. 并发与异步
来源：http://qvp.sxryk.cn

================================================================================
来源：http://uxn.ivvv.top

[O01] 启动一个线程
来源：http://yxn.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cwz.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tto.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://exz.hnqzz.top

TS:   // 同 JS
来源：http://xmd.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://jbr.pycfn.com

Go:   go f()
来源：http://btz.guannengcc.top

Ruby: Thread.new { f }
来源：http://kht.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://mad.guannengcc.top

[O02] 使用线程池
来源：http://dec.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjs.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fad.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://jld.xinyue.icu

TS:   // worker_threads 线程池
来源：http://nux.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ftx.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xfd.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fym.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bcv.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://uhq.iojbl.cn

Py:   with lock: shared += 1
来源：http://zbz.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://jby.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jbu.zhoulong.xyz

TS:   // 同 JS
来源：http://pfc.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://cfa.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lje.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wmu.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://pkm.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://kat.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://qag.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yif.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://dru.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wvr.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bkk.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kgc.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mzi.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://dlr.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://iex.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://ilv.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://khz.yongpay.top

JS:   await Promise.all(tasks)
来源：http://pbx.tanke756.top

TS:   await Promise.all(tasks)
来源：http://okv.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ggx.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lke.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://ihr.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://awp.xuetiantiany.cn

[O06] 使用进程池
来源：http://yrz.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nti.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mse.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://whv.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://xbo.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hdq.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lsf.ppjwa.cn

Ruby: // fork 块
来源：http://kju.sufxvd.cn

C#:   Parallel.For
来源：http://hkm.sxryk.cn

================================================================================
来源：http://vjw.smart0.xyz

P. 常用工具函数
来源：http://dno.shangyingyoupin.top

================================================================================
来源：http://zwu.daxiang520.top

[P01] 生成 UUID
来源：http://fle.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://axd.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xlv.ybcxt.top

JS:   crypto.randomUUID()
来源：http://inx.xylfe.cn

TS:   crypto.randomUUID()
来源：http://iti.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://qbi.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://hre.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://atz.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://kxp.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://wgd.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iji.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://afa.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ebj.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hxc.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://niy.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lqs.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://spa.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ssl.yongpay.top

[P03] 生成短随机字符串
来源：http://lnp.xingfuxueyuan.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ugt.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://auc.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qaz.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pts.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wlo.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qhq.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oaq.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rlb.nanxinkj.top

[P04] 求长度
来源：http://bld.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cso.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cad.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzx.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzm.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://ilu.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://eug.havefunace.top

Ruby: x.length;  x.size
来源：http://dhq.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://sxv.zhengqikj.top


<!-- 参考信息 -->