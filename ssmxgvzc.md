代发 wailian999

C#:   (int)resp.StatusCode
来源：http://rzd.shzxlz.cn

[L08] 并发请求多个地址
来源：http://hsx.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fcd.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://vmq.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ltz.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gro.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gzp.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jqs.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yab.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ryu.jinghuilouyu.cn

================================================================================
来源：http://bjz.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://moq.wangshuangyany.cn

================================================================================
来源：http://kco.guannengcc.top

[M01] 读取命令行参数
来源：http://wtu.yueranfly.top

Py:   sys.argv[1:]
来源：http://imb.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://ysw.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://ago.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://bxm.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://shk.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://uqh.yangfankeji.com

Ruby: ARGV
来源：http://cmh.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://whc.zhongyouzk.top

[M02] 读取环境变量
来源：http://ocg.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://qwn.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nhi.yanxiufei.cn

JS:   process.env.HOME
来源：http://jdu.tanke756.top

TS:   process.env.HOME
来源：http://gyc.iojbl.cn

Java: System.getenv("HOME")
来源：http://bkx.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nek.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://vfb.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gbb.nanxinkj.top

[M03] 执行外部命令
来源：http://bkw.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bdw.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xgg.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zge.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zpv.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cbk.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://skt.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://zbt.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://ecj.tanke756.top

[M04] 获取当前工作目录
来源：http://hra.xuetiantiany.cn

Py:   os.getcwd()
来源：http://jml.yanxiufei.cn

PHP:  getcwd();
来源：http://uoa.feifeiyinyue.top

JS:   process.cwd()
来源：http://gfe.redwolf501.top

TS:   process.cwd()
来源：http://qah.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://qcu.chenjidiqi.icu

Go:   os.Getwd()
来源：http://ojf.jlsjyb.cn

Ruby: Dir.pwd
来源：http://zgc.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tmq.hfpthk.cn

[M05] 设置退出码
来源：http://xwk.bbcook.cn

Py:   sys.exit(1)
来源：http://xnq.sweek.top

PHP:  exit(1);
来源：http://hej.jyoumei.cn

JS:   process.exit(1)
来源：http://pti.hesvh.cn

TS:   process.exit(1)
来源：http://zvx.birdmap.top

Java: System.exit(1)
来源：http://hyb.ctjpmb.com

Go:   os.Exit(1)
来源：http://wpu.bjfxy.top

Ruby: exit 1
来源：http://jrn.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pez.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://ywu.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://tdr.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bup.yuxming.cn

JS:   console.error("err")
来源：http://wpq.chenjidiqi.icu

TS:   console.error("err")
来源：http://aio.vehdjk.com

Java: System.err.println("err")
来源：http://php.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ryi.shanyushiyangtech.top

Ruby: warn "err"
来源：http://smm.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://csa.hcnkem.com

[M07] 判断是否为主入口
来源：http://dmo.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://sas.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aqy.jianghu66.top

JS:   require.main === module
来源：http://jqj.xylfe.cn

TS:   require.main === module
来源：http://lif.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://vyf.fehbvm.com

Go:   func main()
来源：http://arv.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wpp.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://poh.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://ewb.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://boy.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://rhc.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://nbo.yfazqb.com

TS:   process.platform;  process.version
来源：http://xwx.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bau.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gnw.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pvt.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://afg.ctjpmb.com

================================================================================
来源：http://weg.52xcode.cn

N. 数据结构与算法
来源：http://yjb.xinyue.icu

================================================================================
来源：http://jag.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://mxf.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hdm.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jao.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iuh.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jlo.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://xaf.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://edr.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rep.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://eyd.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://dyx.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://uqs.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hiq.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pdk.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vck.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xug.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://lqi.gotoacloud.top

Ruby: arr.sort
来源：http://qpo.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pup.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://cqw.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uec.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://ezz.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpb.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asz.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cyw.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ydj.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pph.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://phj.zdqjudy.top

[N04] 斐波那契数列
来源：http://njs.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gql.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ags.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbw.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivx.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fqs.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wau.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rqj.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fnl.sufxvd.cn

[N05] 最大公约数
来源：http://foz.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://mda.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qre.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jpa.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kyy.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://abz.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jzq.chenzaomai.com

Ruby: a.gcd(b)
来源：http://zwz.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gru.sxryk.cn

[N06] 判断回文字符串
来源：http://tcc.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://hji.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://vjp.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://aqj.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://bgc.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mdi.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://fmv.hnxiangtu.top

Ruby: s == s.reverse
来源：http://ujh.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bdr.yonumen.top

[N07] 两数之和（返回下标）
来源：http://kpw.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zmh.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zwy.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://kop.sweek.top

TS:   // 手写 Map<string, number>
来源：http://vqt.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://ezu.daxiang520.top

Go:   // 手写 map[int]int
来源：http://eog.tian-w.cn

Ruby: // 手写 Hash
来源：http://qmf.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://qjv.gzhubu.top

[N08] 生成全排列
来源：http://crb.yj202588.top

Py:   itertools.permutations(arr)
来源：http://hld.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://ytb.epnwcf.com

JS:   // 手写回溯递归
来源：http://xxg.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://aez.vqdsnc.cn

Java: // 手写回溯递归
来源：http://kwc.uphjek.com

Go:   // 手写回溯递归
来源：http://odm.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://ohe.9152youxi.cn

C#:   // 手写回溯递归
来源：http://rsb.yj20258888.top

[N09] 栈与队列
来源：http://ewm.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tvz.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gxy.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ghn.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://okd.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zmc.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rdv.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kvj.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://giq.cdnleiting.top

[N10] 链表节点定义
来源：http://pnj.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://has.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mjn.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zyk.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fpk.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://knx.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hpc.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://gex.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sfr.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://ohg.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://srt.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://hba.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jml.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gwf.pycfn.com

Java: // 手写递归
来源：http://hxf.zycfv.cn

Go:   // 手写递归
来源：http://mhp.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://axp.cashguo.top

C#:   // 手写递归
来源：http://nbb.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zfi.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nej.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mpb.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://drt.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://obo.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fly.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://emw.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rws.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xza.havefunace.top

================================================================================
来源：http://uhr.jianghu66.top

O. 并发与异步
来源：http://cuk.nanxuanxn.top

================================================================================
来源：http://url.haohaochexian.top

[O01] 启动一个线程
来源：http://oyp.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zaw.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://czs.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ogg.quarkkingdee.top

TS:   // 同 JS
来源：http://epk.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://swp.jinqigfzy.top

Go:   go f()
来源：http://oca.tian-w.cn

Ruby: Thread.new { f }
来源：http://ndb.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://nzv.epnwcf.com

[O02] 使用线程池
来源：http://sdv.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jnc.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kiq.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://hlw.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://crk.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://ndk.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://axg.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rqw.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://diw.redwolf501.top

[O03] 加锁保护共享数据
来源：http://ahz.tian-w.cn

Py:   with lock: shared += 1
来源：http://hot.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://cxe.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ovr.sxryk.cn

TS:   // 同 JS
来源：http://vlj.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://dqp.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oqi.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ahw.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://rhf.yuxming.cn

[O04] 定义异步函数并等待
来源：http://etk.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://zwv.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://seo.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://pxc.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ynx.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://les.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qsp.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://dyj.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://rsc.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://iza.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://tzn.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zlx.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://pjg.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://wxt.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gdp.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pwi.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://wnd.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xpg.quarkkingdee.top

[O06] 使用进程池
来源：http://qie.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mle.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yev.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://hev.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://ixg.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gzu.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rzc.daria6918.cn

Ruby: // fork 块
来源：http://ahw.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://zds.jqgufenzy.top

================================================================================
来源：http://wua.sxryk.cn

P. 常用工具函数
来源：http://rgi.zdqjudy.top

================================================================================
来源：http://bhm.vehdjk.com

[P01] 生成 UUID
来源：http://jmf.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://ykl.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://alo.cucudq.cn

JS:   crypto.randomUUID()
来源：http://nst.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://bxx.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://pqh.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://bya.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://qso.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://mdx.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://als.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gzy.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hrr.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://unw.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhh.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://scs.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dqz.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tnu.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zcd.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://mqr.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ssu.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rvm.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://txz.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xec.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://asp.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wkd.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bjg.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ggq.xuetiantiany.cn

[P04] 求长度
来源：http://rwc.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ixd.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ppi.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfm.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://adn.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://ooc.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://avo.uphjek.com

Ruby: x.length;  x.size
来源：http://aep.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vyu.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://svk.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://fad.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mtu.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://clm.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ngp.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eoi.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cpj.yj20258.top

Ruby: a == b
来源：http://kej.iojbl.cn


<!-- 参考信息 -->