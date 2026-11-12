代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwy.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eyq.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://pvi.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vwi.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://nbq.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://ftk.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://mta.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lql.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ceb.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xdb.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qfz.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://jul.316326.xyz

Ruby: arr.sort
来源：http://fbz.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qwj.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://isu.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yek.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://plu.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogu.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://csz.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cli.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://roa.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uem.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ktd.hesvh.cn

[N04] 斐波那契数列
来源：http://ojw.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uda.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mph.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acj.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwt.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rbk.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://stt.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vgw.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://por.tarul.cn

[N05] 最大公约数
来源：http://hmx.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://cvo.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ddj.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edq.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aax.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jau.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://juw.dianchejie.cn

Ruby: a.gcd(b)
来源：http://cxr.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://apg.tianlin.xyz

[N06] 判断回文字符串
来源：http://abj.hfpthk.cn

Py:   s == s[::-1]
来源：http://qsn.shuidangran.top

PHP:  $s === strrev($s);
来源：http://epg.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://upj.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://unr.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://can.gzhubu.top

Go:   // 双指针从两端比较
来源：http://xpa.fehbvm.com

Ruby: s == s.reverse
来源：http://cij.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lry.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://zzp.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uef.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dhx.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://yfp.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://unf.tianlin.xyz

Java: // 手写 HashMap
来源：http://khz.pycfn.com

Go:   // 手写 map[int]int
来源：http://btu.sysykeji.top

Ruby: // 手写 Hash
来源：http://tvl.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://gid.sjlbkw.cn

[N08] 生成全排列
来源：http://boz.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://key.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://ezv.hesvh.cn

JS:   // 手写回溯递归
来源：http://dvm.hywenlv.cn

TS:   // 手写回溯递归
来源：http://ruz.chenzaomai.com

Java: // 手写回溯递归
来源：http://ssb.yj20258888.top

Go:   // 手写回溯递归
来源：http://icn.meibo888.top

Ruby: arr.permutation.to_a
来源：http://oxf.aizwys.cn

C#:   // 手写回溯递归
来源：http://fce.vehdjk.com

[N09] 栈与队列
来源：http://bia.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lrd.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mtk.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uuh.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jzg.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iku.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ppy.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cvz.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jeb.316326.xyz

[N10] 链表节点定义
来源：http://wwo.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xkq.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://frm.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lte.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://azv.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://vil.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bnd.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://elx.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oou.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://hqd.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uvn.gzhubu.top

PHP:  // 手写递归函数
来源：http://lii.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qub.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqi.daria6918.cn

Java: // 手写递归
来源：http://iws.sjlbkw.cn

Go:   // 手写递归
来源：http://ihw.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mnx.jinqigufen.top

C#:   // 手写递归
来源：http://bel.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mkl.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hqu.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uie.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nzr.pycfn.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpd.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://abp.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qzw.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yyd.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aqq.shangyingyoupin.top

================================================================================
来源：http://cxt.zdqjudy.top

O. 并发与异步
来源：http://mmu.ppjwa.cn

================================================================================
来源：http://vac.aizwys.cn

[O01] 启动一个线程
来源：http://job.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lri.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uzn.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://suk.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://tug.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://pga.haohaochexian.top

Go:   go f()
来源：http://plw.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://qjf.uphjek.com

C#:   Task.Run(() => F());
来源：http://cyj.jqgufenzy.top

[O02] 使用线程池
来源：http://eyj.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hce.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gvs.pycfn.com

JS:   // worker_threads 线程池
来源：http://xlj.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://zgf.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://djn.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pwi.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qih.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kye.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://evv.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://xhr.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://qga.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kmk.tarul.cn

TS:   // 同 JS
来源：http://yit.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://iak.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hnp.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://myk.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://laj.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://jeh.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://dea.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zbs.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://kbo.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rbe.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xhb.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nmn.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://gnh.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://ujd.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://ynn.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://ssk.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://myg.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://med.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://vuq.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rnb.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yos.ywan-chungtsiang.top

Ruby: threads.map(&:join)
来源：http://lki.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ogp.yanxiufei.cn

[O06] 使用进程池
来源：http://qfr.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://miv.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zol.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://snr.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://aww.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xot.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qzz.tarul.cn

Ruby: // fork 块
来源：http://fjn.andypj.xyz

C#:   Parallel.For
来源：http://ija.tanke756.top

================================================================================
来源：http://vtn.xinyue.icu

P. 常用工具函数
来源：http://bny.vehdjk.com

================================================================================
来源：http://dii.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://ylw.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://sus.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bak.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://bbn.sxryk.cn

TS:   crypto.randomUUID()
来源：http://yuf.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://xcw.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://xpt.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://fce.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://mri.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://vab.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wlq.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rbq.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zug.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gfu.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cvd.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ivp.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ysa.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bng.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://qoq.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gbk.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://esz.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nse.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tqs.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cmx.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://trj.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nxm.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ipu.yuxming.cn

[P04] 求长度
来源：http://iip.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dnm.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwu.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://war.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cqm.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://ozw.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://ksi.dashuyun.cn

Ruby: x.length;  x.size
来源：http://iyr.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://git.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://adq.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dfx.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fzd.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ltj.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lpv.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wan.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gue.xuetiantiany.cn

Ruby: a == b
来源：http://htu.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yiz.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dxd.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pky.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://icz.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iyb.nwbrower.top

TS:   if (x == null) {}
来源：http://dvl.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://raf.pengpengdd.cyou

Go:   if x == nil {}
来源：http://yks.hammf.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tjo.jianghu66.top

C#:   if (x is null) {}
来源：http://wof.wangdashe.top

[P07] 防抖与节流
来源：http://lyg.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tav.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://qfz.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywi.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqt.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dfd.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://phm.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kei.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://psq.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://tcy.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zwh.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hvv.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hqm.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hlb.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sgl.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pmj.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hhs.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sff.zhixingplan.top

================================================================================
来源：http://khl.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ubf.zdqjudy.top

================================================================================
来源：http://nuw.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://zza.yvedp.cn

CREATE TABLE users (
来源：http://pzh.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zzy.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://rpf.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://wdj.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fcj.mhx1999.top

);
来源：http://cya.andypj.xyz

[Q02] 创建带外键的表
来源：http://lll.guannengcc.top

CREATE TABLE orders (
来源：http://fpg.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lht.zhengqikj.top

user_id INT NOT NULL,
来源：http://piq.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://spc.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fra.hnxiangtu.top

);
来源：http://edm.52xcode.cn

[Q03] 增加列
来源：http://wyu.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gxa.shangyingyoupin.top

[Q04] 修改列类型
来源：http://tqj.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jan.hammf.cn

[Q05] 重命名列
来源：http://scf.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qvj.pycfn.com

[Q06] 删除列
来源：http://nmv.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zrt.nanxuanxn.top

[Q07] 删除表
来源：http://jur.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://taz.yongpay.top

[Q08] 创建普通索引
来源：http://jfl.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ucn.nanxinkj.top

[Q09] 创建唯一索引
来源：http://nwc.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zhm.shanyushiyangtech.top

[Q10] 插入单行
来源：http://rlt.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mya.fzhhl.top

[Q11] 一次插入多行
来源：http://iic.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kxu.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://wjp.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://yjl.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cic.yuxming.cn

[Q13] 忽略重复插入
来源：http://vyf.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vxi.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://rns.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oxg.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://djt.jiagoushi.top

[Q15] 查询全部
来源：http://vqw.ivvv.top

SELECT * FROM users;
来源：http://dpb.zhoulong.xyz

[Q16] 查询指定列
来源：http://idi.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://pbf.xuetiantiany.cn

[Q17] 条件查询
来源：http://gzi.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dgz.zhongyouzk.top

[Q18] 模糊匹配
来源：http://yit.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://auw.316326.xyz

[Q19] 范围查询
来源：http://zqt.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tfn.hnqzz.top

[Q20] IN 列表
来源：http://haf.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cxm.zdbjq.cn

[Q21] 空值判断
来源：http://jfo.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hju.hywenlv.cn

[Q22] 排序
来源：http://kly.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mff.fktsv.cn

[Q23] 分页
来源：http://pld.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oxx.dashuyun.cn

[Q24] 去重
来源：http://qpx.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://amv.pycfn.com

[Q25] 只取前 N 条
来源：http://iwp.chenzaomai.com


<!-- 参考信息 -->