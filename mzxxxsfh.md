代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://qgv.cqqwz.cn

JS:   console.error("err")
来源：http://dkw.gotoacloud.top

TS:   console.error("err")
来源：http://sxo.dianchejie.cn

Java: System.err.println("err")
来源：http://qzy.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wel.zdqjudy.top

Ruby: warn "err"
来源：http://qaf.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://sxk.smart0.xyz

[M07] 判断是否为主入口
来源：http://tty.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://fak.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://syg.ctjpmb.com

JS:   require.main === module
来源：http://ehh.svipenyu.cn

TS:   require.main === module
来源：http://wod.uphjek.com

Java: public static void main(String[] args)
来源：http://ulh.gotoacloud.top

Go:   func main()
来源：http://rpv.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tru.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://xwx.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://mbx.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://xrv.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://wli.redwolf501.top

JS:   process.platform;  process.version
来源：http://btd.sufxvd.cn

TS:   process.platform;  process.version
来源：http://jpi.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sbn.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wbg.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://are.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mmp.zhengqikj.top

================================================================================
来源：http://dqi.daxiang520.top

N. 数据结构与算法
来源：http://fkj.hysaishi.cn

================================================================================
来源：http://zxp.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://fqj.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mnf.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nys.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kak.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ecc.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://svj.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://mam.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://caq.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://agp.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://snb.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://lzx.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ibv.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://odl.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vam.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aue.yonumen.top

Go:   slices.Sort(arr)
来源：http://ece.tianlin.xyz

Ruby: arr.sort
来源：http://xpb.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jrn.yonumen.top

[N03] 快速排序（分治示例）
来源：http://rgh.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kdy.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://qto.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uaf.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sin.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pff.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kem.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vla.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://ajn.shuidangran.top

[N04] 斐波那契数列
来源：http://ani.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rkr.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://grs.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ubf.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ego.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iij.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ujg.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fle.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://flk.svipenyu.cn

[N05] 最大公约数
来源：http://tid.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://qng.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vnh.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yew.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ubj.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hry.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ley.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://cgm.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pxt.pycfn.com

[N06] 判断回文字符串
来源：http://vhz.cashguo.top

Py:   s == s[::-1]
来源：http://eev.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://vij.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://cur.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://bjn.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ucl.bbcook.cn

Go:   // 双指针从两端比较
来源：http://lar.jiagoushi.top

Ruby: s == s.reverse
来源：http://wex.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ggo.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://svb.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tri.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oym.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wmt.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://ktm.epnwcf.com

Java: // 手写 HashMap
来源：http://bkc.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://gty.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://ixd.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://hak.jqgufenzy.top

[N08] 生成全排列
来源：http://kom.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://xrn.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://fyl.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://qfd.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://shp.cqqwz.cn

Java: // 手写回溯递归
来源：http://kaw.xinyue.icu

Go:   // 手写回溯递归
来源：http://rww.meibo888.top

Ruby: arr.permutation.to_a
来源：http://afz.vehdjk.com

C#:   // 手写回溯递归
来源：http://mga.wangshuangyany.cn

[N09] 栈与队列
来源：http://sxe.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bvh.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hzd.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wbi.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://liv.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://byf.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://meo.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ayt.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://azu.hcnkem.com

[N10] 链表节点定义
来源：http://zkr.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lgx.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bog.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eno.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://twn.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://iek.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://vzq.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cjy.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mll.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://qvq.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ppk.redwolf501.top

PHP:  // 手写递归函数
来源：http://xjx.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://flv.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fps.zdbjq.cn

Java: // 手写递归
来源：http://ssu.xuanzx.com

Go:   // 手写递归
来源：http://ewx.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ezq.daxiang520.top

C#:   // 手写递归
来源：http://vcr.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zkc.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uvy.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gsz.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rvi.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jhm.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hyg.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xaa.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htw.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ngu.zycfv.cn

================================================================================
来源：http://fmw.tianlin.xyz

O. 并发与异步
来源：http://fel.fanxiaobao.xyz

================================================================================
来源：http://ehv.yj202588.top

[O01] 启动一个线程
来源：http://ksw.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yvs.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hea.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qnl.sxryk.cn

TS:   // 同 JS
来源：http://stp.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://fkx.smart0.xyz

Go:   go f()
来源：http://lug.ehwqpu.com

Ruby: Thread.new { f }
来源：http://ehd.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://wan.aizwys.cn

[O02] 使用线程池
来源：http://pdl.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://chd.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aza.uphjek.com

JS:   // worker_threads 线程池
来源：http://cgz.tarul.cn

TS:   // worker_threads 线程池
来源：http://bfd.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ftk.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qrk.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uov.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wib.epnwcf.com

[O03] 加锁保护共享数据
来源：http://jdm.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://qiz.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://yzr.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ous.hcnkem.com

TS:   // 同 JS
来源：http://aez.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://god.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gam.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fie.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://sqs.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://mzs.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://gvs.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eyn.daxiang520.top

JS:   async function f() { await g(); }
来源：http://mgb.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zcg.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dbf.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ihp.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://mkr.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://vvl.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://mkl.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://hfn.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wux.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://gjy.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://her.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uco.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eng.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://uvn.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://oot.dianchejie.cn

[O06] 使用进程池
来源：http://gwu.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://clo.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://urf.yonumen.top

JS:   // child_process / cluster 模块
来源：http://ywy.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://ssv.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pqt.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ksr.havefunace.top

Ruby: // fork 块
来源：http://ecs.sweek.top

C#:   Parallel.For
来源：http://kma.zdbjq.cn

================================================================================
来源：http://qdv.yfazqb.com

P. 常用工具函数
来源：http://kaa.jqgufenzy.top

================================================================================
来源：http://sie.yfazqb.com

[P01] 生成 UUID
来源：http://ltm.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://kxj.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://egn.yj202588.top

JS:   crypto.randomUUID()
来源：http://hkl.xuanzx.com

TS:   crypto.randomUUID()
来源：http://vrr.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://doj.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://goj.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://upb.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://zjt.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://woh.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fzw.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjr.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xph.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dql.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cfy.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bvq.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://efn.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ydl.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://pes.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sxw.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cah.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lxx.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kem.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vie.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ruk.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gma.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ujk.fanxiaobao.xyz

[P04] 求长度
来源：http://stm.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kxd.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mej.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nfn.hywenlv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vtr.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://wzc.redwolf501.top

Go:   len(arr);  len(m)
来源：http://qwu.zhengqikj.top

Ruby: x.length;  x.size
来源：http://ulq.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ukr.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://ifv.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://piy.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mor.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jdr.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fyi.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rzz.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://ces.wangdashe.top

Ruby: a == b
来源：http://inl.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ers.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://elb.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wol.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://eca.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wac.birdmap.top

TS:   if (x == null) {}
来源：http://fyr.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://izt.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://jrq.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pti.yangfankeji.com

C#:   if (x is null) {}
来源：http://thx.yvedp.cn

[P07] 防抖与节流
来源：http://krc.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qbv.cheryme.top

PHP:  // 手写时间戳比较
来源：http://zlq.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gba.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://koj.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vjl.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rft.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqo.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yvf.c1oappe.top

[P08] 处理浮点精度问题
来源：http://fwq.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wzy.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nuv.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pjk.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xnq.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wkv.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zez.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tfv.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://znt.c1oappe.top

================================================================================
来源：http://xrl.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bds.wangdashe.top

================================================================================
来源：http://jbg.ywan-chungtsiang.top

[Q01] 创建表
来源：http://opd.bjfxy.top

CREATE TABLE users (
来源：http://ytv.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nph.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://nkb.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://est.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xcz.sxryk.cn

);
来源：http://kxn.gzhubu.top

[Q02] 创建带外键的表
来源：http://mql.hcnkem.com

CREATE TABLE orders (
来源：http://vqb.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgd.gzhubu.top

user_id INT NOT NULL,
来源：http://ksx.hcnkem.com

amount DECIMAL(10, 2),
来源：http://ssh.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sxl.aizwys.cn

);
来源：http://kxs.uphjek.com

[Q03] 增加列
来源：http://kof.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://klf.sufxvd.cn

[Q04] 修改列类型
来源：http://lyq.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dui.jinqigfzy.top

[Q05] 重命名列
来源：http://alf.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://htt.zhoulong.xyz

[Q06] 删除列
来源：http://igt.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bpc.hywenlv.cn

[Q07] 删除表
来源：http://txo.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://mua.xylfe.cn

[Q08] 创建普通索引
来源：http://cwl.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://bha.nanxinkj.top

[Q09] 创建唯一索引
来源：http://rmc.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hnm.ehwqpu.com

[Q10] 插入单行
来源：http://bph.xziqi.cn


<!-- 参考信息 -->