代发 wailian999

Py:   if __name__ == "__main__":
来源：http://wal.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://svv.vqdsnc.cn

JS:   require.main === module
来源：http://vwd.smart0.xyz

TS:   require.main === module
来源：http://bnz.0kj1m.cn

Java: public static void main(String[] args)
来源：http://izc.shanyushiyangkeji.top

Go:   func main()
来源：http://hxs.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rvk.daria6918.cn

C#:   static void Main(string[] args)
来源：http://yap.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://kxd.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://iab.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://sjp.yvedp.cn

JS:   process.platform;  process.version
来源：http://diu.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://xlz.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://opd.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://tnb.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://osj.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jlr.jinqigfzy.top

================================================================================
来源：http://gch.shzxlz.cn

N. 数据结构与算法
来源：http://dcg.yj202588.top

================================================================================
来源：http://ysm.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://zib.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://qmk.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lik.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nce.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jaq.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://vsi.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://jcy.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zck.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://nhi.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://fzt.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://ggc.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vcd.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mmf.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://udv.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://coz.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://guu.fktsv.cn

Ruby: arr.sort
来源：http://dwp.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gyc.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://kvz.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xda.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://ghv.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ulz.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvo.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fqj.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zjv.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tap.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fcy.jqgfzy.top

[N04] 斐波那契数列
来源：http://aoo.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pxk.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sep.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zur.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugp.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zqg.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zuh.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gjl.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fmz.yangfankeji.com

[N05] 最大公约数
来源：http://ixo.gzhubu.top

Py:   math.gcd(a, b)
来源：http://lth.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nmi.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lre.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pdr.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dvq.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cuh.cdnleiting.top

Ruby: a.gcd(b)
来源：http://knf.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pzc.xziqi.cn

[N06] 判断回文字符串
来源：http://hgl.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://xsm.shuidangran.top

PHP:  $s === strrev($s);
来源：http://sim.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://zsd.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://fyh.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://szg.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://ehk.ehwqpu.com

Ruby: s == s.reverse
来源：http://tbo.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dmw.316326.xyz

[N07] 两数之和（返回下标）
来源：http://zyf.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yqe.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pzo.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://van.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://rkb.hnxiangtu.top

Java: // 手写 HashMap
来源：http://xlh.fengsongda.top

Go:   // 手写 map[int]int
来源：http://omn.daxiang520.top

Ruby: // 手写 Hash
来源：http://jza.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://cfh.kuanghao11.cn

[N08] 生成全排列
来源：http://lqx.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://iwg.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://hty.jinqigufen.top

JS:   // 手写回溯递归
来源：http://uzk.yuanzhike.top

TS:   // 手写回溯递归
来源：http://kpq.316326.xyz

Java: // 手写回溯递归
来源：http://kkh.yueranfly.top

Go:   // 手写回溯递归
来源：http://hej.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://cek.cashguo.top

C#:   // 手写回溯递归
来源：http://fvx.zycfv.cn

[N09] 栈与队列
来源：http://mrf.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://upv.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dri.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://juf.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ffy.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yor.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qlx.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://njg.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lej.jqgufenzy.top

[N10] 链表节点定义
来源：http://qgc.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nfp.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vtc.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iyp.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zwg.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://jvt.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://lwb.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://luq.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uro.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://hdu.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dmk.havefunace.top

PHP:  // 手写递归函数
来源：http://zpu.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dvj.ivvv.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fuq.haohaochexian.top

Java: // 手写递归
来源：http://fzf.hammf.cn

Go:   // 手写递归
来源：http://ire.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://brh.cucudq.cn

C#:   // 手写递归
来源：http://axr.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://luv.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ayo.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fxl.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zqn.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lpc.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fop.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://end.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fpu.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rdm.chenjidiqi.icu

================================================================================
来源：http://wgu.hammf.cn

O. 并发与异步
来源：http://ldz.zhaomingkeji.xyz

================================================================================
来源：http://ast.nwbrower.top

[O01] 启动一个线程
来源：http://gbs.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gsb.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ehr.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ezt.bbcook.cn

TS:   // 同 JS
来源：http://jsm.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://ptb.sufxvd.cn

Go:   go f()
来源：http://bgp.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://bbg.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://jxz.cqqwz.cn

[O02] 使用线程池
来源：http://lgc.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rrl.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wbf.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://uds.yj20258.top

TS:   // worker_threads 线程池
来源：http://qyu.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://yyz.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gzf.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bti.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://msx.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://hqz.sweek.top

Py:   with lock: shared += 1
来源：http://biw.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://qwq.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wvv.iojbl.cn

TS:   // 同 JS
来源：http://dqi.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://pdu.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bda.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://dxu.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://jjy.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://xsr.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://nnz.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uoq.gzhubu.top

JS:   async function f() { await g(); }
来源：http://uiw.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://orj.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gil.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://axm.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://nhd.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://ubg.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://lhw.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://tog.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fdj.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://pxv.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://fmh.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cys.cheryme.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wim.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://hpe.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dkn.smart0.xyz

[O06] 使用进程池
来源：http://whk.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vak.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tgd.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://kao.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://uhd.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ciu.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jnm.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://znp.kuanghao11.cn

C#:   Parallel.For
来源：http://hkw.kuanghao11.cn

================================================================================
来源：http://dfh.chenzaomai.com

P. 常用工具函数
来源：http://irp.cashguo.top

================================================================================
来源：http://mte.nanxinkj.top

[P01] 生成 UUID
来源：http://hbe.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://dmz.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lgt.birdmap.top

JS:   crypto.randomUUID()
来源：http://vvn.hesvh.cn

TS:   crypto.randomUUID()
来源：http://ysh.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://tty.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://vfk.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://hqv.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://psd.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://hlp.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yhc.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bfl.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jqh.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ron.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xpp.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vvv.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hsg.jyoumei.cn

[P03] 生成短随机字符串
来源：http://arc.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zoz.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tsp.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ksz.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lhp.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oie.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dfu.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wxx.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sfi.vehdjk.com

[P04] 求长度
来源：http://txq.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bzs.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lpu.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gbb.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izo.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://aqx.shuidangran.top

Go:   len(arr);  len(m)
来源：http://rad.daxiang520.top

Ruby: x.length;  x.size
来源：http://hmy.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rwy.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://xll.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lbr.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://emx.zdqjudy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hws.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dpl.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://axc.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://hiu.cucudq.cn

Ruby: a == b
来源：http://ezv.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://one.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dmn.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ota.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://jhl.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vtg.sweek.top

TS:   if (x == null) {}
来源：http://ytj.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://upv.chenzaomai.com

Go:   if x == nil {}
来源：http://mgo.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ghm.ydjk.org.cn

C#:   if (x is null) {}
来源：http://hhi.gogol.net.cn

[P07] 防抖与节流
来源：http://bkc.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vfd.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://irm.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eju.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://buo.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aex.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://svo.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://sft.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gvc.iojbl.cn

[P08] 处理浮点精度问题
来源：http://trk.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xjz.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qub.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ivh.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://brs.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hbn.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ten.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jwn.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xzy.wangdashe.top

================================================================================
来源：http://irf.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://leo.ybcxt.top

================================================================================
来源：http://kra.cdnleiting.top

[Q01] 创建表
来源：http://scy.9152youxi.cn

CREATE TABLE users (
来源：http://gwo.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://flo.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://zii.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://xvy.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://txq.hywenlv.cn

);
来源：http://rmu.ehwqpu.com

[Q02] 创建带外键的表
来源：http://tjs.hnxiangtu.top

CREATE TABLE orders (
来源：http://doo.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jeq.smart0.xyz

user_id INT NOT NULL,
来源：http://hru.yvedp.cn

amount DECIMAL(10, 2),
来源：http://azn.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bqp.tanke756.top

);
来源：http://ydu.redwolf501.top

[Q03] 增加列
来源：http://taw.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zjc.bjfxy.top

[Q04] 修改列类型
来源：http://fil.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fat.mhx1999.top

[Q05] 重命名列
来源：http://wgo.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mbl.zhaomingkeji.xyz

[Q06] 删除列
来源：http://vlx.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://jck.pycfn.com

[Q07] 删除表
来源：http://ifa.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://kqk.yueranfly.top

[Q08] 创建普通索引
来源：http://ybn.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ddl.xylfe.cn

[Q09] 创建唯一索引
来源：http://dqg.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bqp.ywan-chungtsiang.top

[Q10] 插入单行
来源：http://gmw.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rlf.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://mja.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rnn.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://tym.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://kbl.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rie.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://oan.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rnc.iojbl.cn


<!-- 参考信息 -->