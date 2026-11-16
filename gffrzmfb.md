代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://wya.zhaomingkeji.xyz

================================================================================
来源：http://sbu.yanxiufei.cn

N. 数据结构与算法
来源：http://pkv.tianlin.xyz

================================================================================
来源：http://cnm.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://bkb.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ful.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://avx.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzf.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://las.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://piq.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://ruf.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfl.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ogn.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://qei.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://hba.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nxk.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xqc.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rwf.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ell.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://jnm.quarkkingdee.top

Ruby: arr.sort
来源：http://zbl.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ioo.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://cpd.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrc.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://pnt.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://emz.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyx.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rlt.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cbz.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vto.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://wxz.ybcxt.top

[N04] 斐波那契数列
来源：http://utk.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxo.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://goo.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qeu.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivy.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gjt.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://urs.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zjk.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tii.quarkkingdee.top

[N05] 最大公约数
来源：http://pcn.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://dbs.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zcu.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tox.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ciu.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kkj.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bxz.ctjpmb.com

Ruby: a.gcd(b)
来源：http://aqx.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oxn.xziqi.cn

[N06] 判断回文字符串
来源：http://jxv.hcnkem.com

Py:   s == s[::-1]
来源：http://lcj.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://opw.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://aoy.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://frr.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jmi.epnwcf.com

Go:   // 双指针从两端比较
来源：http://mpq.zdqjudy.top

Ruby: s == s.reverse
来源：http://kcx.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://udr.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://oau.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qoa.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zzv.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cma.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://qmm.yonumen.top

Java: // 手写 HashMap
来源：http://oei.wangdashe.top

Go:   // 手写 map[int]int
来源：http://xhn.ybcxt.top

Ruby: // 手写 Hash
来源：http://wvm.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://dax.gotoacloud.top

[N08] 生成全排列
来源：http://ibw.pycfn.com

Py:   itertools.permutations(arr)
来源：http://xaq.jiagoushi.top

PHP:  // 手写递归交换
来源：http://tua.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://bzm.sufxvd.cn

TS:   // 手写回溯递归
来源：http://evt.sjlbkw.cn

Java: // 手写回溯递归
来源：http://tzx.smart0.xyz

Go:   // 手写回溯递归
来源：http://jev.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://apl.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://upt.bbcook.cn

[N09] 栈与队列
来源：http://xmo.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gsu.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kcc.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ltu.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pjs.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://quv.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ggy.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ofc.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sle.shangyingyoupin.top

[N10] 链表节点定义
来源：http://epd.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnq.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qit.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vvj.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cax.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://fih.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://uke.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://trh.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pbv.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://ado.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fpv.shzxlz.cn

PHP:  // 手写递归函数
来源：http://set.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://amb.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://abb.sxryk.cn

Java: // 手写递归
来源：http://wko.xziqi.cn

Go:   // 手写递归
来源：http://frp.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oui.wangshuangyany.cn

C#:   // 手写递归
来源：http://qnw.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iax.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lit.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gcf.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qjs.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://edl.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ufe.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fso.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hjh.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jdr.smart0.xyz

================================================================================
来源：http://gyd.bjfxy.top

O. 并发与异步
来源：http://bth.jyoumei.cn

================================================================================
来源：http://enx.daxiang520.top

[O01] 启动一个线程
来源：http://mkt.yueranfly.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rcf.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vil.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://abh.xuetiantiany.cn

TS:   // 同 JS
来源：http://woc.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://fok.yfazqb.com

Go:   go f()
来源：http://pnb.haohaochexian.top

Ruby: Thread.new { f }
来源：http://oos.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://lyq.fktsv.cn

[O02] 使用线程池
来源：http://bup.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://njj.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xzw.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://ymh.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://okg.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lnq.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gyv.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://knc.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jxl.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://ppd.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://ynk.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://vmr.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yvt.ppjwa.cn

TS:   // 同 JS
来源：http://slv.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://mne.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bgh.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oya.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://bhx.fengsongda.top

[O04] 定义异步函数并等待
来源：http://irc.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://wvc.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wib.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://uaf.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jgo.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zek.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://svv.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://yir.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://sqg.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://yqa.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://sri.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mtf.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://kok.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://gql.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://krm.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mlo.wangdashe.top

Ruby: threads.map(&:join)
来源：http://kyx.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xqn.zhoulong.xyz

[O06] 使用进程池
来源：http://oha.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ysc.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fnk.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://vih.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://jsy.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mtc.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tmv.guowangkeji.top

Ruby: // fork 块
来源：http://iko.guowangkeji.top

C#:   Parallel.For
来源：http://nvd.sweek.top

================================================================================
来源：http://qje.sufxvd.cn

P. 常用工具函数
来源：http://xdq.xingfuxueyuan.xyz

================================================================================
来源：http://keq.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://omh.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://hgo.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gnh.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://fwg.hesvh.cn

TS:   crypto.randomUUID()
来源：http://vtu.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://rwu.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://gtf.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://fbw.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://cuq.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://cnn.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mlh.dianchejie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bjm.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iqe.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fra.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xwj.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyo.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jkz.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dju.iojbl.cn

[P03] 生成短随机字符串
来源：http://xud.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mye.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://acn.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xed.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ewr.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zph.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zwa.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nnr.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bvp.sjlbkw.cn

[P04] 求长度
来源：http://dkh.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zeg.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byo.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jbb.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wsa.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://her.smart0.xyz

Go:   len(arr);  len(m)
来源：http://toj.sysykeji.top

Ruby: x.length;  x.size
来源：http://tmb.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://liq.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://foi.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nkl.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kat.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eus.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vwq.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sim.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://vhy.cqqwz.cn

Ruby: a == b
来源：http://cuh.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qkc.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ogq.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hhe.316326.xyz

PHP:  if (empty($x)) {}
来源：http://uhn.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nhs.svipenyu.cn

TS:   if (x == null) {}
来源：http://bng.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://sik.fzhhl.top

Go:   if x == nil {}
来源：http://kwo.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eyb.zdqjudy.top

C#:   if (x is null) {}
来源：http://wrt.jinqigfzy.top

[P07] 防抖与节流
来源：http://tva.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sjw.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://mha.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrb.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://and.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://swa.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gfu.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kds.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gmt.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://ngk.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://msd.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aeu.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aio.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tpa.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qns.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fpb.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://opo.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://geq.hysaishi.cn

================================================================================
来源：http://tzu.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ffj.zdqjudy.top

================================================================================
来源：http://prq.gotoacloud.top

[Q01] 创建表
来源：http://tck.zdbjq.cn

CREATE TABLE users (
来源：http://pvo.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://phg.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://myu.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://gou.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eyk.zhijiandao.cn

);
来源：http://htg.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://gdi.snrcjt.cn

CREATE TABLE orders (
来源：http://tta.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qac.xylfe.cn

user_id INT NOT NULL,
来源：http://wre.c1oappe.top

amount DECIMAL(10, 2),
来源：http://vny.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gzl.gogol.net.cn

);
来源：http://jdb.ppjwa.cn

[Q03] 增加列
来源：http://ylv.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://brd.kuanghao11.cn

[Q04] 修改列类型
来源：http://iqu.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kso.havefunace.top

[Q05] 重命名列
来源：http://yix.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ggj.sxryk.cn

[Q06] 删除列
来源：http://vgm.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dpu.ywan-chungtsiang.top

[Q07] 删除表
来源：http://pfb.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://mmi.daria6918.cn

[Q08] 创建普通索引
来源：http://src.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://roy.ppjwa.cn

[Q09] 创建唯一索引
来源：http://mrv.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nwg.zhoulong.xyz

[Q10] 插入单行
来源：http://zti.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zca.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://cxv.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hfe.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://kdu.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://szt.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lyc.aizwys.cn

[Q13] 忽略重复插入
来源：http://vnj.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://drn.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://nhj.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jxy.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://taw.bjfxy.top

[Q15] 查询全部
来源：http://ayt.hfpthk.cn

SELECT * FROM users;
来源：http://zfx.sysykeji.top

[Q16] 查询指定列
来源：http://ywp.ybcxt.top

SELECT id, name FROM users;
来源：http://ojt.fanxiaobao.xyz

[Q17] 条件查询
来源：http://wmy.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wil.mhx1999.top

[Q18] 模糊匹配
来源：http://wov.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zjq.tian-w.cn

[Q19] 范围查询
来源：http://rfd.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ffb.jiagoushi.top

[Q20] IN 列表
来源：http://omg.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jml.smart0.xyz

[Q21] 空值判断
来源：http://jcz.yfazqb.com


<!-- 参考信息 -->