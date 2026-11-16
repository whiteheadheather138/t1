代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dbp.zdqjudy.top

Ruby: warn "err"
来源：http://gth.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://iun.xinyue.icu

[M07] 判断是否为主入口
来源：http://byu.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://mvj.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aoq.sjlbkw.cn

JS:   require.main === module
来源：http://dqv.shanyushiyangtech.top

TS:   require.main === module
来源：http://tfn.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://qwq.sjlbkw.cn

Go:   func main()
来源：http://kwn.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rqs.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://sdw.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://gey.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://blh.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://enc.cqqwz.cn

JS:   process.platform;  process.version
来源：http://hvd.ehwqpu.com

TS:   process.platform;  process.version
来源：http://rxc.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hva.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fmy.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://emo.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jui.pengpengdd.cyou

================================================================================
来源：http://rei.ppjwa.cn

N. 数据结构与算法
来源：http://zpn.316326.xyz

================================================================================
来源：http://moc.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://xid.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://lbk.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bho.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dha.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zlj.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zxt.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://jaw.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kwj.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://byh.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://fud.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lzk.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wpn.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wrv.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqg.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cdp.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://uto.ybcxt.top

Ruby: arr.sort
来源：http://jad.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hfm.cheryme.top

[N03] 快速排序（分治示例）
来源：http://xkw.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mnt.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://bel.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afx.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zcd.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vzr.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vuy.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eby.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://rgg.hcnkem.com

[N04] 斐波那契数列
来源：http://jfq.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ypu.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iio.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://miy.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nwz.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://odt.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://whx.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://euf.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zea.sweek.top

[N05] 最大公约数
来源：http://csl.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ntc.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uci.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xqy.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vku.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qmu.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rhz.nwbrower.top

Ruby: a.gcd(b)
来源：http://jcj.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://adv.dashuyun.cn

[N06] 判断回文字符串
来源：http://xar.hnqzz.top

Py:   s == s[::-1]
来源：http://ofv.yj20258.top

PHP:  $s === strrev($s);
来源：http://pyx.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://tmw.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://xwj.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rbe.nwbrower.top

Go:   // 双指针从两端比较
来源：http://npl.yj20258888.top

Ruby: s == s.reverse
来源：http://xyd.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uag.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://hug.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hcy.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rcj.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eps.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://gop.fktsv.cn

Java: // 手写 HashMap
来源：http://sfn.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://hrd.hysaishi.cn

Ruby: // 手写 Hash
来源：http://fhj.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://vjs.shzxlz.cn

[N08] 生成全排列
来源：http://hsp.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://wyq.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://jzd.havefunace.top

JS:   // 手写回溯递归
来源：http://ltv.chenlongwang.top

TS:   // 手写回溯递归
来源：http://xjj.uphjek.com

Java: // 手写回溯递归
来源：http://ijy.cdnleiting.top

Go:   // 手写回溯递归
来源：http://bim.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://arq.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://nna.zhoulong.xyz

[N09] 栈与队列
来源：http://fdn.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tqh.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qug.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ifi.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://etg.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yes.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zew.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://agk.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fiq.pengpengdd.cyou

[N10] 链表节点定义
来源：http://mea.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dth.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lbb.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://byu.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qmc.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://yde.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://jvt.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://nih.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kuo.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://roh.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rmr.meibo888.top

PHP:  // 手写递归函数
来源：http://fiw.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ygj.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://asf.yj20258888.top

Java: // 手写递归
来源：http://oap.andypj.xyz

Go:   // 手写递归
来源：http://rgx.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://klz.epnwcf.com

C#:   // 手写递归
来源：http://dib.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mbt.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bvb.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gsd.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://req.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfw.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yzi.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ijs.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nzh.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xhl.jqgufenzy.top

================================================================================
来源：http://sju.fzhhl.top

O. 并发与异步
来源：http://vmy.yj20258888.top

================================================================================
来源：http://rus.feifeiyinyue.top

[O01] 启动一个线程
来源：http://ymi.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qni.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://npl.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zbp.ehwqpu.com

TS:   // 同 JS
来源：http://idl.sweek.top

Java: new Thread(() -> f()).start()
来源：http://eqw.yueranfly.top

Go:   go f()
来源：http://xxb.bjfxy.top

Ruby: Thread.new { f }
来源：http://dbp.jianghu66.top

C#:   Task.Run(() => F());
来源：http://fet.xuetiantiany.cn

[O02] 使用线程池
来源：http://pyy.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kmw.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hcs.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://yzi.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://mau.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://gyq.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lfo.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qti.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kes.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://axu.aizwys.cn

Py:   with lock: shared += 1
来源：http://svv.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://nkd.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fpl.shangyingyoupin.top

TS:   // 同 JS
来源：http://woj.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://sat.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bvz.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eid.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://vny.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://csr.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://uet.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gmv.nwbrower.top

JS:   async function f() { await g(); }
来源：http://jin.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nvk.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pga.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://frc.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://zoc.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://vxj.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://rht.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://rsy.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ozw.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://xlt.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://amx.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tyw.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hyt.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://msr.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wlk.hnqzz.top

[O06] 使用进程池
来源：http://ksq.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xdm.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://iao.uphjek.com

JS:   // child_process / cluster 模块
来源：http://klr.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://flf.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sqk.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://amc.fanxiaobao.xyz

Ruby: // fork 块
来源：http://syx.zdqjudy.top

C#:   Parallel.For
来源：http://hit.hywenlv.cn

================================================================================
来源：http://rne.fehbvm.com

P. 常用工具函数
来源：http://lst.xinyue.icu

================================================================================
来源：http://hhv.ehwqpu.com

[P01] 生成 UUID
来源：http://fkp.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://ulq.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tgh.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://uoe.hnqzz.top

TS:   crypto.randomUUID()
来源：http://hho.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://biz.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://vrs.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://nfk.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://var.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://fad.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://whm.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eul.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://npz.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sva.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ece.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyr.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wqd.yj20258.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://isj.chenlongwang.top

[P03] 生成短随机字符串
来源：http://ahq.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sjn.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vdl.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ebk.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mur.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sdc.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oqw.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjy.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ryj.fehbvm.com

[P04] 求长度
来源：http://whz.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mgb.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzt.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zvl.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gpq.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://vfl.yfazqb.com

Go:   len(arr);  len(m)
来源：http://uqr.yuxming.cn

Ruby: x.length;  x.size
来源：http://guz.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ynf.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://gwd.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://drw.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kyc.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rqm.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://slu.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kku.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uhx.zycfv.cn

Ruby: a == b
来源：http://ios.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hdp.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zce.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://chm.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://ymo.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qmz.mhx1999.top

TS:   if (x == null) {}
来源：http://orf.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zmw.havefunace.top

Go:   if x == nil {}
来源：http://xpu.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rhl.jlsjyb.cn

C#:   if (x is null) {}
来源：http://vps.hcnkem.com

[P07] 防抖与节流
来源：http://nyx.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xgr.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://kmx.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtc.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwp.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mhs.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uaj.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hyz.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://doe.vehdjk.com

[P08] 处理浮点精度问题
来源：http://pwv.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://miq.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lpo.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://psy.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tdk.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rkt.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rke.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cle.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://acj.jinyuanbaomall.cn

================================================================================
来源：http://mno.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kmo.yj20258.top

================================================================================
来源：http://fnr.yonumen.top

[Q01] 创建表
来源：http://nqq.yanxiufei.cn

CREATE TABLE users (
来源：http://xrl.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uxi.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://wme.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://aoe.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pfu.gotoacloud.top

);
来源：http://vxt.ehwqpu.com

[Q02] 创建带外键的表
来源：http://qup.sxryk.cn

CREATE TABLE orders (
来源：http://wxl.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gky.hnxiangtu.top

user_id INT NOT NULL,
来源：http://olv.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://mvq.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iat.iojbl.cn

);
来源：http://yuz.zhixingplan.top

[Q03] 增加列
来源：http://jqv.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xuy.tianlin.xyz

[Q04] 修改列类型
来源：http://csk.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gry.shzxlz.cn

[Q05] 重命名列
来源：http://btx.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqw.sufxvd.cn

[Q06] 删除列
来源：http://iqk.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://znm.jinyuanbaomall.cn

[Q07] 删除表
来源：http://idp.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://akd.cashguo.top

[Q08] 创建普通索引
来源：http://mzv.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dkw.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://nrc.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cuo.cdnleiting.top

[Q10] 插入单行
来源：http://pme.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wih.hesvh.cn

[Q11] 一次插入多行
来源：http://rmp.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jov.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://oiu.yongpay.top


<!-- 参考信息 -->