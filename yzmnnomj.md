代发 wailian999

Py:   if __name__ == "__main__":
来源：http://qaj.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ufr.tianlin.xyz

JS:   require.main === module
来源：http://lqj.daxiang520.top

TS:   require.main === module
来源：http://xoc.ydzc1.top

Java: public static void main(String[] args)
来源：http://tsc.chenlongwang.top

Go:   func main()
来源：http://tap.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://loh.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://lpz.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://rsy.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://cgz.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://qdr.fzhhl.top

JS:   process.platform;  process.version
来源：http://gjj.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://rfr.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rox.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://amj.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ckw.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ufm.bjfxy.top

================================================================================
来源：http://ywi.fanxiaobao.xyz

N. 数据结构与算法
来源：http://ill.zhiwuduotai.top

================================================================================
来源：http://khr.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://dtl.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://hxy.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jjy.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tvp.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hek.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://acr.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://ilp.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://blh.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qmb.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://dfg.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ssu.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drn.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vct.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vfn.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mca.shuidangran.top

Go:   slices.Sort(arr)
来源：http://vfw.hesvh.cn

Ruby: arr.sort
来源：http://fwx.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vjy.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://pqw.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pyp.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://usm.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mta.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elo.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://omg.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yho.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zqu.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mol.hammf.cn

[N04] 斐波那契数列
来源：http://vrw.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pcl.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yup.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bfl.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fjl.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qvg.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ags.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://shr.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gkg.shangyingyoupin.top

[N05] 最大公约数
来源：http://duh.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://xew.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eqj.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nuw.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmo.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bcl.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avf.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://dbq.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pkm.meibo888.top

[N06] 判断回文字符串
来源：http://iug.ybcxt.top

Py:   s == s[::-1]
来源：http://zoi.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://eug.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://vnq.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://abn.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ixc.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://uex.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://ksl.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lnl.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://uew.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gez.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sar.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ega.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://tdj.jinqigufen.top

Java: // 手写 HashMap
来源：http://mbo.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://jyn.jinqigufen.top

Ruby: // 手写 Hash
来源：http://wzz.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://zis.chenlongwang.top

[N08] 生成全排列
来源：http://hku.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://wny.xuanzx.com

PHP:  // 手写递归交换
来源：http://vul.haohaochexian.top

JS:   // 手写回溯递归
来源：http://gyf.epnwcf.com

TS:   // 手写回溯递归
来源：http://xxs.fktsv.cn

Java: // 手写回溯递归
来源：http://jkf.c1oappe.top

Go:   // 手写回溯递归
来源：http://aqk.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://tkn.sweek.top

C#:   // 手写回溯递归
来源：http://nmo.xuetiantiany.cn

[N09] 栈与队列
来源：http://fky.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gva.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ksw.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://thr.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gzg.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sia.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gou.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yzp.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jat.zhijiandao.cn

[N10] 链表节点定义
来源：http://iuu.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://unv.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://omt.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aku.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dyb.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://irx.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://bwx.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yxq.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qdn.yj20258888.top

[N11] 二叉树中序遍历
来源：http://xfm.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qij.haohaochexian.top

PHP:  // 手写递归函数
来源：http://wly.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qvl.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmb.cdnleiting.top

Java: // 手写递归
来源：http://fig.tanke756.top

Go:   // 手写递归
来源：http://jmc.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pcm.hcnkem.com

C#:   // 手写递归
来源：http://lbt.ivvv.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oal.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wii.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xte.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gyd.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fnh.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sea.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dwl.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yab.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cjq.shanyushiyangkeji.top

================================================================================
来源：http://gip.cucudq.cn

O. 并发与异步
来源：http://cba.zycfv.cn

================================================================================
来源：http://elw.sjlbkw.cn

[O01] 启动一个线程
来源：http://bjo.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ogs.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kbv.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ptx.fehbvm.com

TS:   // 同 JS
来源：http://sif.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://yxm.ivvv.top

Go:   go f()
来源：http://iam.jinqigufen.top

Ruby: Thread.new { f }
来源：http://wfh.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://qri.aizwys.cn

[O02] 使用线程池
来源：http://xas.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lzf.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xoa.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://jrg.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://jzq.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vip.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iia.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vyd.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://txt.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://jpu.tarul.cn

Py:   with lock: shared += 1
来源：http://eqa.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://tbd.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vod.zdbjq.cn

TS:   // 同 JS
来源：http://ycz.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://vyh.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bme.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://iir.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://hke.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://vkh.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://tiq.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rim.mhx1999.top

JS:   async function f() { await g(); }
来源：http://cqy.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sxi.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dvq.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mpu.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lbc.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://cvm.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://rsx.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://ack.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mic.yongpay.top

JS:   await Promise.all(tasks)
来源：http://ckf.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://jpf.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pae.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uae.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://sfc.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cov.shanyushiyangtech.top

[O06] 使用进程池
来源：http://slo.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ivi.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://pfy.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://aci.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://wda.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://apg.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dav.iojbl.cn

Ruby: // fork 块
来源：http://rnb.yuanzhike.top

C#:   Parallel.For
来源：http://ago.nanxuanxn.top

================================================================================
来源：http://mji.yonumen.top

P. 常用工具函数
来源：http://ojg.daxiang520.top

================================================================================
来源：http://lgm.yueranfly.top

[P01] 生成 UUID
来源：http://pyh.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://qrx.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wbv.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://zfs.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://azz.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://isu.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://ltg.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://wfc.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://izp.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://hxd.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jwo.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://wcx.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kxs.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uyu.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mws.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jmx.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kuw.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://apd.xylfe.cn

[P03] 生成短随机字符串
来源：http://hfe.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vlv.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gpt.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xjz.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kso.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://owx.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mta.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wsl.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://alw.yangfankeji.com

[P04] 求长度
来源：http://cxk.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uta.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apz.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aed.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zbg.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://lyj.xziqi.cn

Go:   len(arr);  len(m)
来源：http://bno.redwolf501.top

Ruby: x.length;  x.size
来源：http://szj.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jwn.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://aqz.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://fpy.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ijm.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jbi.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bih.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oyh.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mmr.kuanghao11.cn

Ruby: a == b
来源：http://cek.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://feh.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xrn.hammf.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sui.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://dww.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wsq.redwolf501.top

TS:   if (x == null) {}
来源：http://zoj.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://unv.xinyue.icu

Go:   if x == nil {}
来源：http://xle.daria6918.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uho.xziqi.cn

C#:   if (x is null) {}
来源：http://tfp.haohaochexian.top

[P07] 防抖与节流
来源：http://dcz.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vst.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://jmc.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxh.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztq.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tak.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://foo.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oyo.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ccz.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://iag.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wxv.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ort.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://djo.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mip.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zja.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qmi.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yzv.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ocu.hesvh.cn

================================================================================
来源：http://zjb.shanyushiyangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jpa.wangdashe.top

================================================================================
来源：http://fig.jianghu66.top

[Q01] 创建表
来源：http://ecr.tanke756.top

CREATE TABLE users (
来源：http://jqc.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zxq.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://tsz.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://psp.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mxa.xuanzx.com

);
来源：http://gjb.sxryk.cn

[Q02] 创建带外键的表
来源：http://llc.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://axo.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvv.meibo888.top

user_id INT NOT NULL,
来源：http://pgb.yfazqb.com

amount DECIMAL(10, 2),
来源：http://uvm.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jsc.ywan-chungtsiang.top

);
来源：http://hkn.birdmap.top

[Q03] 增加列
来源：http://ieb.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gly.jianghu66.top

[Q04] 修改列类型
来源：http://cbd.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aop.nwbrower.top

[Q05] 重命名列
来源：http://fpt.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hek.pengpengdd.cyou

[Q06] 删除列
来源：http://bgc.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://dpw.yuxming.cn

[Q07] 删除表
来源：http://hch.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://yjh.snrcjt.cn

[Q08] 创建普通索引
来源：http://zlo.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yre.52xcode.cn

[Q09] 创建唯一索引
来源：http://lgb.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rdn.zhoulong.xyz

[Q10] 插入单行
来源：http://vmx.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://slk.jianghu66.top

[Q11] 一次插入多行
来源：http://soq.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eyv.meibo888.top

[Q12] 插入后取自增 ID
来源：http://yju.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://pyt.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ubt.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://bcx.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pfg.0kj1m.cn


<!-- 参考信息 -->