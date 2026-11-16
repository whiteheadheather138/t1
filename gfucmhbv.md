代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://ttv.nanxuanxn.top

================================================================================
来源：http://gxe.jlsjyb.cn

N. 数据结构与算法
来源：http://shj.wangshuangyany.cn

================================================================================
来源：http://slg.tarul.cn

[N01] 二分查找（有序数组）
来源：http://joc.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lvh.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eph.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zom.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpo.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://ujr.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://bxd.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cje.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qxe.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://vwl.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://eln.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qbh.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nom.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iqd.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nap.havefunace.top

Go:   slices.Sort(arr)
来源：http://pdo.9152youxi.cn

Ruby: arr.sort
来源：http://jnt.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yzy.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://rye.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nkt.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://bpz.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sws.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fcm.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ypd.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qpn.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ioy.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://atr.sxryk.cn

[N04] 斐波那契数列
来源：http://sid.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xgm.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wrf.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tps.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ctf.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zqc.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nup.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qpz.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wxt.bjfxy.top

[N05] 最大公约数
来源：http://ydv.andypj.xyz

Py:   math.gcd(a, b)
来源：http://qvb.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vki.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tnz.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ksq.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://twp.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ypu.fehbvm.com

Ruby: a.gcd(b)
来源：http://eam.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xcs.gogol.net.cn

[N06] 判断回文字符串
来源：http://plk.shuidangran.top

Py:   s == s[::-1]
来源：http://sqz.smart0.xyz

PHP:  $s === strrev($s);
来源：http://vpd.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://jjm.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://kht.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kjc.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://miq.ctjpmb.com

Ruby: s == s.reverse
来源：http://lgc.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wps.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://fjs.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kiz.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mkw.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gla.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://ecu.chenzaomai.com

Java: // 手写 HashMap
来源：http://jel.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://qsb.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://pad.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://edm.iojbl.cn

[N08] 生成全排列
来源：http://hut.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://nod.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://qiy.yj20258888.top

JS:   // 手写回溯递归
来源：http://frg.xinyue.icu

TS:   // 手写回溯递归
来源：http://ifr.aizwys.cn

Java: // 手写回溯递归
来源：http://zqy.sysykeji.top

Go:   // 手写回溯递归
来源：http://eeh.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://qos.xuanzx.com

C#:   // 手写回溯递归
来源：http://vrj.shangyingyoupin.top

[N09] 栈与队列
来源：http://rfh.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nxr.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://upa.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rtj.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dbw.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://isp.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hvo.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://url.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jxr.redwolf501.top

[N10] 链表节点定义
来源：http://hdh.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kdz.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zxa.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tcj.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uyq.tanke756.top

Java: class Node { int v; Node next; }
来源：http://wsk.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qtz.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fcu.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yxi.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://cyz.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gqd.daria6918.cn

PHP:  // 手写递归函数
来源：http://ype.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayg.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wmu.sufxvd.cn

Java: // 手写递归
来源：http://ihi.xinyue.icu

Go:   // 手写递归
来源：http://ywl.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lpc.jianghu66.top

C#:   // 手写递归
来源：http://wlt.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://scd.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sfz.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ytd.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://law.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://env.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://flz.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lbl.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rql.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://frw.zycfv.cn

================================================================================
来源：http://ljc.hnqzz.top

O. 并发与异步
来源：http://uxz.redwolf501.top

================================================================================
来源：http://utn.haohaochexian.top

[O01] 启动一个线程
来源：http://kmh.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://snm.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rkj.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qcd.zhoulong.xyz

TS:   // 同 JS
来源：http://ymf.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://ouo.ehwqpu.com

Go:   go f()
来源：http://owj.gzhubu.top

Ruby: Thread.new { f }
来源：http://mzd.ydzc1.top

C#:   Task.Run(() => F());
来源：http://tfm.bjfxy.top

[O02] 使用线程池
来源：http://gnn.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cmp.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xbf.tian-w.cn

JS:   // worker_threads 线程池
来源：http://pkl.yvedp.cn

TS:   // worker_threads 线程池
来源：http://fwu.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://frx.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ovp.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yyd.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://her.fzhhl.top

[O03] 加锁保护共享数据
来源：http://pdu.tian-w.cn

Py:   with lock: shared += 1
来源：http://noh.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://ejc.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vrs.9152youxi.cn

TS:   // 同 JS
来源：http://jcu.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://hjl.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ust.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ulg.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://cmp.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://uqb.yj202588.top

Py:   async def f():⏎    await g()
来源：http://xum.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hgq.yueranfly.top

JS:   async function f() { await g(); }
来源：http://saa.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kvd.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://alv.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yxr.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://mng.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://joq.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://zlk.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://rwv.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ywc.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://fmi.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://plk.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wpe.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://elc.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://xbb.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gew.zhixingplan.top

[O06] 使用进程池
来源：http://yer.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cgf.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mbr.iojbl.cn

JS:   // child_process / cluster 模块
来源：http://hre.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://xfq.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ssn.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nno.jqgfzy.top

Ruby: // fork 块
来源：http://gyk.sufxvd.cn

C#:   Parallel.For
来源：http://usp.jlsjyb.cn

================================================================================
来源：http://nyl.ybcxt.top

P. 常用工具函数
来源：http://gik.pengpengdd.cyou

================================================================================
来源：http://rja.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://dzz.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://fur.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jzi.yfazqb.com

JS:   crypto.randomUUID()
来源：http://rtu.sxryk.cn

TS:   crypto.randomUUID()
来源：http://rxw.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://wtj.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://coq.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://yjm.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://xfe.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://pgz.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hmf.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ozj.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://exs.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sfs.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nzu.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tko.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oxd.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kyi.aizwys.cn

[P03] 生成短随机字符串
来源：http://umg.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zpj.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://owo.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhu.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://idc.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rdm.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kwa.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzw.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://svk.316326.xyz

[P04] 求长度
来源：http://xkb.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mle.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jej.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gxx.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lxk.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://snv.fzhhl.top

Go:   len(arr);  len(m)
来源：http://cru.jqgfzy.top

Ruby: x.length;  x.size
来源：http://rss.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ent.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://ulo.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dwm.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://toj.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baz.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ykk.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kik.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mop.sweek.top

Ruby: a == b
来源：http://bnu.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dxt.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mde.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wsz.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://npb.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wtz.daria6918.cn

TS:   if (x == null) {}
来源：http://die.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://chv.redwolf501.top

Go:   if x == nil {}
来源：http://lzw.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gpe.zycfv.cn

C#:   if (x is null) {}
来源：http://vek.epnwcf.com

[P07] 防抖与节流
来源：http://mpc.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zro.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://zwe.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ety.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://udu.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://upk.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cmb.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://keq.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bst.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://wfn.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://snp.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qcp.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zxe.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pby.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oxi.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rcr.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qyq.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fho.cheryme.top

================================================================================
来源：http://nqj.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://upl.hongshengwenyu.top

================================================================================
来源：http://bzq.sxryk.cn

[Q01] 创建表
来源：http://ndd.daria6918.cn

CREATE TABLE users (
来源：http://lth.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://req.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://dig.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://pzy.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://juv.zhiwuduotai.top

);
来源：http://hzm.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://ilo.daxiang520.top

CREATE TABLE orders (
来源：http://shw.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://peq.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://iox.52xcode.cn

amount DECIMAL(10, 2),
来源：http://brg.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qmb.xylfe.cn

);
来源：http://rfr.hammf.cn

[Q03] 增加列
来源：http://cvh.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://maf.yvedp.cn

[Q04] 修改列类型
来源：http://rrs.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ond.havefunace.top

[Q05] 重命名列
来源：http://mxu.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gat.zhongyouzk.top

[Q06] 删除列
来源：http://wbs.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://lzc.nwbrower.top

[Q07] 删除表
来源：http://qvn.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://bjq.sysykeji.top

[Q08] 创建普通索引
来源：http://uvp.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mel.yvedp.cn

[Q09] 创建唯一索引
来源：http://qwh.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ygj.zhijiandao.cn

[Q10] 插入单行
来源：http://qsh.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xvl.zhengqikj.top

[Q11] 一次插入多行
来源：http://pti.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xxw.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://yhn.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://swx.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ifc.tian-w.cn

[Q13] 忽略重复插入
来源：http://fqp.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sbt.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://dpm.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dua.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://faf.yongpay.top

[Q15] 查询全部
来源：http://kvo.hongshengwenyu.top

SELECT * FROM users;
来源：http://orb.hesvh.cn

[Q16] 查询指定列
来源：http://nle.52xcode.cn

SELECT id, name FROM users;
来源：http://uwf.hywenlv.cn

[Q17] 条件查询
来源：http://eto.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iod.yonumen.top

[Q18] 模糊匹配
来源：http://gzo.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ipw.jinqigufen.top

[Q19] 范围查询
来源：http://qzk.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gkq.jqgufenzy.top

[Q20] IN 列表
来源：http://zks.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gnv.mhx1999.top

[Q21] 空值判断
来源：http://bae.yuanzhike.top


<!-- 参考信息 -->