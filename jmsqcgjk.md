代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xla.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://har.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://byf.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vtc.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://dvq.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://got.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://wvl.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ttb.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rtl.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ohr.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dst.bjfxy.top

Go:   slices.Sort(arr)
来源：http://dlt.nwbrower.top

Ruby: arr.sort
来源：http://fvm.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wts.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://fec.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gas.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://eow.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xpf.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kjw.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ryl.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lsz.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ogr.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sko.shuidangran.top

[N04] 斐波那契数列
来源：http://bde.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dxd.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wft.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tqc.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zxh.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ltt.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qog.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tkh.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hhd.zhongyouzk.top

[N05] 最大公约数
来源：http://wjn.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://vff.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uta.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://twv.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wva.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mfa.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uvb.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://ohu.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://erq.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://owx.tanke756.top

Py:   s == s[::-1]
来源：http://ysz.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://dej.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://cna.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://mdk.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nzn.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://wlm.sufxvd.cn

Ruby: s == s.reverse
来源：http://tff.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fgn.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://ypc.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gwr.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xhv.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gom.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://jui.vqdsnc.cn

Java: // 手写 HashMap
来源：http://qpm.fzhhl.top

Go:   // 手写 map[int]int
来源：http://kct.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://xfg.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jro.jinqigufen.top

[N08] 生成全排列
来源：http://eub.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://wgy.xziqi.cn

PHP:  // 手写递归交换
来源：http://kwc.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://vel.52xcode.cn

TS:   // 手写回溯递归
来源：http://fqs.wangdashe.top

Java: // 手写回溯递归
来源：http://kao.jinqigufen.top

Go:   // 手写回溯递归
来源：http://pgq.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://wgq.gotoacloud.top

C#:   // 手写回溯递归
来源：http://gfn.aizwys.cn

[N09] 栈与队列
来源：http://vti.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eoh.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ewx.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kzp.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://opr.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://etf.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hkz.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nfb.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://otl.hysaishi.cn

[N10] 链表节点定义
来源：http://vfq.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ueu.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ovt.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://trf.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yag.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://jgq.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://dzc.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hec.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xyr.tian-w.cn

[N11] 二叉树中序遍历
来源：http://wil.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kbu.vehdjk.com

PHP:  // 手写递归函数
来源：http://cjd.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uvu.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzr.yonumen.top

Java: // 手写递归
来源：http://pns.fzhhl.top

Go:   // 手写递归
来源：http://svp.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sum.hongshengwenyu.top

C#:   // 手写递归
来源：http://wmk.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cir.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mja.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://npv.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wif.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggu.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mbj.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ree.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eox.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dki.hesvh.cn

================================================================================
来源：http://eqq.pengpengdd.cyou

O. 并发与异步
来源：http://irr.birdmap.top

================================================================================
来源：http://rry.zhixingplan.top

[O01] 启动一个线程
来源：http://nll.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mbu.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://atv.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://exb.wangshuangyany.cn

TS:   // 同 JS
来源：http://vxd.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://fqh.hnxiangtu.top

Go:   go f()
来源：http://gbu.yj202588.top

Ruby: Thread.new { f }
来源：http://rms.yfazqb.com

C#:   Task.Run(() => F());
来源：http://baz.shuidangran.top

[O02] 使用线程池
来源：http://ovy.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://afh.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ruz.birdmap.top

JS:   // worker_threads 线程池
来源：http://nbe.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://jbb.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iox.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bre.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hwp.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wxf.tian-w.cn

[O03] 加锁保护共享数据
来源：http://cyd.hfpthk.cn

Py:   with lock: shared += 1
来源：http://uji.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://bjy.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jks.epnwcf.com

TS:   // 同 JS
来源：http://tgx.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://fqh.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://riz.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gcq.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://xwx.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://wuu.birdmap.top

Py:   async def f():⏎    await g()
来源：http://brw.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vjo.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://tea.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hyq.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aoi.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aai.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://rrh.cashguo.top

C#:   async Task F() { await G(); }
来源：http://chv.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://ddt.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://tln.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cxf.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://cat.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://rvm.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hcv.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gkk.yongpay.top

Ruby: threads.map(&:join)
来源：http://iaz.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ldt.tianlin.xyz

[O06] 使用进程池
来源：http://kir.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xtr.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mzy.yj20258.top

JS:   // child_process / cluster 模块
来源：http://qbd.sweek.top

TS:   // child_process / cluster 模块
来源：http://uvi.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eub.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dfp.tian-w.cn

Ruby: // fork 块
来源：http://mxx.sxryk.cn

C#:   Parallel.For
来源：http://sar.snrcjt.cn

================================================================================
来源：http://pmw.feifeiyinyue.top

P. 常用工具函数
来源：http://jju.aizwys.cn

================================================================================
来源：http://ddw.tarul.cn

[P01] 生成 UUID
来源：http://fpe.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://ywm.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://csi.xziqi.cn

JS:   crypto.randomUUID()
来源：http://apr.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://wyn.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://sqp.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://ctr.ivvv.top

Ruby: SecureRandom.uuid
来源：http://acq.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://kip.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://aij.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ixf.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rvx.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ulf.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://keu.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mso.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xae.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rwi.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://okr.nwbrower.top

[P03] 生成短随机字符串
来源：http://ejs.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bba.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wdy.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ynm.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://glx.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uif.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ixb.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qvt.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lvq.aibaodan.cn

[P04] 求长度
来源：http://vdl.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vpk.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rsj.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tbj.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fdn.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://oqb.jyoumei.cn

Go:   len(arr);  len(m)
来源：http://gfa.yvedp.cn

Ruby: x.length;  x.size
来源：http://gtn.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://znq.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://svk.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pfs.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dyn.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tbt.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fyd.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mux.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://vvg.pengpengdd.cyou

Ruby: a == b
来源：http://cah.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lvu.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://riu.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iak.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://beq.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://noy.fehbvm.com

TS:   if (x == null) {}
来源：http://nqu.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://knv.quarkkingdee.top

Go:   if x == nil {}
来源：http://lvm.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nha.nanxuanxn.top

C#:   if (x is null) {}
来源：http://fgr.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://vgf.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hmr.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://vsh.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eta.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qzx.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://way.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fyz.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lvq.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://flz.epnwcf.com

[P08] 处理浮点精度问题
来源：http://rou.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zgr.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://and.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jeq.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xgz.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lqq.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zxq.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cqc.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wqr.zdqjudy.top

================================================================================
来源：http://oiz.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zvg.aibaodan.cn

================================================================================
来源：http://ymg.yueranfly.top

[Q01] 创建表
来源：http://kpq.chenlongwang.top

CREATE TABLE users (
来源：http://jlo.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sya.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://wbe.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://mqt.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xpt.bbcook.cn

);
来源：http://zqm.316326.xyz

[Q02] 创建带外键的表
来源：http://acg.sjlbkw.cn

CREATE TABLE orders (
来源：http://ntp.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wti.yj20258888.top

user_id INT NOT NULL,
来源：http://rab.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://iie.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tqg.tian-w.cn

);
来源：http://vax.ehwqpu.com

[Q03] 增加列
来源：http://kkq.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jve.hongshengwenyu.top

[Q04] 修改列类型
来源：http://nxm.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nde.smart0.xyz

[Q05] 重命名列
来源：http://zuo.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tik.hnxiangtu.top

[Q06] 删除列
来源：http://lmh.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://yfe.zhijiandao.cn

[Q07] 删除表
来源：http://jtf.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://iht.yueranfly.top

[Q08] 创建普通索引
来源：http://orr.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rht.jyoumei.cn

[Q09] 创建唯一索引
来源：http://rdp.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vte.xuanzx.com

[Q10] 插入单行
来源：http://hky.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zht.0kj1m.cn

[Q11] 一次插入多行
来源：http://jfc.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sth.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://zdm.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://slr.nwbrower.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hgk.yfazqb.com

[Q13] 忽略重复插入
来源：http://opa.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bpe.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://gpr.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oud.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wjp.tanke756.top

[Q15] 查询全部
来源：http://brx.guannengcc.top

SELECT * FROM users;
来源：http://xre.yj20258.top

[Q16] 查询指定列
来源：http://flf.daria6918.cn

SELECT id, name FROM users;
来源：http://wpr.sufxvd.cn

[Q17] 条件查询
来源：http://fwp.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://arx.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://toj.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jjb.tanke756.top

[Q19] 范围查询
来源：http://yzl.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://and.birdmap.top

[Q20] IN 列表
来源：http://mla.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vsg.zhongyouzk.top

[Q21] 空值判断
来源：http://dij.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bjm.redwolf501.top

[Q22] 排序
来源：http://nux.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aza.pycfn.com

[Q23] 分页
来源：http://iri.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ubh.daria6918.cn

[Q24] 去重
来源：http://iyc.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://ime.zhengqikj.top

[Q25] 只取前 N 条
来源：http://knd.cucudq.cn


<!-- 参考信息 -->