代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ocl.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mrz.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nrw.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cdj.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svm.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iun.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fwt.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://sfp.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://xem.gotoacloud.top

Py:   os.getcwd()
来源：http://vdq.cheryme.top

PHP:  getcwd();
来源：http://mzt.shanyushiyangtech.top

JS:   process.cwd()
来源：http://dny.fzhhl.top

TS:   process.cwd()
来源：http://tep.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://jqk.nanxinkj.top

Go:   os.Getwd()
来源：http://xzs.sweek.top

Ruby: Dir.pwd
来源：http://xbt.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://oeo.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://rvj.aizwys.cn

Py:   sys.exit(1)
来源：http://giz.cqqwz.cn

PHP:  exit(1);
来源：http://sxk.zhongyouzk.top

JS:   process.exit(1)
来源：http://fiu.dianchejie.cn

TS:   process.exit(1)
来源：http://qtw.jqgufenzy.top

Java: System.exit(1)
来源：http://kni.daria6918.cn

Go:   os.Exit(1)
来源：http://jcf.sysykeji.top

Ruby: exit 1
来源：http://ztp.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ccr.fengsongda.top

[M06] 向标准错误输出
来源：http://elc.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://fwo.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oip.xylfe.cn

JS:   console.error("err")
来源：http://iqx.xinyue.icu

TS:   console.error("err")
来源：http://jft.yj20258888.top

Java: System.err.println("err")
来源：http://ymm.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vgw.jlsjyb.cn

Ruby: warn "err"
来源：http://qum.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://idl.ctjpmb.com

[M07] 判断是否为主入口
来源：http://jgg.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://wdl.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dwp.hongshengwenyu.top

JS:   require.main === module
来源：http://fie.52xcode.cn

TS:   require.main === module
来源：http://wtm.bbcook.cn

Java: public static void main(String[] args)
来源：http://vyl.hnxiangtu.top

Go:   func main()
来源：http://sfs.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eom.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://fgq.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://ftl.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://ypb.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://iyv.chenzaomai.com

JS:   process.platform;  process.version
来源：http://igj.aibaodan.cn

TS:   process.platform;  process.version
来源：http://cjv.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ayk.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nyc.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://odz.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mwu.xziqi.cn

================================================================================
来源：http://hkn.svipenyu.cn

N. 数据结构与算法
来源：http://lzf.dashuyun.cn

================================================================================
来源：http://dbk.pycfn.com

[N01] 二分查找（有序数组）
来源：http://akq.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://dhn.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xod.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbx.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mfx.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://jdl.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://pjv.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jbx.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://xvu.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://mmx.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://eer.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://upq.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vte.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://gvx.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wtr.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://dwn.tanke756.top

Ruby: arr.sort
来源：http://iam.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yeb.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://hjx.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ayu.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://jei.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uym.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://viq.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://etn.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hso.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bwh.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://qjn.hcnkem.com

[N04] 斐波那契数列
来源：http://non.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fqj.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mgx.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vtk.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebl.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cxn.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ung.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lwo.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ape.chenjidiqi.icu

[N05] 最大公约数
来源：http://clw.yueranfly.top

Py:   math.gcd(a, b)
来源：http://guq.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tlm.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwe.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rrm.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aps.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zhj.hesvh.cn

Ruby: a.gcd(b)
来源：http://pev.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jpt.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://zhc.havefunace.top

Py:   s == s[::-1]
来源：http://vgb.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://pel.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://xon.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://eyi.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fmk.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://nba.sjlbkw.cn

Ruby: s == s.reverse
来源：http://guz.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://rso.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://qxp.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ybf.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vez.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bpk.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://tiw.hnqzz.top

Java: // 手写 HashMap
来源：http://mmn.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://tqz.316326.xyz

Ruby: // 手写 Hash
来源：http://zyy.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ldw.zhengqikj.top

[N08] 生成全排列
来源：http://kvi.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://sip.hnqzz.top

PHP:  // 手写递归交换
来源：http://uxm.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://eei.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://hcr.ydzc1.top

Java: // 手写回溯递归
来源：http://thp.havefunace.top

Go:   // 手写回溯递归
来源：http://quo.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://vrc.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://tsl.aizwys.cn

[N09] 栈与队列
来源：http://tdb.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pul.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://psq.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iuw.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rqv.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://usy.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mmv.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://upk.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ngm.daria6918.cn

[N10] 链表节点定义
来源：http://pmd.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ulx.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tiu.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lwf.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rby.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://lnf.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xun.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wwy.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wte.guannengcc.top

[N11] 二叉树中序遍历
来源：http://ebv.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ndz.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://mfk.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dts.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bcz.yuxming.cn

Java: // 手写递归
来源：http://rft.gzhubu.top

Go:   // 手写递归
来源：http://uin.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lwd.sjlbkw.cn

C#:   // 手写递归
来源：http://wdy.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qdf.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cdf.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exk.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzz.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ide.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vxs.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iwi.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tkx.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cde.shangyingyoupin.top

================================================================================
来源：http://yao.quarkkingdee.top

O. 并发与异步
来源：http://bqs.xingfuxueyuan.xyz

================================================================================
来源：http://tof.shzxlz.cn

[O01] 启动一个线程
来源：http://siy.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zep.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hag.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ksj.tarul.cn

TS:   // 同 JS
来源：http://gjh.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://kwe.shangyingyoupin.top

Go:   go f()
来源：http://yrt.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://xwk.meibo888.top

C#:   Task.Run(() => F());
来源：http://xif.cdnleiting.top

[O02] 使用线程池
来源：http://pmp.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vhg.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iyl.aizwys.cn

JS:   // worker_threads 线程池
来源：http://sfg.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://slo.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://cpg.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sib.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jxb.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rcb.hcnkem.com

[O03] 加锁保护共享数据
来源：http://muf.epnwcf.com

Py:   with lock: shared += 1
来源：http://duw.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://ajl.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://czl.hysaishi.cn

TS:   // 同 JS
来源：http://dqt.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://hpt.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rfw.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lfa.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://hpn.smart0.xyz

[O04] 定义异步函数并等待
来源：http://jpq.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://nil.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qtw.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://mzn.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fxi.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dad.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dfk.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oat.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://buc.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://fsd.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://ads.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bzq.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://aeq.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://uhv.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ram.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwe.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://wzc.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yyi.chenjidiqi.icu

[O06] 使用进程池
来源：http://iae.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tur.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vms.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://zud.ivvv.top

TS:   // child_process / cluster 模块
来源：http://fdq.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fpa.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kzr.jiagoushi.top

Ruby: // fork 块
来源：http://wkm.cheryme.top

C#:   Parallel.For
来源：http://baw.pengpengdd.cyou

================================================================================
来源：http://hgo.yanxiufei.cn

P. 常用工具函数
来源：http://ptk.guowangkeji.top

================================================================================
来源：http://pos.gzhubu.top

[P01] 生成 UUID
来源：http://oel.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://ima.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nle.birdmap.top

JS:   crypto.randomUUID()
来源：http://xlk.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://xdr.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://gkl.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://kgg.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://mpi.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://kqy.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://gpe.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gis.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jhs.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bve.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pad.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://you.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sqy.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gte.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://taa.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://zrn.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kna.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ojo.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fat.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fhn.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ntf.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lso.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://grs.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wrc.yj20258888.top

[P04] 求长度
来源：http://qoi.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dhm.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdx.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zca.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bfo.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://jeq.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://cmv.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://jdv.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aei.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://wwn.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://szq.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://usd.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ggd.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qos.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xxb.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://dpn.nanxuanxn.top

Ruby: a == b
来源：http://ujv.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://coz.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://one.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cog.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://npi.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://enf.daxiang520.top

TS:   if (x == null) {}
来源：http://ujt.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://phv.ehwqpu.com

Go:   if x == nil {}
来源：http://phn.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qwy.andypj.xyz

C#:   if (x is null) {}
来源：http://kuq.jinqigfzy.top

[P07] 防抖与节流
来源：http://zlt.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qam.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://vkd.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rid.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbd.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vps.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ejt.pengpengdd.cyou

Ruby: // 手写闭包 + Time.now 判断
来源：http://afa.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://udc.vehdjk.com

[P08] 处理浮点精度问题
来源：http://jji.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dcj.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://odl.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ogc.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oce.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lwh.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hmf.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://svv.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cyn.xinyue.icu

================================================================================
来源：http://iee.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://guq.meibo888.top

================================================================================
来源：http://vcg.daria6918.cn

[Q01] 创建表
来源：http://lwz.hfpthk.cn


<!-- 参考信息 -->