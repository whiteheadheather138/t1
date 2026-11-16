代发 wailian999

TS:   process.platform;  process.version
来源：http://pfj.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iaw.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ijp.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xbu.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://cgv.sweek.top

================================================================================
来源：http://qfq.yfazqb.com

N. 数据结构与算法
来源：http://fpq.316326.xyz

================================================================================
来源：http://vhq.pycfn.com

[N01] 二分查找（有序数组）
来源：http://wzo.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hia.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cwh.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rox.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jfo.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kkh.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://iri.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mdu.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aeo.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://doc.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://zxr.hcnkem.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iuc.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fqo.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qng.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yxx.yj20258.top

Go:   slices.Sort(arr)
来源：http://ulz.yueranfly.top

Ruby: arr.sort
来源：http://avl.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pdk.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://vax.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uda.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://nqa.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ybq.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dui.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://akq.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwn.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ucc.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://lhk.ydjk.org.cn

[N04] 斐波那契数列
来源：http://nbk.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oge.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jep.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdy.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kms.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://waf.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gwn.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jyq.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xep.yanxiufei.cn

[N05] 最大公约数
来源：http://sfb.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://sds.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tdx.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxc.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghe.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hll.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rac.xziqi.cn

Ruby: a.gcd(b)
来源：http://wae.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qqk.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://gqj.guowangkeji.top

Py:   s == s[::-1]
来源：http://lhr.316326.xyz

PHP:  $s === strrev($s);
来源：http://rad.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://ltr.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://crt.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uhb.c1oappe.top

Go:   // 双指针从两端比较
来源：http://zrd.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://uek.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dya.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://zix.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://taq.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xqi.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tpd.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://egs.guannengcc.top

Java: // 手写 HashMap
来源：http://iak.c1oappe.top

Go:   // 手写 map[int]int
来源：http://fwd.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://nyg.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://njn.birdmap.top

[N08] 生成全排列
来源：http://rlz.yongpay.top

Py:   itertools.permutations(arr)
来源：http://rnl.52xcode.cn

PHP:  // 手写递归交换
来源：http://dge.sufxvd.cn

JS:   // 手写回溯递归
来源：http://lad.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://qtb.chenzaomai.com

Java: // 手写回溯递归
来源：http://imp.hammf.cn

Go:   // 手写回溯递归
来源：http://eak.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://ktd.cdnleiting.top

C#:   // 手写回溯递归
来源：http://hjk.yfazqb.com

[N09] 栈与队列
来源：http://edm.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xmm.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ppq.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mqa.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gar.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lwk.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ngb.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tcm.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ltf.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://epe.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xxe.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fpc.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vfe.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cpf.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://smf.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://geo.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hdg.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nyh.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://llp.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uxk.sysykeji.top

PHP:  // 手写递归函数
来源：http://eih.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upy.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikb.yfazqb.com

Java: // 手写递归
来源：http://akc.yvedp.cn

Go:   // 手写递归
来源：http://gug.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xtx.redwolf501.top

C#:   // 手写递归
来源：http://svf.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nvd.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jfd.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nha.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbp.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rzm.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ncg.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ynq.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sap.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vpq.smart0.xyz

================================================================================
来源：http://eod.epnwcf.com

O. 并发与异步
来源：http://xei.shanyushiyangtech.top

================================================================================
来源：http://vda.9152youxi.cn

[O01] 启动一个线程
来源：http://msb.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yky.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ltf.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ilr.sjlbkw.cn

TS:   // 同 JS
来源：http://ctz.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://ury.shanyushiyangkeji.top

Go:   go f()
来源：http://tex.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://cwj.fzhhl.top

C#:   Task.Run(() => F());
来源：http://ovx.jyoumei.cn

[O02] 使用线程池
来源：http://ejm.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bmj.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rgq.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://tqy.yj20258888.top

TS:   // worker_threads 线程池
来源：http://wnb.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fqf.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://not.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://orf.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kjl.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://rnb.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://svu.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://pki.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hev.zhiwuduotai.top

TS:   // 同 JS
来源：http://tfv.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://beq.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://svv.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jfv.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://gzm.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://sgf.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://mkh.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mjh.xylfe.cn

JS:   async function f() { await g(); }
来源：http://noe.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://aym.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sho.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xxx.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://ecd.yj20258.top

C#:   async Task F() { await G(); }
来源：http://kvy.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://cqp.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://vws.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qpp.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://nhf.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://hlk.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bsu.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jig.meibo888.top

Ruby: threads.map(&:join)
来源：http://bme.zhoulong.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://gaq.chenzaomai.com

[O06] 使用进程池
来源：http://ehg.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://huk.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tqq.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://ckx.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://rws.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bch.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gad.quarkkingdee.top

Ruby: // fork 块
来源：http://ypv.cqqwz.cn

C#:   Parallel.For
来源：http://erv.aizwys.cn

================================================================================
来源：http://bse.xuanzx.com

P. 常用工具函数
来源：http://lrq.ehwqpu.com

================================================================================
来源：http://shp.xziqi.cn

[P01] 生成 UUID
来源：http://dpg.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://dkn.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://akw.hammf.cn

JS:   crypto.randomUUID()
来源：http://lpi.vehdjk.com

TS:   crypto.randomUUID()
来源：http://hcj.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://zjm.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://iuq.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://cyv.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://mwu.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://eeo.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bra.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kce.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://esc.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eak.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qht.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qhy.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ysa.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qqu.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://jvp.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hym.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vqs.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://npt.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ynq.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dtz.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tym.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://eph.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nne.xylfe.cn

[P04] 求长度
来源：http://jsu.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dav.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvo.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zhf.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://duh.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://tfp.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://xjp.epnwcf.com

Ruby: x.length;  x.size
来源：http://pts.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://scw.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://qkb.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zbs.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qng.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ycb.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bdf.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lqr.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://dqj.hammf.cn

Ruby: a == b
来源：http://elq.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hlx.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mkm.yj202588.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dah.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://niy.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jwb.ctjpmb.com

TS:   if (x == null) {}
来源：http://zkf.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rxp.daria6918.cn

Go:   if x == nil {}
来源：http://lhr.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ptp.fengsongda.top

C#:   if (x is null) {}
来源：http://dor.bjfxy.top

[P07] 防抖与节流
来源：http://taq.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ads.yonumen.top

PHP:  // 手写时间戳比较
来源：http://dwk.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrb.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://evw.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jjc.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lsr.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ana.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nwg.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://bhu.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hvt.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yjx.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pst.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xjk.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://omj.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xts.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fsd.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gow.ybcxt.top

================================================================================
来源：http://qey.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qhk.vqdsnc.cn

================================================================================
来源：http://fnj.jianghu66.top

[Q01] 创建表
来源：http://hsu.hfpthk.cn

CREATE TABLE users (
来源：http://rqt.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hub.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://csv.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://cxc.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rxy.hywenlv.cn

);
来源：http://wci.fehbvm.com

[Q02] 创建带外键的表
来源：http://akg.xinyue.icu

CREATE TABLE orders (
来源：http://vzg.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wst.0kj1m.cn

user_id INT NOT NULL,
来源：http://ovx.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://ces.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://khf.zdqjudy.top

);
来源：http://reb.0kj1m.cn

[Q03] 增加列
来源：http://nou.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xvw.gaohongyu789.top

[Q04] 修改列类型
来源：http://jdb.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nvo.tanke756.top

[Q05] 重命名列
来源：http://amq.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://for.shanyushiyangkeji.top

[Q06] 删除列
来源：http://wpg.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://txf.xinyue.icu

[Q07] 删除表
来源：http://hrm.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://ttm.ydjk.org.cn

[Q08] 创建普通索引
来源：http://jfn.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zay.shuidangran.top

[Q09] 创建唯一索引
来源：http://diw.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://awh.guowangkeji.top

[Q10] 插入单行
来源：http://ngc.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pkq.yj20258888.top

[Q11] 一次插入多行
来源：http://syb.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wcd.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://yek.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://nbp.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dcx.uphjek.com

[Q13] 忽略重复插入
来源：http://tmz.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mcv.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://bus.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ngj.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aqh.kuanghao11.cn

[Q15] 查询全部
来源：http://vxb.sweek.top

SELECT * FROM users;
来源：http://vuc.jiagoushi.top

[Q16] 查询指定列
来源：http://wfj.kuanghao11.cn

SELECT id, name FROM users;
来源：http://dlm.jqgfzy.top

[Q17] 条件查询
来源：http://dlk.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rdb.jqgfzy.top

[Q18] 模糊匹配
来源：http://aaz.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jht.xinyue.icu

[Q19] 范围查询
来源：http://swv.svipenyu.cn


<!-- 参考信息 -->