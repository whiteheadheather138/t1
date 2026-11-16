代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://qya.fengsongda.top

JS:   console.error("err")
来源：http://ebj.cdnleiting.top

TS:   console.error("err")
来源：http://tdz.guowangkeji.top

Java: System.err.println("err")
来源：http://obp.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ski.sjlbkw.cn

Ruby: warn "err"
来源：http://wqw.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://sqk.epnwcf.com

[M07] 判断是否为主入口
来源：http://gmk.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://zit.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hkg.hysaishi.cn

JS:   require.main === module
来源：http://gyw.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://bzr.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://zik.sweek.top

Go:   func main()
来源：http://phf.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://agr.cheryme.top

C#:   static void Main(string[] args)
来源：http://bvk.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://gxy.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://med.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vkr.ctjpmb.com

JS:   process.platform;  process.version
来源：http://gmd.guannengcc.top

TS:   process.platform;  process.version
来源：http://ucy.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jod.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyt.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pvz.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jen.kuanghao11.cn

================================================================================
来源：http://ogr.ctjpmb.com

N. 数据结构与算法
来源：http://jyx.mhx1999.top

================================================================================
来源：http://zpp.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://xkm.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nst.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qei.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwq.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgg.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://umn.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://csl.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://snb.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://ijj.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://gbg.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://ijm.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iul.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fld.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rry.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uyu.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://bqq.zhixingplan.top

Ruby: arr.sort
来源：http://hzx.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ivf.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://kbr.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mya.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://hzg.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzr.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dua.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iqf.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ifh.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kuo.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://aem.tianlin.xyz

[N04] 斐波那契数列
来源：http://atd.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://amv.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dfs.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmx.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ide.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jba.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bsn.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://stb.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zwf.jyoumei.cn

[N05] 最大公约数
来源：http://xbr.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://sbt.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xxz.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gss.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbp.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vjr.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nam.sweek.top

Ruby: a.gcd(b)
来源：http://rut.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://owk.xinyue.icu

[N06] 判断回文字符串
来源：http://vyp.cucudq.cn

Py:   s == s[::-1]
来源：http://aqx.bjfxy.top

PHP:  $s === strrev($s);
来源：http://izw.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://obr.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://qil.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mdj.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://jwk.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://orr.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dav.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://euk.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ufo.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xcr.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qqp.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://phr.zhijiandao.cn

Java: // 手写 HashMap
来源：http://omw.hnqzz.top

Go:   // 手写 map[int]int
来源：http://yie.c1oappe.top

Ruby: // 手写 Hash
来源：http://rok.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://vde.pycfn.com

[N08] 生成全排列
来源：http://hki.birdmap.top

Py:   itertools.permutations(arr)
来源：http://hzi.ehwqpu.com

PHP:  // 手写递归交换
来源：http://qhf.hammf.cn

JS:   // 手写回溯递归
来源：http://hra.vehdjk.com

TS:   // 手写回溯递归
来源：http://vsn.mhx1999.top

Java: // 手写回溯递归
来源：http://ykt.chenzaomai.com

Go:   // 手写回溯递归
来源：http://tgb.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://jxr.wangdashe.top

C#:   // 手写回溯递归
来源：http://ick.ybcxt.top

[N09] 栈与队列
来源：http://lyu.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ypr.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jni.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bzr.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvn.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qqm.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qxo.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://weq.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ufd.pycfn.com

[N10] 链表节点定义
来源：http://dpz.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://noc.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://heu.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nzi.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qqs.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://djm.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kbd.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vtq.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yie.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://ekw.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://azc.yuanzhike.top

PHP:  // 手写递归函数
来源：http://otr.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tfc.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xnm.jianghu66.top

Java: // 手写递归
来源：http://lgd.yanxiufei.cn

Go:   // 手写递归
来源：http://uxs.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xdq.shuidangran.top

C#:   // 手写递归
来源：http://piz.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uhs.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dke.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://juo.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ckz.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vie.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aex.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vvs.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fsi.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nzd.yonumen.top

================================================================================
来源：http://wcw.chenjidiqi.icu

O. 并发与异步
来源：http://vvs.jinqigfzy.top

================================================================================
来源：http://wdp.316326.xyz

[O01] 启动一个线程
来源：http://hgs.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjj.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mue.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sfo.cucudq.cn

TS:   // 同 JS
来源：http://vnt.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://cdx.svipenyu.cn

Go:   go f()
来源：http://nje.redwolf501.top

Ruby: Thread.new { f }
来源：http://zkw.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://alx.tanke756.top

[O02] 使用线程池
来源：http://rqx.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eed.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ipp.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://suy.sxryk.cn

TS:   // worker_threads 线程池
来源：http://xow.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://vje.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ozn.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://edf.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rvw.aizwys.cn

[O03] 加锁保护共享数据
来源：http://aws.xinyue.icu

Py:   with lock: shared += 1
来源：http://cjn.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://cqj.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ijh.ctjpmb.com

TS:   // 同 JS
来源：http://lbq.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://ssu.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fgd.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://esr.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://vmp.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://nat.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://gmj.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iuq.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://gtg.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kco.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dzp.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://irh.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://fpe.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://wry.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://nze.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://fxb.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ujx.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://blf.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://mna.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xrm.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mkw.bbcook.cn

Ruby: threads.map(&:join)
来源：http://qkm.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://huc.yongpay.top

[O06] 使用进程池
来源：http://oai.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uxu.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kiy.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://tpj.sweek.top

TS:   // child_process / cluster 模块
来源：http://poe.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iqj.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://spz.havefunace.top

Ruby: // fork 块
来源：http://jkk.uphjek.com

C#:   Parallel.For
来源：http://iuc.cheryme.top

================================================================================
来源：http://waq.zhijiandao.cn

P. 常用工具函数
来源：http://ihi.birdmap.top

================================================================================
来源：http://pqv.svipenyu.cn

[P01] 生成 UUID
来源：http://ict.tarul.cn

Py:   str(uuid.uuid4())
来源：http://fub.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://muk.fktsv.cn

JS:   crypto.randomUUID()
来源：http://xwr.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://qsy.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://rxz.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://zft.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://csx.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://rwx.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://abe.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ajx.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dro.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jxm.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ydg.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://reo.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bqk.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wcb.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gbr.iojbl.cn

[P03] 生成短随机字符串
来源：http://zlq.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iau.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ljz.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tcw.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://crd.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yqe.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wrf.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hhz.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wrw.wangshuangyany.cn

[P04] 求长度
来源：http://tex.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://swb.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgc.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://srn.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qdm.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://sxu.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://ata.daxiang520.top

Ruby: x.length;  x.size
来源：http://arj.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wvy.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://cej.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lqx.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://azm.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kzl.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tyz.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://boi.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vkn.cheryme.top

Ruby: a == b
来源：http://wyj.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lei.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bcr.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mhv.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://zih.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zvp.sweek.top

TS:   if (x == null) {}
来源：http://tkg.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://jlp.feifeiyinyue.top

Go:   if x == nil {}
来源：http://ksk.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://prm.ydjk.org.cn

C#:   if (x is null) {}
来源：http://msb.xylfe.cn

[P07] 防抖与节流
来源：http://vgf.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lev.ivvv.top

PHP:  // 手写时间戳比较
来源：http://dsy.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijo.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ylj.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vyu.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cti.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lbm.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nlk.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://jhf.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rpm.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://asu.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kij.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cky.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oee.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iog.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tay.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://suh.ybcxt.top

================================================================================
来源：http://xfp.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivm.wangdashe.top

================================================================================
来源：http://bwu.hnxiangtu.top

[Q01] 创建表
来源：http://unz.tarul.cn

CREATE TABLE users (
来源：http://xag.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gfk.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://xbc.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://zxx.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://boe.tarul.cn

);
来源：http://gre.zhengqikj.top

[Q02] 创建带外键的表
来源：http://jzi.tianlin.xyz

CREATE TABLE orders (
来源：http://nmy.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://elf.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://vyv.cucudq.cn

amount DECIMAL(10, 2),
来源：http://btv.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bry.snrcjt.cn

);
来源：http://apj.zhijiandao.cn

[Q03] 增加列
来源：http://tda.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://laf.cucudq.cn

[Q04] 修改列类型
来源：http://zkj.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hit.hnxiangtu.top

[Q05] 重命名列
来源：http://rri.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rby.ivvv.top

[Q06] 删除列
来源：http://vrt.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://bhy.quarkkingdee.top

[Q07] 删除表
来源：http://fct.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://jxs.mhx1999.top

[Q08] 创建普通索引
来源：http://pvv.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xiw.guowangkeji.top

[Q09] 创建唯一索引
来源：http://nua.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mhx.ydzc1.top

[Q10] 插入单行
来源：http://lfh.jianghu66.top


<!-- 参考信息 -->