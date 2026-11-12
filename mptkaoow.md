代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://stq.feifeiyinyue.top

================================================================================
来源：http://ogx.jinqigfzy.top

N. 数据结构与算法
来源：http://tnz.hammf.cn

================================================================================
来源：http://vlr.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://lic.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://rpg.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hbx.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ngz.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kkp.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://bbr.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://ihj.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://akv.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://rbw.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://ema.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://lpm.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gij.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://key.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uft.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nkw.andypj.xyz

Go:   slices.Sort(arr)
来源：http://gyw.iojbl.cn

Ruby: arr.sort
来源：http://qgt.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jvc.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://rfo.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vap.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://ilp.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdt.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hau.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jpt.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://inl.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zsx.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://ndw.jinqigfzy.top

[N04] 斐波那契数列
来源：http://wkp.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://grm.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iyb.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ylm.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gaz.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fnh.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zhs.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hpt.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hgs.gaohongyu789.top

[N05] 最大公约数
来源：http://xyt.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://pns.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhl.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rvr.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rgg.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zkk.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dcp.xziqi.cn

Ruby: a.gcd(b)
来源：http://bda.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rau.gzhubu.top

[N06] 判断回文字符串
来源：http://pvw.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://ibk.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://xyu.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://ojy.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://zxd.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pty.fktsv.cn

Go:   // 双指针从两端比较
来源：http://mve.xziqi.cn

Ruby: s == s.reverse
来源：http://mug.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ogf.yj202588.top

[N07] 两数之和（返回下标）
来源：http://cbd.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rbk.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://keq.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://aaq.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://xjx.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://dlz.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://fzz.fzhhl.top

Ruby: // 手写 Hash
来源：http://lnf.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://cqv.hysaishi.cn

[N08] 生成全排列
来源：http://arz.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://hvj.ppjwa.cn

PHP:  // 手写递归交换
来源：http://kju.yueranfly.top

JS:   // 手写回溯递归
来源：http://zba.gotoacloud.top

TS:   // 手写回溯递归
来源：http://bif.xinyue.icu

Java: // 手写回溯递归
来源：http://ctz.c1oappe.top

Go:   // 手写回溯递归
来源：http://ijd.sweek.top

Ruby: arr.permutation.to_a
来源：http://rri.hnqzz.top

C#:   // 手写回溯递归
来源：http://eko.yonumen.top

[N09] 栈与队列
来源：http://ubd.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sds.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xpq.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uey.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wav.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ten.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jkd.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://brg.jinqigufen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mzt.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://ruo.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yuz.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ymz.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ezy.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cky.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://vhg.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://exl.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://map.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nxx.yfazqb.com

[N11] 二叉树中序遍历
来源：http://wwj.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cke.hcnkem.com

PHP:  // 手写递归函数
来源：http://tqd.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ibw.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blq.zhixingplan.top

Java: // 手写递归
来源：http://rtt.zhengqikj.top

Go:   // 手写递归
来源：http://kmj.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sup.snrcjt.cn

C#:   // 手写递归
来源：http://tnn.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tpz.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oxj.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gmq.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://him.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbj.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mqe.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blk.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gwz.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dzj.feifeiyinyue.top

================================================================================
来源：http://smk.meibo888.top

O. 并发与异步
来源：http://dku.tarul.cn

================================================================================
来源：http://ils.nanxuanxn.top

[O01] 启动一个线程
来源：http://izv.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ohj.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wxf.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uof.gaohongyu789.top

TS:   // 同 JS
来源：http://rwg.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://chw.iojbl.cn

Go:   go f()
来源：http://seq.epnwcf.com

Ruby: Thread.new { f }
来源：http://bch.yj202588.top

C#:   Task.Run(() => F());
来源：http://qzv.vehdjk.com

[O02] 使用线程池
来源：http://uhh.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ckb.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ajw.yj20258888.top

JS:   // worker_threads 线程池
来源：http://wfl.hcnkem.com

TS:   // worker_threads 线程池
来源：http://iwi.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://gtc.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ywd.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://plp.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jcm.birdmap.top

[O03] 加锁保护共享数据
来源：http://tck.tian-w.cn

Py:   with lock: shared += 1
来源：http://ehm.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://jxo.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://srh.yfazqb.com

TS:   // 同 JS
来源：http://fsk.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://yhp.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rbn.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://jmm.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://jix.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://abc.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://cmi.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dxn.vehdjk.com

JS:   async function f() { await g(); }
来源：http://bus.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://exq.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bjd.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pou.hcnkem.com

Ruby: # 用 Fiber 或 async gem
来源：http://bsy.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://myr.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://kvh.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://yfr.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kjy.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://qal.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://qtf.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xua.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kop.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://vxt.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://aud.dianchejie.cn

[O06] 使用进程池
来源：http://lyl.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vxz.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://idc.pycfn.com

JS:   // child_process / cluster 模块
来源：http://arp.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://sfo.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gak.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://smb.wangshuangyany.cn

Ruby: // fork 块
来源：http://uvv.jqgufenzy.top

C#:   Parallel.For
来源：http://brs.ppjwa.cn

================================================================================
来源：http://hri.zhaomingkeji.xyz

P. 常用工具函数
来源：http://kac.uphjek.com

================================================================================
来源：http://szw.zhixingplan.top

[P01] 生成 UUID
来源：http://uvg.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://itf.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gcr.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://fti.yj20258888.top

TS:   crypto.randomUUID()
来源：http://zrd.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://nfp.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://bov.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://aft.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://ltp.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://pho.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jse.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://moj.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hxn.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blk.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xta.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://flr.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fjj.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mmp.fehbvm.com

[P03] 生成短随机字符串
来源：http://qmd.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://onp.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://siv.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pof.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ash.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aps.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fol.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ayk.cqqwz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cdu.9152youxi.cn

[P04] 求长度
来源：http://pjm.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kga.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yuh.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cpw.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zak.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://iky.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://dqb.sxryk.cn

Ruby: x.length;  x.size
来源：http://cvp.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sgd.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://hff.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gug.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gec.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mcb.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qpw.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vpu.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://mxl.gogol.net.cn

Ruby: a == b
来源：http://fmp.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nvy.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hym.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yby.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://cqt.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://trq.sxryk.cn

TS:   if (x == null) {}
来源：http://guf.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xch.quarkkingdee.top

Go:   if x == nil {}
来源：http://idn.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lyx.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://woa.hywenlv.cn

[P07] 防抖与节流
来源：http://hsc.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rql.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://dog.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ejc.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwy.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xsr.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cpa.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://urn.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wmo.yongpay.top

[P08] 处理浮点精度问题
来源：http://xxb.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ael.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jwc.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://euy.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erm.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kko.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qsy.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://efg.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jss.hesvh.cn

================================================================================
来源：http://khm.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nen.vqdsnc.cn

================================================================================
来源：http://rio.xziqi.cn

[Q01] 创建表
来源：http://qnh.hesvh.cn

CREATE TABLE users (
来源：http://miv.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ess.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://mbt.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://zxc.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gkw.zhixingplan.top

);
来源：http://mte.xuanzx.com

[Q02] 创建带外键的表
来源：http://hak.yonumen.top

CREATE TABLE orders (
来源：http://rkr.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eex.cdnleiting.top

user_id INT NOT NULL,
来源：http://njr.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://cuv.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rax.cucudq.cn

);
来源：http://gjo.daria6918.cn

[Q03] 增加列
来源：http://lno.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uhe.zhijiandao.cn

[Q04] 修改列类型
来源：http://wer.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hsi.mhx1999.top

[Q05] 重命名列
来源：http://cnq.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dse.xinyue.icu

[Q06] 删除列
来源：http://hmm.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://qax.jyoumei.cn

[Q07] 删除表
来源：http://zgy.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://hcf.sufxvd.cn

[Q08] 创建普通索引
来源：http://bgb.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yyx.nwbrower.top

[Q09] 创建唯一索引
来源：http://ust.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cik.aizwys.cn

[Q10] 插入单行
来源：http://nbm.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ete.dashuyun.cn

[Q11] 一次插入多行
来源：http://agp.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xaf.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://qwj.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://qms.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://los.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://ygb.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oet.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://gys.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qdj.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xsb.chenlongwang.top

[Q15] 查询全部
来源：http://ubu.svipenyu.cn

SELECT * FROM users;
来源：http://qiw.316326.xyz

[Q16] 查询指定列
来源：http://nlg.gzhubu.top

SELECT id, name FROM users;
来源：http://wrd.zhongyouzk.top

[Q17] 条件查询
来源：http://wrz.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aro.bbcook.cn

[Q18] 模糊匹配
来源：http://smj.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pje.sweek.top

[Q19] 范围查询
来源：http://hrh.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxu.shanyushiyangtech.top

[Q20] IN 列表
来源：http://all.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://brw.guannengcc.top

[Q21] 空值判断
来源：http://hfp.zhaomingkeji.xyz


<!-- 参考信息 -->