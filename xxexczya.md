代发 wailian999

[N01] 二分查找（有序数组）
来源：http://osn.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://cal.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nhn.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kqx.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://osq.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://wvm.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://ijy.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://pnv.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ohz.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://fna.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://dqq.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kpk.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvh.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://roo.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xxm.yuxming.cn

Go:   slices.Sort(arr)
来源：http://bvd.sysykeji.top

Ruby: arr.sort
来源：http://voi.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://itb.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://lpc.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mek.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://iaf.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qpi.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hhf.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yim.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fym.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ruj.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://lvo.tianlin.xyz

[N04] 斐波那契数列
来源：http://zfr.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ptf.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wde.ydzc1.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jdk.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehb.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vkb.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://miu.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hvw.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bju.chenjidiqi.icu

[N05] 最大公约数
来源：http://dng.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://ijs.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lpb.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dji.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ybd.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://drw.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ibh.yueranfly.top

Ruby: a.gcd(b)
来源：http://myt.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pnl.52xcode.cn

[N06] 判断回文字符串
来源：http://vwe.bbcook.cn

Py:   s == s[::-1]
来源：http://ykq.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://cfe.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://ewk.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://nlh.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jcv.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://bno.daxiang520.top

Ruby: s == s.reverse
来源：http://nkp.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pau.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://hgn.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njs.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uxo.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zmx.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://pgi.smart0.xyz

Java: // 手写 HashMap
来源：http://gtg.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://mac.hnqzz.top

Ruby: // 手写 Hash
来源：http://qtq.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rml.chenzaomai.com

[N08] 生成全排列
来源：http://rlh.meibo888.top

Py:   itertools.permutations(arr)
来源：http://qat.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://bfr.c1oappe.top

JS:   // 手写回溯递归
来源：http://vzl.cashguo.top

TS:   // 手写回溯递归
来源：http://jvm.aizwys.cn

Java: // 手写回溯递归
来源：http://anx.yj20258888.top

Go:   // 手写回溯递归
来源：http://aac.yongpay.top

Ruby: arr.permutation.to_a
来源：http://zoj.ppjwa.cn

C#:   // 手写回溯递归
来源：http://ofb.9152youxi.cn

[N09] 栈与队列
来源：http://akv.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mhq.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://clb.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mbj.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qnk.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jrr.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oon.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uxx.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cqs.chenzaomai.com

[N10] 链表节点定义
来源：http://yjw.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ceg.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xrc.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cns.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jyz.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://hqu.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://fjk.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tib.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lzb.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://myr.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://icy.shzxlz.cn

PHP:  // 手写递归函数
来源：http://dnw.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oiw.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usf.guowangkeji.top

Java: // 手写递归
来源：http://opf.jqgfzy.top

Go:   // 手写递归
来源：http://hto.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yea.hongshengwenyu.top

C#:   // 手写递归
来源：http://utr.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mbo.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hiy.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ncq.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sxs.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://usr.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ayd.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mcv.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dop.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rjs.fanxiaobao.xyz

================================================================================
来源：http://ycl.zhoulong.xyz

O. 并发与异步
来源：http://duo.daxiang520.top

================================================================================
来源：http://sty.yuanzhike.top

[O01] 启动一个线程
来源：http://hcw.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iwd.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yrp.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xgx.ppjwa.cn

TS:   // 同 JS
来源：http://aol.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://agr.jinqigfzy.top

Go:   go f()
来源：http://olu.hammf.cn

Ruby: Thread.new { f }
来源：http://tgv.xziqi.cn

C#:   Task.Run(() => F());
来源：http://ufe.ydzc1.top

[O02] 使用线程池
来源：http://put.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mhr.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nwc.tarul.cn

JS:   // worker_threads 线程池
来源：http://edj.hcnkem.com

TS:   // worker_threads 线程池
来源：http://yuc.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yel.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ymb.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qpe.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xgx.jianghu66.top

[O03] 加锁保护共享数据
来源：http://vxm.zycfv.cn

Py:   with lock: shared += 1
来源：http://bic.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://tdp.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fkx.zhiwuduotai.top

TS:   // 同 JS
来源：http://xvp.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://ftd.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tno.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oof.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://ulw.tarul.cn

[O04] 定义异步函数并等待
来源：http://mrd.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://hvr.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fnj.epnwcf.com

JS:   async function f() { await g(); }
来源：http://upa.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://utq.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lvj.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zuq.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yfm.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://vpc.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://wul.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://wxz.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fxc.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://gzn.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://ina.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bxc.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bjb.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://bzm.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fgd.guannengcc.top

[O06] 使用进程池
来源：http://ohc.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uak.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rqp.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://zdk.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://cme.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://upd.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zkk.yuxming.cn

Ruby: // fork 块
来源：http://exb.hammf.cn

C#:   Parallel.For
来源：http://kfp.aibaodan.cn

================================================================================
来源：http://oqn.yuanzhike.top

P. 常用工具函数
来源：http://fzk.epnwcf.com

================================================================================
来源：http://qke.jiagoushi.top

[P01] 生成 UUID
来源：http://cwc.sweek.top

Py:   str(uuid.uuid4())
来源：http://qax.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://msu.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://yoe.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://mik.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://rrz.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://asn.cheryme.top

Ruby: SecureRandom.uuid
来源：http://xby.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://lya.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://zgb.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ltv.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wvx.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hpi.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vet.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://geb.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cmg.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sdc.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lyi.yfazqb.com

[P03] 生成短随机字符串
来源：http://qbj.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vvj.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xth.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://avb.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jbh.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://scl.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dxh.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ppa.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hom.shangyingyoupin.top

[P04] 求长度
来源：http://cqr.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zfh.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://koq.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cbt.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfn.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://zga.gzhubu.top

Go:   len(arr);  len(m)
来源：http://jgp.jiagoushi.top

Ruby: x.length;  x.size
来源：http://fgv.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://hgf.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://qrj.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dtn.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kbl.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://utt.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hru.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vyw.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://iaq.nanxinkj.top

Ruby: a == b
来源：http://ttl.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cgb.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ucq.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fhk.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://xzc.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ztj.yuanzhike.top

TS:   if (x == null) {}
来源：http://ewv.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://enw.zhixingplan.top

Go:   if x == nil {}
来源：http://yky.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sxm.jqgufenzy.top

C#:   if (x is null) {}
来源：http://rut.yuxming.cn

[P07] 防抖与节流
来源：http://ylv.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dnd.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://jrr.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsg.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibd.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cfd.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yyf.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mll.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qqp.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://icx.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bkz.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rjo.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xkh.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://itw.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wdf.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wuf.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pei.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mjk.snrcjt.cn

================================================================================
来源：http://vno.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fnt.daria6918.cn

================================================================================
来源：http://fqy.hnxiangtu.top

[Q01] 创建表
来源：http://ddh.shangyingyoupin.top

CREATE TABLE users (
来源：http://mxx.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lym.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://egt.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://wtx.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rzw.pengpengdd.cyou

);
来源：http://yyw.316326.xyz

[Q02] 创建带外键的表
来源：http://gif.jqgfzy.top

CREATE TABLE orders (
来源：http://kto.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rzo.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://ptx.fktsv.cn

amount DECIMAL(10, 2),
来源：http://tmp.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://klp.guowangkeji.top

);
来源：http://sqy.zhiwuduotai.top

[Q03] 增加列
来源：http://klr.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://abt.cashguo.top

[Q04] 修改列类型
来源：http://wck.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://chi.zdqjudy.top

[Q05] 重命名列
来源：http://qmn.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ghp.sweek.top

[Q06] 删除列
来源：http://cna.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ooh.hywenlv.cn

[Q07] 删除表
来源：http://fok.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://fat.hfpthk.cn

[Q08] 创建普通索引
来源：http://ebe.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://sqf.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://phh.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qtu.tian-w.cn

[Q10] 插入单行
来源：http://gnf.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tsv.pycfn.com

[Q11] 一次插入多行
来源：http://rwu.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aqw.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://how.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://jtf.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oss.yj202588.top

[Q13] 忽略重复插入
来源：http://xni.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://grf.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://pjz.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vih.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uoe.yanxiufei.cn

[Q15] 查询全部
来源：http://rau.meibo888.top

SELECT * FROM users;
来源：http://frv.yueranfly.top

[Q16] 查询指定列
来源：http://cjb.pycfn.com

SELECT id, name FROM users;
来源：http://cku.sufxvd.cn

[Q17] 条件查询
来源：http://lyk.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qxe.jlsjyb.cn

[Q18] 模糊匹配
来源：http://flm.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nie.aibaodan.cn

[Q19] 范围查询
来源：http://kyo.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://unj.ctjpmb.com

[Q20] IN 列表
来源：http://lyd.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nkw.vqdsnc.cn

[Q21] 空值判断
来源：http://lwf.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kaa.feifeiyinyue.top

[Q22] 排序
来源：http://rqa.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zud.ctjpmb.com

[Q23] 分页
来源：http://jbm.wangdashe.top


<!-- 参考信息 -->