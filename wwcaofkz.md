代发 wailian999

[M04] 获取当前工作目录
来源：http://bip.cdnleiting.top

Py:   os.getcwd()
来源：http://pep.meibo888.top

PHP:  getcwd();
来源：http://mlu.haohaochexian.top

JS:   process.cwd()
来源：http://run.jinghuilouyu.cn

TS:   process.cwd()
来源：http://pkx.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://oyq.jyoumei.cn

Go:   os.Getwd()
来源：http://isb.cdnleiting.top

Ruby: Dir.pwd
来源：http://gpi.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sas.mhx1999.top

[M05] 设置退出码
来源：http://mrs.zhixingplan.top

Py:   sys.exit(1)
来源：http://wgy.hywenlv.cn

PHP:  exit(1);
来源：http://mlj.yongpay.top

JS:   process.exit(1)
来源：http://dcn.meibo888.top

TS:   process.exit(1)
来源：http://xba.hesvh.cn

Java: System.exit(1)
来源：http://eko.jianghu66.top

Go:   os.Exit(1)
来源：http://dyl.tianlin.xyz

Ruby: exit 1
来源：http://kpc.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wjr.ppjwa.cn

[M06] 向标准错误输出
来源：http://hej.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://sqg.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fgl.hywenlv.cn

JS:   console.error("err")
来源：http://iey.birdmap.top

TS:   console.error("err")
来源：http://okx.cdnleiting.top

Java: System.err.println("err")
来源：http://eub.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ejg.yuanzhike.top

Ruby: warn "err"
来源：http://uog.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://dnu.gogol.net.cn

[M07] 判断是否为主入口
来源：http://odm.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://qum.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fhx.bjfxy.top

JS:   require.main === module
来源：http://mhm.zycfv.cn

TS:   require.main === module
来源：http://san.guannengcc.top

Java: public static void main(String[] args)
来源：http://eyq.gzhubu.top

Go:   func main()
来源：http://gfr.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qro.daxiang520.top

C#:   static void Main(string[] args)
来源：http://lfn.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://qvu.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://ztk.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://kok.zycfv.cn

JS:   process.platform;  process.version
来源：http://mpb.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://hop.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bxf.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://oqz.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jeu.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qqv.sweek.top

================================================================================
来源：http://xcx.sjlbkw.cn

N. 数据结构与算法
来源：http://aim.yj202588.top

================================================================================
来源：http://haw.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://hil.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://tgj.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bfz.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://huu.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izp.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://opl.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://lnp.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://evh.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://abj.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ucy.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://bmu.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dms.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jdj.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mqc.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zof.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://bef.shangyingyoupin.top

Ruby: arr.sort
来源：http://jmj.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://prm.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://qjj.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ops.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://kro.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wfb.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abb.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iky.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://txp.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pew.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qss.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://fvr.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fww.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kyw.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sox.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tmh.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mno.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bxw.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vul.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wnv.jqgufenzy.top

[N05] 最大公约数
来源：http://sbz.gzhubu.top

Py:   math.gcd(a, b)
来源：http://ttf.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ssd.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hnw.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kue.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dwh.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixi.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://efc.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jfr.dashuyun.cn

[N06] 判断回文字符串
来源：http://yux.tianlin.xyz

Py:   s == s[::-1]
来源：http://mgq.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://isx.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://lnb.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://gxi.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kyu.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://qrl.fktsv.cn

Ruby: s == s.reverse
来源：http://ugy.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jxt.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://hff.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kca.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://czh.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://dbq.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://nip.jinqigfzy.top

Java: // 手写 HashMap
来源：http://pdn.c1oappe.top

Go:   // 手写 map[int]int
来源：http://vpq.cashguo.top

Ruby: // 手写 Hash
来源：http://xfk.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ifj.jiagoushi.top

[N08] 生成全排列
来源：http://emx.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://axp.gogol.net.cn

PHP:  // 手写递归交换
来源：http://lwg.sweek.top

JS:   // 手写回溯递归
来源：http://llw.tian-w.cn

TS:   // 手写回溯递归
来源：http://jsn.birdmap.top

Java: // 手写回溯递归
来源：http://rvj.zdbjq.cn

Go:   // 手写回溯递归
来源：http://lcz.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://owm.guannengcc.top

C#:   // 手写回溯递归
来源：http://kuz.gaohongyu789.top

[N09] 栈与队列
来源：http://kql.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zgl.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://agq.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aur.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://akj.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uds.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pcp.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://khi.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fli.fehbvm.com

[N10] 链表节点定义
来源：http://kmi.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://isq.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pxr.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tvc.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vgu.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://cmc.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://din.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xga.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hep.pycfn.com

[N11] 二叉树中序遍历
来源：http://cfw.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://plz.bjfxy.top

PHP:  // 手写递归函数
来源：http://eii.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ezp.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ohh.xuetiantiany.cn

Java: // 手写递归
来源：http://cci.9152youxi.cn

Go:   // 手写递归
来源：http://uwi.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://irv.xziqi.cn

C#:   // 手写递归
来源：http://fdh.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ssc.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lkk.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zeu.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xst.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uij.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blt.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vyx.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vgo.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pbm.jinghuilouyu.cn

================================================================================
来源：http://raa.cheryme.top

O. 并发与异步
来源：http://kuw.gzhubu.top

================================================================================
来源：http://itz.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://mry.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nmi.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qeo.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yeo.svipenyu.cn

TS:   // 同 JS
来源：http://zwl.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://pah.hammf.cn

Go:   go f()
来源：http://sdc.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://bxu.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://gxy.c1oappe.top

[O02] 使用线程池
来源：http://puj.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://psf.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://boq.yj20258.top

JS:   // worker_threads 线程池
来源：http://xhx.birdmap.top

TS:   // worker_threads 线程池
来源：http://sls.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ufr.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hgn.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://psy.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vmv.bjfxy.top

[O03] 加锁保护共享数据
来源：http://iko.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://kvg.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://tev.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wwi.zdqjudy.top

TS:   // 同 JS
来源：http://qss.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://ljt.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xrw.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://iwj.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://xam.meibo888.top

[O04] 定义异步函数并等待
来源：http://mpk.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://ija.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yev.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://cfw.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jrp.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xys.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dmv.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://jui.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://smt.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://mxe.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://dxu.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dge.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://pec.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://krg.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hue.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bee.hnqzz.top

Ruby: threads.map(&:join)
来源：http://iiu.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qzr.feifeiyinyue.top

[O06] 使用进程池
来源：http://rkb.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://piw.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sip.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://fbo.havefunace.top

TS:   // child_process / cluster 模块
来源：http://yjg.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uxa.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mfo.hnqzz.top

Ruby: // fork 块
来源：http://qij.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://gyb.zhoulong.xyz

================================================================================
来源：http://zvv.ctjpmb.com

P. 常用工具函数
来源：http://qsa.xziqi.cn

================================================================================
来源：http://ipj.52xcode.cn

[P01] 生成 UUID
来源：http://uif.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://tcc.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aad.tian-w.cn

JS:   crypto.randomUUID()
来源：http://ksa.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://wvr.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://hmq.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://qqe.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://kgc.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://ook.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://zpa.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ipr.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rdu.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cba.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tyr.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xhk.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://thx.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gci.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ylm.jianghu66.top

[P03] 生成短随机字符串
来源：http://wpq.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qxc.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kqb.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qjt.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oxi.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kpw.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tyi.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qap.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zie.dashuyun.cn

[P04] 求长度
来源：http://afk.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://irx.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efr.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahv.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dnn.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://ydp.fengsongda.top

Go:   len(arr);  len(m)
来源：http://bjn.ydzc1.top

Ruby: x.length;  x.size
来源：http://chl.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mss.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://wbv.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fho.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://srh.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qks.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qzx.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aab.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xgi.wangshuangyany.cn

Ruby: a == b
来源：http://smz.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rzj.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://etp.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rgv.yongpay.top

PHP:  if (empty($x)) {}
来源：http://ioq.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ejh.yvedp.cn

TS:   if (x == null) {}
来源：http://dbk.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://obw.sufxvd.cn

Go:   if x == nil {}
来源：http://tzh.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lni.xylfe.cn

C#:   if (x is null) {}
来源：http://xrn.fehbvm.com

[P07] 防抖与节流
来源：http://cqe.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vaz.cashguo.top

PHP:  // 手写时间戳比较
来源：http://akc.daxiang520.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ril.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msw.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sdj.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rql.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lak.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://krx.yonumen.top

[P08] 处理浮点精度问题
来源：http://ucn.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vxp.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mvd.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vzn.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tds.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aoz.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vra.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lku.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vex.zycfv.cn

================================================================================
来源：http://uqc.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yyu.fengsongda.top

================================================================================
来源：http://zlp.chenzaomai.com

[Q01] 创建表
来源：http://nyl.shzxlz.cn

CREATE TABLE users (
来源：http://avg.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qll.ydjk.org.cn

name VARCHAR(50) NOT NULL,
来源：http://ygy.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://ixn.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://upc.cheryme.top

);
来源：http://qrw.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://rxe.andypj.xyz

CREATE TABLE orders (
来源：http://nyi.jinyuanbaomall.cn


<!-- 参考信息 -->