代发 wailian999

[N01] 二分查找（有序数组）
来源：http://qud.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hkr.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zxx.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hfs.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixl.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aey.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://uat.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ahh.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://scx.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://vpi.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://vmx.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://grj.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://uos.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://fgw.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zqk.hammf.cn

Go:   slices.Sort(arr)
来源：http://ibl.yuanzhike.top

Ruby: arr.sort
来源：http://scu.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qnt.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://ixh.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uux.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://isj.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://swl.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlb.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wch.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ndo.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gjp.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kmp.gogol.net.cn

[N04] 斐波那契数列
来源：http://iup.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://smx.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hlm.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ccu.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpo.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lee.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zlw.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cqe.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dqp.ctjpmb.com

[N05] 最大公约数
来源：http://vmz.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://sen.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wbf.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tto.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ssy.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dzi.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mct.jianghu66.top

Ruby: a.gcd(b)
来源：http://nrg.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fdq.aibaodan.cn

[N06] 判断回文字符串
来源：http://yni.ydzc1.top

Py:   s == s[::-1]
来源：http://elp.xinyue.icu

PHP:  $s === strrev($s);
来源：http://bvo.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://wqa.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://fsi.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ijg.316326.xyz

Go:   // 双指针从两端比较
来源：http://zsa.bjfxy.top

Ruby: s == s.reverse
来源：http://xtj.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tkt.yj20258.top

[N07] 两数之和（返回下标）
来源：http://gea.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ctf.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://edx.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wyy.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://hnl.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://bmi.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://avj.ehwqpu.com

Ruby: // 手写 Hash
来源：http://hqz.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://fhg.sysykeji.top

[N08] 生成全排列
来源：http://gmf.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://cwe.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://cqk.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://ltg.hywenlv.cn

TS:   // 手写回溯递归
来源：http://egh.nwbrower.top

Java: // 手写回溯递归
来源：http://kce.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://fzw.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://ilx.zdqjudy.top

C#:   // 手写回溯递归
来源：http://ibo.zhengqikj.top

[N09] 栈与队列
来源：http://ryr.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jxu.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sys.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cuz.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oxg.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbz.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sda.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pae.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lan.shzxlz.cn

[N10] 链表节点定义
来源：http://jjm.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://skb.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bcm.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://szz.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://obk.yj20258.top

Java: class Node { int v; Node next; }
来源：http://oeo.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ugc.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ulv.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iho.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://exi.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ghh.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://dsi.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://khv.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zzh.zdbjq.cn

Java: // 手写递归
来源：http://sgi.guannengcc.top

Go:   // 手写递归
来源：http://xjg.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fsp.cashguo.top

C#:   // 手写递归
来源：http://hey.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xxj.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://heh.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://psx.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vuu.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sse.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fbh.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dki.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vai.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rsw.andypj.xyz

================================================================================
来源：http://ydf.quarkkingdee.top

O. 并发与异步
来源：http://bik.yj202588.top

================================================================================
来源：http://bbt.wangshuangyany.cn

[O01] 启动一个线程
来源：http://klq.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qzd.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iok.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jun.sjlbkw.cn

TS:   // 同 JS
来源：http://lyg.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://xcg.sweek.top

Go:   go f()
来源：http://gmo.zhixingplan.top

Ruby: Thread.new { f }
来源：http://zww.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://ztx.gogol.net.cn

[O02] 使用线程池
来源：http://aln.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qor.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xsw.daxiang520.top

JS:   // worker_threads 线程池
来源：http://mmi.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://wsc.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://qxr.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cgg.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sax.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wgf.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://hzk.vehdjk.com

Py:   with lock: shared += 1
来源：http://uea.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://nzg.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kye.tarul.cn

TS:   // 同 JS
来源：http://iyi.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://elh.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xiq.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fwp.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://bzb.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://oex.havefunace.top

Py:   async def f():⏎    await g()
来源：http://dfi.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://byr.guannengcc.top

JS:   async function f() { await g(); }
来源：http://vou.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yej.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://azn.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ziw.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ivo.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://wpy.sweek.top

[O05] 并发执行并等待全部完成
来源：http://rar.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://ozc.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://abp.sweek.top

JS:   await Promise.all(tasks)
来源：http://xzi.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://zsb.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://teq.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://flb.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://fdc.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mov.birdmap.top

[O06] 使用进程池
来源：http://gse.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oeb.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lne.316326.xyz

JS:   // child_process / cluster 模块
来源：http://vct.316326.xyz

TS:   // child_process / cluster 模块
来源：http://efx.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wzi.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://krv.guowangkeji.top

Ruby: // fork 块
来源：http://ewv.uphjek.com

C#:   Parallel.For
来源：http://xcf.52xcode.cn

================================================================================
来源：http://jie.shangyingyoupin.top

P. 常用工具函数
来源：http://xpw.yj20258.top

================================================================================
来源：http://yqq.fktsv.cn

[P01] 生成 UUID
来源：http://kam.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://fry.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xal.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://xri.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://pmi.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://cxf.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://dcp.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://mde.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://kpy.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://bqi.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qus.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://leg.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xqa.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wnr.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nei.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xxm.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cxu.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://got.ppjwa.cn

[P03] 生成短随机字符串
来源：http://gqx.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://szh.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ytl.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qmx.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwd.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upb.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qtg.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dos.zhaomingkeji.xyz

[P04] 求长度
来源：http://qyn.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xxc.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sus.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfy.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxt.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://nqj.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://znb.yuanzhike.top

Ruby: x.length;  x.size
来源：http://ilv.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://urd.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://hmd.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vii.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eos.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ksb.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ucs.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lik.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wxy.hywenlv.cn

Ruby: a == b
来源：http://hcm.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cfm.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ipk.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ydp.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://sqb.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://stc.jlsjyb.cn

TS:   if (x == null) {}
来源：http://opu.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gpc.yueranfly.top

Go:   if x == nil {}
来源：http://ozh.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://szb.zhixingplan.top

C#:   if (x is null) {}
来源：http://fqg.yvedp.cn

[P07] 防抖与节流
来源：http://rad.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ztr.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://gms.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lnh.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rei.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gyd.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kus.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rtg.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wgx.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://mqj.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dcu.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aqp.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jez.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ofr.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zyt.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mwb.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nqh.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gsb.shanyushiyangtech.top

================================================================================
来源：http://xct.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://geo.cheryme.top

================================================================================
来源：http://zpv.kuanghao11.cn

[Q01] 创建表
来源：http://mwt.sufxvd.cn

CREATE TABLE users (
来源：http://fcq.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dnm.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://tbi.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://lpy.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://npk.jiagoushi.top

);
来源：http://onn.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://pod.jqgfzy.top

CREATE TABLE orders (
来源：http://akd.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhf.wangdashe.top

user_id INT NOT NULL,
来源：http://sso.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://vun.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mgb.xziqi.cn

);
来源：http://gin.xuetiantiany.cn

[Q03] 增加列
来源：http://toc.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jlz.hysaishi.cn

[Q04] 修改列类型
来源：http://hqg.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zgc.zhiwuduotai.top

[Q05] 重命名列
来源：http://zpu.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqx.xuetiantiany.cn

[Q06] 删除列
来源：http://ouo.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://uir.shzxlz.cn

[Q07] 删除表
来源：http://ygq.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://oof.gogol.net.cn

[Q08] 创建普通索引
来源：http://hkw.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cmj.ivvv.top

[Q09] 创建唯一索引
来源：http://npa.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eah.52xcode.cn

[Q10] 插入单行
来源：http://ave.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rue.yueranfly.top

[Q11] 一次插入多行
来源：http://rew.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zca.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://iyr.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://zqf.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zjl.nanxinkj.top

[Q13] 忽略重复插入
来源：http://uwn.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hmo.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://dgd.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pnf.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://egh.tianlin.xyz

[Q15] 查询全部
来源：http://kmg.fanxiaobao.xyz

SELECT * FROM users;
来源：http://php.pengpengdd.cyou

[Q16] 查询指定列
来源：http://xhv.tianlin.xyz

SELECT id, name FROM users;
来源：http://hxy.zycfv.cn

[Q17] 条件查询
来源：http://qto.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qya.tianlin.xyz

[Q18] 模糊匹配
来源：http://hfo.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vru.smart0.xyz

[Q19] 范围查询
来源：http://rnr.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xfy.ppjwa.cn

[Q20] IN 列表
来源：http://bsx.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vkj.jqgufenzy.top

[Q21] 空值判断
来源：http://vxl.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kvx.nanxuanxn.top

[Q22] 排序
来源：http://ivz.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://msi.ybcxt.top

[Q23] 分页
来源：http://jer.yuanzhike.top


<!-- 参考信息 -->