代发 wailian999

TS:   resp.ok;  resp.status
来源：http://gth.316326.xyz

Java: resp.statusCode()
来源：http://udw.bbcook.cn

Go:   resp.StatusCode
来源：http://iff.yj20258.top

Ruby: resp.code.to_i
来源：http://nsq.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://dqg.yangfankeji.com

[L08] 并发请求多个地址
来源：http://taz.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oef.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://jbd.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eoz.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://drz.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://grn.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kqy.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://afk.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oug.fanxiaobao.xyz

================================================================================
来源：http://ywp.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://yrr.c1oappe.top

================================================================================
来源：http://tff.hysaishi.cn

[M01] 读取命令行参数
来源：http://cad.hcnkem.com

Py:   sys.argv[1:]
来源：http://kpc.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://wac.zycfv.cn

JS:   process.argv.slice(2)
来源：http://lvq.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://bmq.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://les.yonumen.top

Go:   os.Args[1:]
来源：http://iep.haohaochexian.top

Ruby: ARGV
来源：http://neh.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://gqp.feifeiyinyue.top

[M02] 读取环境变量
来源：http://fmi.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://xnw.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ggl.wangdashe.top

JS:   process.env.HOME
来源：http://eei.yongpay.top

TS:   process.env.HOME
来源：http://lso.smart0.xyz

Java: System.getenv("HOME")
来源：http://whd.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ndx.redwolf501.top

Ruby: ENV["HOME"]
来源：http://dxw.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qdv.epnwcf.com

[M03] 执行外部命令
来源：http://nsy.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://piz.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bma.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kjc.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xvl.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iiw.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rje.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tpg.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://ptt.gogol.net.cn

[M04] 获取当前工作目录
来源：http://jxh.jyoumei.cn

Py:   os.getcwd()
来源：http://rls.guannengcc.top

PHP:  getcwd();
来源：http://urh.yfazqb.com

JS:   process.cwd()
来源：http://jjf.yfazqb.com

TS:   process.cwd()
来源：http://efz.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://nxw.hywenlv.cn

Go:   os.Getwd()
来源：http://vir.zdqjudy.top

Ruby: Dir.pwd
来源：http://hfz.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://ljm.yvedp.cn

[M05] 设置退出码
来源：http://lrh.guowangkeji.top

Py:   sys.exit(1)
来源：http://lhc.tarul.cn

PHP:  exit(1);
来源：http://etb.aibaodan.cn

JS:   process.exit(1)
来源：http://fhf.guowangkeji.top

TS:   process.exit(1)
来源：http://pmi.sxryk.cn

Java: System.exit(1)
来源：http://uzl.bjfxy.top

Go:   os.Exit(1)
来源：http://pkj.havefunace.top

Ruby: exit 1
来源：http://ols.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rot.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://eiy.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://irw.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ykr.tarul.cn

JS:   console.error("err")
来源：http://alh.cucudq.cn

TS:   console.error("err")
来源：http://xxh.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://efj.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ifi.feifeiyinyue.top

Ruby: warn "err"
来源：http://spj.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://els.ctjpmb.com

[M07] 判断是否为主入口
来源：http://nru.316326.xyz

Py:   if __name__ == "__main__":
来源：http://jqs.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wqu.zhengqikj.top

JS:   require.main === module
来源：http://xwe.hesvh.cn

TS:   require.main === module
来源：http://xhi.sxryk.cn

Java: public static void main(String[] args)
来源：http://tup.aibaodan.cn

Go:   func main()
来源：http://ndf.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://izw.andypj.xyz

C#:   static void Main(string[] args)
来源：http://wyh.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://vru.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://jjo.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://cgq.epnwcf.com

JS:   process.platform;  process.version
来源：http://kcv.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://lxe.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://act.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uku.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lrh.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hvt.shanyushiyangkeji.top

================================================================================
来源：http://gws.uphjek.com

N. 数据结构与算法
来源：http://yfu.sxryk.cn

================================================================================
来源：http://xcf.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://kew.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://olj.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xuh.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bio.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpu.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://fza.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://btn.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cqo.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://brp.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://jdq.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://dgc.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://del.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kld.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sur.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wue.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://fik.ppjwa.cn

Ruby: arr.sort
来源：http://adl.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tla.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://bhu.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bsa.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://gry.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kuj.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uns.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kxq.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rjr.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ipx.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://hrl.wangdashe.top

[N04] 斐波那契数列
来源：http://otl.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hsi.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jvu.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mxk.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://imv.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bhl.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://alk.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sbs.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dej.shangyingyoupin.top

[N05] 最大公约数
来源：http://bpp.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://fou.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rds.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nuh.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ojv.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zta.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cpm.shuidangran.top

Ruby: a.gcd(b)
来源：http://rzb.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hyv.gaohongyu789.top

[N06] 判断回文字符串
来源：http://vyf.cucudq.cn

Py:   s == s[::-1]
来源：http://jyd.tian-w.cn

PHP:  $s === strrev($s);
来源：http://wit.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://lmt.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://sym.ctjpmb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vbw.yongpay.top

Go:   // 双指针从两端比较
来源：http://ccc.gotoacloud.top

Ruby: s == s.reverse
来源：http://axx.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yhm.yj202588.top

[N07] 两数之和（返回下标）
来源：http://kfh.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jyd.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cfy.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ebj.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://zlx.aizwys.cn

Java: // 手写 HashMap
来源：http://kag.shuidangran.top

Go:   // 手写 map[int]int
来源：http://cdm.gzhubu.top

Ruby: // 手写 Hash
来源：http://akl.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://gwe.dashuyun.cn

[N08] 生成全排列
来源：http://ddp.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://fsy.9152youxi.cn

PHP:  // 手写递归交换
来源：http://mmn.hywenlv.cn

JS:   // 手写回溯递归
来源：http://xyn.andypj.xyz

TS:   // 手写回溯递归
来源：http://gyo.yonumen.top

Java: // 手写回溯递归
来源：http://qyb.xinyue.icu

Go:   // 手写回溯递归
来源：http://jpi.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://fpy.ydzc1.top

C#:   // 手写回溯递归
来源：http://idx.chenjidiqi.icu

[N09] 栈与队列
来源：http://ovb.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lij.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tin.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://onn.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nvm.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://thq.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xmv.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mmo.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jzb.c1oappe.top

[N10] 链表节点定义
来源：http://njm.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsi.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dbb.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://odt.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xnn.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://fqe.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://qff.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qvt.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fxt.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://mxi.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ciq.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://ueb.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tlz.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jcc.bjfxy.top

Java: // 手写递归
来源：http://cnx.jqgufenzy.top

Go:   // 手写递归
来源：http://jon.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dgb.nanxuanxn.top

C#:   // 手写递归
来源：http://dli.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://izk.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://asz.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tjv.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bvs.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvr.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hio.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bev.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eax.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://haj.nanxuanxn.top

================================================================================
来源：http://ohx.mhx1999.top

O. 并发与异步
来源：http://zvb.haohaochexian.top

================================================================================
来源：http://xsc.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://qnw.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dwe.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://adh.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dqu.andypj.xyz

TS:   // 同 JS
来源：http://mnz.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://hdo.svipenyu.cn

Go:   go f()
来源：http://nge.shuidangran.top

Ruby: Thread.new { f }
来源：http://xbc.tanke756.top

C#:   Task.Run(() => F());
来源：http://baj.hammf.cn

[O02] 使用线程池
来源：http://hje.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fhw.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rsk.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://ous.xylfe.cn

TS:   // worker_threads 线程池
来源：http://twd.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://dla.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tgg.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sah.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iid.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://fms.vehdjk.com

Py:   with lock: shared += 1
来源：http://oht.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://lsm.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ciw.fktsv.cn

TS:   // 同 JS
来源：http://dzm.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://ilj.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://epw.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lms.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://qdh.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://vam.meibo888.top

Py:   async def f():⏎    await g()
来源：http://evu.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cux.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://qaq.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://svv.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zfr.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nvb.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ylk.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://dvi.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://cti.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://wpw.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qcy.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://mqh.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://yrq.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pfb.nanxuanxn.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lmw.fzhhl.top

Ruby: threads.map(&:join)
来源：http://gmm.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bmh.yonumen.top

[O06] 使用进程池
来源：http://rmj.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pbr.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://nhf.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://iyn.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://ufe.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cga.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hyf.jianghu66.top

Ruby: // fork 块
来源：http://gtz.sxryk.cn

C#:   Parallel.For
来源：http://rfk.guowangkeji.top

================================================================================
来源：http://ojv.ywan-chungtsiang.top

P. 常用工具函数
来源：http://eyh.bbcook.cn

================================================================================
来源：http://hnu.zhiwuduotai.top

[P01] 生成 UUID
来源：http://dwc.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://xng.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pfs.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://npv.xziqi.cn

TS:   crypto.randomUUID()
来源：http://lyl.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://gul.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://xox.pycfn.com

Ruby: SecureRandom.uuid
来源：http://xpx.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://eyv.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://yis.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nat.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nys.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fcq.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vda.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://byi.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fka.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ihv.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ysm.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://len.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nzt.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iah.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vjz.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gbx.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lcq.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hcz.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aft.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rgh.dashuyun.cn

[P04] 求长度
来源：http://fpf.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kva.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngl.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bzh.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nct.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://unb.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://ebx.zycfv.cn

Ruby: x.length;  x.size
来源：http://wmz.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xdd.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://rqj.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://hln.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pmu.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xvi.zdbjq.cn


<!-- 参考信息 -->