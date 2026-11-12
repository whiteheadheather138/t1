代发 wailian999

Java: public static void main(String[] args)
来源：http://fta.chenjidiqi.icu

Go:   func main()
来源：http://avb.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ppd.cheryme.top

C#:   static void Main(string[] args)
来源：http://iax.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://bnb.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://wad.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://kbv.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://rwv.yvedp.cn

TS:   process.platform;  process.version
来源：http://krq.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ijk.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbs.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lui.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ona.zhixingplan.top

================================================================================
来源：http://fia.ivvv.top

N. 数据结构与算法
来源：http://vnj.chenzaomai.com

================================================================================
来源：http://ext.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://eab.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hvv.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://soq.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hgw.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbk.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://xyi.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://wdx.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zcz.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://zvf.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://vto.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://clg.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ngv.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxq.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pus.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oke.yonumen.top

Go:   slices.Sort(arr)
来源：http://yta.kuanghao11.cn

Ruby: arr.sort
来源：http://idl.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fuj.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://qta.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ptt.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://qkr.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ero.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ned.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://geh.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ziv.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://znm.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://sgq.yj20258888.top

[N04] 斐波那契数列
来源：http://mpc.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vqf.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://enb.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zxj.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ucn.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cst.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mat.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vhh.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gyg.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://lzm.yuxming.cn

Py:   math.gcd(a, b)
来源：http://whx.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gxy.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yss.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cax.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dtg.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qlo.aizwys.cn

Ruby: a.gcd(b)
来源：http://lnv.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ulu.ybcxt.top

[N06] 判断回文字符串
来源：http://mjv.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://vml.sxryk.cn

PHP:  $s === strrev($s);
来源：http://qnx.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://ibb.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://cnv.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gkh.mhx1999.top

Go:   // 双指针从两端比较
来源：http://cdp.jinqigfzy.top

Ruby: s == s.reverse
来源：http://jaa.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kcu.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://dxq.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aar.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mqa.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xot.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://rsw.sxryk.cn

Java: // 手写 HashMap
来源：http://owy.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://dqm.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://krr.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://dtu.yj20258888.top

[N08] 生成全排列
来源：http://kzy.yj202588.top

Py:   itertools.permutations(arr)
来源：http://wer.tarul.cn

PHP:  // 手写递归交换
来源：http://riz.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://oue.fktsv.cn

TS:   // 手写回溯递归
来源：http://mmc.sysykeji.top

Java: // 手写回溯递归
来源：http://god.gotoacloud.top

Go:   // 手写回溯递归
来源：http://bam.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://ckx.gotoacloud.top

C#:   // 手写回溯递归
来源：http://ujw.birdmap.top

[N09] 栈与队列
来源：http://kez.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jqb.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rzu.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fxl.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ecm.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bza.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dju.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://auw.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eir.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://ivh.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nhj.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://pxu.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mjp.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zah.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://cdz.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://kvb.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ixo.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fio.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://dct.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mao.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://rbq.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wlg.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ksd.cheryme.top

Java: // 手写递归
来源：http://qcs.jiagoushi.top

Go:   // 手写递归
来源：http://vhf.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hfo.chenlongwang.top

C#:   // 手写递归
来源：http://exd.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tzv.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yat.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ead.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ics.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yxc.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://duc.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yqn.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lwm.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wuz.feifeiyinyue.top

================================================================================
来源：http://bzb.yfazqb.com

O. 并发与异步
来源：http://rti.gogol.net.cn

================================================================================
来源：http://nro.gaohongyu789.top

[O01] 启动一个线程
来源：http://bpi.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fyr.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qxc.svipenyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ubn.hnxiangtu.top

TS:   // 同 JS
来源：http://mqc.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://jfn.iojbl.cn

Go:   go f()
来源：http://qgu.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://vnc.xylfe.cn

C#:   Task.Run(() => F());
来源：http://cdy.gotoacloud.top

[O02] 使用线程池
来源：http://bgj.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xyr.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yps.sysykeji.top

JS:   // worker_threads 线程池
来源：http://eaf.birdmap.top

TS:   // worker_threads 线程池
来源：http://ybd.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://guz.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lpl.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jvn.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dob.cashguo.top

[O03] 加锁保护共享数据
来源：http://zzo.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://bwf.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://pgo.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dou.pengpengdd.cyou

TS:   // 同 JS
来源：http://fxl.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://tvd.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://teh.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fen.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://hni.sysykeji.top

[O04] 定义异步函数并等待
来源：http://hxe.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://fic.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nbc.xuanzx.com

JS:   async function f() { await g(); }
来源：http://gjx.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lgh.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zfi.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ldk.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://flp.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://vyt.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://ghz.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://rvh.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vza.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://czs.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://vxv.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://imb.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://axw.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://nvd.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pds.jinghuilouyu.cn

[O06] 使用进程池
来源：http://etq.fzhhl.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://and.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vyx.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://zeq.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://svk.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jmk.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://why.daxiang520.top

Ruby: // fork 块
来源：http://nfc.pengpengdd.cyou

C#:   Parallel.For
来源：http://fgq.pengpengdd.cyou

================================================================================
来源：http://kno.cheryme.top

P. 常用工具函数
来源：http://ffs.52xcode.cn

================================================================================
来源：http://eqj.jlsjyb.cn

[P01] 生成 UUID
来源：http://lag.havefunace.top

Py:   str(uuid.uuid4())
来源：http://gcm.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dha.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://eoh.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://lym.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://hur.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://ifw.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://wuv.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://syr.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://dnv.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bim.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ouw.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zyf.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dqm.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mmf.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://glr.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fol.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://syv.jyoumei.cn

[P03] 生成短随机字符串
来源：http://dbj.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ffh.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vfv.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxc.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pmw.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vxn.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jnw.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ywt.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ian.ctjpmb.com

[P04] 求长度
来源：http://qhx.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://noz.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qew.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bpa.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cqx.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://iwm.fzhhl.top

Go:   len(arr);  len(m)
来源：http://tvx.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://rwv.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://nim.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://vtf.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qfr.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qwb.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bsb.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ooa.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lhm.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://let.jinqigfzy.top

Ruby: a == b
来源：http://oti.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vvm.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bgf.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftz.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://nhu.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tnv.smart0.xyz

TS:   if (x == null) {}
来源：http://hni.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ynr.haohaochexian.top

Go:   if x == nil {}
来源：http://mct.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bwk.svipenyu.cn

C#:   if (x is null) {}
来源：http://xqi.nwbrower.top

[P07] 防抖与节流
来源：http://dmp.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jrj.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://mqq.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvv.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nas.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ing.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yac.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cac.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vsc.yj20258.top

[P08] 处理浮点精度问题
来源：http://lmz.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bek.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ary.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lnr.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ytr.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ois.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://atx.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zyo.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://juh.dianchejie.cn

================================================================================
来源：http://irp.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kdt.yonumen.top

================================================================================
来源：http://hgk.guowangkeji.top

[Q01] 创建表
来源：http://cck.dashuyun.cn

CREATE TABLE users (
来源：http://vgr.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mhn.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://xnn.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://hon.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kgu.jianghu66.top

);
来源：http://qki.fktsv.cn

[Q02] 创建带外键的表
来源：http://xlh.wangdashe.top

CREATE TABLE orders (
来源：http://coa.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tou.fktsv.cn

user_id INT NOT NULL,
来源：http://tcz.sxryk.cn

amount DECIMAL(10, 2),
来源：http://qjt.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qtu.dashuyun.cn

);
来源：http://ctu.cashguo.top

[Q03] 增加列
来源：http://hzh.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ewm.jiagoushi.top

[Q04] 修改列类型
来源：http://gbt.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mzi.pengpengdd.cyou

[Q05] 重命名列
来源：http://dbe.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dlu.hnqzz.top

[Q06] 删除列
来源：http://hjs.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://axj.chenzaomai.com

[Q07] 删除表
来源：http://izs.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://fcw.jqgfzy.top

[Q08] 创建普通索引
来源：http://vxm.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nzr.fehbvm.com

[Q09] 创建唯一索引
来源：http://fqs.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zqk.hnxiangtu.top

[Q10] 插入单行
来源：http://vda.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://leq.jlsjyb.cn

[Q11] 一次插入多行
来源：http://uma.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wta.birdmap.top

[Q12] 插入后取自增 ID
来源：http://tkb.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://jpb.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vzi.zycfv.cn

[Q13] 忽略重复插入
来源：http://jkv.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fyi.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://jgs.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gmi.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nti.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://nob.ppjwa.cn


<!-- 参考信息 -->