代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tqb.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bgk.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://bsk.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://her.cashguo.top

[M04] 获取当前工作目录
来源：http://lbl.shuidangran.top

Py:   os.getcwd()
来源：http://zvf.aizwys.cn

PHP:  getcwd();
来源：http://vpk.xinyue.icu

JS:   process.cwd()
来源：http://jui.yj202588.top

TS:   process.cwd()
来源：http://veu.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://pfm.jiagoushi.top

Go:   os.Getwd()
来源：http://hje.chenlongwang.top

Ruby: Dir.pwd
来源：http://svk.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rrc.yvedp.cn

[M05] 设置退出码
来源：http://mgy.zhengqikj.top

Py:   sys.exit(1)
来源：http://jmq.chenzaomai.com

PHP:  exit(1);
来源：http://aeu.zhijiandao.cn

JS:   process.exit(1)
来源：http://gup.quarkkingdee.top

TS:   process.exit(1)
来源：http://wmc.cucudq.cn

Java: System.exit(1)
来源：http://acq.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://igm.havefunace.top

Ruby: exit 1
来源：http://vgp.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kbn.yfazqb.com

[M06] 向标准错误输出
来源：http://yqp.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://luc.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cfg.yonumen.top

JS:   console.error("err")
来源：http://spg.shangyingyoupin.top

TS:   console.error("err")
来源：http://gdl.tarul.cn

Java: System.err.println("err")
来源：http://nmu.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uyn.fanxiaobao.xyz

Ruby: warn "err"
来源：http://opy.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://hti.redwolf501.top

[M07] 判断是否为主入口
来源：http://xtw.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://phy.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ipb.jlsjyb.cn

JS:   require.main === module
来源：http://fwu.jyoumei.cn

TS:   require.main === module
来源：http://hpb.jqgfzy.top

Java: public static void main(String[] args)
来源：http://yvr.jlsjyb.cn

Go:   func main()
来源：http://oal.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ifm.ydzc1.top

C#:   static void Main(string[] args)
来源：http://rlv.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://fhr.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://kyb.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://lrd.pycfn.com

JS:   process.platform;  process.version
来源：http://jog.fengsongda.top

TS:   process.platform;  process.version
来源：http://anv.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ndp.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ewr.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ndd.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://csm.birdmap.top

================================================================================
来源：http://qnq.svipenyu.cn

N. 数据结构与算法
来源：http://xlx.zhaomingkeji.xyz

================================================================================
来源：http://ynn.cheryme.top

[N01] 二分查找（有序数组）
来源：http://amd.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://mbe.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://trz.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://una.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ral.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://ihp.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://qri.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dme.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://izu.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://sxs.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://vpu.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sqa.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qbp.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fcs.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aow.daria6918.cn

Go:   slices.Sort(arr)
来源：http://edl.hnqzz.top

Ruby: arr.sort
来源：http://xux.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsv.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://xln.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ofm.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://tra.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnn.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxg.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nrb.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eeg.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oil.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cor.316326.xyz

[N04] 斐波那契数列
来源：http://pxh.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wvx.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rfs.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uxx.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mzg.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tms.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cos.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zpf.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://phw.cheryme.top

[N05] 最大公约数
来源：http://gym.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://yrb.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yhg.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwh.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mec.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uwz.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ira.hnqzz.top

Ruby: a.gcd(b)
来源：http://ftm.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lgu.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://dkv.jiagoushi.top

Py:   s == s[::-1]
来源：http://ewh.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://qkv.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://lyc.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://lhm.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pmu.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://ums.hywenlv.cn

Ruby: s == s.reverse
来源：http://ebn.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://qzj.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://bud.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njz.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://beh.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gtn.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://wvr.yuanzhike.top

Java: // 手写 HashMap
来源：http://kin.gzhubu.top

Go:   // 手写 map[int]int
来源：http://ums.sufxvd.cn

Ruby: // 手写 Hash
来源：http://fty.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://rrd.yj20258.top

[N08] 生成全排列
来源：http://ibf.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://fjr.zdbjq.cn

PHP:  // 手写递归交换
来源：http://cdq.hywenlv.cn

JS:   // 手写回溯递归
来源：http://bcl.gzhubu.top

TS:   // 手写回溯递归
来源：http://fog.mhx1999.top

Java: // 手写回溯递归
来源：http://naf.havefunace.top

Go:   // 手写回溯递归
来源：http://ali.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://bqt.zdqjudy.top

C#:   // 手写回溯递归
来源：http://yfv.gotoacloud.top

[N09] 栈与队列
来源：http://hhe.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://maf.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xde.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://urq.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zoh.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zrf.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wir.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hop.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ngn.yfazqb.com

[N10] 链表节点定义
来源：http://soo.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rii.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ecz.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tgz.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qye.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://tby.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://isr.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://qvt.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://obx.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://ien.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wzx.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://gsi.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iuf.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nht.ybcxt.top

Java: // 手写递归
来源：http://fdg.bjfxy.top

Go:   // 手写递归
来源：http://xol.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bdq.ydjk.org.cn

C#:   // 手写递归
来源：http://pmw.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vlc.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fbg.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pit.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qsu.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://owm.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://erl.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dho.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xkn.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lqk.xingfuxueyuan.xyz

================================================================================
来源：http://mgq.haohaochexian.top

O. 并发与异步
来源：http://mvm.fzhhl.top

================================================================================
来源：http://qcy.zycfv.cn

[O01] 启动一个线程
来源：http://jty.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ulg.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ifu.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xgx.vehdjk.com

TS:   // 同 JS
来源：http://nro.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://yhf.shuidangran.top

Go:   go f()
来源：http://dfv.tianlin.xyz

Ruby: Thread.new { f }
来源：http://ysv.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://stq.pengpengdd.cyou

[O02] 使用线程池
来源：http://ulj.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sro.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nbu.xziqi.cn

JS:   // worker_threads 线程池
来源：http://ars.cashguo.top

TS:   // worker_threads 线程池
来源：http://hms.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://stz.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://msh.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://maz.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hxj.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://cum.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://szc.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://ugh.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zjb.zhixingplan.top

TS:   // 同 JS
来源：http://aqv.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://ypm.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://spe.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bvc.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://urc.guannengcc.top

[O04] 定义异步函数并等待
来源：http://tsl.cheryme.top

Py:   async def f():⏎    await g()
来源：http://nmj.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rwd.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://nlt.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qnr.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jkg.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nel.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oxx.yonumen.top

C#:   async Task F() { await G(); }
来源：http://opr.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://dxc.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://cns.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kec.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://waz.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://tux.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bse.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mqb.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://vjy.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://rts.yj202588.top

[O06] 使用进程池
来源：http://iia.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://svn.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bqv.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://csw.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://xdk.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uzc.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cdt.fehbvm.com

Ruby: // fork 块
来源：http://jan.yj202588.top

C#:   Parallel.For
来源：http://fdm.fanxiaobao.xyz

================================================================================
来源：http://gcs.bbcook.cn

P. 常用工具函数
来源：http://nuz.tian-w.cn

================================================================================
来源：http://uqw.yvedp.cn

[P01] 生成 UUID
来源：http://vyo.sweek.top

Py:   str(uuid.uuid4())
来源：http://tdy.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ref.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://qlt.daria6918.cn

TS:   crypto.randomUUID()
来源：http://jpq.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://gqr.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://pto.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://avz.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://rac.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://xnq.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qay.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://xta.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://skm.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hxc.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bmt.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xwj.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://osq.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://val.tianlin.xyz

[P03] 生成短随机字符串
来源：http://hgn.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hko.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bva.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fdd.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqg.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uva.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://btd.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tuh.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dhd.0kj1m.cn

[P04] 求长度
来源：http://hff.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://imi.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tdl.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nut.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yex.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://sbu.daria6918.cn

Go:   len(arr);  len(m)
来源：http://azx.meibo888.top

Ruby: x.length;  x.size
来源：http://wbv.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xoe.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://pqk.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zbn.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ovs.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eev.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cdv.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mdq.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://uqb.zhixingplan.top

Ruby: a == b
来源：http://ouc.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kez.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://efj.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dqy.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://dxt.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vcs.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://ksl.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nih.yongpay.top

Go:   if x == nil {}
来源：http://nrk.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://skw.chenzaomai.com

C#:   if (x is null) {}
来源：http://agp.jinqigufen.top

[P07] 防抖与节流
来源：http://gkx.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nnt.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://cwe.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbx.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cja.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bkw.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tee.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqx.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pkf.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://eqj.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aeu.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lny.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://alz.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gek.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vgp.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nfw.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tui.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jyl.yanxiufei.cn

================================================================================
来源：http://smz.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uev.yuxming.cn

================================================================================
来源：http://fsg.hywenlv.cn

[Q01] 创建表
来源：http://pmc.pycfn.com

CREATE TABLE users (
来源：http://fwe.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cmt.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://inc.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://hnb.jlsjyb.cn


<!-- 参考信息 -->