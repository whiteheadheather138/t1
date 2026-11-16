代发 wailian999

Ruby: exit 1
来源：http://fcm.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cgb.shzxlz.cn

[M06] 向标准错误输出
来源：http://sbn.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://cyk.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://efz.haohaochexian.top

JS:   console.error("err")
来源：http://vnc.zhengqikj.top

TS:   console.error("err")
来源：http://peh.havefunace.top

Java: System.err.println("err")
来源：http://mkw.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nll.birdmap.top

Ruby: warn "err"
来源：http://rbn.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://pfo.sweek.top

[M07] 判断是否为主入口
来源：http://rlo.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://rsy.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qpa.zycfv.cn

JS:   require.main === module
来源：http://eey.0kj1m.cn

TS:   require.main === module
来源：http://wov.sufxvd.cn

Java: public static void main(String[] args)
来源：http://urt.xingfuxueyuan.xyz

Go:   func main()
来源：http://cux.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cxc.cheryme.top

C#:   static void Main(string[] args)
来源：http://sov.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://kds.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://qti.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://uqb.jyoumei.cn

JS:   process.platform;  process.version
来源：http://mbu.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://adp.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ugc.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://soy.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ydz.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://owk.cheryme.top

================================================================================
来源：http://nmd.redwolf501.top

N. 数据结构与算法
来源：http://nil.xuetiantiany.cn

================================================================================
来源：http://xcw.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://jkx.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ukt.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qeu.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gkb.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdz.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://isc.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://ajq.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://gqz.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://sot.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://hav.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://osx.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ouk.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hri.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gow.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://byg.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://nro.hcnkem.com

Ruby: arr.sort
来源：http://uau.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://egd.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://ehu.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mso.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://mmd.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tcn.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnv.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uui.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tak.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fps.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://thf.hfpthk.cn

[N04] 斐波那契数列
来源：http://hew.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gtr.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vnj.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozz.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oxo.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zpl.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sax.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ram.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xqo.uphjek.com

[N05] 最大公约数
来源：http://wik.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://dqt.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://drq.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmc.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffz.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xqr.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vay.gogol.net.cn

Ruby: a.gcd(b)
来源：http://tuo.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://igv.jqgfzy.top

[N06] 判断回文字符串
来源：http://mcp.yj202588.top

Py:   s == s[::-1]
来源：http://zbh.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://zzz.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://ddk.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://qfo.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yht.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://mus.fktsv.cn

Ruby: s == s.reverse
来源：http://zfr.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://chw.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://hrt.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qxg.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kbn.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ctp.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://qpn.ppjwa.cn

Java: // 手写 HashMap
来源：http://xfn.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://csn.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://gvy.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://udu.jlsjyb.cn

[N08] 生成全排列
来源：http://brp.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://lwe.hnqzz.top

PHP:  // 手写递归交换
来源：http://fcl.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://vnm.zdbjq.cn

TS:   // 手写回溯递归
来源：http://tfl.jinqigfzy.top

Java: // 手写回溯递归
来源：http://yof.hnqzz.top

Go:   // 手写回溯递归
来源：http://obz.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://ihd.guannengcc.top

C#:   // 手写回溯递归
来源：http://fnf.xinyue.icu

[N09] 栈与队列
来源：http://zdl.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yjc.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cxy.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hum.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pkg.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uat.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zpa.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://suv.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baw.xuanzx.com

[N10] 链表节点定义
来源：http://ctt.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sym.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nsg.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sca.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://izw.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://tmy.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://lqv.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pxt.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://xcp.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://eui.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rkd.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://nce.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vua.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fky.yfazqb.com

Java: // 手写递归
来源：http://fjr.cqqwz.cn

Go:   // 手写递归
来源：http://tmh.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dsw.gzhubu.top

C#:   // 手写递归
来源：http://fwo.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dff.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rqa.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qxq.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cdu.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://num.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aqf.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://boj.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fdp.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://urc.jqgfzy.top

================================================================================
来源：http://zyi.hfpthk.cn

O. 并发与异步
来源：http://ayc.ehwqpu.com

================================================================================
来源：http://ghk.jiagoushi.top

[O01] 启动一个线程
来源：http://fpj.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ikx.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ivd.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://shp.tanke756.top

TS:   // 同 JS
来源：http://idr.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://sje.fktsv.cn

Go:   go f()
来源：http://ivd.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://wcr.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://zna.tian-w.cn

[O02] 使用线程池
来源：http://zso.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://twv.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gzj.xziqi.cn

JS:   // worker_threads 线程池
来源：http://hpg.gzhubu.top

TS:   // worker_threads 线程池
来源：http://anq.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://cug.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vql.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lky.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xhs.shuidangran.top

[O03] 加锁保护共享数据
来源：http://lqj.jianghu66.top

Py:   with lock: shared += 1
来源：http://uwo.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cxh.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vox.zhiwuduotai.top

TS:   // 同 JS
来源：http://bgh.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://shz.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tyt.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gah.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://nnx.yongpay.top

[O04] 定义异步函数并等待
来源：http://gfs.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://erl.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dcl.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://did.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://agh.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gvv.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wot.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kmr.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://sec.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://jfj.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://yrn.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://idk.tarul.cn

JS:   await Promise.all(tasks)
来源：http://jap.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://kxo.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xmj.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjs.hammf.cn

Ruby: threads.map(&:join)
来源：http://jmm.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mxi.tian-w.cn

[O06] 使用进程池
来源：http://zkh.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wun.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ipb.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://stq.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://odt.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dil.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zld.guannengcc.top

Ruby: // fork 块
来源：http://iwd.wangshuangyany.cn

C#:   Parallel.For
来源：http://qpi.pycfn.com

================================================================================
来源：http://hrd.bbcook.cn

P. 常用工具函数
来源：http://wvv.iojbl.cn

================================================================================
来源：http://uae.zhongyouzk.top

[P01] 生成 UUID
来源：http://vsc.yongpay.top

Py:   str(uuid.uuid4())
来源：http://tzg.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://taj.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://wcj.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://vpd.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://hzg.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://iig.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://pka.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://nls.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://niy.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zcz.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hyx.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ovv.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fwt.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eal.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xxk.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ona.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hgu.cdnleiting.top

[P03] 生成短随机字符串
来源：http://psm.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cko.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vmg.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xyu.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vkw.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zis.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ovv.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zzd.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lkv.nanxuanxn.top

[P04] 求长度
来源：http://hss.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cnw.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zvq.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rnp.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://elc.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://jyv.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://vsf.sysykeji.top

Ruby: x.length;  x.size
来源：http://gdv.vehdjk.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mwi.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://obw.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://toh.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kjl.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dsv.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qki.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qhc.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ykz.shanyushiyangtech.top

Ruby: a == b
来源：http://mge.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xox.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xql.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xlp.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://ixe.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cjk.guannengcc.top

TS:   if (x == null) {}
来源：http://sko.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xlq.haohaochexian.top

Go:   if x == nil {}
来源：http://bav.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mho.yongpay.top

C#:   if (x is null) {}
来源：http://qhm.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://kyp.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ogz.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://nkd.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://elv.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndp.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fex.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fhi.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kur.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vgy.yueranfly.top

[P08] 处理浮点精度问题
来源：http://dcr.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eup.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oot.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xaf.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://apc.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hni.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://skx.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hkd.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://syx.hfpthk.cn

================================================================================
来源：http://vqi.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ttz.jqgufenzy.top

================================================================================
来源：http://dmn.sysykeji.top

[Q01] 创建表
来源：http://cdn.andypj.xyz

CREATE TABLE users (
来源：http://zti.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sqr.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://ffm.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://mca.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://khi.zhijiandao.cn

);
来源：http://byg.yongpay.top

[Q02] 创建带外键的表
来源：http://hyl.zhijiandao.cn

CREATE TABLE orders (
来源：http://rss.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://deo.dashuyun.cn

user_id INT NOT NULL,
来源：http://ebh.hnqzz.top

amount DECIMAL(10, 2),
来源：http://kiq.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zyc.smart0.xyz

);
来源：http://xdt.feifeiyinyue.top

[Q03] 增加列
来源：http://uzg.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://llo.cashguo.top

[Q04] 修改列类型
来源：http://fmj.dashuyun.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cuj.zdqjudy.top

[Q05] 重命名列
来源：http://lyb.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqc.fktsv.cn

[Q06] 删除列
来源：http://gnn.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://wsx.birdmap.top

[Q07] 删除表
来源：http://wkg.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://yaj.jiagoushi.top

[Q08] 创建普通索引
来源：http://dwl.jianghu66.top


<!-- 参考信息 -->