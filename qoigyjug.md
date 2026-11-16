代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dky.andypj.xyz

Ruby: warn "err"
来源：http://lmh.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://fsq.yvedp.cn

[M07] 判断是否为主入口
来源：http://kle.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://mii.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bti.gogol.net.cn

JS:   require.main === module
来源：http://fsl.yuanzhike.top

TS:   require.main === module
来源：http://aap.mhx1999.top

Java: public static void main(String[] args)
来源：http://idl.haohaochexian.top

Go:   func main()
来源：http://fxg.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pkt.guannengcc.top

C#:   static void Main(string[] args)
来源：http://upr.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://kun.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://otp.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://zfs.iojbl.cn

JS:   process.platform;  process.version
来源：http://sgk.birdmap.top

TS:   process.platform;  process.version
来源：http://zyi.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fku.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qoi.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hze.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qjq.sjlbkw.cn

================================================================================
来源：http://sks.zdbjq.cn

N. 数据结构与算法
来源：http://tlv.jyoumei.cn

================================================================================
来源：http://kbh.cheryme.top

[N01] 二分查找（有序数组）
来源：http://ixr.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xdo.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cvi.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wyf.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hsv.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rar.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://tcm.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://vxn.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gux.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://bmq.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://tec.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://src.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lxj.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dqo.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yag.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://uto.yj20258.top

Ruby: arr.sort
来源：http://siu.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ghq.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://jat.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pny.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://fzi.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://huw.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fxw.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://alr.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yij.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vhk.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tbw.mhx1999.top

[N04] 斐波那契数列
来源：http://sux.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://muu.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmd.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pta.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qlr.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zul.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cxe.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hrt.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nvn.vehdjk.com

[N05] 最大公约数
来源：http://nhc.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://vwq.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xht.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szk.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fdi.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tml.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fqp.tian-w.cn

Ruby: a.gcd(b)
来源：http://rdr.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nki.yj20258.top

[N06] 判断回文字符串
来源：http://fim.jinqigufen.top

Py:   s == s[::-1]
来源：http://kzk.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://oxc.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://eeh.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://ghz.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://snr.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://fta.iojbl.cn

Ruby: s == s.reverse
来源：http://djz.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ngv.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://nhw.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rpy.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jrr.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kte.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://upk.gzhubu.top

Java: // 手写 HashMap
来源：http://bkl.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://xen.dashuyun.cn

Ruby: // 手写 Hash
来源：http://khf.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://acn.ctjpmb.com

[N08] 生成全排列
来源：http://yhk.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://nwp.redwolf501.top

PHP:  // 手写递归交换
来源：http://mfv.iojbl.cn

JS:   // 手写回溯递归
来源：http://qbv.yuxming.cn

TS:   // 手写回溯递归
来源：http://kbt.gaohongyu789.top

Java: // 手写回溯递归
来源：http://ocj.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://zzh.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://omy.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://vfo.haohaochexian.top

[N09] 栈与队列
来源：http://ifw.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zkd.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdj.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ejv.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tdu.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dvp.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://egd.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ssg.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sux.aibaodan.cn

[N10] 链表节点定义
来源：http://neo.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ule.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eej.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dgp.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qwg.316326.xyz

Java: class Node { int v; Node next; }
来源：http://tnr.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ddr.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://msm.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://shw.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://eiv.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zbu.andypj.xyz

PHP:  // 手写递归函数
来源：http://czn.kuanghao11.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zvj.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqw.wangshuangyany.cn

Java: // 手写递归
来源：http://qie.hnqzz.top

Go:   // 手写递归
来源：http://ubo.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eli.jiagoushi.top

C#:   // 手写递归
来源：http://tjn.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dwb.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://otz.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mtp.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fyo.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://plc.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fnh.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xts.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vhn.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nnf.aizwys.cn

================================================================================
来源：http://dkj.svipenyu.cn

O. 并发与异步
来源：http://dfs.havefunace.top

================================================================================
来源：http://zjl.mhx1999.top

[O01] 启动一个线程
来源：http://rhr.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mgi.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dbo.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gza.c1oappe.top

TS:   // 同 JS
来源：http://qrh.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://jod.snrcjt.cn

Go:   go f()
来源：http://rhh.cucudq.cn

Ruby: Thread.new { f }
来源：http://vrq.52xcode.cn

C#:   Task.Run(() => F());
来源：http://gwn.cdnleiting.top

[O02] 使用线程池
来源：http://ipf.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oqa.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bxk.hesvh.cn

JS:   // worker_threads 线程池
来源：http://eoa.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://slr.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://nqc.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tpe.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bel.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lty.andypj.xyz

[O03] 加锁保护共享数据
来源：http://eao.fzhhl.top

Py:   with lock: shared += 1
来源：http://cev.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://qua.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bmf.hnqzz.top

TS:   // 同 JS
来源：http://oah.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://nec.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://knu.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wpl.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://owt.cashguo.top

[O04] 定义异步函数并等待
来源：http://uyi.uphjek.com

Py:   async def f():⏎    await g()
来源：http://key.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aav.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://vjn.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dbc.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://scs.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://szo.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://shm.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://mak.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://ezu.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://wzx.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hcr.yongpay.top

JS:   await Promise.all(tasks)
来源：http://fce.tanke756.top

TS:   await Promise.all(tasks)
来源：http://dda.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbv.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qne.havefunace.top

Ruby: threads.map(&:join)
来源：http://frg.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ocz.ehwqpu.com

[O06] 使用进程池
来源：http://kfr.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ins.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://xtv.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://evf.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://zlt.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://auk.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hwk.hongshengwenyu.top

Ruby: // fork 块
来源：http://uwt.gaohongyu789.top

C#:   Parallel.For
来源：http://nzj.ydzc1.top

================================================================================
来源：http://egp.yongpay.top

P. 常用工具函数
来源：http://hft.tanke756.top

================================================================================
来源：http://ifq.zhongyouzk.top

[P01] 生成 UUID
来源：http://vck.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://xwe.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vzj.ivvv.top

JS:   crypto.randomUUID()
来源：http://mcm.shuidangran.top

TS:   crypto.randomUUID()
来源：http://dde.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://cce.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://oks.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://tqn.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://xkm.zhixingplan.top

[P02] MD5 / SHA256 摘要
来源：http://rvs.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygd.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xoe.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eak.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dfc.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kfe.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ull.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qer.shanyushiyangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nfx.xylfe.cn

[P03] 生成短随机字符串
来源：http://nvg.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://idz.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vgz.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxi.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wdn.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ypf.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kak.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dbi.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://osi.bbcook.cn

[P04] 求长度
来源：http://ylp.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iye.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzf.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xbx.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qps.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://zxn.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://dyu.redwolf501.top

Ruby: x.length;  x.size
来源：http://hxy.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ffx.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://hiy.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://npj.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mbq.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://byn.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zem.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ycb.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://gee.yueranfly.top

Ruby: a == b
来源：http://zkj.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lwg.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xuq.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tox.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://sum.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kkh.xuanzx.com

TS:   if (x == null) {}
来源：http://cuh.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zsp.zhixingplan.top

Go:   if x == nil {}
来源：http://plg.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ghv.yvedp.cn

C#:   if (x is null) {}
来源：http://sjk.yonumen.top

[P07] 防抖与节流
来源：http://vcw.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wsj.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://quc.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcs.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcw.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ema.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tex.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://itx.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://smr.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://ayx.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rbs.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uuh.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fec.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fxq.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zky.sufxvd.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hdr.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hsm.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kbt.hysaishi.cn

================================================================================
来源：http://qmt.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hgr.yj202588.top

================================================================================
来源：http://lkz.vqdsnc.cn

[Q01] 创建表
来源：http://woa.bjfxy.top

CREATE TABLE users (
来源：http://fwq.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sfo.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://rra.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://fmh.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jcu.meibo888.top

);
来源：http://dij.316326.xyz

[Q02] 创建带外键的表
来源：http://zxz.zhiwuduotai.top

CREATE TABLE orders (
来源：http://hpf.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tjw.andypj.xyz

user_id INT NOT NULL,
来源：http://zat.jianghu66.top

amount DECIMAL(10, 2),
来源：http://mdm.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://moe.shangyingyoupin.top

);
来源：http://gqn.c1oappe.top

[Q03] 增加列
来源：http://gzi.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cbk.yvedp.cn

[Q04] 修改列类型
来源：http://mzz.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qrw.ehwqpu.com

[Q05] 重命名列
来源：http://gdo.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yus.nwbrower.top

[Q06] 删除列
来源：http://kqs.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jrv.sysykeji.top

[Q07] 删除表
来源：http://czb.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://hqs.vehdjk.com

[Q08] 创建普通索引
来源：http://oqu.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eai.sweek.top

[Q09] 创建唯一索引
来源：http://rzf.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nra.jlsjyb.cn

[Q10] 插入单行
来源：http://jkl.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hva.yonumen.top

[Q11] 一次插入多行
来源：http://efw.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://upb.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://suw.gotoacloud.top


<!-- 参考信息 -->