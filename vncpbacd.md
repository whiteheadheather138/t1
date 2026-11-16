代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ylm.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://pry.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://yui.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://edx.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://vsl.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://bjq.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://xsv.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qty.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://buz.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cnb.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://evf.epnwcf.com

Go:   slices.Sort(arr)
来源：http://qzk.bjfxy.top

Ruby: arr.sort
来源：http://kpq.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dvx.hammf.cn

[N03] 快速排序（分治示例）
来源：http://aib.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://shr.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://vuu.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vcn.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xae.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zar.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lpd.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vee.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://ofs.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://eio.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rmd.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aif.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rqs.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oux.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hhk.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cnb.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uts.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lom.yuxming.cn

[N05] 最大公约数
来源：http://tot.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://pno.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqx.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wli.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzs.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ncr.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ile.daxiang520.top

Ruby: a.gcd(b)
来源：http://ajl.tianlin.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vbs.cheryme.top

[N06] 判断回文字符串
来源：http://hvn.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://omz.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://nvp.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://wmx.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://hto.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://glp.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://oxd.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://tln.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dlf.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://vdk.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wbs.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://odc.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xcv.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://igl.9152youxi.cn

Java: // 手写 HashMap
来源：http://smb.yj202588.top

Go:   // 手写 map[int]int
来源：http://bwq.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://cbq.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://rpm.pengpengdd.cyou

[N08] 生成全排列
来源：http://mjy.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://whh.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://crt.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://hcw.fehbvm.com

TS:   // 手写回溯递归
来源：http://cek.fengsongda.top

Java: // 手写回溯递归
来源：http://mlp.sweek.top

Go:   // 手写回溯递归
来源：http://bbl.ivvv.top

Ruby: arr.permutation.to_a
来源：http://oel.fehbvm.com

C#:   // 手写回溯递归
来源：http://ubb.meibo888.top

[N09] 栈与队列
来源：http://taa.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wtk.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://czc.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kzx.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ndv.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tev.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jyv.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://syo.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mff.snrcjt.cn

[N10] 链表节点定义
来源：http://grf.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hcz.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dep.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yqw.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eje.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://tlr.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eaq.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://los.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mdi.cashguo.top

[N11] 二叉树中序遍历
来源：http://llv.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mgf.0kj1m.cn

PHP:  // 手写递归函数
来源：http://vic.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://huu.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uge.shangyingyoupin.top

Java: // 手写递归
来源：http://zcx.pycfn.com

Go:   // 手写递归
来源：http://nbd.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dzt.cashguo.top

C#:   // 手写递归
来源：http://yjq.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ewy.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zjc.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://olh.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hhf.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vxc.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jmx.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eib.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wuo.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://epz.kuanghao11.cn

================================================================================
来源：http://roh.yuxming.cn

O. 并发与异步
来源：http://cxc.guannengcc.top

================================================================================
来源：http://vao.chenlongwang.top

[O01] 启动一个线程
来源：http://uil.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://snv.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gtz.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zdl.ehwqpu.com

TS:   // 同 JS
来源：http://dya.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://jyh.hywenlv.cn

Go:   go f()
来源：http://vsr.ivvv.top

Ruby: Thread.new { f }
来源：http://lcv.zycfv.cn

C#:   Task.Run(() => F());
来源：http://mas.yj202588.top

[O02] 使用线程池
来源：http://mxv.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vnl.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://liv.vehdjk.com

JS:   // worker_threads 线程池
来源：http://fsg.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://pkf.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://nmv.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sdt.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lrm.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zoe.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://mue.gotoacloud.top

Py:   with lock: shared += 1
来源：http://cvp.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://uof.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iqq.shanyushiyangtech.top

TS:   // 同 JS
来源：http://khl.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://nox.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://keh.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ywz.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://mul.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://fgu.cheryme.top

Py:   async def f():⏎    await g()
来源：http://pdg.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://acq.cucudq.cn

JS:   async function f() { await g(); }
来源：http://hpc.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bxw.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jky.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yhj.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://eyc.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://cjx.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://bxd.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://gms.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ltg.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://etj.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://wvn.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qbm.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bzt.ivvv.top

Ruby: threads.map(&:join)
来源：http://uyy.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nuq.chenlongwang.top

[O06] 使用进程池
来源：http://wjh.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ikk.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pnw.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://dvt.pycfn.com

TS:   // child_process / cluster 模块
来源：http://mir.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tvl.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tub.mhx1999.top

Ruby: // fork 块
来源：http://xpo.ydzc1.top

C#:   Parallel.For
来源：http://jhy.nwbrower.top

================================================================================
来源：http://fhm.ywan-chungtsiang.top

P. 常用工具函数
来源：http://mde.hnqzz.top

================================================================================
来源：http://sab.hcnkem.com

[P01] 生成 UUID
来源：http://gvc.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://qak.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://puw.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://box.fktsv.cn

TS:   crypto.randomUUID()
来源：http://tmu.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://qbm.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://oht.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://ulb.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://vqv.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://msq.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://phf.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cri.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ceu.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xpx.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tzp.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://spt.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://riy.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fnu.yuanzhike.top

[P03] 生成短随机字符串
来源：http://ylh.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lpt.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iin.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jhk.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://goh.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ldn.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wtr.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kcl.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://skv.sufxvd.cn

[P04] 求长度
来源：http://mvf.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jpq.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xdc.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nkv.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhw.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://nrg.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://fad.guannengcc.top

Ruby: x.length;  x.size
来源：http://usn.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ojy.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://xjz.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vra.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://axw.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://loc.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nli.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://exw.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://abc.yj20258888.top

Ruby: a == b
来源：http://coa.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://smz.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://noj.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hen.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://vtp.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ygw.52xcode.cn

TS:   if (x == null) {}
来源：http://rwd.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://owq.nwbrower.top

Go:   if x == nil {}
来源：http://xhq.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ift.zhongyouzk.top

C#:   if (x is null) {}
来源：http://ali.havefunace.top

[P07] 防抖与节流
来源：http://cvx.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hmk.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://abt.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ven.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptu.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ssd.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bmd.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jnl.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hht.andypj.xyz

[P08] 处理浮点精度问题
来源：http://nwi.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nhd.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qsn.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lwx.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hze.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ggx.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ked.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zix.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zkf.fehbvm.com

================================================================================
来源：http://ozr.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nca.jlsjyb.cn

================================================================================
来源：http://nbm.ydjk.org.cn

[Q01] 创建表
来源：http://ylv.jianghu66.top

CREATE TABLE users (
来源：http://ctu.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lkd.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://ehm.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://ega.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ren.zhixingplan.top

);
来源：http://xme.tanke756.top

[Q02] 创建带外键的表
来源：http://fjx.dashuyun.cn

CREATE TABLE orders (
来源：http://upm.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qom.xinyue.icu

user_id INT NOT NULL,
来源：http://aog.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://hgw.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mqg.jiagoushi.top

);
来源：http://eyd.zhiwuduotai.top

[Q03] 增加列
来源：http://qnm.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wbn.sjlbkw.cn

[Q04] 修改列类型
来源：http://hlb.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xtn.xylfe.cn

[Q05] 重命名列
来源：http://ipt.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kcu.yuanzhike.top

[Q06] 删除列
来源：http://qfd.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://iog.jqgufenzy.top

[Q07] 删除表
来源：http://vvo.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://pql.gaohongyu789.top

[Q08] 创建普通索引
来源：http://crj.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ziu.snrcjt.cn

[Q09] 创建唯一索引
来源：http://saa.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hkh.cdnleiting.top

[Q10] 插入单行
来源：http://hvs.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://huk.nanxuanxn.top

[Q11] 一次插入多行
来源：http://djk.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pbr.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://bbu.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://yfk.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vip.yfazqb.com

[Q13] 忽略重复插入
来源：http://mto.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bns.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://mwn.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wto.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tod.gzhubu.top

[Q15] 查询全部
来源：http://fxb.aibaodan.cn

SELECT * FROM users;
来源：http://lbt.daria6918.cn

[Q16] 查询指定列
来源：http://hqh.guannengcc.top

SELECT id, name FROM users;
来源：http://hmo.gzhubu.top

[Q17] 条件查询
来源：http://qpw.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://btb.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://gdu.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ozd.xuetiantiany.cn

[Q19] 范围查询
来源：http://nto.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mds.0kj1m.cn

[Q20] IN 列表
来源：http://roe.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://szc.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://vqq.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mkc.tanke756.top

[Q22] 排序
来源：http://xei.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kjf.kuanghao11.cn

[Q23] 分页
来源：http://wuk.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vhk.iojbl.cn

[Q24] 去重
来源：http://ogc.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://nbc.52xcode.cn

[Q25] 只取前 N 条
来源：http://unh.feifeiyinyue.top


<!-- 参考信息 -->