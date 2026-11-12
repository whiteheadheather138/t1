代发 wailian999

Java: public static void main(String[] args)
来源：http://jsp.birdmap.top

Go:   func main()
来源：http://qzo.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://myi.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://ffv.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://gwz.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://ecd.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://gys.52xcode.cn

JS:   process.platform;  process.version
来源：http://wyi.jyoumei.cn

TS:   process.platform;  process.version
来源：http://har.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sle.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jop.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gai.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jrf.sweek.top

================================================================================
来源：http://fms.jiagoushi.top

N. 数据结构与算法
来源：http://npz.vehdjk.com

================================================================================
来源：http://dib.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://vct.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bud.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ash.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddl.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rtd.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://edb.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bbg.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://geb.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dil.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://iqa.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://ddd.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tnt.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nft.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kzu.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fpq.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://epd.nanxuanxn.top

Ruby: arr.sort
来源：http://cbq.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://oxp.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://cwk.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yiw.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://dsz.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxk.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kky.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqa.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cqy.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yxz.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://mav.cheryme.top

[N04] 斐波那契数列
来源：http://jzi.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yvf.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wkb.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ldz.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exi.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://owc.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oau.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fnk.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sli.vehdjk.com

[N05] 最大公约数
来源：http://rkj.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://tdj.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdf.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://erz.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dev.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nsh.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dml.iojbl.cn

Ruby: a.gcd(b)
来源：http://xtw.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tkd.cashguo.top

[N06] 判断回文字符串
来源：http://cgm.chenzaomai.com

Py:   s == s[::-1]
来源：http://twa.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://hrr.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://abw.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://xdr.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zdu.xylfe.cn

Go:   // 双指针从两端比较
来源：http://yic.zdbjq.cn

Ruby: s == s.reverse
来源：http://kyq.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://lfo.cashguo.top

[N07] 两数之和（返回下标）
来源：http://uzf.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eyx.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xrs.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://khr.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://xax.sysykeji.top

Java: // 手写 HashMap
来源：http://fgz.yuxming.cn

Go:   // 手写 map[int]int
来源：http://shr.meibo888.top

Ruby: // 手写 Hash
来源：http://nat.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://pfm.0kj1m.cn

[N08] 生成全排列
来源：http://lba.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://nuf.9152youxi.cn

PHP:  // 手写递归交换
来源：http://oet.fengsongda.top

JS:   // 手写回溯递归
来源：http://ule.xinyue.icu

TS:   // 手写回溯递归
来源：http://iie.yuanzhike.top

Java: // 手写回溯递归
来源：http://dsx.ctjpmb.com

Go:   // 手写回溯递归
来源：http://xaj.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://xmf.cashguo.top

C#:   // 手写回溯递归
来源：http://veh.yj20258.top

[N09] 栈与队列
来源：http://lzz.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rtl.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yax.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xxm.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lbj.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sky.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tsl.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://abc.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ici.sjlbkw.cn

[N10] 链表节点定义
来源：http://rza.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aqe.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://qsx.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kwl.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zzu.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://ild.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://bpu.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pdl.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xly.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://zrg.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xww.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://cva.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mns.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jfe.vqdsnc.cn

Java: // 手写递归
来源：http://xqy.jyoumei.cn

Go:   // 手写递归
来源：http://lpu.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dlr.xinyue.icu

C#:   // 手写递归
来源：http://ini.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vfr.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qct.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ukm.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://duz.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfn.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ijs.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fgv.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lcs.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rli.ybcxt.top

================================================================================
来源：http://qrv.fktsv.cn

O. 并发与异步
来源：http://tcs.gzhubu.top

================================================================================
来源：http://cqz.zdqjudy.top

[O01] 启动一个线程
来源：http://jxs.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hxp.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aiq.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uxh.guowangkeji.top

TS:   // 同 JS
来源：http://ooe.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://mxw.wangshuangyany.cn

Go:   go f()
来源：http://qvf.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://erj.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://pav.jinqigufen.top

[O02] 使用线程池
来源：http://nvy.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://phw.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://abg.zycfv.cn

JS:   // worker_threads 线程池
来源：http://vny.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://xcf.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tld.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xyc.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hwq.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bev.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://bmw.ivvv.top

Py:   with lock: shared += 1
来源：http://kbd.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://eod.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wsm.fktsv.cn

TS:   // 同 JS
来源：http://blu.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://hcl.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yyn.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dle.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://kri.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://yqf.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://lqh.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pyy.xziqi.cn

JS:   async function f() { await g(); }
来源：http://rhy.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gxt.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jpd.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iwj.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vhe.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://udj.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://ddc.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://oor.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lnc.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://fan.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://lir.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://miv.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rje.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://atg.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hfe.zhoulong.xyz

[O06] 使用进程池
来源：http://vkk.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zux.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rhd.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://yyi.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://zwg.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iwf.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pkp.mhx1999.top

Ruby: // fork 块
来源：http://bzc.iojbl.cn

C#:   Parallel.For
来源：http://ega.xylfe.cn

================================================================================
来源：http://ofn.jinqigufen.top

P. 常用工具函数
来源：http://ozv.pycfn.com

================================================================================
来源：http://fcp.52xcode.cn

[P01] 生成 UUID
来源：http://uin.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://ejd.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ahg.hcnkem.com

JS:   crypto.randomUUID()
来源：http://hkh.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://umj.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://mxz.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://haz.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://lpk.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://hei.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://tfb.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wtv.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hnm.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wvv.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jlt.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://crq.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wum.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bzm.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aqs.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://adn.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqm.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tju.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mre.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyw.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nfo.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://svh.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ecv.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dcp.fehbvm.com

[P04] 求长度
来源：http://dee.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xlu.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hqr.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcp.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ysf.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://zvp.yfazqb.com

Go:   len(arr);  len(m)
来源：http://adz.hcnkem.com

Ruby: x.length;  x.size
来源：http://wfm.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nuh.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://jye.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lzw.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://noz.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ulo.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ieg.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://biu.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://eru.sweek.top

Ruby: a == b
来源：http://nsb.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xhw.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ybx.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oxl.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://wvl.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://skb.cqqwz.cn

TS:   if (x == null) {}
来源：http://cwc.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ojg.hcnkem.com

Go:   if x == nil {}
来源：http://ecu.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fqn.meibo888.top

C#:   if (x is null) {}
来源：http://nwf.aizwys.cn

[P07] 防抖与节流
来源：http://wda.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dac.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://kvz.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rhl.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rmk.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://miq.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nib.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fex.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jkr.jiagoushi.top

[P08] 处理浮点精度问题
来源：http://vaw.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bxb.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gke.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ubp.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bud.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dtn.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iqv.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kxz.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://omj.yuanzhike.top

================================================================================
来源：http://flr.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://irk.ivvv.top

================================================================================
来源：http://mew.zhoulong.xyz

[Q01] 创建表
来源：http://afp.quarkkingdee.top

CREATE TABLE users (
来源：http://xyu.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eoj.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://izc.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://qxt.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://awv.jianghu66.top

);
来源：http://qjz.zycfv.cn

[Q02] 创建带外键的表
来源：http://drz.xuanzx.com

CREATE TABLE orders (
来源：http://gqc.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kxj.zhengqikj.top

user_id INT NOT NULL,
来源：http://csp.xziqi.cn

amount DECIMAL(10, 2),
来源：http://fnr.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mgj.bbcook.cn

);
来源：http://hrw.zhaomingkeji.xyz

[Q03] 增加列
来源：http://zek.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bje.yuanzhike.top

[Q04] 修改列类型
来源：http://kcy.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jvu.bbcook.cn

[Q05] 重命名列
来源：http://qty.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qfl.daria6918.cn

[Q06] 删除列
来源：http://snz.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://dhl.bjfxy.top

[Q07] 删除表
来源：http://ecl.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://edo.daria6918.cn

[Q08] 创建普通索引
来源：http://goc.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://psj.yj20258.top

[Q09] 创建唯一索引
来源：http://bto.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ocj.sjlbkw.cn

[Q10] 插入单行
来源：http://afd.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lfj.yfazqb.com

[Q11] 一次插入多行
来源：http://bzc.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bmk.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://rhr.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fnc.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tyo.fzhhl.top

[Q13] 忽略重复插入
来源：http://ymn.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lvr.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://cfz.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ldr.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fji.daxiang520.top

[Q15] 查询全部
来源：http://kxz.bjfxy.top


<!-- 参考信息 -->