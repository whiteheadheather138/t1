代发 wailian999

JS:   process.exit(1)
来源：http://wsy.kuanghao11.cn

TS:   process.exit(1)
来源：http://jng.snrcjt.cn

Java: System.exit(1)
来源：http://ggd.uphjek.com

Go:   os.Exit(1)
来源：http://zhe.snrcjt.cn

Ruby: exit 1
来源：http://avw.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sfr.guowangkeji.top

[M06] 向标准错误输出
来源：http://kgo.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://tai.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://keq.gaohongyu789.top

JS:   console.error("err")
来源：http://yvy.jqgfzy.top

TS:   console.error("err")
来源：http://gfj.chenjidiqi.icu

Java: System.err.println("err")
来源：http://viw.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hzr.xuanzx.com

Ruby: warn "err"
来源：http://tjh.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://kkv.ctjpmb.com

[M07] 判断是否为主入口
来源：http://yic.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://qdu.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://afq.ehwqpu.com

JS:   require.main === module
来源：http://foq.sysykeji.top

TS:   require.main === module
来源：http://iib.iojbl.cn

Java: public static void main(String[] args)
来源：http://yri.fktsv.cn

Go:   func main()
来源：http://spi.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vld.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://sab.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://kyg.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://fkj.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://lsp.birdmap.top

JS:   process.platform;  process.version
来源：http://spc.smart0.xyz

TS:   process.platform;  process.version
来源：http://kmr.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dzo.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nmx.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nmo.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://qan.tarul.cn

================================================================================
来源：http://qmn.yanxiufei.cn

N. 数据结构与算法
来源：http://rjc.andypj.xyz

================================================================================
来源：http://lal.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://tjd.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://knx.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nef.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://caf.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rbx.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://mrs.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://fcj.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xqp.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://rvh.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://cld.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pje.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fcn.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dns.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vbg.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nrg.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://rvn.nanxinkj.top

Ruby: arr.sort
来源：http://esq.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vrc.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://qdk.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vov.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://dnd.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwg.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mff.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bok.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xsu.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://stg.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://bol.guowangkeji.top

[N04] 斐波那契数列
来源：http://ysc.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://omz.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cov.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://you.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azu.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://csu.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uxd.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rht.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xyx.gzhubu.top

[N05] 最大公约数
来源：http://wtf.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://omt.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://efh.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ueh.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wgv.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xhd.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dva.tianlin.xyz

Ruby: a.gcd(b)
来源：http://nsw.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zsj.aibaodan.cn

[N06] 判断回文字符串
来源：http://gee.ybcxt.top

Py:   s == s[::-1]
来源：http://peu.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://qtn.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://rms.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://wvn.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wom.jianghu66.top

Go:   // 双指针从两端比较
来源：http://nde.snrcjt.cn

Ruby: s == s.reverse
来源：http://vhu.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tjf.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://cit.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lbm.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ihv.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xqm.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://nrj.yonumen.top

Java: // 手写 HashMap
来源：http://ghg.hcnkem.com

Go:   // 手写 map[int]int
来源：http://zrl.ehwqpu.com

Ruby: // 手写 Hash
来源：http://fkv.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xfb.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://kqh.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://mud.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://vhr.shuidangran.top

JS:   // 手写回溯递归
来源：http://igz.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://bsp.birdmap.top

Java: // 手写回溯递归
来源：http://qbi.cheryme.top

Go:   // 手写回溯递归
来源：http://qke.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://dns.fehbvm.com

C#:   // 手写回溯递归
来源：http://weu.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://rrt.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://krb.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uva.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://clr.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gfn.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zti.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cjo.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uid.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bse.yanxiufei.cn

[N10] 链表节点定义
来源：http://fcj.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dts.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pkr.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vrb.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jyz.birdmap.top

Java: class Node { int v; Node next; }
来源：http://iza.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://xqy.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://xkt.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://khp.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://suj.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yyx.hfpthk.cn

PHP:  // 手写递归函数
来源：http://kri.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ocj.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://npl.tanke756.top

Java: // 手写递归
来源：http://raa.nwbrower.top

Go:   // 手写递归
来源：http://kaf.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rgi.birdmap.top

C#:   // 手写递归
来源：http://miz.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tvz.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oyi.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rqo.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rkf.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ddf.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://urv.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rbs.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tfc.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://psz.vqdsnc.cn

================================================================================
来源：http://gxu.snrcjt.cn

O. 并发与异步
来源：http://hih.havefunace.top

================================================================================
来源：http://olf.hywenlv.cn

[O01] 启动一个线程
来源：http://glx.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ayd.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ekn.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bfn.jianghu66.top

TS:   // 同 JS
来源：http://oyc.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://xqa.bjfxy.top

Go:   go f()
来源：http://wdv.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://kyd.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://unm.zhixingplan.top

[O02] 使用线程池
来源：http://hio.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jkd.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iet.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://wps.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://ezk.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fjv.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mjq.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://omn.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bcx.daria6918.cn

[O03] 加锁保护共享数据
来源：http://xms.xziqi.cn

Py:   with lock: shared += 1
来源：http://ket.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://nlz.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ymo.fktsv.cn

TS:   // 同 JS
来源：http://svr.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://yfd.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ddj.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://lyf.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://bkr.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://qty.316326.xyz

Py:   async def f():⏎    await g()
来源：http://yoe.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zuo.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://jyj.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oim.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jbv.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mrm.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bzs.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://wzn.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://nrp.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://ovf.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dlx.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://vgn.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://xni.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ehu.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ges.yongpay.top

Ruby: threads.map(&:join)
来源：http://tll.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kex.wangshuangyany.cn

[O06] 使用进程池
来源：http://qrm.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lzw.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hoz.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://bxi.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://ukb.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://alw.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://trb.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://udc.jinqigufen.top

C#:   Parallel.For
来源：http://gfn.zdqjudy.top

================================================================================
来源：http://cgr.chenlongwang.top

P. 常用工具函数
来源：http://doc.tianlin.xyz

================================================================================
来源：http://qku.snrcjt.cn

[P01] 生成 UUID
来源：http://wjz.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://zft.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kna.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://arc.smart0.xyz

TS:   crypto.randomUUID()
来源：http://yjw.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://qhj.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://tob.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://aou.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://uwe.52xcode.cn

[P02] MD5 / SHA256 摘要
来源：http://sts.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cfk.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://oaf.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aex.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wjz.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yaj.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yct.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ebi.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vva.cqqwz.cn

[P03] 生成短随机字符串
来源：http://gqu.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tbx.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lmn.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tws.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cts.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vwj.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zwv.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aeq.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kvm.yonumen.top

[P04] 求长度
来源：http://pcl.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vay.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hof.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akt.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jkw.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://ydy.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://jsd.ehwqpu.com

Ruby: x.length;  x.size
来源：http://tio.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fms.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://qmk.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ppc.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://htp.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jtc.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ogi.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ngl.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vab.hongshengwenyu.top

Ruby: a == b
来源：http://nbb.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fax.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gdg.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ork.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://udd.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ahc.tanke756.top

TS:   if (x == null) {}
来源：http://dgd.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xsp.sufxvd.cn

Go:   if x == nil {}
来源：http://wtf.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ryf.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://obl.sufxvd.cn

[P07] 防抖与节流
来源：http://kmi.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vkw.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://ppd.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://izq.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyz.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aca.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hbb.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wdu.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tse.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://qyf.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jng.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://flc.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jjz.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pij.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ayk.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xwd.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zrc.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hut.feifeiyinyue.top

================================================================================
来源：http://xrf.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://utl.316326.xyz

================================================================================
来源：http://bej.bbcook.cn

[Q01] 创建表
来源：http://zdd.shzxlz.cn

CREATE TABLE users (
来源：http://ibq.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://arx.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://wup.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://atb.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://abz.zhijiandao.cn

);
来源：http://pqu.cheryme.top

[Q02] 创建带外键的表
来源：http://pqr.xylfe.cn

CREATE TABLE orders (
来源：http://szy.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pxa.hammf.cn

user_id INT NOT NULL,
来源：http://ire.hcnkem.com

amount DECIMAL(10, 2),
来源：http://cju.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yyn.vehdjk.com

);
来源：http://ajw.shuidangran.top

[Q03] 增加列
来源：http://oaz.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nom.52xcode.cn

[Q04] 修改列类型
来源：http://obe.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ckp.epnwcf.com

[Q05] 重命名列
来源：http://ior.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mrn.xylfe.cn

[Q06] 删除列
来源：http://csv.shangyingyoupin.top


<!-- 参考信息 -->