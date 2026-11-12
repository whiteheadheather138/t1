代发 wailian999

[N01] 二分查找（有序数组）
来源：http://vph.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fto.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hts.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://six.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dwz.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gjm.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://qan.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rgm.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://fda.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://gyk.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ded.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jjp.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fzq.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ykr.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jpe.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://fjj.hesvh.cn

Ruby: arr.sort
来源：http://gsc.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gzh.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://xzm.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://grh.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://oja.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnd.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zdb.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ihi.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ulr.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kmw.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jar.jianghu66.top

[N04] 斐波那契数列
来源：http://gub.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zkm.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rbo.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgi.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pvh.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mxy.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lgu.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tbj.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fhu.daxiang520.top

[N05] 最大公约数
来源：http://rcv.gzhubu.top

Py:   math.gcd(a, b)
来源：http://mhx.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rrw.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwr.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xjb.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cyu.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xmt.xziqi.cn

Ruby: a.gcd(b)
来源：http://xmy.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dic.sweek.top

[N06] 判断回文字符串
来源：http://vng.yfazqb.com

Py:   s == s[::-1]
来源：http://zly.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://uca.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://qsu.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://cyj.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tdc.tanke756.top

Go:   // 双指针从两端比较
来源：http://zgd.quarkkingdee.top

Ruby: s == s.reverse
来源：http://mri.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bke.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://tmz.nanxuanxn.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdg.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cpa.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vqh.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://vdg.aibaodan.cn

Java: // 手写 HashMap
来源：http://yey.shuidangran.top

Go:   // 手写 map[int]int
来源：http://vts.fzhhl.top

Ruby: // 手写 Hash
来源：http://hub.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ufr.cdnleiting.top

[N08] 生成全排列
来源：http://rfe.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://lkj.guowangkeji.top

PHP:  // 手写递归交换
来源：http://cvj.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://wwc.yueranfly.top

TS:   // 手写回溯递归
来源：http://zso.nanxinkj.top

Java: // 手写回溯递归
来源：http://pnm.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://epu.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://ptt.9152youxi.cn

C#:   // 手写回溯递归
来源：http://npo.snrcjt.cn

[N09] 栈与队列
来源：http://xdt.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aaa.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zwm.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xzw.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ynw.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nbd.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xnd.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fah.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lnq.gogol.net.cn

[N10] 链表节点定义
来源：http://lqg.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sqr.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fhr.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ncu.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zah.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://fxw.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://lhj.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ywq.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://onw.yj202588.top

[N11] 二叉树中序遍历
来源：http://zex.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qwg.nanxinkj.top

PHP:  // 手写递归函数
来源：http://bkx.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://byi.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jua.shangyingyoupin.top

Java: // 手写递归
来源：http://nxy.yuanzhike.top

Go:   // 手写递归
来源：http://rcp.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sad.quarkkingdee.top

C#:   // 手写递归
来源：http://jgx.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ija.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cxn.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ktd.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://syr.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmn.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vfk.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pxt.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wuc.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pep.epnwcf.com

================================================================================
来源：http://lbx.bbcook.cn

O. 并发与异步
来源：http://okf.guannengcc.top

================================================================================
来源：http://xlh.zdqjudy.top

[O01] 启动一个线程
来源：http://fcg.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tsz.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tjq.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ybv.havefunace.top

TS:   // 同 JS
来源：http://qgt.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://mnb.zdbjq.cn

Go:   go f()
来源：http://qti.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://srg.jianghu66.top

C#:   Task.Run(() => F());
来源：http://mto.jinqigfzy.top

[O02] 使用线程池
来源：http://wmk.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zri.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hrb.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://hfr.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://rav.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://rdu.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vrj.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rdb.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zco.sxryk.cn

[O03] 加锁保护共享数据
来源：http://xvp.9152youxi.cn

Py:   with lock: shared += 1
来源：http://yoi.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://rlm.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ywd.ivvv.top

TS:   // 同 JS
来源：http://qor.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://svc.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ofv.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ccf.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://rwk.wangdashe.top

[O04] 定义异步函数并等待
来源：http://riq.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://iea.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vil.redwolf501.top

JS:   async function f() { await g(); }
来源：http://mru.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://exf.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hle.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zls.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://rwi.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://qjo.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://yxm.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://krx.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cet.yonumen.top

JS:   await Promise.all(tasks)
来源：http://ryh.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://lgz.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zyl.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gpr.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://qit.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lgq.bbcook.cn

[O06] 使用进程池
来源：http://xwd.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aqp.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://tls.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://uet.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://eon.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fmw.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cpo.gotoacloud.top

Ruby: // fork 块
来源：http://jtr.316326.xyz

C#:   Parallel.For
来源：http://amm.0kj1m.cn

================================================================================
来源：http://vtm.jinqigufen.top

P. 常用工具函数
来源：http://hfk.xuanzx.com

================================================================================
来源：http://nas.iojbl.cn

[P01] 生成 UUID
来源：http://kyf.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://xtx.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cii.yfazqb.com

JS:   crypto.randomUUID()
来源：http://wpd.mhx1999.top

TS:   crypto.randomUUID()
来源：http://vqr.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://mmn.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://tpc.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://rwz.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://hhc.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://heu.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wml.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sbp.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ylv.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tqk.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fuo.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://chi.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kda.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://msc.bbcook.cn

[P03] 生成短随机字符串
来源：http://ynz.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://chg.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cav.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hiz.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xug.zhongyouzk.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gan.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ias.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xvk.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hnz.hongshengwenyu.top

[P04] 求长度
来源：http://ilr.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nge.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kee.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vly.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hmu.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://spl.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://jyr.guannengcc.top

Ruby: x.length;  x.size
来源：http://oxv.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xal.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://pdi.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://goj.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hnw.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tdc.fktsv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://axn.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tof.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://yww.hesvh.cn

Ruby: a == b
来源：http://blx.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wwz.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jgw.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://drw.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://wgx.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cxq.xylfe.cn

TS:   if (x == null) {}
来源：http://ghn.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bhs.cqqwz.cn

Go:   if x == nil {}
来源：http://rxx.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ybu.fehbvm.com

C#:   if (x is null) {}
来源：http://tbm.tarul.cn

[P07] 防抖与节流
来源：http://des.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bbi.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://nzx.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://olg.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvy.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qiq.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gch.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dvi.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://spm.vehdjk.com

[P08] 处理浮点精度问题
来源：http://pij.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wak.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bai.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bue.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gxw.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vnk.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ybj.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gix.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://knt.ywan-chungtsiang.top

================================================================================
来源：http://jtn.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://apn.ehwqpu.com

================================================================================
来源：http://ibf.yanxiufei.cn

[Q01] 创建表
来源：http://uze.gogol.net.cn

CREATE TABLE users (
来源：http://hvg.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmn.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://cbx.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://ldj.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zwu.xuanzx.com

);
来源：http://zsx.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://wtz.quarkkingdee.top

CREATE TABLE orders (
来源：http://iny.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmb.vqdsnc.cn

user_id INT NOT NULL,
来源：http://dov.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://uvk.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tzi.xziqi.cn

);
来源：http://zvx.feifeiyinyue.top

[Q03] 增加列
来源：http://ced.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yxd.zhixingplan.top

[Q04] 修改列类型
来源：http://ljp.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://smt.dianchejie.cn

[Q05] 重命名列
来源：http://kky.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ytp.ehwqpu.com

[Q06] 删除列
来源：http://pft.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://iov.wangshuangyany.cn

[Q07] 删除表
来源：http://vct.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://bek.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://yxh.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dpj.tianlin.xyz

[Q09] 创建唯一索引
来源：http://ple.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pry.yongpay.top

[Q10] 插入单行
来源：http://xgv.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bgg.iojbl.cn

[Q11] 一次插入多行
来源：http://iio.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rbz.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://oib.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://zbo.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fah.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://zgt.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rkp.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://rxp.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gln.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sna.smart0.xyz

[Q15] 查询全部
来源：http://xss.zhoulong.xyz

SELECT * FROM users;
来源：http://mlr.ybcxt.top

[Q16] 查询指定列
来源：http://ebk.cqqwz.cn

SELECT id, name FROM users;
来源：http://yyx.zhoulong.xyz

[Q17] 条件查询
来源：http://trs.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dqd.hysaishi.cn

[Q18] 模糊匹配
来源：http://wga.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://izk.yj20258888.top

[Q19] 范围查询
来源：http://fpl.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://opd.jiagoushi.top

[Q20] IN 列表
来源：http://lvh.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://txk.sufxvd.cn

[Q21] 空值判断
来源：http://jbn.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gba.chenlongwang.top

[Q22] 排序
来源：http://apm.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xhk.gzhubu.top

[Q23] 分页
来源：http://uxp.iojbl.cn


<!-- 参考信息 -->