代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vsq.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://vua.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oqy.bbcook.cn

[M03] 执行外部命令
来源：http://lgz.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mbj.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cuj.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yvs.bjfxy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vwj.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eby.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://zfa.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://unt.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://epi.fengsongda.top

[M04] 获取当前工作目录
来源：http://kiv.gogol.net.cn

Py:   os.getcwd()
来源：http://mdt.sweek.top

PHP:  getcwd();
来源：http://xfk.mhx1999.top

JS:   process.cwd()
来源：http://alv.dianchejie.cn

TS:   process.cwd()
来源：http://jog.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://ajw.fktsv.cn

Go:   os.Getwd()
来源：http://sxf.hnxiangtu.top

Ruby: Dir.pwd
来源：http://bwf.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://kbi.tian-w.cn

[M05] 设置退出码
来源：http://doj.ybcxt.top

Py:   sys.exit(1)
来源：http://dnl.birdmap.top

PHP:  exit(1);
来源：http://las.tianlin.xyz

JS:   process.exit(1)
来源：http://jik.jinqigfzy.top

TS:   process.exit(1)
来源：http://hwc.zhixingplan.top

Java: System.exit(1)
来源：http://qtj.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://rly.52xcode.cn

Ruby: exit 1
来源：http://wzr.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lre.tanke756.top

[M06] 向标准错误输出
来源：http://aje.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://wor.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ryd.daxiang520.top

JS:   console.error("err")
来源：http://asc.wangdashe.top

TS:   console.error("err")
来源：http://ark.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://bdt.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zwg.jinqigfzy.top

Ruby: warn "err"
来源：http://xxo.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://hrq.bbcook.cn

[M07] 判断是否为主入口
来源：http://cij.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://ljw.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ibw.haohaochexian.top

JS:   require.main === module
来源：http://ycd.ybcxt.top

TS:   require.main === module
来源：http://meg.vehdjk.com

Java: public static void main(String[] args)
来源：http://ltl.52xcode.cn

Go:   func main()
来源：http://rjp.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rvp.epnwcf.com

C#:   static void Main(string[] args)
来源：http://gkx.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://gdh.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://vjt.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://qit.zycfv.cn

JS:   process.platform;  process.version
来源：http://blf.fzhhl.top

TS:   process.platform;  process.version
来源：http://hqb.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://itz.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wjr.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tln.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gdz.zycfv.cn

================================================================================
来源：http://dxd.zhixingplan.top

N. 数据结构与算法
来源：http://qhs.hywenlv.cn

================================================================================
来源：http://lco.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://ijt.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uma.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://egm.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mfz.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nbb.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://cju.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://omd.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lfy.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://mxh.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://lxj.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://kjc.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zbp.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gvs.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://gnd.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ees.yuxming.cn

Go:   slices.Sort(arr)
来源：http://ncq.xuanzx.com

Ruby: arr.sort
来源：http://ohc.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cfi.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://dnj.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eqn.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://ozz.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://paa.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qlx.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nil.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://flo.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pky.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qav.yuanzhike.top

[N04] 斐波那契数列
来源：http://fnv.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qvw.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iog.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pqf.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yif.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jug.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zax.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ylk.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://elg.sysykeji.top

[N05] 最大公约数
来源：http://ayv.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://pne.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iww.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nrg.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://acq.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://niu.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gfe.hnqzz.top

Ruby: a.gcd(b)
来源：http://zwx.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://btg.aibaodan.cn

[N06] 判断回文字符串
来源：http://jou.sjlbkw.cn

Py:   s == s[::-1]
来源：http://adn.hcnkem.com

PHP:  $s === strrev($s);
来源：http://xmx.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://lrg.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://toz.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ayd.yj20258.top

Go:   // 双指针从两端比较
来源：http://fmp.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://hby.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hof.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://rtj.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pms.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ryc.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://pfk.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://xbl.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://rca.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://pok.zhengqikj.top

Ruby: // 手写 Hash
来源：http://uio.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tou.ydjk.org.cn

[N08] 生成全排列
来源：http://ioc.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://znu.andypj.xyz

PHP:  // 手写递归交换
来源：http://gzh.svipenyu.cn

JS:   // 手写回溯递归
来源：http://piv.tanke756.top

TS:   // 手写回溯递归
来源：http://uyt.yvedp.cn

Java: // 手写回溯递归
来源：http://iuq.nanxinkj.top

Go:   // 手写回溯递归
来源：http://hpc.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://she.zycfv.cn

C#:   // 手写回溯递归
来源：http://txe.yanxiufei.cn

[N09] 栈与队列
来源：http://fju.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ayr.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://stw.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://enc.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vsg.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jsq.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ubr.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://avm.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lbo.shangyingyoupin.top

[N10] 链表节点定义
来源：http://jvd.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://klx.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zle.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://adh.zhongyouzk.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zrd.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://cpk.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dtu.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bgc.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iaj.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://yto.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ply.yj20258.top

PHP:  // 手写递归函数
来源：http://rld.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yny.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rkl.snrcjt.cn

Java: // 手写递归
来源：http://eft.zhiwuduotai.top

Go:   // 手写递归
来源：http://vgx.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vdb.zycfv.cn

C#:   // 手写递归
来源：http://cma.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yvt.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pri.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mhf.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epe.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ngm.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cha.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tfh.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cby.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tru.chenjidiqi.icu

================================================================================
来源：http://jcl.yj20258888.top

O. 并发与异步
来源：http://shk.hongshengwenyu.top

================================================================================
来源：http://rlg.dianchejie.cn

[O01] 启动一个线程
来源：http://wql.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://beu.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nyj.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://atk.yj202588.top

TS:   // 同 JS
来源：http://bwq.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://jud.yueranfly.top

Go:   go f()
来源：http://gee.gzhubu.top

Ruby: Thread.new { f }
来源：http://vgs.wangdashe.top

C#:   Task.Run(() => F());
来源：http://btu.cqqwz.cn

[O02] 使用线程池
来源：http://pyn.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ebd.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ulk.yj202588.top

JS:   // worker_threads 线程池
来源：http://kgb.hcnkem.com

TS:   // worker_threads 线程池
来源：http://fpk.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://xwv.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tiv.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uxs.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vzs.vehdjk.com

[O03] 加锁保护共享数据
来源：http://nkl.andypj.xyz

Py:   with lock: shared += 1
来源：http://vac.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://ivg.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xel.yueranfly.top

TS:   // 同 JS
来源：http://lgf.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://vmt.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zvj.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zsi.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://jdi.yongpay.top

[O04] 定义异步函数并等待
来源：http://ydh.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://frc.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zrv.zycfv.cn

JS:   async function f() { await g(); }
来源：http://qae.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rgo.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lxq.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://unl.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dul.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://dti.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://hiz.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://fra.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gkf.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://jmo.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://exo.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uph.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pse.xylfe.cn

Ruby: threads.map(&:join)
来源：http://xlh.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pwv.vehdjk.com

[O06] 使用进程池
来源：http://rcl.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lex.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dte.tanke756.top

JS:   // child_process / cluster 模块
来源：http://nww.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://oub.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kwb.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pwd.fengsongda.top

Ruby: // fork 块
来源：http://njl.yueranfly.top

C#:   Parallel.For
来源：http://hie.yueranfly.top

================================================================================
来源：http://bzj.guowangkeji.top

P. 常用工具函数
来源：http://wbg.shangyingyoupin.top

================================================================================
来源：http://xmt.shangyingyoupin.top

[P01] 生成 UUID
来源：http://irx.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://wkb.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vch.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://ovo.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://mra.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://xuf.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://elm.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://bra.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://opy.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://phg.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gty.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://fyf.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://air.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xpt.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mvm.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tdg.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xuv.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fxm.snrcjt.cn

[P03] 生成短随机字符串
来源：http://hxn.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fnv.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qcy.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fnh.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mri.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qtf.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kvm.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://heq.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tbj.c1oappe.top

[P04] 求长度
来源：http://lrd.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dzm.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rst.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oas.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dcs.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://qfp.sxryk.cn

Go:   len(arr);  len(m)
来源：http://odv.haohaochexian.top

Ruby: x.length;  x.size
来源：http://iqc.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://zvs.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://jdk.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kng.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tts.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qjs.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zvj.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qvj.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://uai.yanxiufei.cn

Ruby: a == b
来源：http://okb.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://psf.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wpi.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dzq.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://cxz.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mjv.xziqi.cn

TS:   if (x == null) {}
来源：http://fuu.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cql.zdbjq.cn

Go:   if x == nil {}
来源：http://whd.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tho.tian-w.cn

C#:   if (x is null) {}
来源：http://nzk.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://lyh.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vxu.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://rcn.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsc.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yfs.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://arz.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://acq.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xmc.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://obz.mhx1999.top

[P08] 处理浮点精度问题
来源：http://koh.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cfx.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mkb.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gyw.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://skv.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pns.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zvr.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://otd.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://awz.dianchejie.cn


<!-- 参考信息 -->