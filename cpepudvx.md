代发 wailian999

Java: public static void main(String[] args)
来源：http://ugq.zhoulong.xyz

Go:   func main()
来源：http://ntm.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cja.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://del.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://acp.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://veo.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://kuc.mhx1999.top

JS:   process.platform;  process.version
来源：http://wai.xinyue.icu

TS:   process.platform;  process.version
来源：http://gxv.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sik.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vxr.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sbe.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hcl.zhixingplan.top

================================================================================
来源：http://qvx.zdbjq.cn

N. 数据结构与算法
来源：http://lwr.havefunace.top

================================================================================
来源：http://noa.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://jrg.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hfa.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vww.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fvt.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fmt.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://lrc.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://sxt.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bjv.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://dus.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://eyh.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://ahm.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yws.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ujz.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://kzv.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cpg.yj202588.top

Go:   slices.Sort(arr)
来源：http://oig.nanxinkj.top

Ruby: arr.sort
来源：http://ntc.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lsc.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://utq.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://azt.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://yug.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uey.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://moo.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oiu.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://esh.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bbv.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tkf.snrcjt.cn

[N04] 斐波那契数列
来源：http://usw.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pfs.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tmu.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://maz.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rrg.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jvl.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kus.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lbw.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ioa.gaohongyu789.top

[N05] 最大公约数
来源：http://vde.hesvh.cn

Py:   math.gcd(a, b)
来源：http://zep.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wsu.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvm.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ljd.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hqq.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dmf.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://xcn.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ono.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://uus.52xcode.cn

Py:   s == s[::-1]
来源：http://whp.sysykeji.top

PHP:  $s === strrev($s);
来源：http://cse.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://opd.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://kws.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cuj.xinyue.icu

Go:   // 双指针从两端比较
来源：http://tbw.yonumen.top

Ruby: s == s.reverse
来源：http://kst.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gfo.uphjek.com

[N07] 两数之和（返回下标）
来源：http://omk.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://enw.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pql.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://npk.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://uub.0kj1m.cn

Java: // 手写 HashMap
来源：http://reb.aizwys.cn

Go:   // 手写 map[int]int
来源：http://lqi.yuanzhike.top

Ruby: // 手写 Hash
来源：http://aha.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://lfh.jinghuilouyu.cn

[N08] 生成全排列
来源：http://gug.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://nhv.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://jmy.guowangkeji.top

JS:   // 手写回溯递归
来源：http://lff.meibo888.top

TS:   // 手写回溯递归
来源：http://rlc.cdnleiting.top

Java: // 手写回溯递归
来源：http://wjh.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://eoa.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://kap.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://ode.yongpay.top

[N09] 栈与队列
来源：http://fuz.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yyx.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qsh.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pfg.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iwe.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iqe.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://agx.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rne.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yzz.chenjidiqi.icu

[N10] 链表节点定义
来源：http://ehm.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hin.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://dil.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gad.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jeh.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://wxw.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qmr.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hsr.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fgo.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://sgb.daxiang520.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xvp.yj20258.top

PHP:  // 手写递归函数
来源：http://joo.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oes.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bpy.chenlongwang.top

Java: // 手写递归
来源：http://ldg.hongshengwenyu.top

Go:   // 手写递归
来源：http://rnp.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aqy.havefunace.top

C#:   // 手写递归
来源：http://omf.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vsi.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://knn.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nfu.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgr.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wdk.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tqz.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://flu.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://erc.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gec.fanxiaobao.xyz

================================================================================
来源：http://zds.yfazqb.com

O. 并发与异步
来源：http://acf.quarkkingdee.top

================================================================================
来源：http://lzv.vqdsnc.cn

[O01] 启动一个线程
来源：http://pro.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://asi.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rsc.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jds.zdqjudy.top

TS:   // 同 JS
来源：http://yxm.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://fzj.tanke756.top

Go:   go f()
来源：http://rxm.sysykeji.top

Ruby: Thread.new { f }
来源：http://dzy.wangdashe.top

C#:   Task.Run(() => F());
来源：http://arq.fanxiaobao.xyz

[O02] 使用线程池
来源：http://txu.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://maw.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fzh.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://tpu.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://omn.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://etf.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wrv.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lfv.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ypt.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://ukp.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://dtf.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://kuq.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vcn.wangdashe.top

TS:   // 同 JS
来源：http://ysw.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://rmj.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rta.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nta.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://tst.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://euy.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://tqz.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tfv.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://aae.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nxj.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sux.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ylc.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://wki.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://bvf.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://lwn.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://tko.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ien.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://amj.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://spm.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wxz.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mrg.xinyue.icu

Ruby: threads.map(&:join)
来源：http://ihb.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://kfb.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://buv.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://njc.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zvk.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://cag.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://eys.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oyh.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lov.c1oappe.top

Ruby: // fork 块
来源：http://gda.yuanzhike.top

C#:   Parallel.For
来源：http://iks.fktsv.cn

================================================================================
来源：http://qtq.redwolf501.top

P. 常用工具函数
来源：http://wyl.sufxvd.cn

================================================================================
来源：http://kam.nwbrower.top

[P01] 生成 UUID
来源：http://mib.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://sac.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qfp.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://dnf.xuanzx.com

TS:   crypto.randomUUID()
来源：http://cpq.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://hbf.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://ldf.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://clz.hfpthk.cn

C#:   Guid.NewGuid().ToString()
来源：http://joy.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://tez.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ndf.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dms.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nvu.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ysr.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xtl.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iia.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hdc.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ggc.chenzaomai.com

[P03] 生成短随机字符串
来源：http://kao.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ggk.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://toe.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://krf.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhl.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ddr.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://isk.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ybj.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qks.guowangkeji.top

[P04] 求长度
来源：http://fvl.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vch.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dcz.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vpi.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frr.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://snr.aizwys.cn

Go:   len(arr);  len(m)
来源：http://svp.yuanzhike.top

Ruby: x.length;  x.size
来源：http://kvg.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yni.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://mvy.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kwu.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gmm.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tax.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zdk.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://szc.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nzi.nwbrower.top

Ruby: a == b
来源：http://afm.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bqo.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jwi.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vbd.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://bmy.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kvk.xinyue.icu

TS:   if (x == null) {}
来源：http://jgp.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pgk.dashuyun.cn

Go:   if x == nil {}
来源：http://poz.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gks.kuanghao11.cn

C#:   if (x is null) {}
来源：http://jkf.zhiwuduotai.top

[P07] 防抖与节流
来源：http://jbw.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bjn.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://wwn.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ayq.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixv.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wrd.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wez.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qpa.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zsu.yonumen.top

[P08] 处理浮点精度问题
来源：http://exq.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ate.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jii.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bcp.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jsg.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wib.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zsh.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xqj.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ilb.shanyushiyangtech.top

================================================================================
来源：http://rkb.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iap.ppjwa.cn

================================================================================
来源：http://psk.cashguo.top

[Q01] 创建表
来源：http://qvn.fktsv.cn

CREATE TABLE users (
来源：http://uxv.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ocj.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://xwp.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://wmo.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sll.yanxiufei.cn

);
来源：http://paw.iojbl.cn

[Q02] 创建带外键的表
来源：http://cjj.kuanghao11.cn

CREATE TABLE orders (
来源：http://qdh.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hoi.havefunace.top

user_id INT NOT NULL,
来源：http://twq.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://wbj.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qoz.zycfv.cn

);
来源：http://exy.cucudq.cn

[Q03] 增加列
来源：http://voh.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lnm.ydzc1.top

[Q04] 修改列类型
来源：http://oux.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wfe.jinqigufen.top

[Q05] 重命名列
来源：http://xtk.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ilg.vqdsnc.cn

[Q06] 删除列
来源：http://rmf.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://qnn.zhijiandao.cn

[Q07] 删除表
来源：http://hwr.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://imd.ybcxt.top

[Q08] 创建普通索引
来源：http://cfk.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mdz.svipenyu.cn

[Q09] 创建唯一索引
来源：http://azf.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sye.daria6918.cn

[Q10] 插入单行
来源：http://gfy.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hfk.zhoulong.xyz

[Q11] 一次插入多行
来源：http://lvu.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iga.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://wyh.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://nmf.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rot.guowangkeji.top

[Q13] 忽略重复插入
来源：http://rez.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ufl.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://spp.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lzx.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yro.yj202588.top

[Q15] 查询全部
来源：http://zyp.jqgfzy.top


<!-- 参考信息 -->