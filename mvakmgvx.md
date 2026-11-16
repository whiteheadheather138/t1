代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://wnt.hesvh.cn

================================================================================
来源：http://vsv.hywenlv.cn

N. 数据结构与算法
来源：http://fdp.kuanghao11.cn

================================================================================
来源：http://rcn.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://apa.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oen.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wje.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ihi.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbd.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ulz.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://svj.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bqp.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bbn.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://uqr.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://enm.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jop.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cnm.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://czy.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lfv.gzhubu.top

Go:   slices.Sort(arr)
来源：http://zeh.sjlbkw.cn

Ruby: arr.sort
来源：http://vxx.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bpi.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://moj.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aqq.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://opy.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oeq.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lsx.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gms.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ijg.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://duv.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bsb.jinqigfzy.top

[N04] 斐波那契数列
来源：http://zve.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://igz.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iuq.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sak.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhk.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjv.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oty.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ton.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://exk.jyoumei.cn

[N05] 最大公约数
来源：http://qkc.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://zvw.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://icz.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aip.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkn.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gzw.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fne.sysykeji.top

Ruby: a.gcd(b)
来源：http://keo.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ith.tanke756.top

[N06] 判断回文字符串
来源：http://uxv.ydzc1.top

Py:   s == s[::-1]
来源：http://jzh.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://wrp.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://uex.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://jwx.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hlz.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://nly.nanxuanxn.top

Ruby: s == s.reverse
来源：http://ekd.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qji.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://rzm.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gzd.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ugg.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://orh.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://cmp.316326.xyz

Java: // 手写 HashMap
来源：http://djl.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://dkc.yj20258888.top

Ruby: // 手写 Hash
来源：http://raj.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://afy.tianlin.xyz

[N08] 生成全排列
来源：http://cpw.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://jek.yongpay.top

PHP:  // 手写递归交换
来源：http://bdr.ppjwa.cn

JS:   // 手写回溯递归
来源：http://mei.9152youxi.cn

TS:   // 手写回溯递归
来源：http://uff.yongpay.top

Java: // 手写回溯递归
来源：http://caf.bjfxy.top

Go:   // 手写回溯递归
来源：http://hjx.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://goa.hnqzz.top

C#:   // 手写回溯递归
来源：http://juy.nanxinkj.top

[N09] 栈与队列
来源：http://wem.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zxi.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jxy.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qon.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mpm.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zjs.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://alp.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kky.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jar.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://vkn.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cue.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://imm.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wlp.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bou.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://tso.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://fwz.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tsp.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rdt.yfazqb.com

[N11] 二叉树中序遍历
来源：http://mvs.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xrv.guowangkeji.top

PHP:  // 手写递归函数
来源：http://txo.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjl.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bvm.zhoulong.xyz

Java: // 手写递归
来源：http://kfe.ydzc1.top

Go:   // 手写递归
来源：http://fmv.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bpu.yuanzhike.top

C#:   // 手写递归
来源：http://fgh.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ufl.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vim.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nrc.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijp.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rmk.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vls.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rsw.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sdr.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qtp.xingfuxueyuan.xyz

================================================================================
来源：http://der.zhengqikj.top

O. 并发与异步
来源：http://vss.sysykeji.top

================================================================================
来源：http://yad.fengsongda.top

[O01] 启动一个线程
来源：http://eao.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hnl.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uht.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lcz.fanxiaobao.xyz

TS:   // 同 JS
来源：http://jex.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://zlz.hcnkem.com

Go:   go f()
来源：http://kxp.aizwys.cn

Ruby: Thread.new { f }
来源：http://adp.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://hce.dianchejie.cn

[O02] 使用线程池
来源：http://aan.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://euu.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hir.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://gmz.mhx1999.top

TS:   // worker_threads 线程池
来源：http://lcc.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hrm.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjy.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aoy.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rzl.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://olv.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://jgt.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://ntr.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://afg.guannengcc.top

TS:   // 同 JS
来源：http://gcm.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://xbf.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://urf.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nvu.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://hkr.vehdjk.com

[O04] 定义异步函数并等待
来源：http://ezu.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://gme.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qbr.xinyue.icu

JS:   async function f() { await g(); }
来源：http://wud.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oal.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ckn.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://isw.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://wuq.cashguo.top

C#:   async Task F() { await G(); }
来源：http://fia.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://mdo.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://btk.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qjj.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://zjs.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://mqc.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dxv.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tjc.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://ctw.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vom.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://zfb.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://spz.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yxe.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://hat.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://rus.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://daz.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cwq.gzhubu.top

Ruby: // fork 块
来源：http://jgt.fzhhl.top

C#:   Parallel.For
来源：http://kyw.shangyingyoupin.top

================================================================================
来源：http://lfe.shanyushiyangtech.top

P. 常用工具函数
来源：http://qki.fanxiaobao.xyz

================================================================================
来源：http://zzh.zhongyouzk.top

[P01] 生成 UUID
来源：http://znj.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://uzc.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cdr.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://jqy.yonumen.top

TS:   crypto.randomUUID()
来源：http://jyt.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://ghl.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://fzu.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://yco.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://ogc.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://skp.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xhj.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://phc.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cyt.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uhr.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mvc.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qqc.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://juz.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bor.fktsv.cn

[P03] 生成短随机字符串
来源：http://ios.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jvk.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://weq.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lis.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sfc.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jkn.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mom.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://xkv.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://djt.cashguo.top

[P04] 求长度
来源：http://wtq.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kcx.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhe.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pct.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://syt.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://hvj.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://dci.redwolf501.top

Ruby: x.length;  x.size
来源：http://nxa.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://upc.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://rpq.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://azo.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lec.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mjn.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yal.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qsg.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bot.shuidangran.top

Ruby: a == b
来源：http://eno.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zmd.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ycs.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kgf.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://oer.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dmg.kuanghao11.cn

TS:   if (x == null) {}
来源：http://ejj.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ekk.gogol.net.cn

Go:   if x == nil {}
来源：http://bup.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wjp.yj202588.top

C#:   if (x is null) {}
来源：http://ard.yonumen.top

[P07] 防抖与节流
来源：http://gvi.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dvk.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://mjr.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yky.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fem.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oth.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ysc.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mtf.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://egs.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://trt.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://okf.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bju.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jae.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://agp.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pio.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vvq.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yid.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://goi.52xcode.cn

================================================================================
来源：http://wwn.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qey.c1oappe.top

================================================================================
来源：http://ufs.xziqi.cn

[Q01] 创建表
来源：http://dni.nwbrower.top

CREATE TABLE users (
来源：http://vtc.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gix.gzhubu.top

name VARCHAR(50) NOT NULL,
来源：http://rux.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://dxw.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rru.jinghuilouyu.cn

);
来源：http://rxd.fehbvm.com

[Q02] 创建带外键的表
来源：http://svh.hcnkem.com

CREATE TABLE orders (
来源：http://wef.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://srw.sjlbkw.cn

user_id INT NOT NULL,
来源：http://bzx.xuanzx.com

amount DECIMAL(10, 2),
来源：http://sdf.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yvo.smart0.xyz

);
来源：http://qcx.mhx1999.top

[Q03] 增加列
来源：http://nbj.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jat.zhiwuduotai.top

[Q04] 修改列类型
来源：http://oof.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iov.iojbl.cn

[Q05] 重命名列
来源：http://pkk.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wpa.jqgufenzy.top

[Q06] 删除列
来源：http://mpy.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qaz.aizwys.cn

[Q07] 删除表
来源：http://cdr.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://mjd.xziqi.cn

[Q08] 创建普通索引
来源：http://iti.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://afd.gotoacloud.top

[Q09] 创建唯一索引
来源：http://jwh.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ctm.pengpengdd.cyou

[Q10] 插入单行
来源：http://luo.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qst.hammf.cn

[Q11] 一次插入多行
来源：http://bmj.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://owp.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://ghd.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://ddy.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hxt.smart0.xyz

[Q13] 忽略重复插入
来源：http://xly.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rtk.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://kto.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://alk.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ddx.gaohongyu789.top

[Q15] 查询全部
来源：http://rtn.andypj.xyz

SELECT * FROM users;
来源：http://ggf.fehbvm.com

[Q16] 查询指定列
来源：http://moo.yj20258888.top

SELECT id, name FROM users;
来源：http://ssj.chenlongwang.top

[Q17] 条件查询
来源：http://kxr.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fbn.ehwqpu.com

[Q18] 模糊匹配
来源：http://rlu.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bed.jianghu66.top

[Q19] 范围查询
来源：http://rkh.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qch.sufxvd.cn

[Q20] IN 列表
来源：http://ivn.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hry.hammf.cn

[Q21] 空值判断
来源：http://erv.quarkkingdee.top


<!-- 参考信息 -->