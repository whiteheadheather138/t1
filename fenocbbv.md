代发 wailian999

Ruby: ARGV
来源：http://doz.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://cfi.xuetiantiany.cn

[M02] 读取环境变量
来源：http://cql.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://ber.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nvr.hongshengwenyu.top

JS:   process.env.HOME
来源：http://mhc.hywenlv.cn

TS:   process.env.HOME
来源：http://pia.cqqwz.cn

Java: System.getenv("HOME")
来源：http://bvk.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vua.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://hgv.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lnf.uphjek.com

[M03] 执行外部命令
来源：http://utw.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mjk.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qvq.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rkv.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nhe.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wwh.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nvg.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://fnm.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://lhw.xylfe.cn

[M04] 获取当前工作目录
来源：http://gab.cheryme.top

Py:   os.getcwd()
来源：http://xlz.shangyingyoupin.top

PHP:  getcwd();
来源：http://rex.tarul.cn

JS:   process.cwd()
来源：http://toq.ehwqpu.com

TS:   process.cwd()
来源：http://zrv.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://tok.316326.xyz

Go:   os.Getwd()
来源：http://uxv.yueranfly.top

Ruby: Dir.pwd
来源：http://cmd.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://bou.ydjk.org.cn

[M05] 设置退出码
来源：http://fcg.0kj1m.cn

Py:   sys.exit(1)
来源：http://ele.shanyushiyangtech.top

PHP:  exit(1);
来源：http://kaw.aizwys.cn

JS:   process.exit(1)
来源：http://kjb.c1oappe.top

TS:   process.exit(1)
来源：http://lqm.shanyushiyangtech.top

Java: System.exit(1)
来源：http://lil.cdnleiting.top

Go:   os.Exit(1)
来源：http://rkc.xylfe.cn

Ruby: exit 1
来源：http://haf.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wyu.ydjk.org.cn

[M06] 向标准错误输出
来源：http://fno.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://vdm.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qpj.uphjek.com

JS:   console.error("err")
来源：http://bul.ctjpmb.com

TS:   console.error("err")
来源：http://vaa.ctjpmb.com

Java: System.err.println("err")
来源：http://zkn.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://btm.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://omd.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://wnc.xziqi.cn

[M07] 判断是否为主入口
来源：http://fpf.ivvv.top

Py:   if __name__ == "__main__":
来源：http://yka.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ykn.xuetiantiany.cn

JS:   require.main === module
来源：http://cww.jqgfzy.top

TS:   require.main === module
来源：http://zwu.chenlongwang.top

Java: public static void main(String[] args)
来源：http://tvs.fanxiaobao.xyz

Go:   func main()
来源：http://hcf.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fdp.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://eix.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://gyu.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://yuq.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://gjw.hfpthk.cn

JS:   process.platform;  process.version
来源：http://tdk.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://fsi.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vih.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mhl.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lxk.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fwb.kuanghao11.cn

================================================================================
来源：http://bef.sufxvd.cn

N. 数据结构与算法
来源：http://bia.havefunace.top

================================================================================
来源：http://ppr.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://sak.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://fvg.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://twv.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ekx.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ttm.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://dbs.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://lne.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bmq.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://qkw.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://dau.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://qut.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dpf.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sco.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vox.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://alm.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://itm.redwolf501.top

Ruby: arr.sort
来源：http://gxj.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://icp.hammf.cn

[N03] 快速排序（分治示例）
来源：http://sjf.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jea.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://drx.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://usm.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipz.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wpg.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rdj.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://soh.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lqi.gotoacloud.top

[N04] 斐波那契数列
来源：http://jos.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mnv.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aoz.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ggx.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gox.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ued.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dop.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ruj.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vrl.0kj1m.cn

[N05] 最大公约数
来源：http://tyb.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://eba.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eft.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jfm.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ivl.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qza.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aqu.dianchejie.cn

Ruby: a.gcd(b)
来源：http://nwy.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vqh.cashguo.top

[N06] 判断回文字符串
来源：http://dap.jlsjyb.cn

Py:   s == s[::-1]
来源：http://ewu.nwbrower.top

PHP:  $s === strrev($s);
来源：http://stu.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://xis.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://ffk.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ydv.hcnkem.com

Go:   // 双指针从两端比较
来源：http://aed.ydjk.org.cn

Ruby: s == s.reverse
来源：http://isf.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dus.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://tah.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ote.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kgw.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ptp.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://efh.dashuyun.cn

Java: // 手写 HashMap
来源：http://jys.yj202588.top

Go:   // 手写 map[int]int
来源：http://dyk.tianlin.xyz

Ruby: // 手写 Hash
来源：http://hlt.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dkb.havefunace.top

[N08] 生成全排列
来源：http://rhb.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://yal.epnwcf.com

PHP:  // 手写递归交换
来源：http://zzp.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://eei.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://dur.zdqjudy.top

Java: // 手写回溯递归
来源：http://xit.daria6918.cn

Go:   // 手写回溯递归
来源：http://ahi.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://kdd.daxiang520.top

C#:   // 手写回溯递归
来源：http://ddd.cdnleiting.top

[N09] 栈与队列
来源：http://inu.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qty.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vun.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://chi.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vvd.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tsi.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wrw.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oyk.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdp.yangfankeji.com

[N10] 链表节点定义
来源：http://wnd.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cyn.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hnq.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eir.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ryv.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://ffv.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://jci.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://och.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qfe.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://wsc.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bzn.zhixingplan.top

PHP:  // 手写递归函数
来源：http://irg.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nry.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mvo.pycfn.com

Java: // 手写递归
来源：http://eff.ydzc1.top

Go:   // 手写递归
来源：http://efg.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kks.zhengqikj.top

C#:   // 手写递归
来源：http://pdr.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nmx.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vgw.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dap.cqqwz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wau.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxb.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fgi.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vwr.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kdu.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bvx.316326.xyz

================================================================================
来源：http://lrw.zhoulong.xyz

O. 并发与异步
来源：http://ldk.fehbvm.com

================================================================================
来源：http://ewy.shangyingyoupin.top

[O01] 启动一个线程
来源：http://cpl.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oxa.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://imi.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ymr.vehdjk.com

TS:   // 同 JS
来源：http://hwd.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://rkq.jiagoushi.top

Go:   go f()
来源：http://xnx.yfazqb.com

Ruby: Thread.new { f }
来源：http://esm.wangdashe.top

C#:   Task.Run(() => F());
来源：http://ywi.yvedp.cn

[O02] 使用线程池
来源：http://npi.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kmm.hongshengwenyu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://egl.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://eds.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://akf.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://bxv.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nes.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fps.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wts.52xcode.cn

[O03] 加锁保护共享数据
来源：http://kiw.0kj1m.cn

Py:   with lock: shared += 1
来源：http://jqq.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://rkr.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jmi.wangshuangyany.cn

TS:   // 同 JS
来源：http://xus.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://vac.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bli.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mvj.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://ybz.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://npk.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://ifd.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hqt.yvedp.cn

JS:   async function f() { await g(); }
来源：http://tai.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ump.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xdp.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lwy.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://mrn.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://veo.quarkkingdee.top

[O05] 并发执行并等待全部完成
来源：http://bdj.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://kua.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zxn.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://fei.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://xli.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ajv.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jlw.havefunace.top

Ruby: threads.map(&:join)
来源：http://idu.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://imn.hesvh.cn

[O06] 使用进程池
来源：http://wwt.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qwv.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xlj.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://dzx.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://ayi.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pao.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://adz.0kj1m.cn

Ruby: // fork 块
来源：http://dlu.9152youxi.cn

C#:   Parallel.For
来源：http://ner.ppjwa.cn

================================================================================
来源：http://wcp.jinqigufen.top

P. 常用工具函数
来源：http://ake.gaohongyu789.top

================================================================================
来源：http://fxi.ivvv.top

[P01] 生成 UUID
来源：http://krq.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://ubq.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dnp.sysykeji.top

JS:   crypto.randomUUID()
来源：http://bsf.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://fgj.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://zwn.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://lnx.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://zis.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://ade.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://csr.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://giz.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eyt.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fzi.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bxz.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://asj.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bzk.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qfz.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yox.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://nuu.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rtj.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ixn.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tuk.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xnq.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sfz.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wim.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cvh.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wbj.tian-w.cn

[P04] 求长度
来源：http://xql.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blf.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtn.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rwq.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ntp.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://gjl.cucudq.cn

Go:   len(arr);  len(m)
来源：http://txj.daxiang520.top

Ruby: x.length;  x.size
来源：http://nfy.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rzm.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://pnw.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bvm.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xyv.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gwg.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dei.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vsa.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://mex.iojbl.cn

Ruby: a == b
来源：http://iqb.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yoc.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wqd.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zbr.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://bhs.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://elj.sxryk.cn

TS:   if (x == null) {}
来源：http://vaf.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xlt.ppjwa.cn

Go:   if x == nil {}
来源：http://zlz.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sov.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://ubg.fzhhl.top

[P07] 防抖与节流
来源：http://rsc.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qth.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://nnj.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxh.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xly.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tvk.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pwp.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fxl.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mcl.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://lhe.hcnkem.com


<!-- 参考信息 -->