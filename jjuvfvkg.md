代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://jkx.pengpengdd.cyou

================================================================================
来源：http://bor.havefunace.top

N. 数据结构与算法
来源：http://gzj.ivvv.top

================================================================================
来源：http://wnp.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://oqi.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://quh.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pce.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwq.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxr.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://ivt.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://hjn.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xll.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://tkf.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://ken.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kdz.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://itn.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://wlo.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://mjb.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://roo.sysykeji.top

Go:   slices.Sort(arr)
来源：http://erf.hammf.cn

Ruby: arr.sort
来源：http://tbx.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sjk.316326.xyz

[N03] 快速排序（分治示例）
来源：http://dia.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xcf.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://hkm.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nng.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rod.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pom.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qhf.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ccl.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://pzg.quarkkingdee.top

[N04] 斐波那契数列
来源：http://uqr.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mmh.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://igh.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nkl.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yke.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dkx.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zbw.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vmm.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mdh.yueranfly.top

[N05] 最大公约数
来源：http://bsc.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://rts.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rqz.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tmf.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sfw.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gbi.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hxk.dianchejie.cn

Ruby: a.gcd(b)
来源：http://pqp.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iti.daxiang520.top

[N06] 判断回文字符串
来源：http://jab.sjlbkw.cn

Py:   s == s[::-1]
来源：http://jbp.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://loa.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://xxk.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://jsq.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ufc.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://tco.yvedp.cn

Ruby: s == s.reverse
来源：http://jsc.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mbn.yj202588.top

[N07] 两数之和（返回下标）
来源：http://htp.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wpu.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kpk.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dfa.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://rju.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://xzo.yj202588.top

Go:   // 手写 map[int]int
来源：http://whj.52xcode.cn

Ruby: // 手写 Hash
来源：http://jsp.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wir.gotoacloud.top

[N08] 生成全排列
来源：http://pfl.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://lud.shzxlz.cn

PHP:  // 手写递归交换
来源：http://ksv.svipenyu.cn

JS:   // 手写回溯递归
来源：http://wzc.ybcxt.top

TS:   // 手写回溯递归
来源：http://zym.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://ipz.chenzaomai.com

Go:   // 手写回溯递归
来源：http://vli.yj20258.top

Ruby: arr.permutation.to_a
来源：http://zds.iojbl.cn

C#:   // 手写回溯递归
来源：http://kuf.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://fhv.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xss.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mxu.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gus.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hxo.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qvh.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://orw.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://plc.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ltb.tanke756.top

[N10] 链表节点定义
来源：http://uzb.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zey.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://agl.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pxy.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hrh.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://bpw.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://lps.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zwj.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://foy.iojbl.cn

[N11] 二叉树中序遍历
来源：http://dkq.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vfh.yj20258.top

PHP:  // 手写递归函数
来源：http://cti.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqa.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpw.jqgufenzy.top

Java: // 手写递归
来源：http://esf.hysaishi.cn

Go:   // 手写递归
来源：http://tdo.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://djc.yongpay.top

C#:   // 手写递归
来源：http://vhv.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ofv.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jnk.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ehv.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oor.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxb.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://omw.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lar.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eeo.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yqe.bjfxy.top

================================================================================
来源：http://nhq.bbcook.cn

O. 并发与异步
来源：http://ntt.ydzc1.top

================================================================================
来源：http://cgr.ydjk.org.cn

[O01] 启动一个线程
来源：http://giq.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rik.iojbl.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cvo.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rvx.yanxiufei.cn

TS:   // 同 JS
来源：http://rot.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://eiw.hammf.cn

Go:   go f()
来源：http://hjh.xinyue.icu

Ruby: Thread.new { f }
来源：http://gqb.smart0.xyz

C#:   Task.Run(() => F());
来源：http://pbb.jlsjyb.cn

[O02] 使用线程池
来源：http://bga.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qvz.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://glf.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://vqk.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://rwx.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://kud.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xol.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pku.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sri.bjfxy.top

[O03] 加锁保护共享数据
来源：http://kxt.sysykeji.top

Py:   with lock: shared += 1
来源：http://fct.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://qgt.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jbv.jyoumei.cn

TS:   // 同 JS
来源：http://hnk.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://pab.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ocu.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wbq.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://khp.ivvv.top

[O04] 定义异步函数并等待
来源：http://tlq.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://luo.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eev.uphjek.com

JS:   async function f() { await g(); }
来源：http://kkz.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xnu.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ece.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dtz.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uvb.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://rnr.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://vxt.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://zgl.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gmy.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://ctk.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://fyf.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aii.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mpd.vehdjk.com

Ruby: threads.map(&:join)
来源：http://etm.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ybt.yj202588.top

[O06] 使用进程池
来源：http://wke.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ujt.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://tcz.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://dgm.havefunace.top

TS:   // child_process / cluster 模块
来源：http://avf.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://spp.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mjq.nwbrower.top

Ruby: // fork 块
来源：http://ghk.hnqzz.top

C#:   Parallel.For
来源：http://glo.xuanzx.com

================================================================================
来源：http://xam.nanxuanxn.top

P. 常用工具函数
来源：http://tly.fzhhl.top

================================================================================
来源：http://bfo.zycfv.cn

[P01] 生成 UUID
来源：http://gma.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://exx.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lwh.yueranfly.top

JS:   crypto.randomUUID()
来源：http://ljv.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://hfi.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://yzf.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://gsj.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://zre.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://cbr.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://lze.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bgc.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zwu.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pwx.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://veh.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://byr.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nqk.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eny.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bfl.xuanzx.com

[P03] 生成短随机字符串
来源：http://gug.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://giy.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uuu.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhy.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lcr.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wxq.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yhf.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://phj.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://agd.tianlin.xyz

[P04] 求长度
来源：http://spf.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lqd.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kzs.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ffu.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://etf.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://rbg.yueranfly.top

Go:   len(arr);  len(m)
来源：http://bri.hesvh.cn

Ruby: x.length;  x.size
来源：http://yfq.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gay.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://dbs.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tuu.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ibd.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pzt.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eeh.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://seb.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://hcg.ehwqpu.com

Ruby: a == b
来源：http://xnb.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tit.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hcf.jiagoushi.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zxm.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://bfe.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eqo.hnqzz.top

TS:   if (x == null) {}
来源：http://xpt.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eec.pengpengdd.cyou

Go:   if x == nil {}
来源：http://svy.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ekp.jyoumei.cn

C#:   if (x is null) {}
来源：http://zbx.ydjk.org.cn

[P07] 防抖与节流
来源：http://cgf.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ggj.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://iwd.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wyl.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zmx.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cig.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cry.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cik.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://swh.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://yny.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qbc.yueranfly.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nny.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://map.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xcp.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://stg.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://orn.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qfr.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vfy.zhengqikj.top

================================================================================
来源：http://rkr.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ygn.yongpay.top

================================================================================
来源：http://sds.jlsjyb.cn

[Q01] 创建表
来源：http://gep.quarkkingdee.top

CREATE TABLE users (
来源：http://bpk.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dkg.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://kjm.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://crz.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ahl.dianchejie.cn

);
来源：http://wib.jqgfzy.top

[Q02] 创建带外键的表
来源：http://elf.jinqigufen.top

CREATE TABLE orders (
来源：http://asu.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bpm.bjfxy.top

user_id INT NOT NULL,
来源：http://vjy.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://rfq.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ckp.jinyuanbaomall.cn

);
来源：http://fsb.shanyushiyangkeji.top

[Q03] 增加列
来源：http://xgp.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kcy.gotoacloud.top

[Q04] 修改列类型
来源：http://axs.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://usg.gogol.net.cn

[Q05] 重命名列
来源：http://tru.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bqh.chenzaomai.com

[Q06] 删除列
来源：http://aqy.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tbg.shzxlz.cn

[Q07] 删除表
来源：http://mbh.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://nbt.gzhubu.top

[Q08] 创建普通索引
来源：http://rvp.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wjq.sysykeji.top

[Q09] 创建唯一索引
来源：http://kok.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hxd.yfazqb.com

[Q10] 插入单行
来源：http://kzx.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bfx.yuxming.cn

[Q11] 一次插入多行
来源：http://kph.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kkj.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://zog.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://ftv.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vnt.gogol.net.cn

[Q13] 忽略重复插入
来源：http://uzf.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://trv.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://bvi.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wdx.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eww.yuanzhike.top

[Q15] 查询全部
来源：http://rxb.ivvv.top

SELECT * FROM users;
来源：http://xdm.jinqigufen.top

[Q16] 查询指定列
来源：http://nfu.xylfe.cn

SELECT id, name FROM users;
来源：http://fhz.cashguo.top

[Q17] 条件查询
来源：http://kag.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iuq.sufxvd.cn

[Q18] 模糊匹配
来源：http://rru.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ktl.yj20258888.top

[Q19] 范围查询
来源：http://yfh.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eeg.jqgfzy.top

[Q20] IN 列表
来源：http://cij.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ufx.zhijiandao.cn

[Q21] 空值判断
来源：http://soc.yueranfly.top


<!-- 参考信息 -->