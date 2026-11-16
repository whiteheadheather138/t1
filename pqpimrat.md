代发 wailian999

TS:   process.platform;  process.version
来源：http://bjt.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://erd.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qxi.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ybc.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ndl.dianchejie.cn

================================================================================
来源：http://zwa.shangyingyoupin.top

N. 数据结构与算法
来源：http://enj.yongpay.top

================================================================================
来源：http://vua.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://tly.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://jig.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mgb.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rcl.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xvc.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://crt.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://lyt.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hpx.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nfh.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://wgo.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://log.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iqy.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bgz.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fsu.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uhk.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://sfu.nanxinkj.top

Ruby: arr.sort
来源：http://sad.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dkd.tarul.cn

[N03] 快速排序（分治示例）
来源：http://ijc.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dwg.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://gpt.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rgd.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aaq.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://soa.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cfl.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vkj.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://pvy.nanxuanxn.top

[N04] 斐波那契数列
来源：http://fjy.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wsu.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fix.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qrk.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iwc.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eur.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yjb.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iwi.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nis.sufxvd.cn

[N05] 最大公约数
来源：http://ldu.ydzc1.top

Py:   math.gcd(a, b)
来源：http://yky.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ogt.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmu.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uqy.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jns.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vms.shzxlz.cn

Ruby: a.gcd(b)
来源：http://xxb.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ncb.tian-w.cn

[N06] 判断回文字符串
来源：http://bae.jiagoushi.top

Py:   s == s[::-1]
来源：http://odn.tanke756.top

PHP:  $s === strrev($s);
来源：http://ljz.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://cdc.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://gmr.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zcq.wangdashe.top

Go:   // 双指针从两端比较
来源：http://gag.fktsv.cn

Ruby: s == s.reverse
来源：http://lwx.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://qse.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://dgm.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jmd.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jys.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://yae.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://gqo.0kj1m.cn

Java: // 手写 HashMap
来源：http://dvo.aizwys.cn

Go:   // 手写 map[int]int
来源：http://gwf.redwolf501.top

Ruby: // 手写 Hash
来源：http://zlc.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://lci.chenlongwang.top

[N08] 生成全排列
来源：http://jhx.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://iur.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://dsk.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://jyj.sweek.top

TS:   // 手写回溯递归
来源：http://rof.hcnkem.com

Java: // 手写回溯递归
来源：http://eta.mhx1999.top

Go:   // 手写回溯递归
来源：http://zhk.meibo888.top

Ruby: arr.permutation.to_a
来源：http://dle.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://voh.wangdashe.top

[N09] 栈与队列
来源：http://iat.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hdf.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://neg.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hzh.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fvi.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rwx.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kzk.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tkz.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qtz.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://sit.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://guo.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://opa.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://phe.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sjp.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://azb.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://kmv.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://djp.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lrq.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://rdl.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mqj.svipenyu.cn

PHP:  // 手写递归函数
来源：http://upc.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gke.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vtq.dianchejie.cn

Java: // 手写递归
来源：http://mjx.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://ywn.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ytg.hcnkem.com

C#:   // 手写递归
来源：http://aox.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wpv.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hus.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bvi.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfr.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ifg.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://edb.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fkx.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://faz.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yfy.zdqjudy.top

================================================================================
来源：http://vrj.shanyushiyangtech.top

O. 并发与异步
来源：http://nyb.havefunace.top

================================================================================
来源：http://bqj.quarkkingdee.top

[O01] 启动一个线程
来源：http://vix.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bag.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://igi.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wcu.vehdjk.com

TS:   // 同 JS
来源：http://jbo.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://vif.dianchejie.cn

Go:   go f()
来源：http://egp.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://ciu.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://oea.pengpengdd.cyou

[O02] 使用线程池
来源：http://boh.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jch.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hdf.cucudq.cn

JS:   // worker_threads 线程池
来源：http://tak.hcnkem.com

TS:   // worker_threads 线程池
来源：http://iua.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uql.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jzu.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qiq.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://amz.xinyue.icu

[O03] 加锁保护共享数据
来源：http://ryw.guowangkeji.top

Py:   with lock: shared += 1
来源：http://xip.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://nil.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qpj.zhongyouzk.top

TS:   // 同 JS
来源：http://aet.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://tie.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fdd.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://stk.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://ihe.smart0.xyz

[O04] 定义异步函数并等待
来源：http://zto.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://ouo.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pbi.fengsongda.top

JS:   async function f() { await g(); }
来源：http://wgt.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nab.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jps.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fxj.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://lro.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://xgo.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://ohd.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://zic.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hpu.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://rvp.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://wxd.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://olo.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vyx.hammf.cn

Ruby: threads.map(&:join)
来源：http://pac.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hft.hammf.cn

[O06] 使用进程池
来源：http://ono.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvx.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oaq.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://kan.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://okc.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rba.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xod.zhixingplan.top

Ruby: // fork 块
来源：http://rbf.yj20258.top

C#:   Parallel.For
来源：http://dce.dashuyun.cn

================================================================================
来源：http://ohg.jinyuanbaomall.cn

P. 常用工具函数
来源：http://ulr.daria6918.cn

================================================================================
来源：http://kmz.iojbl.cn

[P01] 生成 UUID
来源：http://qkw.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://yfe.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ock.fzhhl.top

JS:   crypto.randomUUID()
来源：http://exm.cheryme.top

TS:   crypto.randomUUID()
来源：http://cbt.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://eam.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://jae.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://dfq.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://tsv.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://atk.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://boh.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vkt.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xvl.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://auk.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ewz.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pru.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nqo.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zaf.jianghu66.top

[P03] 生成短随机字符串
来源：http://yji.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://liw.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uuj.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cpu.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://joy.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kkc.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ztt.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://duz.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://spb.dianchejie.cn

[P04] 求长度
来源：http://rai.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rff.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ujx.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ddq.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jus.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://ajl.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://xjn.yueranfly.top

Ruby: x.length;  x.size
来源：http://isu.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ary.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://gsl.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qgh.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cml.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mpx.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://thc.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jyc.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://ekn.jqgufenzy.top

Ruby: a == b
来源：http://hui.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vin.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kwq.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://coo.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://gro.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://flf.ydzc1.top

TS:   if (x == null) {}
来源：http://cnv.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jll.havefunace.top

Go:   if x == nil {}
来源：http://wrm.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wvw.vehdjk.com

C#:   if (x is null) {}
来源：http://wyf.xuanzx.com

[P07] 防抖与节流
来源：http://owz.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://thy.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://fjh.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpr.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcy.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cuf.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yar.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xlk.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sgd.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://pvn.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uce.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://evv.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uwk.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hfy.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kbl.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fkh.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mls.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nzv.cdnleiting.top

================================================================================
来源：http://tpj.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vti.gzhubu.top

================================================================================
来源：http://nir.wangshuangyany.cn

[Q01] 创建表
来源：http://bit.sufxvd.cn

CREATE TABLE users (
来源：http://cqz.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfq.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://lka.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://buo.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bic.kuanghao11.cn

);
来源：http://pxs.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://sks.wangshuangyany.cn

CREATE TABLE orders (
来源：http://ucj.xuetiantiany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://edk.0kj1m.cn

user_id INT NOT NULL,
来源：http://afh.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://yqy.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eex.yj202588.top

);
来源：http://zfj.quarkkingdee.top

[Q03] 增加列
来源：http://qng.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yeb.yfazqb.com

[Q04] 修改列类型
来源：http://pql.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nlj.ehwqpu.com

[Q05] 重命名列
来源：http://ygo.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://phs.316326.xyz

[Q06] 删除列
来源：http://ekq.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mbr.aibaodan.cn

[Q07] 删除表
来源：http://hmv.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://obw.hesvh.cn

[Q08] 创建普通索引
来源：http://rvx.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vrk.hesvh.cn

[Q09] 创建唯一索引
来源：http://wai.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ghi.chenzaomai.com

[Q10] 插入单行
来源：http://jps.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gar.gaohongyu789.top

[Q11] 一次插入多行
来源：http://jhh.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jsk.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://xcp.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://moo.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mne.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://hke.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cts.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://nug.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mnk.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xiz.wangdashe.top

[Q15] 查询全部
来源：http://bmb.zycfv.cn

SELECT * FROM users;
来源：http://kie.zhijiandao.cn

[Q16] 查询指定列
来源：http://pzj.wangdashe.top

SELECT id, name FROM users;
来源：http://ggx.yvedp.cn

[Q17] 条件查询
来源：http://dgy.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wpz.fengsongda.top

[Q18] 模糊匹配
来源：http://ugf.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://duq.sysykeji.top

[Q19] 范围查询
来源：http://dsr.nanxuanxn.top


<!-- 参考信息 -->