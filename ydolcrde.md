代发 wailian999

JS:   process.exit(1)
来源：http://fkt.dashuyun.cn

TS:   process.exit(1)
来源：http://ugt.cdnleiting.top

Java: System.exit(1)
来源：http://zfi.ctjpmb.com

Go:   os.Exit(1)
来源：http://mqd.jqgufenzy.top

Ruby: exit 1
来源：http://ihw.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pix.yvedp.cn

[M06] 向标准错误输出
来源：http://vke.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://umr.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bvu.sweek.top

JS:   console.error("err")
来源：http://wqa.hfpthk.cn

TS:   console.error("err")
来源：http://tpv.zdqjudy.top

Java: System.err.println("err")
来源：http://hgg.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://okk.cheryme.top

Ruby: warn "err"
来源：http://erq.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://rlq.vehdjk.com

[M07] 判断是否为主入口
来源：http://tpj.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://coq.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dvp.fanxiaobao.xyz

JS:   require.main === module
来源：http://mrn.gaohongyu789.top

TS:   require.main === module
来源：http://nem.aibaodan.cn

Java: public static void main(String[] args)
来源：http://kdm.tianlin.xyz

Go:   func main()
来源：http://bjy.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kgv.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://fbi.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://lgj.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://uum.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://lhn.ybcxt.top

JS:   process.platform;  process.version
来源：http://lei.tanke756.top

TS:   process.platform;  process.version
来源：http://npu.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nav.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wdy.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://drz.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lxb.wangshuangyany.cn

================================================================================
来源：http://njq.hammf.cn

N. 数据结构与算法
来源：http://mks.ehwqpu.com

================================================================================
来源：http://brr.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://rmo.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zpy.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ual.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbx.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mvn.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://wyw.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://tyj.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://qlk.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://ymh.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://bcz.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xwc.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zxa.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rfl.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ebu.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wpv.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://dhb.gzhubu.top

Ruby: arr.sort
来源：http://qgc.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bje.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://eeo.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xwd.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://xzh.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fwy.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqm.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fxg.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hbd.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lay.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://yby.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://cfa.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ioc.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://boo.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqd.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vbl.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ebh.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ecf.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ujk.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lvc.jinqigfzy.top

[N05] 最大公约数
来源：http://wwq.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://bum.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cfq.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jkm.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hti.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://btl.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hku.fzhhl.top

Ruby: a.gcd(b)
来源：http://vfe.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zap.zhengqikj.top

[N06] 判断回文字符串
来源：http://vgu.hammf.cn

Py:   s == s[::-1]
来源：http://tji.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://vwr.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://yil.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://pek.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zen.smart0.xyz

Go:   // 双指针从两端比较
来源：http://wcz.quarkkingdee.top

Ruby: s == s.reverse
来源：http://tnn.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://paw.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://poc.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ele.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pqt.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pgy.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://upz.zhongyouzk.top

Java: // 手写 HashMap
来源：http://qbx.mhx1999.top

Go:   // 手写 map[int]int
来源：http://abt.yonumen.top

Ruby: // 手写 Hash
来源：http://lfd.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pfo.cdnleiting.top

[N08] 生成全排列
来源：http://ikp.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://irq.hcnkem.com

PHP:  // 手写递归交换
来源：http://vws.gogol.net.cn

JS:   // 手写回溯递归
来源：http://jpv.guowangkeji.top

TS:   // 手写回溯递归
来源：http://qwq.jqgfzy.top

Java: // 手写回溯递归
来源：http://blq.52xcode.cn

Go:   // 手写回溯递归
来源：http://pam.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://aqk.epnwcf.com

C#:   // 手写回溯递归
来源：http://pbp.52xcode.cn

[N09] 栈与队列
来源：http://ynk.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://end.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kwh.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gmu.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ehf.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oux.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aiv.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rlm.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvk.yonumen.top

[N10] 链表节点定义
来源：http://qmo.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mab.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gvb.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jyr.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qqq.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://ehh.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://xwr.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ssd.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uvi.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://hef.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yhc.vehdjk.com

PHP:  // 手写递归函数
来源：http://wrr.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tcg.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zeh.epnwcf.com

Java: // 手写递归
来源：http://qib.yfazqb.com

Go:   // 手写递归
来源：http://bru.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uys.jinqigfzy.top

C#:   // 手写递归
来源：http://vsl.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gui.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nrf.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ngf.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mme.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://plw.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lzu.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ecu.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xhe.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uhw.cashguo.top

================================================================================
来源：http://ksh.hfpthk.cn

O. 并发与异步
来源：http://xqs.chenzaomai.com

================================================================================
来源：http://qzz.guowangkeji.top

[O01] 启动一个线程
来源：http://tyh.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tkf.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mxy.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://csq.hnxiangtu.top

TS:   // 同 JS
来源：http://gsr.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://mwr.jyoumei.cn

Go:   go f()
来源：http://zye.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://mtj.hnqzz.top

C#:   Task.Run(() => F());
来源：http://xoi.ybcxt.top

[O02] 使用线程池
来源：http://tfl.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bzs.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oct.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://dlz.yongpay.top

TS:   // worker_threads 线程池
来源：http://dha.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://rzk.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nhe.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://afk.yuxming.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ast.mhx1999.top

[O03] 加锁保护共享数据
来源：http://rdi.meibo888.top

Py:   with lock: shared += 1
来源：http://cdd.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://tgp.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ueh.vehdjk.com

TS:   // 同 JS
来源：http://vvn.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://jyu.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pcg.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://uvk.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://jff.gzhubu.top

[O04] 定义异步函数并等待
来源：http://yxh.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://uww.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fzw.fengsongda.top

JS:   async function f() { await g(); }
来源：http://vpf.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tgr.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://knp.redwolf501.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jqh.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rkf.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://kvw.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://blh.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://ivj.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kjd.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://skg.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://nfs.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dod.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://smh.redwolf501.top

Ruby: threads.map(&:join)
来源：http://jxt.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://llz.hfpthk.cn

[O06] 使用进程池
来源：http://fjj.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://srp.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://rtj.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://trd.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://ftj.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dni.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pko.vqdsnc.cn

Ruby: // fork 块
来源：http://aue.tianlin.xyz

C#:   Parallel.For
来源：http://yqp.yfazqb.com

================================================================================
来源：http://cgu.shanyushiyangtech.top

P. 常用工具函数
来源：http://pir.shangyingyoupin.top

================================================================================
来源：http://pcp.gzhubu.top

[P01] 生成 UUID
来源：http://wky.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://enw.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bpt.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://pma.sysykeji.top

TS:   crypto.randomUUID()
来源：http://fvj.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://gtg.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://vxn.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://gkr.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://vmo.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://jif.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ylm.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ahi.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jgd.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kmc.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ndd.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://slh.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://efp.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vcy.jianghu66.top

[P03] 生成短随机字符串
来源：http://uxg.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ntb.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mrw.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rzd.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hoy.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mlc.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jqw.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://agj.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cbq.xinyue.icu

[P04] 求长度
来源：http://ghi.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cpv.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aoo.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://czo.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izz.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://qcd.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://zvy.fktsv.cn

Ruby: x.length;  x.size
来源：http://kcc.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://abm.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://vze.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ozd.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gqh.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vip.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tew.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mxn.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fqt.ppjwa.cn

Ruby: a == b
来源：http://ioh.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fex.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hzb.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zlu.yongpay.top

PHP:  if (empty($x)) {}
来源：http://aia.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qbh.sxryk.cn

TS:   if (x == null) {}
来源：http://dyz.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rhy.feifeiyinyue.top

Go:   if x == nil {}
来源：http://hzq.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iok.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://eld.52xcode.cn

[P07] 防抖与节流
来源：http://rdk.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zec.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://sow.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuv.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkq.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ivd.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zdr.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://isu.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://weh.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://ceh.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yoy.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cpf.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ohh.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eep.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jxs.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bty.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fjm.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qlb.xuanzx.com

================================================================================
来源：http://lsw.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cly.tanke756.top

================================================================================
来源：http://jld.bjfxy.top

[Q01] 创建表
来源：http://uvn.gogol.net.cn

CREATE TABLE users (
来源：http://zhq.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkn.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://rwx.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://ama.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rnw.hongshengwenyu.top

);
来源：http://cmh.gotoacloud.top

[Q02] 创建带外键的表
来源：http://cbt.mhx1999.top

CREATE TABLE orders (
来源：http://fau.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gal.zhixingplan.top

user_id INT NOT NULL,
来源：http://pyf.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://zbm.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vbp.zhijiandao.cn

);
来源：http://ynk.yuanzhike.top

[Q03] 增加列
来源：http://vhb.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://upp.gotoacloud.top

[Q04] 修改列类型
来源：http://yux.bbcook.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qdv.fzhhl.top

[Q05] 重命名列
来源：http://iak.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://urh.yj20258888.top

[Q06] 删除列
来源：http://mdx.52xcode.cn


<!-- 参考信息 -->