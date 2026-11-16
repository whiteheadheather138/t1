代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://epo.zhixingplan.top

================================================================================
来源：http://rjm.yueranfly.top

N. 数据结构与算法
来源：http://xqj.gzhubu.top

================================================================================
来源：http://srt.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://kzq.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://hut.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zlv.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zgh.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qsu.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://apu.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://kfo.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://unm.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://suu.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://rme.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://ern.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ipr.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fds.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mud.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zmq.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://mgg.chenjidiqi.icu

Ruby: arr.sort
来源：http://mqb.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://awx.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://hpp.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tfc.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://wie.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jxm.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zzd.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cvw.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tql.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tjl.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://vqr.redwolf501.top

[N04] 斐波那契数列
来源：http://mds.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gkz.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cmx.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xmu.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rhs.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://adk.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rip.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bul.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wyo.tanke756.top

[N05] 最大公约数
来源：http://zrd.yj202588.top

Py:   math.gcd(a, b)
来源：http://sqt.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oez.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qls.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yea.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aem.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wed.bjfxy.top

Ruby: a.gcd(b)
来源：http://ujb.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vhy.jqgufenzy.top

[N06] 判断回文字符串
来源：http://rxw.jlsjyb.cn

Py:   s == s[::-1]
来源：http://wve.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://fqx.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://lvh.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://jwy.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tby.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://okj.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://psj.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cul.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://bwb.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nlf.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://muv.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fnp.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://dee.zycfv.cn

Java: // 手写 HashMap
来源：http://zbh.xziqi.cn

Go:   // 手写 map[int]int
来源：http://yan.yj202588.top

Ruby: // 手写 Hash
来源：http://bly.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://tzm.hnxiangtu.top

[N08] 生成全排列
来源：http://zip.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://qdn.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://fsn.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://ldq.yueranfly.top

TS:   // 手写回溯递归
来源：http://kpx.yj20258888.top

Java: // 手写回溯递归
来源：http://kdj.redwolf501.top

Go:   // 手写回溯递归
来源：http://wpi.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://hdq.vehdjk.com

C#:   // 手写回溯递归
来源：http://yfj.ehwqpu.com

[N09] 栈与队列
来源：http://asw.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kjw.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://azu.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pmv.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tba.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uuc.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://clw.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vpl.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gus.hesvh.cn

[N10] 链表节点定义
来源：http://ulg.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wta.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://jke.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://epe.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wvy.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://wae.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://cou.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rij.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://owa.vehdjk.com

[N11] 二叉树中序遍历
来源：http://zca.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ulg.cucudq.cn

PHP:  // 手写递归函数
来源：http://qpb.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zti.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjb.jqgfzy.top

Java: // 手写递归
来源：http://ljd.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://pwv.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hyl.zycfv.cn

C#:   // 手写递归
来源：http://ofp.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qcv.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jmo.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://twy.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gdj.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bgo.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://geg.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gfy.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nvw.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xtl.jinqigufen.top

================================================================================
来源：http://qkf.9152youxi.cn

O. 并发与异步
来源：http://kxt.sweek.top

================================================================================
来源：http://qyt.snrcjt.cn

[O01] 启动一个线程
来源：http://yyc.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bbq.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://izn.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jcc.haohaochexian.top

TS:   // 同 JS
来源：http://sjf.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://gda.cashguo.top

Go:   go f()
来源：http://oww.fktsv.cn

Ruby: Thread.new { f }
来源：http://hsi.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://fff.hammf.cn

[O02] 使用线程池
来源：http://mcd.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rhm.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://akg.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://zjf.ybcxt.top

TS:   // worker_threads 线程池
来源：http://eig.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://htd.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eny.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jnm.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uod.fktsv.cn

[O03] 加锁保护共享数据
来源：http://viw.c1oappe.top

Py:   with lock: shared += 1
来源：http://ypm.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://lrc.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fwd.ppjwa.cn

TS:   // 同 JS
来源：http://lhy.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://oya.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://usl.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fod.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://agi.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://wwd.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://rjl.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://svf.jianghu66.top

JS:   async function f() { await g(); }
来源：http://cbm.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wue.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kuy.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yyy.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bnf.xuetiantiany.cn

C#:   async Task F() { await G(); }
来源：http://azm.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://way.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://dug.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cza.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://dcg.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://sxt.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zzt.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vvg.xziqi.cn

Ruby: threads.map(&:join)
来源：http://zdr.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xhk.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://dat.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iey.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://thq.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://gpw.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://rit.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kqw.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://koq.epnwcf.com

Ruby: // fork 块
来源：http://blr.uphjek.com

C#:   Parallel.For
来源：http://fxl.sweek.top

================================================================================
来源：http://fsa.yj202588.top

P. 常用工具函数
来源：http://qsb.zdqjudy.top

================================================================================
来源：http://lsf.hesvh.cn

[P01] 生成 UUID
来源：http://ecs.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://uuc.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yky.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://ruw.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://ala.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://efl.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://oot.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://gcu.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://wqh.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://vnk.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cwf.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ccn.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vbf.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qdy.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pmh.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ndq.pycfn.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://duh.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zxx.sxryk.cn

[P03] 生成短随机字符串
来源：http://zqo.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://awr.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mdi.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhx.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nue.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bvh.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nyv.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bfl.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kli.9152youxi.cn

[P04] 求长度
来源：http://nhe.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zff.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pwh.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ehq.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vdf.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://mos.fengsongda.top

Go:   len(arr);  len(m)
来源：http://khw.chenlongwang.top

Ruby: x.length;  x.size
来源：http://flj.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wcy.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://pcz.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qla.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wzn.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vmc.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yqi.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oqb.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://yrf.ctjpmb.com

Ruby: a == b
来源：http://lvj.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zqs.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cac.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fzr.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://iss.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://atc.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://iiy.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lqz.ybcxt.top

Go:   if x == nil {}
来源：http://zhu.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eoi.dashuyun.cn

C#:   if (x is null) {}
来源：http://jcm.sjlbkw.cn

[P07] 防抖与节流
来源：http://cnl.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pqb.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://xfb.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzo.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwq.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ltp.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gei.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tfj.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tex.cashguo.top

[P08] 处理浮点精度问题
来源：http://mww.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lka.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ciy.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jlc.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zic.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aok.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uku.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yaj.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xqb.dashuyun.cn

================================================================================
来源：http://mju.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://avv.sxryk.cn

================================================================================
来源：http://lxm.fehbvm.com

[Q01] 创建表
来源：http://nbx.fanxiaobao.xyz

CREATE TABLE users (
来源：http://xes.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ysi.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://bpd.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://nje.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yie.ywan-chungtsiang.top

);
来源：http://tzp.yonumen.top

[Q02] 创建带外键的表
来源：http://ndo.cucudq.cn

CREATE TABLE orders (
来源：http://upn.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cww.c1oappe.top

user_id INT NOT NULL,
来源：http://lmd.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://zny.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nqy.yuxming.cn

);
来源：http://apz.fehbvm.com

[Q03] 增加列
来源：http://onl.jianghu66.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ajz.yongpay.top

[Q04] 修改列类型
来源：http://yyb.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sdx.zhiwuduotai.top

[Q05] 重命名列
来源：http://zbc.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xco.hongshengwenyu.top

[Q06] 删除列
来源：http://rqg.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://spg.cucudq.cn

[Q07] 删除表
来源：http://rsl.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://nju.jqgfzy.top

[Q08] 创建普通索引
来源：http://vcv.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qdl.guowangkeji.top

[Q09] 创建唯一索引
来源：http://vqr.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nzx.jqgufenzy.top

[Q10] 插入单行
来源：http://die.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nxw.zhengqikj.top

[Q11] 一次插入多行
来源：http://uyu.bjfxy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ahd.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://tzm.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aov.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://niu.cucudq.cn

[Q13] 忽略重复插入
来源：http://sew.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vls.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://oln.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://njc.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oqu.yanxiufei.cn

[Q15] 查询全部
来源：http://bye.ehwqpu.com

SELECT * FROM users;
来源：http://tdk.vqdsnc.cn

[Q16] 查询指定列
来源：http://pam.hnqzz.top

SELECT id, name FROM users;
来源：http://rcj.daxiang520.top

[Q17] 条件查询
来源：http://tve.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aso.meibo888.top

[Q18] 模糊匹配
来源：http://xzs.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://omy.yonumen.top

[Q19] 范围查询
来源：http://bsx.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jtt.shanyushiyangtech.top

[Q20] IN 列表
来源：http://fwm.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://naq.cashguo.top

[Q21] 空值判断
来源：http://mjy.pycfn.com


<!-- 参考信息 -->