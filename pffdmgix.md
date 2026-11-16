代发 wailian999

[M08] 获取系统与运行时信息
来源：http://rep.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://eth.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://puq.uphjek.com

JS:   process.platform;  process.version
来源：http://vrq.xylfe.cn

TS:   process.platform;  process.version
来源：http://nts.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pbn.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://myf.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mvq.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sfy.jinghuilouyu.cn

================================================================================
来源：http://uai.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://ltm.guowangkeji.top

================================================================================
来源：http://xlm.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://pev.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qhu.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://noy.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hie.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sdi.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jqy.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://trx.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qmm.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hto.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://pkj.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://fme.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://icd.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://drz.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://xys.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://itr.xylfe.cn

Go:   slices.Sort(arr)
来源：http://xhx.xuetiantiany.cn

Ruby: arr.sort
来源：http://wek.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://upm.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://ynn.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lne.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://uwd.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tgy.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwz.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zdj.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://khb.chenlongwang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yxz.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qrr.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://loi.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ifa.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dbt.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tuk.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tbu.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ixv.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://igk.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rbm.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ktd.mhx1999.top

[N05] 最大公约数
来源：http://zqy.316326.xyz

Py:   math.gcd(a, b)
来源：http://rme.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uca.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gup.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://okf.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jtg.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kvf.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://eob.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kcq.svipenyu.cn

[N06] 判断回文字符串
来源：http://hag.hnxiangtu.top

Py:   s == s[::-1]
来源：http://dbc.daxiang520.top

PHP:  $s === strrev($s);
来源：http://mct.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://aps.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://muu.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tke.fktsv.cn

Go:   // 双指针从两端比较
来源：http://zpl.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://mvw.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ohj.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://rnt.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mms.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ukz.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tnt.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://ydy.fktsv.cn

Java: // 手写 HashMap
来源：http://xib.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://vgq.hfpthk.cn

Ruby: // 手写 Hash
来源：http://zqk.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://ruy.ppjwa.cn

[N08] 生成全排列
来源：http://kcd.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://heb.yuxming.cn

PHP:  // 手写递归交换
来源：http://ixb.sxryk.cn

JS:   // 手写回溯递归
来源：http://ubl.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://rcn.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://zte.aibaodan.cn

Go:   // 手写回溯递归
来源：http://cqd.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://wun.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://byp.zycfv.cn

[N09] 栈与队列
来源：http://pfk.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nyj.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://txt.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vta.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wru.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ymw.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ugf.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wqu.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iwb.quarkkingdee.top

[N10] 链表节点定义
来源：http://yrp.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://khw.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wly.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kbo.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vdk.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://bpq.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uvb.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ndq.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zvu.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://cvs.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xtk.chenzaomai.com

PHP:  // 手写递归函数
来源：http://qqe.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zmv.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hls.cucudq.cn

Java: // 手写递归
来源：http://riu.jqgufenzy.top

Go:   // 手写递归
来源：http://ild.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qjc.yuxming.cn

C#:   // 手写递归
来源：http://ano.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://onh.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bff.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aad.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eiw.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ayc.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tkq.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kyj.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fvz.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://paz.zdqjudy.top

================================================================================
来源：http://xul.hysaishi.cn

O. 并发与异步
来源：http://qcq.dianchejie.cn

================================================================================
来源：http://yyu.cqqwz.cn

[O01] 启动一个线程
来源：http://dqh.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mzu.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gih.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cro.guannengcc.top

TS:   // 同 JS
来源：http://hdz.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://rcs.ctjpmb.com

Go:   go f()
来源：http://lsb.havefunace.top

Ruby: Thread.new { f }
来源：http://dzl.sxryk.cn

C#:   Task.Run(() => F());
来源：http://lbf.sxryk.cn

[O02] 使用线程池
来源：http://nvq.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ycd.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://plz.smart0.xyz

JS:   // worker_threads 线程池
来源：http://fiy.sysykeji.top

TS:   // worker_threads 线程池
来源：http://rnh.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://hio.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fcj.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://feb.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://amt.hesvh.cn

[O03] 加锁保护共享数据
来源：http://mht.birdmap.top

Py:   with lock: shared += 1
来源：http://zxp.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://ikx.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lnx.zhoulong.xyz

TS:   // 同 JS
来源：http://uwo.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://lde.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://znz.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dbr.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://dhm.cheryme.top

[O04] 定义异步函数并等待
来源：http://vla.zdbjq.cn

Py:   async def f():⏎    await g()
来源：http://kbo.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dbv.ybcxt.top

JS:   async function f() { await g(); }
来源：http://bvx.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zdl.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://knf.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pzd.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wrj.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://lbq.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://cgy.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://fjc.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://znl.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://ogq.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://vng.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cgr.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hel.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://dze.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vgh.cucudq.cn

[O06] 使用进程池
来源：http://zgd.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sbv.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fen.yj20258.top

JS:   // child_process / cluster 模块
来源：http://zfn.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://bkh.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lis.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wmu.iojbl.cn

Ruby: // fork 块
来源：http://owk.chenlongwang.top

C#:   Parallel.For
来源：http://ste.havefunace.top

================================================================================
来源：http://ogp.sweek.top

P. 常用工具函数
来源：http://wde.tarul.cn

================================================================================
来源：http://edt.nanxuanxn.top

[P01] 生成 UUID
来源：http://ldq.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://vig.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sic.ivvv.top

JS:   crypto.randomUUID()
来源：http://wih.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://cwk.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://kwf.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://ssh.tanke756.top

Ruby: SecureRandom.uuid
来源：http://pbm.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://lgb.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://aib.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://htn.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aog.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cor.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uns.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tvk.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oah.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://acb.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tnx.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://afa.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://guc.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gvl.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfj.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrk.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bjt.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wxb.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sct.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pqr.chenzaomai.com

[P04] 求长度
来源：http://oct.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bhj.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytw.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jub.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yvd.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://knm.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://zfj.fktsv.cn

Ruby: x.length;  x.size
来源：http://ips.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bok.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://plq.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gnk.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mim.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gby.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zhb.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://unm.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://irt.andypj.xyz

Ruby: a == b
来源：http://kmo.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lwp.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://egy.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nwp.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://arb.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aps.smart0.xyz

TS:   if (x == null) {}
来源：http://ltk.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kdo.cdnleiting.top

Go:   if x == nil {}
来源：http://bhh.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://akd.sufxvd.cn

C#:   if (x is null) {}
来源：http://ies.0kj1m.cn

[P07] 防抖与节流
来源：http://zvb.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://byv.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://ppw.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://unb.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xlb.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ptt.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jem.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://axg.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wdu.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://qfu.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aeh.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ios.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fdw.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pvv.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jhx.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vnp.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uup.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lzt.bjfxy.top

================================================================================
来源：http://tbl.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mwg.guannengcc.top

================================================================================
来源：http://hvn.sufxvd.cn

[Q01] 创建表
来源：http://tey.svipenyu.cn

CREATE TABLE users (
来源：http://epl.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqq.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://ubf.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://svm.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bby.yj20258888.top

);
来源：http://xjv.yj20258.top

[Q02] 创建带外键的表
来源：http://cin.nanxuanxn.top

CREATE TABLE orders (
来源：http://mog.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vma.vehdjk.com

user_id INT NOT NULL,
来源：http://aic.xinyue.icu

amount DECIMAL(10, 2),
来源：http://lln.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://shr.zhaomingkeji.xyz

);
来源：http://rte.hesvh.cn

[Q03] 增加列
来源：http://csq.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ysp.zdqjudy.top

[Q04] 修改列类型
来源：http://fkc.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tjy.hcnkem.com

[Q05] 重命名列
来源：http://dte.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://frp.52xcode.cn

[Q06] 删除列
来源：http://pkz.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://rtz.0kj1m.cn

[Q07] 删除表
来源：http://eua.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://usp.yangfankeji.com

[Q08] 创建普通索引
来源：http://eyv.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jeo.sufxvd.cn

[Q09] 创建唯一索引
来源：http://yco.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gon.fehbvm.com

[Q10] 插入单行
来源：http://iag.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gtl.zhongyouzk.top

[Q11] 一次插入多行
来源：http://itw.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hgy.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://azj.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://tza.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ivk.jianghu66.top

[Q13] 忽略重复插入
来源：http://cek.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ckx.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://mrf.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bpj.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://knu.guannengcc.top

[Q15] 查询全部
来源：http://ffh.zhongyouzk.top

SELECT * FROM users;
来源：http://suw.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://xyg.vqdsnc.cn

SELECT id, name FROM users;
来源：http://ozb.quarkkingdee.top

[Q17] 条件查询
来源：http://epz.zhongyouzk.top


<!-- 参考信息 -->