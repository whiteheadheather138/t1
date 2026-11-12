代发 wailian999

[N01] 二分查找（有序数组）
来源：http://yrh.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://hfl.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kgp.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npa.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mxa.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dnu.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://zok.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://qqu.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://fcd.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://yzl.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ivr.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gbb.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gqj.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://noz.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nol.aizwys.cn

Go:   slices.Sort(arr)
来源：http://wdw.birdmap.top

Ruby: arr.sort
来源：http://yzn.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vjt.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://owp.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rbe.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://kbu.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dwf.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fyp.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fjs.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ylq.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hyw.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tpg.hammf.cn

[N04] 斐波那契数列
来源：http://odf.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vna.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://knc.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pwa.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqf.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vid.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mpo.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vdx.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fgk.haohaochexian.top

[N05] 最大公约数
来源：http://yzv.sweek.top

Py:   math.gcd(a, b)
来源：http://ztk.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eil.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://arj.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovu.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ckw.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oxq.9152youxi.cn

Ruby: a.gcd(b)
来源：http://pzp.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gfq.jqgfzy.top

[N06] 判断回文字符串
来源：http://gpw.zhixingplan.top

Py:   s == s[::-1]
来源：http://lnb.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://zyp.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://xai.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://ukj.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zxa.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://jpw.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://gwf.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lbg.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://sno.yongpay.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ukd.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bee.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://btd.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://jyc.52xcode.cn

Java: // 手写 HashMap
来源：http://xvz.meibo888.top

Go:   // 手写 map[int]int
来源：http://nuc.snrcjt.cn

Ruby: // 手写 Hash
来源：http://drk.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://dyf.epnwcf.com

[N08] 生成全排列
来源：http://dle.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://gzy.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://ogi.hywenlv.cn

JS:   // 手写回溯递归
来源：http://hpr.yvedp.cn

TS:   // 手写回溯递归
来源：http://gyh.hnqzz.top

Java: // 手写回溯递归
来源：http://vfr.ehwqpu.com

Go:   // 手写回溯递归
来源：http://idu.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://jnf.smart0.xyz

C#:   // 手写回溯递归
来源：http://wfw.316326.xyz

[N09] 栈与队列
来源：http://ikg.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mrb.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ujo.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gov.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wzc.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vtw.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zmc.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zcx.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wiu.zhoulong.xyz

[N10] 链表节点定义
来源：http://xfk.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lgr.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pqp.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vkv.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://znu.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://swu.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hzv.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qar.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fmo.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://sjs.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gqz.nanxinkj.top

PHP:  // 手写递归函数
来源：http://mhy.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lav.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zkd.tanke756.top

Java: // 手写递归
来源：http://fqe.cqqwz.cn

Go:   // 手写递归
来源：http://loz.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qhk.hongshengwenyu.top

C#:   // 手写递归
来源：http://qwq.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gyn.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jeu.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xdg.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ecq.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://euv.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgn.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://chx.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yjg.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jvf.tian-w.cn

================================================================================
来源：http://kfq.kuanghao11.cn

O. 并发与异步
来源：http://fvw.wangshuangyany.cn

================================================================================
来源：http://tgs.nanxuanxn.top

[O01] 启动一个线程
来源：http://ekn.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://twq.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pue.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://urs.daria6918.cn

TS:   // 同 JS
来源：http://qtk.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://szb.gogol.net.cn

Go:   go f()
来源：http://deo.zdbjq.cn

Ruby: Thread.new { f }
来源：http://zbw.ydzc1.top

C#:   Task.Run(() => F());
来源：http://qfe.sxryk.cn

[O02] 使用线程池
来源：http://lac.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bxj.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hpo.52xcode.cn

JS:   // worker_threads 线程池
来源：http://koy.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://hkk.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://zed.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://czj.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hhy.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ofg.yonumen.top

[O03] 加锁保护共享数据
来源：http://rqb.0kj1m.cn

Py:   with lock: shared += 1
来源：http://ivo.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://ucg.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tqh.ivvv.top

TS:   // 同 JS
来源：http://pve.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://wrx.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ory.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bur.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://ouy.sweek.top

[O04] 定义异步函数并等待
来源：http://lgx.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://lef.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jxp.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://zpt.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ysd.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bsq.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vbs.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://ctk.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://mnr.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://rmu.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://jep.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rod.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://tng.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://pfg.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://frz.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dlc.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://zkc.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qab.hnxiangtu.top

[O06] 使用进程池
来源：http://pzd.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zwm.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ezr.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://kzj.meibo888.top

TS:   // child_process / cluster 模块
来源：http://dhh.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tpo.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aty.yuxming.cn

Ruby: // fork 块
来源：http://yum.0kj1m.cn

C#:   Parallel.For
来源：http://jrk.wangdashe.top

================================================================================
来源：http://cyx.sweek.top

P. 常用工具函数
来源：http://jth.epnwcf.com

================================================================================
来源：http://grk.fengsongda.top

[P01] 生成 UUID
来源：http://xlx.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://ivw.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hvq.pycfn.com

JS:   crypto.randomUUID()
来源：http://dei.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://gtt.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://bbh.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://hhk.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://qex.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://hlt.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://afp.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ppt.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kye.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iwv.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://csi.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fdr.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kqo.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dfd.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nhv.dashuyun.cn

[P03] 生成短随机字符串
来源：http://ydm.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wtq.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mms.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vxr.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pcf.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rdo.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fjv.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vtn.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://asm.pengpengdd.cyou

[P04] 求长度
来源：http://kal.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wku.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kim.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://edc.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tzq.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://cgk.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://tpk.hesvh.cn

Ruby: x.length;  x.size
来源：http://byd.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://osq.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://fqa.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ftq.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ktg.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qev.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kuw.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ekx.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://lce.epnwcf.com

Ruby: a == b
来源：http://krk.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gtd.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oxe.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tup.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://mas.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mqb.guannengcc.top

TS:   if (x == null) {}
来源：http://wcd.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://fku.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://ofq.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eqq.iojbl.cn

C#:   if (x is null) {}
来源：http://uls.nanxuanxn.top

[P07] 防抖与节流
来源：http://pll.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oxr.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://mxf.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcv.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://laj.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dhu.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kxy.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xwr.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mwb.cashguo.top

[P08] 处理浮点精度问题
来源：http://flx.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kie.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xnz.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ynu.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://emz.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lok.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qgv.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rgq.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zis.tianlin.xyz

================================================================================
来源：http://rzj.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ifi.fktsv.cn

================================================================================
来源：http://jap.jianghu66.top

[Q01] 创建表
来源：http://ajl.zycfv.cn

CREATE TABLE users (
来源：http://gyj.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kmp.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://tmb.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://kjf.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qal.yvedp.cn

);
来源：http://qkz.ppjwa.cn

[Q02] 创建带外键的表
来源：http://dhq.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://aov.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ghj.cashguo.top

user_id INT NOT NULL,
来源：http://xfe.yueranfly.top

amount DECIMAL(10, 2),
来源：http://gkk.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jrd.tanke756.top

);
来源：http://wlp.c1oappe.top

[Q03] 增加列
来源：http://oau.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jty.daria6918.cn

[Q04] 修改列类型
来源：http://dio.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pmp.hammf.cn

[Q05] 重命名列
来源：http://rdt.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ext.fktsv.cn

[Q06] 删除列
来源：http://fql.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://itu.vehdjk.com

[Q07] 删除表
来源：http://iqk.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://vav.nwbrower.top

[Q08] 创建普通索引
来源：http://nzh.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lzf.wangshuangyany.cn

[Q09] 创建唯一索引
来源：http://fky.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uoi.hcnkem.com

[Q10] 插入单行
来源：http://fdn.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://myy.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://fld.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gqu.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://ahd.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://bcg.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fgv.daxiang520.top

[Q13] 忽略重复插入
来源：http://zrl.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ocu.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://uix.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sin.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sjt.hywenlv.cn

[Q15] 查询全部
来源：http://xvn.feifeiyinyue.top

SELECT * FROM users;
来源：http://lvq.sufxvd.cn

[Q16] 查询指定列
来源：http://zub.9152youxi.cn

SELECT id, name FROM users;
来源：http://ilp.tanke756.top

[Q17] 条件查询
来源：http://xrj.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tep.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://eps.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jzr.pycfn.com

[Q19] 范围查询
来源：http://jnw.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zmo.wangdashe.top

[Q20] IN 列表
来源：http://czg.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jtc.quarkkingdee.top

[Q21] 空值判断
来源：http://pcs.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://vfc.cucudq.cn

[Q22] 排序
来源：http://bai.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iut.ctjpmb.com

[Q23] 分页
来源：http://gwt.cdnleiting.top


<!-- 参考信息 -->