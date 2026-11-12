代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://chh.fzhhl.top

JS:   process.env.HOME
来源：http://mqt.zhengqikj.top

TS:   process.env.HOME
来源：http://nsj.hnqzz.top

Java: System.getenv("HOME")
来源：http://xdq.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xee.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://wyc.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bnl.zdbjq.cn

[M03] 执行外部命令
来源：http://xpx.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ixw.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://csr.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://moc.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hnp.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fxe.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jks.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lke.jlsjyb.cn

C#:   Process.Start("ls", "-l");
来源：http://aag.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://meq.nwbrower.top

Py:   os.getcwd()
来源：http://bcc.jinqigufen.top

PHP:  getcwd();
来源：http://zxk.ydzc1.top

JS:   process.cwd()
来源：http://evb.xuanzx.com

TS:   process.cwd()
来源：http://dsq.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://lxs.zhiwuduotai.top

Go:   os.Getwd()
来源：http://pbf.yanxiufei.cn

Ruby: Dir.pwd
来源：http://gxo.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ysw.gogol.net.cn

[M05] 设置退出码
来源：http://zjn.xziqi.cn

Py:   sys.exit(1)
来源：http://aiu.jyoumei.cn

PHP:  exit(1);
来源：http://tdv.hcnkem.com

JS:   process.exit(1)
来源：http://ydl.mhx1999.top

TS:   process.exit(1)
来源：http://gno.jyoumei.cn

Java: System.exit(1)
来源：http://hky.aizwys.cn

Go:   os.Exit(1)
来源：http://emz.cheryme.top

Ruby: exit 1
来源：http://dtr.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://obk.ydjk.org.cn

[M06] 向标准错误输出
来源：http://eia.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://yuc.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zfw.zdbjq.cn

JS:   console.error("err")
来源：http://kew.wangdashe.top

TS:   console.error("err")
来源：http://cdf.chenzaomai.com

Java: System.err.println("err")
来源：http://nct.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dca.hongshengwenyu.top

Ruby: warn "err"
来源：http://tft.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://xmg.ybcxt.top

[M07] 判断是否为主入口
来源：http://fws.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://bvm.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gad.9152youxi.cn

JS:   require.main === module
来源：http://fnf.nanxuanxn.top

TS:   require.main === module
来源：http://pqv.yonumen.top

Java: public static void main(String[] args)
来源：http://kuk.ivvv.top

Go:   func main()
来源：http://vgp.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rdv.ybcxt.top

C#:   static void Main(string[] args)
来源：http://oju.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://qrm.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://fch.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://wbv.svipenyu.cn

JS:   process.platform;  process.version
来源：http://njs.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://ozs.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lgn.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dex.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iyz.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://clv.hfpthk.cn

================================================================================
来源：http://jzj.guannengcc.top

N. 数据结构与算法
来源：http://ami.jyoumei.cn

================================================================================
来源：http://omu.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://xkw.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://etz.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eoo.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xne.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yio.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://rka.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://rws.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jac.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://dlx.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://tsq.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://mzu.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nra.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://khi.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zqf.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ptq.sweek.top

Go:   slices.Sort(arr)
来源：http://kfg.c1oappe.top

Ruby: arr.sort
来源：http://khq.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tpo.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://euw.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hnf.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://mpr.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qum.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wmg.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dsv.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lgs.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pib.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://rhu.shzxlz.cn

[N04] 斐波那契数列
来源：http://sxf.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://byr.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wqt.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hrg.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zty.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nyi.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ruj.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dij.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wvx.mhx1999.top

[N05] 最大公约数
来源：http://dui.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ujp.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bvo.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qpw.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://upz.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bih.guowangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kze.sysykeji.top

Ruby: a.gcd(b)
来源：http://pfg.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uxf.ctjpmb.com

[N06] 判断回文字符串
来源：http://myn.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://vjy.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://qii.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://cmk.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://yva.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ygs.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://nwv.smart0.xyz

Ruby: s == s.reverse
来源：http://efn.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qmc.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://dfm.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://buo.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kqn.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rqo.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://ivm.zdbjq.cn

Java: // 手写 HashMap
来源：http://oli.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://qlb.hywenlv.cn

Ruby: // 手写 Hash
来源：http://mge.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://qmx.fengsongda.top

[N08] 生成全排列
来源：http://zde.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://eis.snrcjt.cn

PHP:  // 手写递归交换
来源：http://zjb.redwolf501.top

JS:   // 手写回溯递归
来源：http://mrs.yj20258.top

TS:   // 手写回溯递归
来源：http://pgb.hfpthk.cn

Java: // 手写回溯递归
来源：http://diw.fehbvm.com

Go:   // 手写回溯递归
来源：http://emo.havefunace.top

Ruby: arr.permutation.to_a
来源：http://ocg.zdqjudy.top

C#:   // 手写回溯递归
来源：http://pex.jinqigufen.top

[N09] 栈与队列
来源：http://nqx.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tgm.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://daw.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ehu.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dvh.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://arj.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zeu.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fjx.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wxk.hcnkem.com

[N10] 链表节点定义
来源：http://iuj.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jzn.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zey.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://caz.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rns.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://hnr.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ohd.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ulv.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lmc.mhx1999.top

[N11] 二叉树中序遍历
来源：http://ams.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aaq.yj20258.top

PHP:  // 手写递归函数
来源：http://hcx.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nqi.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfu.ppjwa.cn

Java: // 手写递归
来源：http://unu.cashguo.top

Go:   // 手写递归
来源：http://tng.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vdx.nanxinkj.top

C#:   // 手写递归
来源：http://cew.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qla.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vez.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iew.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://par.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://axi.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wwi.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tyy.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tmj.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bdo.jyoumei.cn

================================================================================
来源：http://pej.shuidangran.top

O. 并发与异步
来源：http://rqx.snrcjt.cn

================================================================================
来源：http://pdi.sweek.top

[O01] 启动一个线程
来源：http://srp.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xwo.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vku.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kcq.sufxvd.cn

TS:   // 同 JS
来源：http://efd.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://xbk.xuetiantiany.cn

Go:   go f()
来源：http://lrz.smart0.xyz

Ruby: Thread.new { f }
来源：http://nlg.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://wum.cqqwz.cn

[O02] 使用线程池
来源：http://hil.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://doy.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mui.yuxming.cn

JS:   // worker_threads 线程池
来源：http://wgq.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://uqn.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fqs.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kkl.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uev.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vfp.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://nak.sweek.top

Py:   with lock: shared += 1
来源：http://kud.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://znv.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pth.gogol.net.cn

TS:   // 同 JS
来源：http://wxz.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://ifd.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oqy.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nbg.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://ggw.zhengqikj.top

[O04] 定义异步函数并等待
来源：http://urm.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://tco.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://isd.xinyue.icu

JS:   async function f() { await g(); }
来源：http://wbm.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://whu.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hbf.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://klf.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://npv.meibo888.top

C#:   async Task F() { await G(); }
来源：http://heb.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://bim.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://ket.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ajb.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://ckg.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://lro.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://krg.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wxu.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://gpt.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ozp.jiagoushi.top

[O06] 使用进程池
来源：http://qru.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dnk.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ras.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://yta.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://sub.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zyr.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bmg.hesvh.cn

Ruby: // fork 块
来源：http://efp.smart0.xyz

C#:   Parallel.For
来源：http://wtv.aizwys.cn

================================================================================
来源：http://hwp.sweek.top

P. 常用工具函数
来源：http://nrr.nwbrower.top

================================================================================
来源：http://uio.shuidangran.top

[P01] 生成 UUID
来源：http://qcy.birdmap.top

Py:   str(uuid.uuid4())
来源：http://abx.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://azx.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://etf.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://ynn.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://wuj.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://pca.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://zau.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://dhc.zhixingplan.top

[P02] MD5 / SHA256 摘要
来源：http://nou.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rty.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qiy.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nlx.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hrb.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zxa.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://suc.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ycx.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ayd.havefunace.top

[P03] 生成短随机字符串
来源：http://tff.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vip.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hwi.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rmk.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jqx.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vec.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aoz.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cvb.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tew.yangfankeji.com

[P04] 求长度
来源：http://xqs.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tsm.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://isz.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qfw.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://btc.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://nwk.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://xua.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://waz.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jdu.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://npm.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tvj.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lre.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rwy.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ubu.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fnh.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://jld.xziqi.cn

Ruby: a == b
来源：http://azc.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ahf.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tqy.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://spb.havefunace.top

PHP:  if (empty($x)) {}
来源：http://vyl.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yuz.snrcjt.cn

TS:   if (x == null) {}
来源：http://sdr.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pze.yueranfly.top

Go:   if x == nil {}
来源：http://lsa.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mkx.hnxiangtu.top

C#:   if (x is null) {}
来源：http://aip.zhiwuduotai.top

[P07] 防抖与节流
来源：http://psc.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jrd.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://kff.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tkg.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpp.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tae.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hir.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://nac.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pef.yonumen.top

[P08] 处理浮点精度问题
来源：http://qos.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rka.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ogy.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hjr.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fwi.fzhhl.top


<!-- 参考信息 -->