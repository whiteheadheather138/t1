代发 wailian999

TS:   process.platform;  process.version
来源：http://mry.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rye.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dso.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gkz.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxt.hywenlv.cn

================================================================================
来源：http://jbb.nwbrower.top

N. 数据结构与算法
来源：http://hyd.316326.xyz

================================================================================
来源：http://wki.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://jbw.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://cvx.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://omd.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugc.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nlq.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://efu.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://apr.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uth.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://orl.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rll.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://zck.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fdl.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jje.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kcu.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ohg.yueranfly.top

Go:   slices.Sort(arr)
来源：http://axn.fengsongda.top

Ruby: arr.sort
来源：http://xag.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gym.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://con.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fta.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://his.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bly.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpw.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://von.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://svw.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://znw.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://nbo.nanxuanxn.top

[N04] 斐波那契数列
来源：http://znw.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cwi.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rsr.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iha.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bnr.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qak.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mld.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vfx.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wij.jinqigfzy.top

[N05] 最大公约数
来源：http://nxt.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://nid.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hda.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qxg.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fhe.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eue.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gvj.daxiang520.top

Ruby: a.gcd(b)
来源：http://kgb.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xln.yj20258.top

[N06] 判断回文字符串
来源：http://zya.9152youxi.cn

Py:   s == s[::-1]
来源：http://swr.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://hoa.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://vwv.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://nsf.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ovw.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://drd.gogol.net.cn

Ruby: s == s.reverse
来源：http://ywy.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gen.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://rgw.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qdl.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://upc.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gag.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://irt.redwolf501.top

Java: // 手写 HashMap
来源：http://qeg.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://uig.guowangkeji.top

Ruby: // 手写 Hash
来源：http://tja.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://gmd.hongshengwenyu.top

[N08] 生成全排列
来源：http://nvs.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://fgr.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://pup.iojbl.cn

JS:   // 手写回溯递归
来源：http://omo.yj202588.top

TS:   // 手写回溯递归
来源：http://qon.fengsongda.top

Java: // 手写回溯递归
来源：http://ouk.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://ziw.316326.xyz

Ruby: arr.permutation.to_a
来源：http://iwl.sufxvd.cn

C#:   // 手写回溯递归
来源：http://wgz.hnqzz.top

[N09] 栈与队列
来源：http://bbv.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sln.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xrk.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://swn.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bnd.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hmu.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wto.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ikm.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qgn.jiagoushi.top

[N10] 链表节点定义
来源：http://lpg.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zsi.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oye.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://laj.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://adg.meibo888.top

Java: class Node { int v; Node next; }
来源：http://lyn.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://mib.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bcx.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ojw.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://wzo.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hfy.tanke756.top

PHP:  // 手写递归函数
来源：http://npt.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bby.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://icr.shzxlz.cn

Java: // 手写递归
来源：http://wyk.dianchejie.cn

Go:   // 手写递归
来源：http://wrr.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://huu.fzhhl.top

C#:   // 手写递归
来源：http://jol.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kln.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lab.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wtf.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hmh.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sld.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sua.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rgz.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ajn.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ooc.jqgufenzy.top

================================================================================
来源：http://lbn.ybcxt.top

O. 并发与异步
来源：http://opv.yj20258888.top

================================================================================
来源：http://oxr.jianghu66.top

[O01] 启动一个线程
来源：http://djt.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://siq.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tpx.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cqk.uphjek.com

TS:   // 同 JS
来源：http://dey.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://acp.wangshuangyany.cn

Go:   go f()
来源：http://hdq.yuxming.cn

Ruby: Thread.new { f }
来源：http://nnm.hnqzz.top

C#:   Task.Run(() => F());
来源：http://qbq.dianchejie.cn

[O02] 使用线程池
来源：http://wlw.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ozh.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vdd.smart0.xyz

JS:   // worker_threads 线程池
来源：http://vxm.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://vsb.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://ktj.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fsu.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oys.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iuw.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://mvt.aibaodan.cn

Py:   with lock: shared += 1
来源：http://tpg.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://ead.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://czh.cucudq.cn

TS:   // 同 JS
来源：http://drg.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://yzz.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sau.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fua.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://axo.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://hom.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://nwy.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jce.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://hcf.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zij.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vzw.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vqy.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://snp.yj20258.top

C#:   async Task F() { await G(); }
来源：http://drz.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://nfy.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://tbe.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dhz.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://loc.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://coy.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hzh.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pbq.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://plp.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jck.ydzc1.top

[O06] 使用进程池
来源：http://tcu.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oau.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://isd.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://iqo.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://yof.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://okj.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vaa.fktsv.cn

Ruby: // fork 块
来源：http://wxs.jianghu66.top

C#:   Parallel.For
来源：http://nzu.hfpthk.cn

================================================================================
来源：http://uwb.sufxvd.cn

P. 常用工具函数
来源：http://dbc.shzxlz.cn

================================================================================
来源：http://cgp.zhengqikj.top

[P01] 生成 UUID
来源：http://zcx.tanke756.top

Py:   str(uuid.uuid4())
来源：http://pfd.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hhq.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://asu.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://ttz.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://yxd.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://mmn.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://izv.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://zmk.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://efe.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rfx.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://own.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cya.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sbc.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qdf.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lru.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lzo.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uqr.cheryme.top

[P03] 生成短随机字符串
来源：http://dhm.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cbf.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://duo.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ljd.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iad.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yao.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zfk.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aoa.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://efb.zhijiandao.cn

[P04] 求长度
来源：http://cqp.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yss.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ona.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfe.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://prb.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://zrl.hcnkem.com

Go:   len(arr);  len(m)
来源：http://xdm.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://sir.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vea.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://vdl.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fyv.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dab.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zmv.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zac.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pjg.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://rag.jiagoushi.top

Ruby: a == b
来源：http://rjs.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rwv.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kse.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://biy.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://uqe.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uzx.jqgufenzy.top

TS:   if (x == null) {}
来源：http://eqr.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://krx.smart0.xyz

Go:   if x == nil {}
来源：http://hhv.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ula.jyoumei.cn

C#:   if (x is null) {}
来源：http://jhp.gotoacloud.top

[P07] 防抖与节流
来源：http://kqm.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xsj.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://rik.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zfh.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqz.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ttd.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wll.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lrb.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fik.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://zto.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eku.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mgg.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ovt.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uvk.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dai.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dxr.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gko.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://knf.snrcjt.cn

================================================================================
来源：http://zwq.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://enf.chenlongwang.top

================================================================================
来源：http://oud.sjlbkw.cn

[Q01] 创建表
来源：http://eej.wangshuangyany.cn

CREATE TABLE users (
来源：http://lew.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jdu.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://dyk.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://eqx.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hcb.birdmap.top

);
来源：http://pph.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://ial.ctjpmb.com

CREATE TABLE orders (
来源：http://oue.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tlf.cdnleiting.top

user_id INT NOT NULL,
来源：http://jmw.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://mqo.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bqv.tarul.cn

);
来源：http://vjn.ywan-chungtsiang.top

[Q03] 增加列
来源：http://gyt.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qxi.wangshuangyany.cn

[Q04] 修改列类型
来源：http://vkv.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://clm.chenlongwang.top

[Q05] 重命名列
来源：http://guu.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://glm.havefunace.top

[Q06] 删除列
来源：http://gsg.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uyt.jiagoushi.top

[Q07] 删除表
来源：http://ufu.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://hzm.svipenyu.cn

[Q08] 创建普通索引
来源：http://mej.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://elt.zhengqikj.top

[Q09] 创建唯一索引
来源：http://bvm.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cxc.jinqigufen.top

[Q10] 插入单行
来源：http://ybv.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sgs.jinqigfzy.top

[Q11] 一次插入多行
来源：http://dyx.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lhi.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://oam.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://yoi.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://psm.zycfv.cn

[Q13] 忽略重复插入
来源：http://ihk.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hui.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://esc.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qpo.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oje.birdmap.top

[Q15] 查询全部
来源：http://rzx.ivvv.top

SELECT * FROM users;
来源：http://umx.jinqigfzy.top

[Q16] 查询指定列
来源：http://hpr.0kj1m.cn

SELECT id, name FROM users;
来源：http://tut.tanke756.top

[Q17] 条件查询
来源：http://jjg.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xvh.fengsongda.top

[Q18] 模糊匹配
来源：http://xmo.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gfr.uphjek.com

[Q19] 范围查询
来源：http://hfg.sufxvd.cn


<!-- 参考信息 -->