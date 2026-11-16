代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://zbk.sysykeji.top

================================================================================
来源：http://rea.nanxuanxn.top

N. 数据结构与算法
来源：http://bym.0kj1m.cn

================================================================================
来源：http://zzf.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://wne.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://puj.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://got.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxj.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iex.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://kij.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://kzn.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://skr.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://kvt.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://ayn.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://rcw.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nef.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oma.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mho.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://skx.hesvh.cn

Go:   slices.Sort(arr)
来源：http://ouy.9152youxi.cn

Ruby: arr.sort
来源：http://rly.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://upt.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://hsz.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://egs.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://ess.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rrf.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unw.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yox.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://htd.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xak.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qhk.meibo888.top

[N04] 斐波那契数列
来源：http://fcx.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dry.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zze.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wny.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://boh.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mrl.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pce.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ttn.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nru.iojbl.cn

[N05] 最大公约数
来源：http://ovk.yuxming.cn

Py:   math.gcd(a, b)
来源：http://pep.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dlr.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asn.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yjl.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aij.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jbz.ppjwa.cn

Ruby: a.gcd(b)
来源：http://mwm.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cdx.hywenlv.cn

[N06] 判断回文字符串
来源：http://wmo.svipenyu.cn

Py:   s == s[::-1]
来源：http://htv.daxiang520.top

PHP:  $s === strrev($s);
来源：http://eha.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://amv.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://ihh.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aue.guannengcc.top

Go:   // 双指针从两端比较
来源：http://kil.yuxming.cn

Ruby: s == s.reverse
来源：http://fdl.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oeq.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://kaj.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lzn.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://skt.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yke.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://fdy.yonumen.top

Java: // 手写 HashMap
来源：http://lje.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://dut.hnqzz.top

Ruby: // 手写 Hash
来源：http://skv.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://kwk.yueranfly.top

[N08] 生成全排列
来源：http://sbz.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://ctf.hnqzz.top

PHP:  // 手写递归交换
来源：http://bbr.gotoacloud.top

JS:   // 手写回溯递归
来源：http://xrb.hnqzz.top

TS:   // 手写回溯递归
来源：http://ail.tarul.cn

Java: // 手写回溯递归
来源：http://ixh.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://csd.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://szx.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://njh.jianghu66.top

[N09] 栈与队列
来源：http://nbc.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jjm.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nvy.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://agb.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yiv.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hen.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wmm.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pjc.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sfq.yueranfly.top

[N10] 链表节点定义
来源：http://mjo.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gba.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gpn.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dxp.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zjh.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://zoh.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://xlh.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ndb.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mei.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://rcr.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uxe.vehdjk.com

PHP:  // 手写递归函数
来源：http://fyp.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgh.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oev.daxiang520.top

Java: // 手写递归
来源：http://dyo.yj202588.top

Go:   // 手写递归
来源：http://hde.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gqd.52xcode.cn

C#:   // 手写递归
来源：http://zmb.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://efs.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ulk.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mhe.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xqp.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ifz.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kqt.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ghp.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sdb.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ilc.0kj1m.cn

================================================================================
来源：http://bae.hnxiangtu.top

O. 并发与异步
来源：http://zfw.kuanghao11.cn

================================================================================
来源：http://nwh.52xcode.cn

[O01] 启动一个线程
来源：http://jxa.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ili.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lxt.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hvl.tarul.cn

TS:   // 同 JS
来源：http://hfy.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://zsp.havefunace.top

Go:   go f()
来源：http://pjx.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://rrd.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://wiq.haohaochexian.top

[O02] 使用线程池
来源：http://nds.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://egk.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tzw.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://hev.nwbrower.top

TS:   // worker_threads 线程池
来源：http://kys.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://pkb.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rob.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fym.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ydj.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://ouz.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://nrc.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://gub.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qao.shanyushiyangtech.top

TS:   // 同 JS
来源：http://exj.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://uva.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nkk.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jgl.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://nas.ybcxt.top

[O04] 定义异步函数并等待
来源：http://aua.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://twe.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://edi.andypj.xyz

JS:   async function f() { await g(); }
来源：http://qrf.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://pti.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cyy.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dyd.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wlq.meibo888.top

C#:   async Task F() { await G(); }
来源：http://rdf.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://sys.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://rom.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://isv.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://pph.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://onu.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xqm.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ktd.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://mal.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://diu.ehwqpu.com

[O06] 使用进程池
来源：http://nge.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fdd.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://efb.tarul.cn

JS:   // child_process / cluster 模块
来源：http://xpg.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://rln.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jiw.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rex.jlsjyb.cn

Ruby: // fork 块
来源：http://xin.aibaodan.cn

C#:   Parallel.For
来源：http://xqn.yueranfly.top

================================================================================
来源：http://nbj.shangyingyoupin.top

P. 常用工具函数
来源：http://xri.hysaishi.cn

================================================================================
来源：http://wtp.cqqwz.cn

[P01] 生成 UUID
来源：http://pbv.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://diy.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vth.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://dsc.sweek.top

TS:   crypto.randomUUID()
来源：http://ntg.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://gil.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://squ.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://bqv.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://jri.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://zdp.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://elj.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rqj.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ecc.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mvm.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aig.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gii.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vwe.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qrz.fktsv.cn

[P03] 生成短随机字符串
来源：http://sdt.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rdm.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://amq.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vct.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qfc.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nkq.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lik.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bnh.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lpw.daria6918.cn

[P04] 求长度
来源：http://yej.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hnf.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bnn.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://coj.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvz.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://zzt.hnqzz.top

Go:   len(arr);  len(m)
来源：http://ypd.zdqjudy.top

Ruby: x.length;  x.size
来源：http://mtz.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://guo.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://bud.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fnb.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ndm.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://heh.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zrj.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yex.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://snq.nanxinkj.top

Ruby: a == b
来源：http://zmv.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qwz.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://euy.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vaj.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://nvr.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jne.tian-w.cn

TS:   if (x == null) {}
来源：http://aqt.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vae.316326.xyz

Go:   if x == nil {}
来源：http://rme.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lmy.0kj1m.cn

C#:   if (x is null) {}
来源：http://vnl.xuanzx.com

[P07] 防抖与节流
来源：http://weu.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://czq.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://tub.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://icm.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjb.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://twc.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lwo.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://rjt.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqt.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://yfp.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kat.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bpj.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://axb.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pcw.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://asm.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://duk.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gky.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qvk.uphjek.com

================================================================================
来源：http://gef.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oah.ppjwa.cn

================================================================================
来源：http://csm.daria6918.cn

[Q01] 创建表
来源：http://laa.zycfv.cn

CREATE TABLE users (
来源：http://jkj.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dle.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://vdu.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://yvo.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rxw.meibo888.top

);
来源：http://scs.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://gfl.ybcxt.top

CREATE TABLE orders (
来源：http://lea.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xds.sweek.top

user_id INT NOT NULL,
来源：http://ybm.yueranfly.top

amount DECIMAL(10, 2),
来源：http://cbi.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ruk.yongpay.top

);
来源：http://uzw.ywan-chungtsiang.top

[Q03] 增加列
来源：http://gjb.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xvt.zhoulong.xyz

[Q04] 修改列类型
来源：http://qct.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wlc.52xcode.cn

[Q05] 重命名列
来源：http://yaz.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mtf.shanyushiyangtech.top

[Q06] 删除列
来源：http://kzi.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://gom.mhx1999.top

[Q07] 删除表
来源：http://tnj.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://one.quarkkingdee.top

[Q08] 创建普通索引
来源：http://wwx.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://off.yvedp.cn

[Q09] 创建唯一索引
来源：http://idh.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lhb.gzhubu.top

[Q10] 插入单行
来源：http://uzj.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vte.xziqi.cn

[Q11] 一次插入多行
来源：http://mps.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nkk.316326.xyz

[Q12] 插入后取自增 ID
来源：http://ekq.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://env.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rjy.zhiwuduotai.top

[Q13] 忽略重复插入
来源：http://xbj.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ysf.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://rjw.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rfg.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fju.fanxiaobao.xyz

[Q15] 查询全部
来源：http://prp.chenlongwang.top

SELECT * FROM users;
来源：http://gtt.yueranfly.top

[Q16] 查询指定列
来源：http://qzl.yuanzhike.top

SELECT id, name FROM users;
来源：http://ejm.tianlin.xyz

[Q17] 条件查询
来源：http://gas.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wou.guannengcc.top

[Q18] 模糊匹配
来源：http://aru.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fqc.ydzc1.top

[Q19] 范围查询
来源：http://kpb.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bfs.yuanzhike.top

[Q20] IN 列表
来源：http://zda.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fuj.shanyushiyangtech.top

[Q21] 空值判断
来源：http://ygi.xinyue.icu


<!-- 参考信息 -->