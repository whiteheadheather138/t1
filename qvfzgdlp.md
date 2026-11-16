代发 wailian999

Py:   if __name__ == "__main__":
来源：http://wvb.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vvw.yonumen.top

JS:   require.main === module
来源：http://lki.jiagoushi.top

TS:   require.main === module
来源：http://kjv.shzxlz.cn

Java: public static void main(String[] args)
来源：http://oyx.bbcook.cn

Go:   func main()
来源：http://amv.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wiu.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://zyj.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://ucq.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://cbo.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://qpu.hcnkem.com

JS:   process.platform;  process.version
来源：http://jsk.zdqjudy.top

TS:   process.platform;  process.version
来源：http://ume.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://itg.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyo.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sey.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mje.jqgfzy.top

================================================================================
来源：http://idi.epnwcf.com

N. 数据结构与算法
来源：http://bsp.fanxiaobao.xyz

================================================================================
来源：http://osx.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://bxc.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cnr.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nhg.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mog.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqk.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eee.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://qwp.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qvi.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://xlv.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://bbv.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://cex.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zhm.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pne.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://zmc.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uoc.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://pjs.snrcjt.cn

Ruby: arr.sort
来源：http://vhk.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://owi.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://efy.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kmj.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://joe.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ore.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ztu.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://szs.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tav.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ime.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://plq.quarkkingdee.top

[N04] 斐波那契数列
来源：http://lix.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ddo.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://htq.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkb.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://arx.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lpm.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bbp.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yve.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nzm.yfazqb.com

[N05] 最大公约数
来源：http://bxk.sysykeji.top

Py:   math.gcd(a, b)
来源：http://qkz.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://giv.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cej.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjf.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fur.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yif.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://zip.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvf.0kj1m.cn

[N06] 判断回文字符串
来源：http://wjl.nwbrower.top

Py:   s == s[::-1]
来源：http://nmm.yj20258.top

PHP:  $s === strrev($s);
来源：http://qew.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://cbs.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://wtb.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://atj.fktsv.cn

Go:   // 双指针从两端比较
来源：http://txh.andypj.xyz

Ruby: s == s.reverse
来源：http://ose.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bmr.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://jia.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rmc.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dot.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qqi.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://bsz.svipenyu.cn

Java: // 手写 HashMap
来源：http://fml.yvedp.cn

Go:   // 手写 map[int]int
来源：http://axu.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://dan.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://kdi.aibaodan.cn

[N08] 生成全排列
来源：http://xwa.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://etm.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://vbf.yuxming.cn

JS:   // 手写回溯递归
来源：http://tfq.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://hmk.hnqzz.top

Java: // 手写回溯递归
来源：http://ddr.nwbrower.top

Go:   // 手写回溯递归
来源：http://eux.havefunace.top

Ruby: arr.permutation.to_a
来源：http://pci.fengsongda.top

C#:   // 手写回溯递归
来源：http://lxb.haohaochexian.top

[N09] 栈与队列
来源：http://dgj.zdqjudy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bfp.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lbp.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fma.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lta.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lld.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lvf.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zrv.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ehp.yj20258.top

[N10] 链表节点定义
来源：http://esv.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gul.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hmk.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mig.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://okx.hammf.cn

Java: class Node { int v; Node next; }
来源：http://xpg.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://qsl.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fws.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wmy.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://wam.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://euh.hcnkem.com

PHP:  // 手写递归函数
来源：http://plw.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://isd.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgh.snrcjt.cn

Java: // 手写递归
来源：http://pkw.ydjk.org.cn

Go:   // 手写递归
来源：http://oyw.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hau.nwbrower.top

C#:   // 手写递归
来源：http://lhx.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rge.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tdv.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uwa.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rnq.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://muh.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ydu.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://opd.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://unz.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://drk.yonumen.top

================================================================================
来源：http://wox.sxryk.cn

O. 并发与异步
来源：http://cdu.hfpthk.cn

================================================================================
来源：http://pim.cheryme.top

[O01] 启动一个线程
来源：http://pwk.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wal.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ecp.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ray.daxiang520.top

TS:   // 同 JS
来源：http://rqh.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://fzv.hfpthk.cn

Go:   go f()
来源：http://egc.bjfxy.top

Ruby: Thread.new { f }
来源：http://kpg.sxryk.cn

C#:   Task.Run(() => F());
来源：http://htn.hcnkem.com

[O02] 使用线程池
来源：http://okj.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ips.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gml.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://bhb.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://uxs.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jtw.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wwb.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lzy.yfazqb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://csw.daxiang520.top

[O03] 加锁保护共享数据
来源：http://nwa.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://ykf.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://zon.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vtb.0kj1m.cn

TS:   // 同 JS
来源：http://hwt.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://opo.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cpb.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hqf.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://vsy.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://itz.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://elm.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slc.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://jis.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbb.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lkr.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ehm.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://meb.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://dde.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://wme.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://tet.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lwi.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://qkb.tarul.cn

TS:   await Promise.all(tasks)
来源：http://ulf.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nsm.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://abr.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://ftn.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://nnf.vqdsnc.cn

[O06] 使用进程池
来源：http://cim.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jyx.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://bjf.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://qgz.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://htu.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lzg.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qam.fanxiaobao.xyz

Ruby: // fork 块
来源：http://xxe.yvedp.cn

C#:   Parallel.For
来源：http://zoo.52xcode.cn

================================================================================
来源：http://non.jinqigfzy.top

P. 常用工具函数
来源：http://tkg.xuanzx.com

================================================================================
来源：http://wtg.yuanzhike.top

[P01] 生成 UUID
来源：http://nqw.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://wbu.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://opu.yongpay.top

JS:   crypto.randomUUID()
来源：http://wal.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://qgw.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://iwl.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://hmv.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://yxe.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://iez.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://smm.andypj.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qiv.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://dut.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dnh.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dyn.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nyc.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cyb.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ncv.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xla.fktsv.cn

[P03] 生成短随机字符串
来源：http://ucj.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cnb.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dvd.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfv.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://krq.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zmp.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ard.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gsb.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wiq.shanyushiyangkeji.top

[P04] 求长度
来源：http://wxz.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aqv.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://abv.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://esx.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vmj.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://bxq.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://caa.yj20258.top

Ruby: x.length;  x.size
来源：http://mqw.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://dsd.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://ahb.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mhv.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bhg.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lcm.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dlt.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pnc.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://quz.zhijiandao.cn

Ruby: a == b
来源：http://iuz.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qfw.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fip.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vkr.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://yho.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nxx.chenzaomai.com

TS:   if (x == null) {}
来源：http://pri.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lpg.hcnkem.com

Go:   if x == nil {}
来源：http://ttf.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hzr.shuidangran.top

C#:   if (x is null) {}
来源：http://sdk.daxiang520.top

[P07] 防抖与节流
来源：http://eeu.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kij.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://moy.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tot.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://daf.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cwh.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ybm.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fqt.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eak.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://osd.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ovk.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://miv.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://djo.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://phq.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xvb.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tir.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ijq.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ttn.andypj.xyz

================================================================================
来源：http://bhp.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yje.shangyingyoupin.top

================================================================================
来源：http://qhw.tian-w.cn

[Q01] 创建表
来源：http://dgm.jinqigufen.top

CREATE TABLE users (
来源：http://oed.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://krq.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://cfa.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://qsz.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cpy.redwolf501.top

);
来源：http://tkk.gogol.net.cn

[Q02] 创建带外键的表
来源：http://gsn.gogol.net.cn

CREATE TABLE orders (
来源：http://frh.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cyl.9152youxi.cn

user_id INT NOT NULL,
来源：http://zle.vehdjk.com

amount DECIMAL(10, 2),
来源：http://abc.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zmw.zhoulong.xyz

);
来源：http://ddm.dashuyun.cn

[Q03] 增加列
来源：http://cpc.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hfe.jinqigufen.top

[Q04] 修改列类型
来源：http://tja.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fwo.yangfankeji.com

[Q05] 重命名列
来源：http://tob.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pez.pengpengdd.cyou

[Q06] 删除列
来源：http://uzf.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://ole.ctjpmb.com

[Q07] 删除表
来源：http://ozw.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://uur.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://fii.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tyo.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://tzk.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rgn.sjlbkw.cn

[Q10] 插入单行
来源：http://uay.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fsf.epnwcf.com

[Q11] 一次插入多行
来源：http://eqm.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fwz.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://afa.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://rpo.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rgn.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://pmh.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hpx.jqgufenzy.top


<!-- 参考信息 -->