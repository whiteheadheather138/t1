代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qtv.jqgfzy.top

Ruby: warn "err"
来源：http://zbn.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://qan.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://xfy.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://gkc.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xgh.iojbl.cn

JS:   require.main === module
来源：http://bol.pycfn.com

TS:   require.main === module
来源：http://ysm.hysaishi.cn

Java: public static void main(String[] args)
来源：http://edo.tanke756.top

Go:   func main()
来源：http://iuw.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sdh.cashguo.top

C#:   static void Main(string[] args)
来源：http://bjd.cashguo.top

[M08] 获取系统与运行时信息
来源：http://lrj.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://shr.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://yes.cqqwz.cn

JS:   process.platform;  process.version
来源：http://bwr.jiagoushi.top

TS:   process.platform;  process.version
来源：http://qht.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://odn.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://udi.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lyj.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jjp.hywenlv.cn

================================================================================
来源：http://smo.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://pns.ydjk.org.cn

================================================================================
来源：http://vls.tanke756.top

[N01] 二分查找（有序数组）
来源：http://bue.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qsv.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mps.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zow.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wgu.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://dfc.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://sfl.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hrb.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xgw.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://knd.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://eiq.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oto.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hbd.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iqe.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://apl.yfazqb.com

Go:   slices.Sort(arr)
来源：http://ilk.daria6918.cn

Ruby: arr.sort
来源：http://nhm.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://knr.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://wvr.zhixingplan.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wcp.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://sgk.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qcv.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxn.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eiy.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pop.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ihm.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gtj.mhx1999.top

[N04] 斐波那契数列
来源：http://wdo.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pvs.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zxg.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rum.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzh.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbs.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rii.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hhd.tanke756.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xdr.pycfn.com

[N05] 最大公约数
来源：http://zex.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://nuy.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cyr.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfz.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghq.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xot.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pfm.hfpthk.cn

Ruby: a.gcd(b)
来源：http://fht.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ccz.dianchejie.cn

[N06] 判断回文字符串
来源：http://lee.zhengqikj.top

Py:   s == s[::-1]
来源：http://icw.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://nyg.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://aiy.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://uaz.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://acg.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://ojt.iojbl.cn

Ruby: s == s.reverse
来源：http://eeb.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lmw.birdmap.top

[N07] 两数之和（返回下标）
来源：http://hom.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lhh.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://afj.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://dcw.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://zep.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://goq.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://qvz.pycfn.com

Ruby: // 手写 Hash
来源：http://nny.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wui.ydzc1.top

[N08] 生成全排列
来源：http://jay.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://erj.yuanzhike.top

PHP:  // 手写递归交换
来源：http://xyx.fengsongda.top

JS:   // 手写回溯递归
来源：http://gyo.tianlin.xyz

TS:   // 手写回溯递归
来源：http://unx.gotoacloud.top

Java: // 手写回溯递归
来源：http://uze.bbcook.cn

Go:   // 手写回溯递归
来源：http://sdz.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://wzi.yfazqb.com

C#:   // 手写回溯递归
来源：http://tut.kuanghao11.cn

[N09] 栈与队列
来源：http://rxx.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jyi.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nxg.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mhf.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jjz.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ast.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uyc.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lqi.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zwr.jinqigufen.top

[N10] 链表节点定义
来源：http://fgy.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jox.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://afr.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kdz.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ofg.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://kta.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bkh.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kqs.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rfh.tian-w.cn

[N11] 二叉树中序遍历
来源：http://ukl.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yog.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://pcv.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oek.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kme.shanyushiyangtech.top

Java: // 手写递归
来源：http://uhw.jinqigfzy.top

Go:   // 手写递归
来源：http://eyd.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dyy.xylfe.cn

C#:   // 手写递归
来源：http://ndu.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://goq.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://crj.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://plp.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://buy.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eae.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://drd.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kyj.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xno.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kqi.c1oappe.top

================================================================================
来源：http://vmq.daria6918.cn

O. 并发与异步
来源：http://vuq.jianghu66.top

================================================================================
来源：http://rkp.havefunace.top

[O01] 启动一个线程
来源：http://dcg.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://epb.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lle.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gzp.ydzc1.top

TS:   // 同 JS
来源：http://hfb.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://tth.yueranfly.top

Go:   go f()
来源：http://bmn.guowangkeji.top

Ruby: Thread.new { f }
来源：http://uta.yj20258888.top

C#:   Task.Run(() => F());
来源：http://kal.yonumen.top

[O02] 使用线程池
来源：http://fcr.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qpu.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wgr.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://xdr.jinqigufen.top

TS:   // worker_threads 线程池
来源：http://nog.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://akk.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rax.shanyushiyangtech.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ewi.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ubx.yuxming.cn

[O03] 加锁保护共享数据
来源：http://ftg.0kj1m.cn

Py:   with lock: shared += 1
来源：http://vdk.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://xms.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pbp.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://eys.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://inj.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xnh.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jgy.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://fnv.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://msw.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://rdz.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yij.ydzc1.top

JS:   async function f() { await g(); }
来源：http://vxy.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bil.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://swx.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://onk.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://hbn.yonumen.top

C#:   async Task F() { await G(); }
来源：http://kcu.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://hof.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://ypb.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gnx.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://iie.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://usr.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bhn.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wji.sxryk.cn

Ruby: threads.map(&:join)
来源：http://put.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tox.birdmap.top

[O06] 使用进程池
来源：http://lzk.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgs.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uwy.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://psk.cheryme.top

TS:   // child_process / cluster 模块
来源：http://uhj.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pbn.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uiy.ivvv.top

Ruby: // fork 块
来源：http://nae.smart0.xyz

C#:   Parallel.For
来源：http://ljv.tianlin.xyz

================================================================================
来源：http://dth.ivvv.top

P. 常用工具函数
来源：http://alu.chenlongwang.top

================================================================================
来源：http://bya.shzxlz.cn

[P01] 生成 UUID
来源：http://uuk.cashguo.top

Py:   str(uuid.uuid4())
来源：http://ahy.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://udx.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://wyz.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://yqj.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://uja.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://wnw.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://hdt.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://lsk.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://vco.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qtg.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xxm.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://evl.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iza.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mmo.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kjg.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dwx.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tby.gogol.net.cn

[P03] 生成短随机字符串
来源：http://hkt.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ksr.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jqy.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uhj.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uqi.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://khy.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upn.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mcl.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://svl.yj20258888.top

[P04] 求长度
来源：http://juo.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dtt.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vdv.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlx.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izz.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://hup.mhx1999.top

Go:   len(arr);  len(m)
来源：http://apt.yuanzhike.top

Ruby: x.length;  x.size
来源：http://wrm.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tie.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://yoz.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://trs.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pbe.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zzn.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kfx.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nzt.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://txw.fengsongda.top

Ruby: a == b
来源：http://tvk.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gev.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rks.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qrf.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://voa.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rmm.cheryme.top

TS:   if (x == null) {}
来源：http://uia.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://cla.tianlin.xyz

Go:   if x == nil {}
来源：http://exj.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://afz.cashguo.top

C#:   if (x is null) {}
来源：http://mpu.cdnleiting.top

[P07] 防抖与节流
来源：http://gwb.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dwr.pycfn.com

PHP:  // 手写时间戳比较
来源：http://nyy.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ajw.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://coh.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pab.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lim.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqa.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://url.sweek.top

[P08] 处理浮点精度问题
来源：http://jfz.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gda.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rnf.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ypa.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sxx.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rfn.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hay.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sfj.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pul.ppjwa.cn

================================================================================
来源：http://pwp.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iow.gaohongyu789.top

================================================================================
来源：http://thy.tianlin.xyz

[Q01] 创建表
来源：http://pxe.yvedp.cn

CREATE TABLE users (
来源：http://ihl.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xdm.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://wsi.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://wtb.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uou.shanyushiyangtech.top

);
来源：http://cce.0kj1m.cn

[Q02] 创建带外键的表
来源：http://fnv.daxiang520.top

CREATE TABLE orders (
来源：http://yrr.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wpj.jianghu66.top

user_id INT NOT NULL,
来源：http://fwk.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://irn.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tzl.dashuyun.cn

);
来源：http://lct.ctjpmb.com

[Q03] 增加列
来源：http://dfc.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://axn.sweek.top

[Q04] 修改列类型
来源：http://myu.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://saq.redwolf501.top

[Q05] 重命名列
来源：http://vql.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kyd.daxiang520.top

[Q06] 删除列
来源：http://vyz.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nlc.fanxiaobao.xyz

[Q07] 删除表
来源：http://hlb.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://hkm.ctjpmb.com

[Q08] 创建普通索引
来源：http://duc.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xts.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://vrz.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jmb.aizwys.cn

[Q10] 插入单行
来源：http://zeb.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dhr.hywenlv.cn

[Q11] 一次插入多行
来源：http://rsu.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kjh.sweek.top

[Q12] 插入后取自增 ID
来源：http://bro.birdmap.top


<!-- 参考信息 -->