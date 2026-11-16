代发 wailian999

[M04] 获取当前工作目录
来源：http://vus.pycfn.com

Py:   os.getcwd()
来源：http://fwo.aizwys.cn

PHP:  getcwd();
来源：http://msc.hysaishi.cn

JS:   process.cwd()
来源：http://tfa.andypj.xyz

TS:   process.cwd()
来源：http://qoz.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://fzm.ydzc1.top

Go:   os.Getwd()
来源：http://otq.yangfankeji.com

Ruby: Dir.pwd
来源：http://mnf.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://lcv.sufxvd.cn

[M05] 设置退出码
来源：http://qnf.hnqzz.top

Py:   sys.exit(1)
来源：http://stk.jianghu66.top

PHP:  exit(1);
来源：http://gej.ydjk.org.cn

JS:   process.exit(1)
来源：http://ryz.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://arq.yuxming.cn

Java: System.exit(1)
来源：http://twm.ivvv.top

Go:   os.Exit(1)
来源：http://uxy.sweek.top

Ruby: exit 1
来源：http://osp.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qzl.nanxuanxn.top

[M06] 向标准错误输出
来源：http://npd.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://ngy.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://pyf.gotoacloud.top

JS:   console.error("err")
来源：http://kzf.feifeiyinyue.top

TS:   console.error("err")
来源：http://lvf.zycfv.cn

Java: System.err.println("err")
来源：http://cmc.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aoh.hnqzz.top

Ruby: warn "err"
来源：http://pbg.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://luc.fzhhl.top

[M07] 判断是否为主入口
来源：http://fzp.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://fad.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pln.andypj.xyz

JS:   require.main === module
来源：http://jzi.hnxiangtu.top

TS:   require.main === module
来源：http://mcu.sxryk.cn

Java: public static void main(String[] args)
来源：http://tml.yonumen.top

Go:   func main()
来源：http://fov.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://roe.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://gmg.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://ybo.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://kre.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://lwv.tanke756.top

JS:   process.platform;  process.version
来源：http://ghr.fehbvm.com

TS:   process.platform;  process.version
来源：http://euu.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sfq.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://mlf.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pwd.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nag.birdmap.top

================================================================================
来源：http://cdj.hfpthk.cn

N. 数据结构与算法
来源：http://lhs.aibaodan.cn

================================================================================
来源：http://qtp.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://pfm.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://emx.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://juo.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxg.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wnk.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lvs.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://obx.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kic.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://smd.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://ngt.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://hhy.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://avu.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sut.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://chm.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yyg.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://lgi.hnxiangtu.top

Ruby: arr.sort
来源：http://tpf.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://blt.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://wbb.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iby.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://dfw.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jiv.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccm.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://arg.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xbl.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fdw.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://rqt.snrcjt.cn

[N04] 斐波那契数列
来源：http://vqv.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qin.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jpd.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vob.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zsm.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cir.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ilw.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dkq.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lnl.jqgfzy.top

[N05] 最大公约数
来源：http://ezo.mhx1999.top

Py:   math.gcd(a, b)
来源：http://twv.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gna.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kru.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xih.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qib.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iyu.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://uyj.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qnw.hywenlv.cn

[N06] 判断回文字符串
来源：http://auz.hywenlv.cn

Py:   s == s[::-1]
来源：http://hhl.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://mrh.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://hom.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://cll.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fgo.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://dnr.316326.xyz

Ruby: s == s.reverse
来源：http://yfv.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yqv.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://xpq.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mbu.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bbb.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qki.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://kfc.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://lva.birdmap.top

Go:   // 手写 map[int]int
来源：http://bkf.cashguo.top

Ruby: // 手写 Hash
来源：http://kwy.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://bxu.dashuyun.cn

[N08] 生成全排列
来源：http://een.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://qmw.hysaishi.cn

PHP:  // 手写递归交换
来源：http://tlt.dashuyun.cn

JS:   // 手写回溯递归
来源：http://eje.tianlin.xyz

TS:   // 手写回溯递归
来源：http://cxw.daxiang520.top

Java: // 手写回溯递归
来源：http://ces.cdnleiting.top

Go:   // 手写回溯递归
来源：http://okg.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://rhc.hcnkem.com

C#:   // 手写回溯递归
来源：http://zih.redwolf501.top

[N09] 栈与队列
来源：http://cbf.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gkh.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://awq.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lse.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gkn.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aha.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jls.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ovb.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ctn.yvedp.cn

[N10] 链表节点定义
来源：http://shy.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ijr.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pwf.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rvp.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ltg.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://otk.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tar.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://qdy.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rri.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://ibz.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://prd.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://vvg.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfg.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vtx.zhongyouzk.top

Java: // 手写递归
来源：http://kpr.ehwqpu.com

Go:   // 手写递归
来源：http://fbr.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vwl.cdnleiting.top

C#:   // 手写递归
来源：http://tny.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gde.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://opq.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gwq.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wag.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cmf.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://syb.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kmk.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oxm.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://urp.smart0.xyz

================================================================================
来源：http://xha.wangdashe.top

O. 并发与异步
来源：http://hja.shanyushiyangkeji.top

================================================================================
来源：http://kjy.aibaodan.cn

[O01] 启动一个线程
来源：http://qhs.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://etu.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gim.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fak.gogol.net.cn

TS:   // 同 JS
来源：http://wvv.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://tiq.yanxiufei.cn

Go:   go f()
来源：http://yku.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://vtq.zycfv.cn

C#:   Task.Run(() => F());
来源：http://qjl.vehdjk.com

[O02] 使用线程池
来源：http://ejw.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://srv.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vbs.nwbrower.top

JS:   // worker_threads 线程池
来源：http://rig.vehdjk.com

TS:   // worker_threads 线程池
来源：http://ddj.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://drl.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vhb.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xsl.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vfi.cheryme.top

[O03] 加锁保护共享数据
来源：http://gny.gogol.net.cn

Py:   with lock: shared += 1
来源：http://cqo.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://wgs.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nkj.9152youxi.cn

TS:   // 同 JS
来源：http://zov.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://ksw.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ynv.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://pcr.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://par.52xcode.cn

[O04] 定义异步函数并等待
来源：http://rbj.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://law.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ksf.tian-w.cn

JS:   async function f() { await g(); }
来源：http://hlh.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yoz.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ppa.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oxa.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://exz.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://ugh.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://fip.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://aav.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qld.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://fdx.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://oel.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://prd.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hfn.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://iml.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bgr.jinghuilouyu.cn

[O06] 使用进程池
来源：http://uij.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://phs.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wxl.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://kae.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://gkr.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dnv.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nmg.yanxiufei.cn

Ruby: // fork 块
来源：http://sva.guowangkeji.top

C#:   Parallel.For
来源：http://qer.xylfe.cn

================================================================================
来源：http://pjl.chenlongwang.top

P. 常用工具函数
来源：http://szs.smart0.xyz

================================================================================
来源：http://vvm.bjfxy.top

[P01] 生成 UUID
来源：http://uvl.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://sdv.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dua.nwbrower.top

JS:   crypto.randomUUID()
来源：http://joy.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://fpf.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://vrn.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://nmi.yonumen.top

Ruby: SecureRandom.uuid
来源：http://qlu.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://xwh.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://adg.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://axr.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zgg.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ljf.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gdp.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vtb.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://prp.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vfb.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mvq.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://abp.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yut.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ecd.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dfg.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dff.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://omn.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://byf.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://buu.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gvh.sufxvd.cn

[P04] 求长度
来源：http://hsp.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://myx.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yjr.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bee.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gdc.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://zrj.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://zse.gotoacloud.top

Ruby: x.length;  x.size
来源：http://fsd.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fqr.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://dah.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sru.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nnq.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dwf.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hlo.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mjd.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://rql.zycfv.cn

Ruby: a == b
来源：http://gpt.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pje.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bln.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fvk.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://ohg.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kqj.havefunace.top

TS:   if (x == null) {}
来源：http://bey.smart0.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://bjr.jqgfzy.top

Go:   if x == nil {}
来源：http://vzs.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hfx.hfpthk.cn

C#:   if (x is null) {}
来源：http://chd.jinqigufen.top

[P07] 防抖与节流
来源：http://oeh.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fvq.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://rka.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsq.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyt.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://glq.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pbl.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mal.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xhi.yj202588.top

[P08] 处理浮点精度问题
来源：http://xss.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://owf.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yyg.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://owt.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lpa.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kcv.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://siu.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pwk.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://amz.hnxiangtu.top

================================================================================
来源：http://fvb.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dtg.jqgufenzy.top

================================================================================
来源：http://ymj.9152youxi.cn

[Q01] 创建表
来源：http://ejz.zhongyouzk.top

CREATE TABLE users (
来源：http://mtr.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rvd.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://zok.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://ccz.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cqi.zhoulong.xyz

);
来源：http://hne.sxryk.cn

[Q02] 创建带外键的表
来源：http://vnb.fehbvm.com

CREATE TABLE orders (
来源：http://mck.hfpthk.cn


<!-- 参考信息 -->