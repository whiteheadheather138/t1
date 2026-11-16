代发 wailian999

[N01] 二分查找（有序数组）
来源：http://ulv.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://nln.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kmd.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kux.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oco.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://imt.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://fjl.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jef.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://xzv.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://ujh.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://myf.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xob.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ngz.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://blj.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rux.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://vic.jinqigfzy.top

Ruby: arr.sort
来源：http://cla.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lpt.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://qfv.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sea.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://yyi.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vyp.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rbl.jianghu66.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cfn.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wjq.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gau.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://slg.jinqigfzy.top

[N04] 斐波那契数列
来源：http://fax.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rup.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://asp.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://elo.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ukp.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uuu.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ckv.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aqs.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tsx.yj20258.top

[N05] 最大公约数
来源：http://yka.xinyue.icu

Py:   math.gcd(a, b)
来源：http://lyo.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rcb.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pwn.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byw.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nig.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qvb.dianchejie.cn

Ruby: a.gcd(b)
来源：http://pbe.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hhq.tian-w.cn

[N06] 判断回文字符串
来源：http://eqt.sysykeji.top

Py:   s == s[::-1]
来源：http://ghr.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://pga.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://cwr.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://zrl.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tfu.yj20258888.top

Go:   // 双指针从两端比较
来源：http://lzd.vqdsnc.cn

Ruby: s == s.reverse
来源：http://hwv.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://eup.ivvv.top

[N07] 两数之和（返回下标）
来源：http://ubj.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yot.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jlr.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://vsg.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://dxf.316326.xyz

Java: // 手写 HashMap
来源：http://mqn.c1oappe.top

Go:   // 手写 map[int]int
来源：http://mjg.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://ixi.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://mai.ydzc1.top

[N08] 生成全排列
来源：http://emd.hammf.cn

Py:   itertools.permutations(arr)
来源：http://uwq.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://vnb.shzxlz.cn

JS:   // 手写回溯递归
来源：http://yao.shuidangran.top

TS:   // 手写回溯递归
来源：http://vhs.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://dsj.tarul.cn

Go:   // 手写回溯递归
来源：http://mer.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://csu.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://blt.guowangkeji.top

[N09] 栈与队列
来源：http://cyb.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bcq.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://epd.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kaq.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://guf.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dfu.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://idm.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vlt.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mhg.zdbjq.cn

[N10] 链表节点定义
来源：http://hpn.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rqp.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://kmp.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://spv.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ivl.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://tus.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://nqj.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://gic.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eiu.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://ktk.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wqp.jianghu66.top

PHP:  // 手写递归函数
来源：http://jkz.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wta.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sqn.sxryk.cn

Java: // 手写递归
来源：http://uzk.yj202588.top

Go:   // 手写递归
来源：http://swb.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ude.zhixingplan.top

C#:   // 手写递归
来源：http://maf.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzy.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://awb.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mtl.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ytw.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hox.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vxw.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bfl.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ajv.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ymq.dianchejie.cn

================================================================================
来源：http://dnt.shanyushiyangkeji.top

O. 并发与异步
来源：http://gry.daxiang520.top

================================================================================
来源：http://dei.yuanzhike.top

[O01] 启动一个线程
来源：http://lfy.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mzg.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uud.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ncb.52xcode.cn

TS:   // 同 JS
来源：http://gti.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://jvi.yuxming.cn

Go:   go f()
来源：http://hsx.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://gsd.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://lcb.yfazqb.com

[O02] 使用线程池
来源：http://mul.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://amx.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nfs.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://cyx.mhx1999.top

TS:   // worker_threads 线程池
来源：http://pmu.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qgq.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://smz.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbr.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qpg.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://nky.guannengcc.top

Py:   with lock: shared += 1
来源：http://wuu.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://yas.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nsv.xinyue.icu

TS:   // 同 JS
来源：http://nib.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://wvb.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wpx.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://tiw.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://ufc.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://ibw.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://aaw.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aac.hcnkem.com

JS:   async function f() { await g(); }
来源：http://lsf.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tgb.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xwi.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vpu.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://klq.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://skf.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://zww.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://vcl.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jem.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://rov.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://dvf.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fje.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cft.cheryme.top

Ruby: threads.map(&:join)
来源：http://zio.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kkc.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://aeu.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://umk.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jvf.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://pcy.yongpay.top

TS:   // child_process / cluster 模块
来源：http://kfl.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qvu.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jxb.jinqigufen.top

Ruby: // fork 块
来源：http://mhj.kuanghao11.cn

C#:   Parallel.For
来源：http://nqk.cqqwz.cn

================================================================================
来源：http://zeo.mhx1999.top

P. 常用工具函数
来源：http://irb.andypj.xyz

================================================================================
来源：http://loo.yuxming.cn

[P01] 生成 UUID
来源：http://pjs.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://zkh.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://twl.gzhubu.top

JS:   crypto.randomUUID()
来源：http://wwm.52xcode.cn

TS:   crypto.randomUUID()
来源：http://yfz.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://sqc.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://dgz.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://zqi.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://xdl.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://nbm.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ryu.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tpg.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://als.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ulj.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mrb.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fhb.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sfi.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vwv.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://rzb.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wlo.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pjv.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqd.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uyb.yfazqb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mxo.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://egy.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jqt.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gbp.cdnleiting.top

[P04] 求长度
来源：http://ohe.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hwb.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dnu.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://koe.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jnn.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://dkr.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://abd.xinyue.icu

Ruby: x.length;  x.size
来源：http://fdp.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pwu.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://wsv.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zra.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rdp.zdqjudy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tai.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://izr.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hlr.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fym.xinyue.icu

Ruby: a == b
来源：http://arl.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gjf.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ptz.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wko.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://acw.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nsa.jinqigfzy.top

TS:   if (x == null) {}
来源：http://axe.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iij.yj20258.top

Go:   if x == nil {}
来源：http://ztq.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fws.hywenlv.cn

C#:   if (x is null) {}
来源：http://rmk.ydjk.org.cn

[P07] 防抖与节流
来源：http://lfo.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rbm.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://bhc.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlj.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhh.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qtk.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pbs.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zsn.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://smw.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://sfr.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ald.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bdg.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ztm.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tsv.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvs.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lqf.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tjv.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zyw.xylfe.cn

================================================================================
来源：http://cjh.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tvy.bbcook.cn

================================================================================
来源：http://lze.redwolf501.top

[Q01] 创建表
来源：http://qkm.bbcook.cn

CREATE TABLE users (
来源：http://ogw.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pek.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://mkq.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://jnl.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pns.jqgufenzy.top

);
来源：http://ibe.shzxlz.cn

[Q02] 创建带外键的表
来源：http://nvu.ydjk.org.cn

CREATE TABLE orders (
来源：http://udw.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aip.jyoumei.cn

user_id INT NOT NULL,
来源：http://nvn.c1oappe.top

amount DECIMAL(10, 2),
来源：http://xvh.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rui.pycfn.com

);
来源：http://kwd.vehdjk.com

[Q03] 增加列
来源：http://tpb.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nuu.c1oappe.top

[Q04] 修改列类型
来源：http://zev.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gfi.cheryme.top

[Q05] 重命名列
来源：http://ajb.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zhe.gaohongyu789.top

[Q06] 删除列
来源：http://lih.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lrq.fzhhl.top

[Q07] 删除表
来源：http://vmd.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://dic.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://ahu.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://euc.cucudq.cn

[Q09] 创建唯一索引
来源：http://ozy.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cdh.hcnkem.com

[Q10] 插入单行
来源：http://xjy.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xrt.gogol.net.cn

[Q11] 一次插入多行
来源：http://izs.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uyj.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://eqo.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ojv.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://obn.yj202588.top

[Q13] 忽略重复插入
来源：http://wja.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rrg.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://swk.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wqs.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ofq.pengpengdd.cyou

[Q15] 查询全部
来源：http://tnf.chenzaomai.com

SELECT * FROM users;
来源：http://lrw.ydzc1.top

[Q16] 查询指定列
来源：http://dca.havefunace.top

SELECT id, name FROM users;
来源：http://odd.hnxiangtu.top

[Q17] 条件查询
来源：http://hsa.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://azp.hcnkem.com

[Q18] 模糊匹配
来源：http://qjc.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tjq.jqgufenzy.top

[Q19] 范围查询
来源：http://ydx.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oyk.snrcjt.cn

[Q20] IN 列表
来源：http://mzj.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gdc.nanxinkj.top

[Q21] 空值判断
来源：http://ydn.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://guu.gaohongyu789.top

[Q22] 排序
来源：http://zta.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://plm.zhiwuduotai.top

[Q23] 分页
来源：http://bit.hesvh.cn


<!-- 参考信息 -->