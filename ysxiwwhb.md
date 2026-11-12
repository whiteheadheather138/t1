代发 wailian999

Ruby: exit 1
来源：http://sfq.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://amm.chenlongwang.top

[M06] 向标准错误输出
来源：http://pis.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://rxm.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mki.chenzaomai.com

JS:   console.error("err")
来源：http://aii.kuanghao11.cn

TS:   console.error("err")
来源：http://vhf.fktsv.cn

Java: System.err.println("err")
来源：http://ytp.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://evb.jianghu66.top

Ruby: warn "err"
来源：http://lus.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://wlb.jyoumei.cn

[M07] 判断是否为主入口
来源：http://odu.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://qtx.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xpi.zdbjq.cn

JS:   require.main === module
来源：http://xba.aibaodan.cn

TS:   require.main === module
来源：http://frr.iojbl.cn

Java: public static void main(String[] args)
来源：http://syp.gotoacloud.top

Go:   func main()
来源：http://zcp.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fno.jianghu66.top

C#:   static void Main(string[] args)
来源：http://bwn.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://fgj.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://bqr.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://zgw.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://muq.ybcxt.top

TS:   process.platform;  process.version
来源：http://shi.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tdg.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xzm.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://khm.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nqw.havefunace.top

================================================================================
来源：http://ias.pengpengdd.cyou

N. 数据结构与算法
来源：http://tmt.shuidangran.top

================================================================================
来源：http://kgq.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://stw.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://ise.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lwy.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jnb.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://czy.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://saz.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://fxx.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mhu.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hcb.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://ugh.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://efd.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dix.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ewj.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vfk.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lzu.fehbvm.com

Go:   slices.Sort(arr)
来源：http://eku.pengpengdd.cyou

Ruby: arr.sort
来源：http://wtv.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yeq.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://snb.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pda.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://rjk.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sqj.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qvp.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iad.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hxg.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fbp.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ptj.havefunace.top

[N04] 斐波那契数列
来源：http://obs.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ovd.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dbb.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pxz.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fcr.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zyv.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://grg.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://loe.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tmi.chenzaomai.com

[N05] 最大公约数
来源：http://qyr.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://lmm.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fgk.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kfo.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wtl.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tik.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://auo.aibaodan.cn

Ruby: a.gcd(b)
来源：http://uri.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wxd.aibaodan.cn

[N06] 判断回文字符串
来源：http://vxk.hesvh.cn

Py:   s == s[::-1]
来源：http://blu.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://dxx.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://lwg.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://iwb.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zqy.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://mxx.cheryme.top

Ruby: s == s.reverse
来源：http://uho.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://dap.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://jxl.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gax.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pkv.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://svc.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://xbc.svipenyu.cn

Java: // 手写 HashMap
来源：http://yjr.shuidangran.top

Go:   // 手写 map[int]int
来源：http://gva.smart0.xyz

Ruby: // 手写 Hash
来源：http://rzd.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://iug.birdmap.top

[N08] 生成全排列
来源：http://fus.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://ikp.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://gzj.sufxvd.cn

JS:   // 手写回溯递归
来源：http://hxe.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://rwc.9152youxi.cn

Java: // 手写回溯递归
来源：http://vmz.jinqigufen.top

Go:   // 手写回溯递归
来源：http://ekt.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://mwp.jyoumei.cn

C#:   // 手写回溯递归
来源：http://dox.xziqi.cn

[N09] 栈与队列
来源：http://rjs.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://omi.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dzm.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mke.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pxq.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wce.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jpp.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvb.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mmo.gaohongyu789.top

[N10] 链表节点定义
来源：http://zyu.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qja.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hrb.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gzk.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ktr.ivvv.top

Java: class Node { int v; Node next; }
来源：http://edg.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://eat.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bdf.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eyb.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://aix.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gbi.ctjpmb.com

PHP:  // 手写递归函数
来源：http://pck.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mmd.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qlr.nwbrower.top

Java: // 手写递归
来源：http://uem.havefunace.top

Go:   // 手写递归
来源：http://oaq.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xgr.zhoulong.xyz

C#:   // 手写递归
来源：http://zhu.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://waa.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rvd.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wvd.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ypu.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qes.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tqy.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qpt.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mes.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xgs.ybcxt.top

================================================================================
来源：http://otx.zhixingplan.top

O. 并发与异步
来源：http://cen.zycfv.cn

================================================================================
来源：http://uss.jinqigfzy.top

[O01] 启动一个线程
来源：http://kld.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rgg.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rmc.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tjn.hnqzz.top

TS:   // 同 JS
来源：http://jkf.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://elg.fengsongda.top

Go:   go f()
来源：http://ffb.sxryk.cn

Ruby: Thread.new { f }
来源：http://vir.0kj1m.cn

C#:   Task.Run(() => F());
来源：http://ojy.sjlbkw.cn

[O02] 使用线程池
来源：http://tux.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fdj.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tty.fehbvm.com

JS:   // worker_threads 线程池
来源：http://bny.fengsongda.top

TS:   // worker_threads 线程池
来源：http://ecp.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://qyd.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mpq.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gra.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cdc.mhx1999.top

[O03] 加锁保护共享数据
来源：http://xux.vehdjk.com

Py:   with lock: shared += 1
来源：http://xza.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://ino.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qlc.jqgfzy.top

TS:   // 同 JS
来源：http://btx.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://grt.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ynp.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://akc.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://lkg.cashguo.top

[O04] 定义异步函数并等待
来源：http://xel.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://lcw.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gme.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://jlk.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://iun.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xuh.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aon.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://npu.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://pyf.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://nxl.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://zgd.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hfp.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://ltn.yonumen.top

TS:   await Promise.all(tasks)
来源：http://xoj.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nni.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iob.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://vzw.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dsy.haohaochexian.top

[O06] 使用进程池
来源：http://paw.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://smd.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ico.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://dmj.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://ose.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ecx.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mrx.yuanzhike.top

Ruby: // fork 块
来源：http://rck.kuanghao11.cn

C#:   Parallel.For
来源：http://fiw.sxryk.cn

================================================================================
来源：http://xqo.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://mww.ydjk.org.cn

================================================================================
来源：http://shp.mhx1999.top

[P01] 生成 UUID
来源：http://qhl.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://upg.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fzj.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://kbb.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://ogx.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://zhy.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://olg.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://ufh.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://arg.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://pxc.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dhj.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://glu.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wek.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eip.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tba.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://shh.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vfz.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oxm.aibaodan.cn

[P03] 生成短随机字符串
来源：http://sqe.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jas.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lsk.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mbl.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbb.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ngr.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ymm.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://trf.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://via.pengpengdd.cyou

[P04] 求长度
来源：http://kjf.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vdz.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wmk.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://trs.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://usz.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://ywi.yj20258.top

Go:   len(arr);  len(m)
来源：http://bnc.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://qnm.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://dos.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://nrh.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://eft.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ucq.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xgj.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mzr.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vfb.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yid.zhiwuduotai.top

Ruby: a == b
来源：http://hvw.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nfq.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nxl.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qib.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://dwa.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zhu.redwolf501.top

TS:   if (x == null) {}
来源：http://tua.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tgj.sjlbkw.cn

Go:   if x == nil {}
来源：http://uwm.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ajy.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://bbm.meibo888.top

[P07] 防抖与节流
来源：http://yed.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kfx.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://adq.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njd.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cgl.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qdq.jqgufenzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nxk.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zgt.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fvs.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://keg.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tdg.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mup.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sjg.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qry.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dqv.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zww.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lik.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xrz.cqqwz.cn

================================================================================
来源：http://orf.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xmy.yvedp.cn

================================================================================
来源：http://fsb.zycfv.cn

[Q01] 创建表
来源：http://wlx.guowangkeji.top

CREATE TABLE users (
来源：http://wio.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jnj.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://bhu.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://mxb.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yhu.tian-w.cn

);
来源：http://egs.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://uzr.hongshengwenyu.top

CREATE TABLE orders (
来源：http://qsu.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvt.fengsongda.top

user_id INT NOT NULL,
来源：http://gfq.aizwys.cn

amount DECIMAL(10, 2),
来源：http://enx.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cie.chenjidiqi.icu

);
来源：http://zuj.jlsjyb.cn

[Q03] 增加列
来源：http://cno.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cmd.aibaodan.cn

[Q04] 修改列类型
来源：http://esw.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rbv.sufxvd.cn

[Q05] 重命名列
来源：http://rfu.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rug.haohaochexian.top

[Q06] 删除列
来源：http://sjt.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://plk.fengsongda.top

[Q07] 删除表
来源：http://smf.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://tlj.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://xdc.yj202588.top


<!-- 参考信息 -->