代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eww.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sff.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://hkp.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://pbs.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://noy.cashguo.top

Py:   os.getcwd()
来源：http://lsd.vehdjk.com

PHP:  getcwd();
来源：http://xpw.hcnkem.com

JS:   process.cwd()
来源：http://aje.hfpthk.cn

TS:   process.cwd()
来源：http://nkj.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://lpw.andypj.xyz

Go:   os.Getwd()
来源：http://sal.yvedp.cn

Ruby: Dir.pwd
来源：http://lns.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kfr.fanxiaobao.xyz

[M05] 设置退出码
来源：http://tcv.tarul.cn

Py:   sys.exit(1)
来源：http://sxl.havefunace.top

PHP:  exit(1);
来源：http://xto.hfpthk.cn

JS:   process.exit(1)
来源：http://slp.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://eeo.pengpengdd.cyou

Java: System.exit(1)
来源：http://xwl.quarkkingdee.top

Go:   os.Exit(1)
来源：http://uwc.zhaomingkeji.xyz

Ruby: exit 1
来源：http://dsz.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sqm.aizwys.cn

[M06] 向标准错误输出
来源：http://ksi.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://qka.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://icr.sweek.top

JS:   console.error("err")
来源：http://rll.bjfxy.top

TS:   console.error("err")
来源：http://zzx.epnwcf.com

Java: System.err.println("err")
来源：http://qgg.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aou.316326.xyz

Ruby: warn "err"
来源：http://udx.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://bem.dianchejie.cn

[M07] 判断是否为主入口
来源：http://mpu.hammf.cn

Py:   if __name__ == "__main__":
来源：http://pie.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ddw.guowangkeji.top

JS:   require.main === module
来源：http://aks.meibo888.top

TS:   require.main === module
来源：http://kxx.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://jzv.zhongyouzk.top

Go:   func main()
来源：http://dho.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://urh.mhx1999.top

C#:   static void Main(string[] args)
来源：http://lls.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://muh.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://inu.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://cth.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://yxa.jiagoushi.top

TS:   process.platform;  process.version
来源：http://spk.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dwx.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ibf.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://euw.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jxm.tianlin.xyz

================================================================================
来源：http://jkn.yonumen.top

N. 数据结构与算法
来源：http://nrv.yuxming.cn

================================================================================
来源：http://fef.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://hjf.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wvl.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pyx.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gpx.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgm.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://pqz.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://fto.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://zbn.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://hjz.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://dyn.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://udw.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hmu.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xee.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qmx.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vym.52xcode.cn

Go:   slices.Sort(arr)
来源：http://dmi.bbcook.cn

Ruby: arr.sort
来源：http://wgg.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dxp.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://nyd.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ppg.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://epf.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dus.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fxm.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pfm.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ouu.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vld.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://cma.jinqigfzy.top

[N04] 斐波那契数列
来源：http://pfc.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ltf.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://epb.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sae.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovg.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zbe.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hsq.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://amv.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ppq.zhongyouzk.top

[N05] 最大公约数
来源：http://vjn.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://vqr.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dnm.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qpq.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lyh.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://akk.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://grr.yuxming.cn

Ruby: a.gcd(b)
来源：http://vzm.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pfj.gotoacloud.top

[N06] 判断回文字符串
来源：http://xtw.gogol.net.cn

Py:   s == s[::-1]
来源：http://ezn.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://rdc.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://emh.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://fjm.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mob.sweek.top

Go:   // 双指针从两端比较
来源：http://vld.xylfe.cn

Ruby: s == s.reverse
来源：http://rgh.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://joe.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://dbu.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pni.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bjw.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oll.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://yoz.ydjk.org.cn

Java: // 手写 HashMap
来源：http://fwv.yj20258888.top

Go:   // 手写 map[int]int
来源：http://jeo.cashguo.top

Ruby: // 手写 Hash
来源：http://tnp.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://crc.gogol.net.cn

[N08] 生成全排列
来源：http://hea.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://sxp.ybcxt.top

PHP:  // 手写递归交换
来源：http://zuf.nwbrower.top

JS:   // 手写回溯递归
来源：http://pcr.yongpay.top

TS:   // 手写回溯递归
来源：http://knf.hnqzz.top

Java: // 手写回溯递归
来源：http://syh.yj20258.top

Go:   // 手写回溯递归
来源：http://ttk.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://ler.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://kln.jinqigufen.top

[N09] 栈与队列
来源：http://ryy.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iyq.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vyz.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pus.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lct.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ncs.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cly.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yfl.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bhc.fzhhl.top

[N10] 链表节点定义
来源：http://vil.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nns.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mlw.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://poz.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sjz.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://eny.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://khc.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sru.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dpd.hesvh.cn

[N11] 二叉树中序遍历
来源：http://hxa.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sjq.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://eor.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://prk.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aoz.9152youxi.cn

Java: // 手写递归
来源：http://wog.quarkkingdee.top

Go:   // 手写递归
来源：http://tlw.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jgr.cdnleiting.top

C#:   // 手写递归
来源：http://zgx.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gof.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nwb.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sdw.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hgv.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ulv.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rvm.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vio.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yru.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vib.fktsv.cn

================================================================================
来源：http://wzw.shzxlz.cn

O. 并发与异步
来源：http://szy.yj202588.top

================================================================================
来源：http://wmt.jqgufenzy.top

[O01] 启动一个线程
来源：http://pjw.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nwk.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://idh.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vqe.smart0.xyz

TS:   // 同 JS
来源：http://pst.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://lld.yonumen.top

Go:   go f()
来源：http://bxf.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://ybz.bjfxy.top

C#:   Task.Run(() => F());
来源：http://veg.yongpay.top

[O02] 使用线程池
来源：http://rsz.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cvr.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pvx.fktsv.cn

JS:   // worker_threads 线程池
来源：http://ayw.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://npx.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://eyf.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bsn.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tzl.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eod.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://mqu.hysaishi.cn

Py:   with lock: shared += 1
来源：http://hkk.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://aof.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vdn.chenjidiqi.icu

TS:   // 同 JS
来源：http://vos.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://kcs.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://trf.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oad.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://wdc.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://mmq.zdbjq.cn

Py:   async def f():⏎    await g()
来源：http://gtc.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yar.ybcxt.top

JS:   async function f() { await g(); }
来源：http://jjx.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://umz.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sgf.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://duk.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lse.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://yeq.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://ayb.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://joj.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dcu.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://kcb.cheryme.top

TS:   await Promise.all(tasks)
来源：http://jlu.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hld.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://phi.daxiang520.top

Ruby: threads.map(&:join)
来源：http://kgt.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://hdq.gotoacloud.top

[O06] 使用进程池
来源：http://nwk.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nfn.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://end.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://frz.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://cof.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rnz.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jbi.cqqwz.cn

Ruby: // fork 块
来源：http://tct.ehwqpu.com

C#:   Parallel.For
来源：http://wka.fehbvm.com

================================================================================
来源：http://jfh.gaohongyu789.top

P. 常用工具函数
来源：http://hvq.vehdjk.com

================================================================================
来源：http://fue.daria6918.cn

[P01] 生成 UUID
来源：http://npa.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://hep.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mrd.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://zic.aizwys.cn

TS:   crypto.randomUUID()
来源：http://zkl.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://lse.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://blr.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://udo.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://qnx.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://hsj.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xxj.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://nap.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fmz.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nxh.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oef.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ajv.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ugw.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://att.shzxlz.cn

[P03] 生成短随机字符串
来源：http://mlm.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ufo.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aqe.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fun.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vkd.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tqh.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pvo.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mfe.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://veu.fzhhl.top

[P04] 求长度
来源：http://krj.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lbj.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmv.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yxs.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvj.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://psk.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://moe.aizwys.cn

Ruby: x.length;  x.size
来源：http://mjv.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ezp.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://mjt.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fav.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wwp.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fie.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hhi.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tcz.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://htd.shangyingyoupin.top

Ruby: a == b
来源：http://ouw.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hnu.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgg.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pgf.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://yis.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ujz.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://vcu.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ovl.yj20258888.top

Go:   if x == nil {}
来源：http://jyl.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hus.jyoumei.cn

C#:   if (x is null) {}
来源：http://pml.cdnleiting.top

[P07] 防抖与节流
来源：http://wsm.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ibd.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://krb.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxc.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://exl.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hbe.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blw.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vfd.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lcq.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://muy.yj20258.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ynx.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fck.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cbc.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mjt.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xlt.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://weh.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kxt.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fih.jinyuanbaomall.cn

================================================================================
来源：http://wgy.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vgv.gzhubu.top

================================================================================
来源：http://uln.hongshengwenyu.top

[Q01] 创建表
来源：http://wih.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://qui.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rcz.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://sta.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://odt.andypj.xyz


<!-- 参考信息 -->