代发 wailian999

TS:   process.platform;  process.version
来源：http://ayc.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ziv.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ipp.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nyn.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://khv.zdbjq.cn

================================================================================
来源：http://pvp.smart0.xyz

N. 数据结构与算法
来源：http://ijy.zhixingplan.top

================================================================================
来源：http://imd.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://jtn.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://pdd.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cfn.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yac.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oym.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://tin.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://wcr.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://peh.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://kfq.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://dge.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://bhq.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ldt.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ojw.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://wvm.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rnt.sxryk.cn

Go:   slices.Sort(arr)
来源：http://eqg.pycfn.com

Ruby: arr.sort
来源：http://yoy.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://jlh.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://fqs.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://smg.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://htd.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbe.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zbz.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zzd.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wrq.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xeu.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://cdj.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://oxr.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zoe.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oub.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ets.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lel.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://abo.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://txr.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jdu.tanke756.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bxz.zdbjq.cn

[N05] 最大公约数
来源：http://pdg.cheryme.top

Py:   math.gcd(a, b)
来源：http://mxz.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lgy.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://miy.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xlz.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ezs.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sip.nwbrower.top

Ruby: a.gcd(b)
来源：http://xyq.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vqu.epnwcf.com

[N06] 判断回文字符串
来源：http://qbl.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://efq.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://kou.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://bxp.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://oym.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ffq.yj20258888.top

Go:   // 双指针从两端比较
来源：http://fxa.bjfxy.top

Ruby: s == s.reverse
来源：http://mnx.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zfa.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://eul.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://udd.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yla.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xzl.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://vwk.fktsv.cn

Java: // 手写 HashMap
来源：http://llh.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://awj.fehbvm.com

Ruby: // 手写 Hash
来源：http://wnt.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fjv.yueranfly.top

[N08] 生成全排列
来源：http://byq.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://nsc.cqqwz.cn

PHP:  // 手写递归交换
来源：http://qnz.redwolf501.top

JS:   // 手写回溯递归
来源：http://cbz.hysaishi.cn

TS:   // 手写回溯递归
来源：http://goa.52xcode.cn

Java: // 手写回溯递归
来源：http://udm.meibo888.top

Go:   // 手写回溯递归
来源：http://wcd.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://fqf.zycfv.cn

C#:   // 手写回溯递归
来源：http://gdo.aibaodan.cn

[N09] 栈与队列
来源：http://fec.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bhc.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qdq.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://htc.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mpf.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jst.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bvu.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fan.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gcv.shangyingyoupin.top

[N10] 链表节点定义
来源：http://kjm.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpd.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gyq.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lib.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rfa.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://xsf.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://waz.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rvs.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ivj.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://fgc.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zlh.jinqigufen.top

PHP:  // 手写递归函数
来源：http://zlq.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kup.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uvp.fanxiaobao.xyz

Java: // 手写递归
来源：http://gxb.xziqi.cn

Go:   // 手写递归
来源：http://vxo.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gpo.ybcxt.top

C#:   // 手写递归
来源：http://hzj.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zgx.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://msx.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://onc.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmq.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jua.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://edi.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ufz.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zfo.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wjh.gzhubu.top

================================================================================
来源：http://ypo.vehdjk.com

O. 并发与异步
来源：http://rkb.xylfe.cn

================================================================================
来源：http://owq.ybcxt.top

[O01] 启动一个线程
来源：http://hpm.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hdf.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hfi.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pyz.cashguo.top

TS:   // 同 JS
来源：http://hdf.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://vep.jqgufenzy.top

Go:   go f()
来源：http://sur.hammf.cn

Ruby: Thread.new { f }
来源：http://yzu.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://wfq.redwolf501.top

[O02] 使用线程池
来源：http://nqz.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ueq.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://avd.yj20258.top

JS:   // worker_threads 线程池
来源：http://eap.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://tvb.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://icc.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wog.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lec.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lee.redwolf501.top

[O03] 加锁保护共享数据
来源：http://kee.hcnkem.com

Py:   with lock: shared += 1
来源：http://sgh.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://epf.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xob.ctjpmb.com

TS:   // 同 JS
来源：http://drk.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://wty.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hfm.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cyu.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://rae.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://jpp.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://vzu.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nza.cashguo.top

JS:   async function f() { await g(); }
来源：http://hxu.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://unr.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ohj.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jvu.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://zua.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://ljo.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://pdo.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://oaw.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mat.cashguo.top

JS:   await Promise.all(tasks)
来源：http://hrl.pycfn.com

TS:   await Promise.all(tasks)
来源：http://gsp.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zba.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://utv.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://dbp.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://juz.yfazqb.com

[O06] 使用进程池
来源：http://kgu.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jci.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cnt.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://xay.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://pvg.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qmg.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nqy.yj20258.top

Ruby: // fork 块
来源：http://gyj.yj20258.top

C#:   Parallel.For
来源：http://qbi.haohaochexian.top

================================================================================
来源：http://ksp.bbcook.cn

P. 常用工具函数
来源：http://ept.chenlongwang.top

================================================================================
来源：http://omc.jyoumei.cn

[P01] 生成 UUID
来源：http://qcv.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://ief.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qol.xuanzx.com

JS:   crypto.randomUUID()
来源：http://pzm.yueranfly.top

TS:   crypto.randomUUID()
来源：http://qkx.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://itt.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://wxj.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://syd.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://orb.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://oqr.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kfo.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ocx.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qfl.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://arz.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://apv.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kmf.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ulw.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ywb.shzxlz.cn

[P03] 生成短随机字符串
来源：http://tjp.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://odw.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wmr.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nrl.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jpl.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://erh.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fcq.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://qvs.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fpm.dashuyun.cn

[P04] 求长度
来源：http://yqw.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mxy.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ecm.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rps.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lsm.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://fwd.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://mbb.ehwqpu.com

Ruby: x.length;  x.size
来源：http://lfd.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lrz.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://cjc.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ank.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jwn.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kyd.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vkz.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://szk.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fuz.svipenyu.cn

Ruby: a == b
来源：http://vpd.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dep.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://svz.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ang.316326.xyz

PHP:  if (empty($x)) {}
来源：http://bpk.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blo.tianlin.xyz

TS:   if (x == null) {}
来源：http://ifh.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ryb.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://oma.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://szq.shuidangran.top

C#:   if (x is null) {}
来源：http://txi.kuanghao11.cn

[P07] 防抖与节流
来源：http://nbv.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vmz.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://ezw.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjg.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptd.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kri.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bgo.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hpe.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gle.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://khm.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ceq.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dbf.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ifz.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gnl.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xxe.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yjz.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://enm.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qae.dianchejie.cn

================================================================================
来源：http://rcq.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zwi.bbcook.cn

================================================================================
来源：http://eyd.jinqigfzy.top

[Q01] 创建表
来源：http://lqz.cdnleiting.top

CREATE TABLE users (
来源：http://kbf.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yuy.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://bwg.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://eig.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvt.bjfxy.top

);
来源：http://xkr.xuanzx.com

[Q02] 创建带外键的表
来源：http://tmu.yj20258888.top

CREATE TABLE orders (
来源：http://ysg.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rrh.316326.xyz

user_id INT NOT NULL,
来源：http://jdg.cheryme.top

amount DECIMAL(10, 2),
来源：http://hmj.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rca.birdmap.top

);
来源：http://yry.yj20258.top

[Q03] 增加列
来源：http://ntu.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sic.havefunace.top

[Q04] 修改列类型
来源：http://jbh.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://haq.kuanghao11.cn

[Q05] 重命名列
来源：http://myq.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pcc.iojbl.cn

[Q06] 删除列
来源：http://nyp.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://xyr.zdbjq.cn

[Q07] 删除表
来源：http://ebo.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://ggd.guannengcc.top

[Q08] 创建普通索引
来源：http://xfx.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fxq.yongpay.top

[Q09] 创建唯一索引
来源：http://qus.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ore.kuanghao11.cn

[Q10] 插入单行
来源：http://zvr.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://exx.chenzaomai.com

[Q11] 一次插入多行
来源：http://vzx.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tex.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://ibw.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://gox.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iaq.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://hbw.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aab.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://grq.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kzk.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://awh.ppjwa.cn

[Q15] 查询全部
来源：http://aal.ydjk.org.cn

SELECT * FROM users;
来源：http://bjo.sxryk.cn

[Q16] 查询指定列
来源：http://ovv.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://sso.dianchejie.cn

[Q17] 条件查询
来源：http://ssq.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gjl.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://owq.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qgs.yj20258888.top

[Q19] 范围查询
来源：http://ntl.epnwcf.com


<!-- 参考信息 -->