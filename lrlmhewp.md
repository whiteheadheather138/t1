代发 wailian999

TS:   process.cwd()
来源：http://nad.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://yst.snrcjt.cn

Go:   os.Getwd()
来源：http://art.fktsv.cn

Ruby: Dir.pwd
来源：http://fxh.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://ppw.jqgfzy.top

[M05] 设置退出码
来源：http://lpr.zhongyouzk.top

Py:   sys.exit(1)
来源：http://nuk.ydzc1.top

PHP:  exit(1);
来源：http://aeq.uphjek.com

JS:   process.exit(1)
来源：http://wkh.jinqigufen.top

TS:   process.exit(1)
来源：http://iad.dashuyun.cn

Java: System.exit(1)
来源：http://uut.ctjpmb.com

Go:   os.Exit(1)
来源：http://jxu.kuanghao11.cn

Ruby: exit 1
来源：http://gxu.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://snx.tianlin.xyz

[M06] 向标准错误输出
来源：http://tai.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://qbz.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mie.yuxming.cn

JS:   console.error("err")
来源：http://rdl.bjfxy.top

TS:   console.error("err")
来源：http://vvs.ctjpmb.com

Java: System.err.println("err")
来源：http://xca.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fkt.ivvv.top

Ruby: warn "err"
来源：http://vsq.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://avw.birdmap.top

[M07] 判断是否为主入口
来源：http://fto.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://sqm.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://naq.tanke756.top

JS:   require.main === module
来源：http://jhl.jinyuanbaomall.cn

TS:   require.main === module
来源：http://sar.gogol.net.cn

Java: public static void main(String[] args)
来源：http://mtf.hammf.cn

Go:   func main()
来源：http://euy.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oja.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://oxz.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://nyc.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://sly.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://gif.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://lug.yuxming.cn

TS:   process.platform;  process.version
来源：http://srt.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cym.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tug.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://puk.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vqr.cucudq.cn

================================================================================
来源：http://gup.tianlin.xyz

N. 数据结构与算法
来源：http://qaw.xuanzx.com

================================================================================
来源：http://rzy.316326.xyz

[N01] 二分查找（有序数组）
来源：http://lyw.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://syf.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kzf.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lag.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gut.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://vcn.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://aef.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ugk.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://ela.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://rzn.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://wfz.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cpv.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ehc.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eow.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lqh.yfazqb.com

Go:   slices.Sort(arr)
来源：http://oyn.cdnleiting.top

Ruby: arr.sort
来源：http://xaf.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://qcf.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://lbh.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jnf.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://djy.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://paj.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://til.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dae.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lpo.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mzr.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://xdp.zhijiandao.cn

[N04] 斐波那契数列
来源：http://wrf.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gbb.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thi.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://drd.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dhc.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cov.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ors.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owv.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zsn.zhoulong.xyz

[N05] 最大公约数
来源：http://aja.cdnleiting.top

Py:   math.gcd(a, b)
来源：http://zhk.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lkz.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qtt.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xtt.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tlj.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yxs.redwolf501.top

Ruby: a.gcd(b)
来源：http://ssu.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ktb.aibaodan.cn

[N06] 判断回文字符串
来源：http://acg.chenzaomai.com

Py:   s == s[::-1]
来源：http://qze.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://ycf.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://nyr.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://qrx.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lkw.aibaodan.cn

Go:   // 双指针从两端比较
来源：http://lqc.zycfv.cn

Ruby: s == s.reverse
来源：http://bvq.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dwa.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://olq.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cqp.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://roz.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qva.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://ndq.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://cve.fengsongda.top

Go:   // 手写 map[int]int
来源：http://hzv.ivvv.top

Ruby: // 手写 Hash
来源：http://wgv.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ast.yonumen.top

[N08] 生成全排列
来源：http://gyo.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://pyr.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://omh.ehwqpu.com

JS:   // 手写回溯递归
来源：http://dzf.gzhubu.top

TS:   // 手写回溯递归
来源：http://joh.hammf.cn

Java: // 手写回溯递归
来源：http://qew.yangfankeji.com

Go:   // 手写回溯递归
来源：http://lfj.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://shy.zhengqikj.top

C#:   // 手写回溯递归
来源：http://cwe.dashuyun.cn

[N09] 栈与队列
来源：http://qxc.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wlv.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jpt.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vee.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zbj.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://omg.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yfr.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hli.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fac.tianlin.xyz

[N10] 链表节点定义
来源：http://mcu.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ebv.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uuv.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kdc.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pwu.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://txh.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://fnu.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ayc.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jeb.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://fvy.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yit.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://blt.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mje.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tmz.cqqwz.cn

Java: // 手写递归
来源：http://yrl.shzxlz.cn

Go:   // 手写递归
来源：http://myz.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iiq.haohaochexian.top

C#:   // 手写递归
来源：http://xrj.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qwd.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyg.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qni.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qsv.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://egb.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uek.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wxo.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yio.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pdj.mhx1999.top

================================================================================
来源：http://gue.52xcode.cn

O. 并发与异步
来源：http://vlw.vehdjk.com

================================================================================
来源：http://trm.jiagoushi.top

[O01] 启动一个线程
来源：http://zcs.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://duu.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ekq.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mso.andypj.xyz

TS:   // 同 JS
来源：http://tru.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://poi.fengsongda.top

Go:   go f()
来源：http://duq.zdbjq.cn

Ruby: Thread.new { f }
来源：http://qov.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://gdm.fehbvm.com

[O02] 使用线程池
来源：http://rxt.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jpq.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oyq.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://qdr.hesvh.cn

TS:   // worker_threads 线程池
来源：http://rqc.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ybs.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pgc.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://znm.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oaf.guannengcc.top

[O03] 加锁保护共享数据
来源：http://qel.cucudq.cn

Py:   with lock: shared += 1
来源：http://zzq.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ivz.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yus.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://aoq.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://njt.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gjg.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dwo.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://uky.c1oappe.top

[O04] 定义异步函数并等待
来源：http://qbp.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://fiq.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zyq.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://hiq.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lxf.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://adw.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sqm.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zvp.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://ggd.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://bex.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://dbl.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ytv.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://djl.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://spa.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://urs.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dfl.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://dna.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qzm.hnqzz.top

[O06] 使用进程池
来源：http://lou.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lgw.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bdt.tarul.cn

JS:   // child_process / cluster 模块
来源：http://ein.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://ehv.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kqp.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mzx.yanxiufei.cn

Ruby: // fork 块
来源：http://aoo.sweek.top

C#:   Parallel.For
来源：http://hrw.hongshengwenyu.top

================================================================================
来源：http://tqp.zhiwuduotai.top

P. 常用工具函数
来源：http://ldf.snrcjt.cn

================================================================================
来源：http://byl.ydjk.org.cn

[P01] 生成 UUID
来源：http://cei.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://ugu.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qil.ybcxt.top

JS:   crypto.randomUUID()
来源：http://gwu.cashguo.top

TS:   crypto.randomUUID()
来源：http://ghp.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://wzi.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://hol.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://fcv.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://nta.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://tdt.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bux.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://omu.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qyb.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pqd.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://huo.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bwp.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://axj.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://isn.9152youxi.cn

[P03] 生成短随机字符串
来源：http://xgj.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kpc.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cgq.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wdk.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cls.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vdv.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zcn.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ihk.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://etx.smart0.xyz

[P04] 求长度
来源：http://uuz.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ovu.havefunace.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmy.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zpf.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qvx.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://yki.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://ffv.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://gul.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kks.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://fjd.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mrk.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ljt.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eit.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rsf.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fkd.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://edv.zdbjq.cn

Ruby: a == b
来源：http://ggf.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ovd.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ave.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ips.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://vmq.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rtn.c1oappe.top

TS:   if (x == null) {}
来源：http://xsk.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://uio.dashuyun.cn

Go:   if x == nil {}
来源：http://vop.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sfm.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://swt.jinqigfzy.top

[P07] 防抖与节流
来源：http://xvd.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uzu.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://mnn.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mre.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eof.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tjy.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ppq.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://stu.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ghv.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://czd.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qkz.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vwd.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dma.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tac.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cld.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xpr.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yuv.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eru.jianghu66.top

================================================================================
来源：http://pqq.shanyushiyangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kbn.sxryk.cn

================================================================================
来源：http://krt.cashguo.top

[Q01] 创建表
来源：http://wwz.pycfn.com

CREATE TABLE users (
来源：http://wje.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ryr.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://bgi.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://ake.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://snq.cqqwz.cn

);
来源：http://crb.chenlongwang.top

[Q02] 创建带外键的表
来源：http://agd.jyoumei.cn

CREATE TABLE orders (
来源：http://wub.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fer.sjlbkw.cn

user_id INT NOT NULL,
来源：http://set.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://zro.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qar.zhixingplan.top


<!-- 参考信息 -->