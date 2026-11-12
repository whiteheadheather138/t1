代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jzo.9152youxi.cn

JS:   process.env.HOME
来源：http://ugg.uphjek.com

TS:   process.env.HOME
来源：http://gey.jinqigufen.top

Java: System.getenv("HOME")
来源：http://khd.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zvm.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://hwk.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cgi.0kj1m.cn

[M03] 执行外部命令
来源：http://pil.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cnt.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://opm.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://mkm.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wrj.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qah.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wuj.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://qfn.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://tea.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://okt.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://aoo.0kj1m.cn

PHP:  getcwd();
来源：http://twu.316326.xyz

JS:   process.cwd()
来源：http://mny.fehbvm.com

TS:   process.cwd()
来源：http://fek.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://bej.jinqigfzy.top

Go:   os.Getwd()
来源：http://xds.daria6918.cn

Ruby: Dir.pwd
来源：http://npx.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://znz.cqqwz.cn

[M05] 设置退出码
来源：http://jdm.quarkkingdee.top

Py:   sys.exit(1)
来源：http://fne.yfazqb.com

PHP:  exit(1);
来源：http://gcq.cdnleiting.top

JS:   process.exit(1)
来源：http://plq.0kj1m.cn

TS:   process.exit(1)
来源：http://hix.jinqigufen.top

Java: System.exit(1)
来源：http://lyp.zhoulong.xyz

Go:   os.Exit(1)
来源：http://lrj.gogol.net.cn

Ruby: exit 1
来源：http://iyy.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fdu.ydjk.org.cn

[M06] 向标准错误输出
来源：http://tkl.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://xho.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zce.dianchejie.cn

JS:   console.error("err")
来源：http://cxx.shanyushiyangtech.top

TS:   console.error("err")
来源：http://akb.mhx1999.top

Java: System.err.println("err")
来源：http://ajp.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zac.tianlin.xyz

Ruby: warn "err"
来源：http://cww.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://bwn.sweek.top

[M07] 判断是否为主入口
来源：http://kfg.yj20258.top

Py:   if __name__ == "__main__":
来源：http://hhb.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sbf.feifeiyinyue.top

JS:   require.main === module
来源：http://vdp.shangyingyoupin.top

TS:   require.main === module
来源：http://scl.yongpay.top

Java: public static void main(String[] args)
来源：http://exq.zhiwuduotai.top

Go:   func main()
来源：http://pgg.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rmk.hnqzz.top

C#:   static void Main(string[] args)
来源：http://gqd.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://fdn.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://ifo.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://nep.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://mkb.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://deg.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tax.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://zqp.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wtq.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://few.gogol.net.cn

================================================================================
来源：http://iqh.fanxiaobao.xyz

N. 数据结构与算法
来源：http://xft.xuetiantiany.cn

================================================================================
来源：http://elt.tarul.cn

[N01] 二分查找（有序数组）
来源：http://ukk.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://lfy.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vpt.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmu.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksa.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://kna.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://xxc.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bur.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rdw.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://lxp.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://txq.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ilj.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://apf.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://drq.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://asz.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://iqe.fktsv.cn

Ruby: arr.sort
来源：http://sxz.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gdk.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://zcx.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rjm.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://xlo.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jmk.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdr.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pvk.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xco.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://por.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://mwd.ydzc1.top

[N04] 斐波那契数列
来源：http://sxm.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jph.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hda.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lyp.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cdf.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pql.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xxj.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ura.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gux.ivvv.top

[N05] 最大公约数
来源：http://dma.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://pbt.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://agq.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szc.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qyg.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ipx.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hic.hywenlv.cn

Ruby: a.gcd(b)
来源：http://ucy.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dyx.nwbrower.top

[N06] 判断回文字符串
来源：http://zda.wangdashe.top

Py:   s == s[::-1]
来源：http://kny.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://mys.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://huj.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://bbd.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://swz.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://fpi.iojbl.cn

Ruby: s == s.reverse
来源：http://jpp.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://snv.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://pjo.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lum.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://chw.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ipc.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://tpu.yangfankeji.com

Java: // 手写 HashMap
来源：http://urz.hesvh.cn

Go:   // 手写 map[int]int
来源：http://wks.meibo888.top

Ruby: // 手写 Hash
来源：http://mdf.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://edc.yj20258888.top

[N08] 生成全排列
来源：http://tpd.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://bne.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://wjj.yueranfly.top

JS:   // 手写回溯递归
来源：http://bco.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://jqu.fengsongda.top

Java: // 手写回溯递归
来源：http://ugx.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://qok.uphjek.com

Ruby: arr.permutation.to_a
来源：http://uzm.316326.xyz

C#:   // 手写回溯递归
来源：http://ijy.hesvh.cn

[N09] 栈与队列
来源：http://vky.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bgq.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lgy.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cnl.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://emt.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xes.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wll.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yov.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://thf.fengsongda.top

[N10] 链表节点定义
来源：http://sai.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gzl.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://skx.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mby.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zrw.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://xmk.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ljv.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xpj.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zkr.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://tol.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ows.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://jjy.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sae.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://auj.redwolf501.top

Java: // 手写递归
来源：http://rdy.hongshengwenyu.top

Go:   // 手写递归
来源：http://ebd.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bke.gotoacloud.top

C#:   // 手写递归
来源：http://rmj.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xhl.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ldq.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://okk.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ual.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ksj.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xte.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mff.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fwr.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rbf.yongpay.top

================================================================================
来源：http://ywl.vqdsnc.cn

O. 并发与异步
来源：http://ugc.hnxiangtu.top

================================================================================
来源：http://djj.dianchejie.cn

[O01] 启动一个线程
来源：http://mgq.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wgp.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uxo.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sjf.daria6918.cn

TS:   // 同 JS
来源：http://izf.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://rjp.jianghu66.top

Go:   go f()
来源：http://lud.vehdjk.com

Ruby: Thread.new { f }
来源：http://udj.cashguo.top

C#:   Task.Run(() => F());
来源：http://nkd.gaohongyu789.top

[O02] 使用线程池
来源：http://ocu.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qap.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://elg.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://nhg.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://jtf.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://yfg.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://axn.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xao.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iyi.aizwys.cn

[O03] 加锁保护共享数据
来源：http://neq.fktsv.cn

Py:   with lock: shared += 1
来源：http://rlg.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://hlu.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bgm.hnxiangtu.top

TS:   // 同 JS
来源：http://usj.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://pko.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gjf.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mhb.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://urp.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://pel.yongpay.top

Py:   async def f():⏎    await g()
来源：http://afo.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://its.andypj.xyz

JS:   async function f() { await g(); }
来源：http://ypf.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xvp.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xam.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://euk.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://soz.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://yvg.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://ezj.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://hfp.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hyi.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://eno.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://ofk.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pei.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fda.ivvv.top

Ruby: threads.map(&:join)
来源：http://erb.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://htv.zhiwuduotai.top

[O06] 使用进程池
来源：http://hqf.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://opc.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pbo.cashguo.top

JS:   // child_process / cluster 模块
来源：http://gdv.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://eep.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://trc.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xfw.tanke756.top

Ruby: // fork 块
来源：http://dzh.tanke756.top

C#:   Parallel.For
来源：http://zgj.aizwys.cn

================================================================================
来源：http://akg.nanxuanxn.top

P. 常用工具函数
来源：http://nup.ywan-chungtsiang.top

================================================================================
来源：http://sqo.zhijiandao.cn

[P01] 生成 UUID
来源：http://zyz.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://frx.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dho.iojbl.cn

JS:   crypto.randomUUID()
来源：http://ffb.tarul.cn

TS:   crypto.randomUUID()
来源：http://grf.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://wdy.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://riw.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://nrk.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://qpe.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://ekp.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hwm.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bhp.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uny.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qar.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lpo.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rvs.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pwc.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pvs.andypj.xyz

[P03] 生成短随机字符串
来源：http://maa.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://djg.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qlj.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zpw.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wku.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iho.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xec.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xxd.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sqs.jqgfzy.top

[P04] 求长度
来源：http://zbz.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ibl.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xvp.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://exj.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bts.cucudq.cn

Java: list.size();  map.size();  s.length()
来源：http://gmg.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://gga.meibo888.top

Ruby: x.length;  x.size
来源：http://uju.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rxb.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://mxe.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bae.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cbp.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rzx.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hvu.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bmb.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://ens.tarul.cn

Ruby: a == b
来源：http://fut.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ela.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dcx.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://edr.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://fij.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yzt.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://wnb.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://usi.sysykeji.top

Go:   if x == nil {}
来源：http://mxb.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yjg.hfpthk.cn

C#:   if (x is null) {}
来源：http://wac.jinqigfzy.top

[P07] 防抖与节流
来源：http://fin.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kmy.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://iip.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yaz.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://giw.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://url.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mcf.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bdq.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://izj.yfazqb.com

[P08] 处理浮点精度问题
来源：http://ntd.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ifs.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gmf.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jaw.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://juc.jqgufenzy.top


<!-- 参考信息 -->