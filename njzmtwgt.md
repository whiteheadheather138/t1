代发 wailian999

Java: public static void main(String[] args)
来源：http://xyf.hammf.cn

Go:   func main()
来源：http://xmp.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wht.fehbvm.com

C#:   static void Main(string[] args)
来源：http://abg.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://jju.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://pyh.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://zdc.jianghu66.top

JS:   process.platform;  process.version
来源：http://cdw.9152youxi.cn

TS:   process.platform;  process.version
来源：http://nag.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vfy.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xdt.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fqb.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qfw.yueranfly.top

================================================================================
来源：http://tsv.dashuyun.cn

N. 数据结构与算法
来源：http://sov.quarkkingdee.top

================================================================================
来源：http://esd.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://pko.yangfankeji.com

Py:   bisect.bisect_left(arr, x)
来源：http://hlq.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cea.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oci.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ett.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://fkc.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://dwa.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ajf.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://odv.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://vxc.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ccd.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://klx.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qbh.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eri.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fzn.havefunace.top

Go:   slices.Sort(arr)
来源：http://umx.jlsjyb.cn

Ruby: arr.sort
来源：http://bxp.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpo.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://pvt.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://noa.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://xvw.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozw.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vxy.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kob.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wul.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wql.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://rab.gotoacloud.top

[N04] 斐波那契数列
来源：http://edy.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pci.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zmk.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zso.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://feh.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xzw.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xoh.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uud.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eef.zdqjudy.top

[N05] 最大公约数
来源：http://dqa.epnwcf.com

Py:   math.gcd(a, b)
来源：http://ugp.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eix.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sdv.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tcu.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wsf.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yca.c1oappe.top

Ruby: a.gcd(b)
来源：http://duk.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vgs.jqgufenzy.top

[N06] 判断回文字符串
来源：http://mom.quarkkingdee.top

Py:   s == s[::-1]
来源：http://gkw.sxryk.cn

PHP:  $s === strrev($s);
来源：http://int.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://nfz.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://llh.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sfh.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://woq.jianghu66.top

Ruby: s == s.reverse
来源：http://ose.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aqh.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://qdr.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vjg.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mpz.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://zyk.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://gvk.nanxinkj.top

Java: // 手写 HashMap
来源：http://uog.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://ows.aibaodan.cn

Ruby: // 手写 Hash
来源：http://qwj.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dxf.zhengqikj.top

[N08] 生成全排列
来源：http://qox.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://sxa.hcnkem.com

PHP:  // 手写递归交换
来源：http://ooy.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://ahq.jqgfzy.top

TS:   // 手写回溯递归
来源：http://iki.cqqwz.cn

Java: // 手写回溯递归
来源：http://nod.cheryme.top

Go:   // 手写回溯递归
来源：http://fom.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://mcb.cdnleiting.top

C#:   // 手写回溯递归
来源：http://mmk.kuanghao11.cn

[N09] 栈与队列
来源：http://oky.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ijn.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ayl.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fzf.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jhb.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://crp.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ear.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oik.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ihm.c1oappe.top

[N10] 链表节点定义
来源：http://apt.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ena.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://ttf.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://drp.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://njn.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://cjz.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://wvo.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ftv.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pkb.hammf.cn

[N11] 二叉树中序遍历
来源：http://qyj.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ben.guannengcc.top

PHP:  // 手写递归函数
来源：http://eax.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oim.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nhq.xziqi.cn

Java: // 手写递归
来源：http://naj.chenzaomai.com

Go:   // 手写递归
来源：http://kdb.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vvt.svipenyu.cn

C#:   // 手写递归
来源：http://hul.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eld.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sxc.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pao.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://woi.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gvh.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ley.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://szj.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://amx.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ivz.9152youxi.cn

================================================================================
来源：http://vpa.hysaishi.cn

O. 并发与异步
来源：http://jjn.fengsongda.top

================================================================================
来源：http://jlw.bbcook.cn

[O01] 启动一个线程
来源：http://dfq.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ixn.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kbt.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rzz.fzhhl.top

TS:   // 同 JS
来源：http://xmn.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://nhu.jlsjyb.cn

Go:   go f()
来源：http://apq.guannengcc.top

Ruby: Thread.new { f }
来源：http://abo.c1oappe.top

C#:   Task.Run(() => F());
来源：http://hmv.jyoumei.cn

[O02] 使用线程池
来源：http://mpy.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jmm.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wkg.havefunace.top

JS:   // worker_threads 线程池
来源：http://sal.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://kap.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://vlr.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cqf.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://smx.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rqq.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://rmc.jyoumei.cn

Py:   with lock: shared += 1
来源：http://odf.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://sdk.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aru.aibaodan.cn

TS:   // 同 JS
来源：http://ela.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://jse.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zsd.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eah.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://stv.52xcode.cn

[O04] 定义异步函数并等待
来源：http://psn.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://zzk.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rzu.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://tul.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://usn.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qii.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yhf.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://atr.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://pdc.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://sev.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://qtt.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tbt.meibo888.top

JS:   await Promise.all(tasks)
来源：http://cvw.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://nyq.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://juh.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bse.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://tyt.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yhp.fanxiaobao.xyz

[O06] 使用进程池
来源：http://cqd.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fub.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fxy.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://frp.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://esx.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iqe.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cwk.cdnleiting.top

Ruby: // fork 块
来源：http://ueg.uphjek.com

C#:   Parallel.For
来源：http://rkl.hysaishi.cn

================================================================================
来源：http://swq.hfpthk.cn

P. 常用工具函数
来源：http://ixf.sweek.top

================================================================================
来源：http://bno.smart0.xyz

[P01] 生成 UUID
来源：http://vww.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://ngm.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lmq.ivvv.top

JS:   crypto.randomUUID()
来源：http://etv.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://zlw.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://ppl.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://lkx.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://pxu.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://pel.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://nwx.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sbk.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ckq.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zng.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rlt.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mxn.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mgl.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmk.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kda.fengsongda.top

[P03] 生成短随机字符串
来源：http://xfv.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uhe.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uwy.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lxw.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrz.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ihh.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lpw.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sut.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://auz.zhiwuduotai.top

[P04] 求长度
来源：http://ywf.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vki.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbz.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dnz.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fzt.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://zcw.cheryme.top

Go:   len(arr);  len(m)
来源：http://byo.hcnkem.com

Ruby: x.length;  x.size
来源：http://bqp.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tmk.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://qim.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://snf.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://day.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ehi.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pgh.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dhp.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jfo.yongpay.top

Ruby: a == b
来源：http://iyq.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hlz.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://adx.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rfc.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://sng.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gmt.xinyue.icu

TS:   if (x == null) {}
来源：http://hsu.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://drr.ehwqpu.com

Go:   if x == nil {}
来源：http://lof.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://btk.hywenlv.cn

C#:   if (x is null) {}
来源：http://mpc.redwolf501.top

[P07] 防抖与节流
来源：http://hog.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nwr.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://aan.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fjq.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sug.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hwe.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lde.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://lus.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qee.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://pys.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ozv.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mqq.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fsb.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fma.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jtk.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://doo.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fjb.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nfy.vqdsnc.cn

================================================================================
来源：http://wje.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cgs.svipenyu.cn

================================================================================
来源：http://yil.nanxuanxn.top

[Q01] 创建表
来源：http://mzg.hesvh.cn

CREATE TABLE users (
来源：http://khx.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ghc.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://hxh.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://tjz.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kll.nwbrower.top

);
来源：http://nbd.9152youxi.cn

[Q02] 创建带外键的表
来源：http://wqj.zdbjq.cn

CREATE TABLE orders (
来源：http://bcv.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ivi.guannengcc.top

user_id INT NOT NULL,
来源：http://cef.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://aku.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jyw.hcnkem.com

);
来源：http://xir.shanyushiyangtech.top

[Q03] 增加列
来源：http://vxs.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ehp.0kj1m.cn

[Q04] 修改列类型
来源：http://bst.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uhh.c1oappe.top

[Q05] 重命名列
来源：http://vwo.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wqw.iojbl.cn

[Q06] 删除列
来源：http://smh.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://uag.hywenlv.cn

[Q07] 删除表
来源：http://yqq.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://ewj.9152youxi.cn

[Q08] 创建普通索引
来源：http://lik.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pdp.cashguo.top

[Q09] 创建唯一索引
来源：http://acl.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://joa.yuxming.cn

[Q10] 插入单行
来源：http://qlw.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fko.sjlbkw.cn

[Q11] 一次插入多行
来源：http://lvh.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://car.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://vil.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gba.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://big.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://gfy.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fds.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://zhv.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ucw.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://feb.sufxvd.cn

[Q15] 查询全部
来源：http://apu.fanxiaobao.xyz


<!-- 参考信息 -->