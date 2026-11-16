代发 wailian999

Ruby: ARGV
来源：http://enl.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://koa.pengpengdd.cyou

[M02] 读取环境变量
来源：http://lks.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://mto.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yak.wangshuangyany.cn

JS:   process.env.HOME
来源：http://hsh.jqgfzy.top

TS:   process.env.HOME
来源：http://rtd.jiagoushi.top

Java: System.getenv("HOME")
来源：http://rga.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aey.birdmap.top

Ruby: ENV["HOME"]
来源：http://axe.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qje.sxryk.cn

[M03] 执行外部命令
来源：http://ufd.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rqr.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tpp.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cja.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hso.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yya.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qsf.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vil.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://kcu.aizwys.cn

[M04] 获取当前工作目录
来源：http://mmt.cdnleiting.top

Py:   os.getcwd()
来源：http://sdl.zhengqikj.top

PHP:  getcwd();
来源：http://oid.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://gyj.gaohongyu789.top

TS:   process.cwd()
来源：http://uyy.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://osz.bbcook.cn

Go:   os.Getwd()
来源：http://eng.gzhubu.top

Ruby: Dir.pwd
来源：http://oml.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kks.hysaishi.cn

[M05] 设置退出码
来源：http://dbj.c1oappe.top

Py:   sys.exit(1)
来源：http://bfr.tian-w.cn

PHP:  exit(1);
来源：http://tpk.fktsv.cn

JS:   process.exit(1)
来源：http://yuc.nanxuanxn.top

TS:   process.exit(1)
来源：http://gxh.shuidangran.top

Java: System.exit(1)
来源：http://aar.xuanzx.com

Go:   os.Exit(1)
来源：http://ikp.quarkkingdee.top

Ruby: exit 1
来源：http://ytn.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rri.nwbrower.top

[M06] 向标准错误输出
来源：http://sfo.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://ybq.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tfi.fzhhl.top

JS:   console.error("err")
来源：http://zql.hysaishi.cn

TS:   console.error("err")
来源：http://hkw.jlsjyb.cn

Java: System.err.println("err")
来源：http://jaw.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rgb.andypj.xyz

Ruby: warn "err"
来源：http://avq.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://ghf.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://cpe.birdmap.top

Py:   if __name__ == "__main__":
来源：http://lgw.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cim.shzxlz.cn

JS:   require.main === module
来源：http://xth.nanxuanxn.top

TS:   require.main === module
来源：http://svi.jyoumei.cn

Java: public static void main(String[] args)
来源：http://mfi.redwolf501.top

Go:   func main()
来源：http://yod.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jzc.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://ksb.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://ohp.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://wqp.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://jmv.fzhhl.top

JS:   process.platform;  process.version
来源：http://nbd.9152youxi.cn

TS:   process.platform;  process.version
来源：http://lft.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cbo.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://ncv.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cyy.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mbb.yangfankeji.com

================================================================================
来源：http://onv.zhiwuduotai.top

N. 数据结构与算法
来源：http://pqp.hesvh.cn

================================================================================
来源：http://qbu.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://nnz.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xwz.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://azt.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwd.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hjh.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wrr.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://wne.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mqw.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://jhe.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://syr.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://kfk.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eip.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cur.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uwz.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vdy.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://qrz.aibaodan.cn

Ruby: arr.sort
来源：http://eap.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zbv.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://mtf.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://crp.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://mke.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rjc.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsf.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://akg.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hvz.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tun.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zuc.hcnkem.com

[N04] 斐波那契数列
来源：http://hlh.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kmv.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ukn.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnr.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jor.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wpc.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sio.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wtq.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oki.xylfe.cn

[N05] 最大公约数
来源：http://kwh.yonumen.top

Py:   math.gcd(a, b)
来源：http://tap.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gfn.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edw.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kdg.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bab.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nho.guannengcc.top

Ruby: a.gcd(b)
来源：http://urr.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rvy.316326.xyz

[N06] 判断回文字符串
来源：http://mwy.daxiang520.top

Py:   s == s[::-1]
来源：http://myj.jianghu66.top

PHP:  $s === strrev($s);
来源：http://utj.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://jjc.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://ube.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kzz.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://ybd.zdqjudy.top

Ruby: s == s.reverse
来源：http://lon.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xwl.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://jec.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dfw.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ijc.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pql.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://lnr.daxiang520.top

Java: // 手写 HashMap
来源：http://maf.zycfv.cn

Go:   // 手写 map[int]int
来源：http://voo.hysaishi.cn

Ruby: // 手写 Hash
来源：http://xmo.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://dtr.vehdjk.com

[N08] 生成全排列
来源：http://fuj.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://ncp.fktsv.cn

PHP:  // 手写递归交换
来源：http://hyh.fktsv.cn

JS:   // 手写回溯递归
来源：http://ldn.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://uho.tian-w.cn

Java: // 手写回溯递归
来源：http://pmu.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://anf.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://lcx.havefunace.top

C#:   // 手写回溯递归
来源：http://fnt.quarkkingdee.top

[N09] 栈与队列
来源：http://bpk.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://put.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ldd.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tco.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ttm.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gff.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://equ.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yyu.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wvu.zhongyouzk.top

[N10] 链表节点定义
来源：http://bhg.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ncz.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cfo.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rmf.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://woy.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://xaz.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://adm.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yrw.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rlu.fengsongda.top

[N11] 二叉树中序遍历
来源：http://sth.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kpx.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://xqp.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mdb.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjd.ydzc1.top

Java: // 手写递归
来源：http://usv.chenjidiqi.icu

Go:   // 手写递归
来源：http://shx.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zuk.quarkkingdee.top

C#:   // 手写递归
来源：http://zfh.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tpe.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cfg.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://elp.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hwm.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nlh.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mav.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vvf.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gkz.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wns.hfpthk.cn

================================================================================
来源：http://mdf.aibaodan.cn

O. 并发与异步
来源：http://qmj.jyoumei.cn

================================================================================
来源：http://zal.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://xfz.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kpt.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hnf.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kxs.hongshengwenyu.top

TS:   // 同 JS
来源：http://zrg.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://wnv.mhx1999.top

Go:   go f()
来源：http://jhm.svipenyu.cn

Ruby: Thread.new { f }
来源：http://jjc.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://mdz.aibaodan.cn

[O02] 使用线程池
来源：http://kwg.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mtg.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://piw.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://tle.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://kep.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://rid.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://agt.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cta.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://til.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://jgk.tanke756.top

Py:   with lock: shared += 1
来源：http://oco.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://oxd.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bwx.pycfn.com

TS:   // 同 JS
来源：http://nym.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://owd.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fgj.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fnc.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://hoi.ybcxt.top

[O04] 定义异步函数并等待
来源：http://zhv.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://xly.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xnq.yvedp.cn

JS:   async function f() { await g(); }
来源：http://lkt.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://npo.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ltn.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dmi.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://tus.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://onu.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://wki.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://wty.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oph.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://trm.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://rve.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pzy.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyk.uphjek.com

Ruby: threads.map(&:join)
来源：http://noc.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qws.yj20258888.top

[O06] 使用进程池
来源：http://boz.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yxx.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rrm.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://npx.tanke756.top

TS:   // child_process / cluster 模块
来源：http://mim.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ati.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mkz.c1oappe.top

Ruby: // fork 块
来源：http://uul.ydzc1.top

C#:   Parallel.For
来源：http://erg.redwolf501.top

================================================================================
来源：http://egm.guannengcc.top

P. 常用工具函数
来源：http://mrp.hysaishi.cn

================================================================================
来源：http://hop.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://gsw.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://pdr.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bwv.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://unr.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://vvy.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://tgx.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://jxa.meibo888.top

Ruby: SecureRandom.uuid
来源：http://whe.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://ccz.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://rju.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://inv.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gci.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dfd.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gae.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nes.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kot.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cch.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dbi.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://rza.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fir.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fal.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbf.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jjn.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kgz.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jqm.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tre.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://phn.aizwys.cn

[P04] 求长度
来源：http://jgk.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bwj.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hyy.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://syb.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://clb.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://htt.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://xyd.dashuyun.cn

Ruby: x.length;  x.size
来源：http://had.xziqi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fdh.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://oju.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kpm.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ufu.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pjl.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://csu.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lhn.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://bbj.c1oappe.top

Ruby: a == b
来源：http://acw.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hpk.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fpj.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hyr.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://dkm.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://slo.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://uam.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://sdk.nwbrower.top

Go:   if x == nil {}
来源：http://jhg.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gdd.yongpay.top

C#:   if (x is null) {}
来源：http://vak.hywenlv.cn

[P07] 防抖与节流
来源：http://qcp.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fqe.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://tft.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tjl.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uoo.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oyo.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fpc.pengpengdd.cyou

Ruby: // 手写闭包 + Time.now 判断
来源：http://rbg.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zmg.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://ccy.chenjidiqi.icu


<!-- 参考信息 -->