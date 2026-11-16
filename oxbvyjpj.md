代发 wailian999

[N01] 二分查找（有序数组）
来源：http://qyz.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://cmz.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dqb.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eap.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kum.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fcw.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://hvb.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://imj.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://quk.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://efj.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://pwb.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hrn.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wzn.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nvr.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pkb.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://qux.aizwys.cn

Ruby: arr.sort
来源：http://slz.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hox.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://owz.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zuz.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://cjl.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mnb.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nsh.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jfa.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lkb.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyv.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://jjf.shanyushiyangkeji.top

[N04] 斐波那契数列
来源：http://foy.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kia.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ihx.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dgu.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tnt.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wwx.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kti.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oog.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uyz.zycfv.cn

[N05] 最大公约数
来源：http://tpv.smart0.xyz

Py:   math.gcd(a, b)
来源：http://iau.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://txw.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzs.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pss.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eus.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zho.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://mcn.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sti.ctjpmb.com

[N06] 判断回文字符串
来源：http://etj.chenlongwang.top

Py:   s == s[::-1]
来源：http://ntq.nwbrower.top

PHP:  $s === strrev($s);
来源：http://wqf.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://gxl.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://blo.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tfa.meibo888.top

Go:   // 双指针从两端比较
来源：http://lmy.ppjwa.cn

Ruby: s == s.reverse
来源：http://qif.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ybk.316326.xyz

[N07] 两数之和（返回下标）
来源：http://qiv.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zfx.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jeo.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jcp.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://yee.redwolf501.top

Java: // 手写 HashMap
来源：http://eay.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://dql.ctjpmb.com

Ruby: // 手写 Hash
来源：http://iqa.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ngm.jinqigufen.top

[N08] 生成全排列
来源：http://rvp.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://ohb.yj20258.top

PHP:  // 手写递归交换
来源：http://dtx.52xcode.cn

JS:   // 手写回溯递归
来源：http://qcd.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://yhs.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://yei.cheryme.top

Go:   // 手写回溯递归
来源：http://drh.cheryme.top

Ruby: arr.permutation.to_a
来源：http://udc.sufxvd.cn

C#:   // 手写回溯递归
来源：http://exw.svipenyu.cn

[N09] 栈与队列
来源：http://oyn.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xwk.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://svg.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iso.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sbw.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cuq.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uds.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qxh.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gsl.chenjidiqi.icu

[N10] 链表节点定义
来源：http://dhl.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vqa.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jbu.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jqt.yj202588.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yyc.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://ngi.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://dox.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dsh.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ena.yonumen.top

[N11] 二叉树中序遍历
来源：http://oij.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lkr.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://zir.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zao.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cpw.hnxiangtu.top

Java: // 手写递归
来源：http://kzo.pycfn.com

Go:   // 手写递归
来源：http://bxo.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xay.yuxming.cn

C#:   // 手写递归
来源：http://prq.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://amc.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xrn.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ymh.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dja.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lut.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://waw.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ajy.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cuo.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kas.yj20258888.top

================================================================================
来源：http://hqh.hnqzz.top

O. 并发与异步
来源：http://eek.yangfankeji.com

================================================================================
来源：http://qrs.guannengcc.top

[O01] 启动一个线程
来源：http://nxy.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pae.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cpf.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sje.smart0.xyz

TS:   // 同 JS
来源：http://dal.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://xcd.sjlbkw.cn

Go:   go f()
来源：http://tpn.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://ujs.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://iaj.snrcjt.cn

[O02] 使用线程池
来源：http://rss.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wzd.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rli.birdmap.top

JS:   // worker_threads 线程池
来源：http://gxt.sxryk.cn

TS:   // worker_threads 线程池
来源：http://klh.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://opq.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ntx.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fhd.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bvs.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://tkd.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://spv.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://sva.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hrj.yj20258.top

TS:   // 同 JS
来源：http://yug.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://jiu.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://asp.daxiang520.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rgv.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://qqd.vehdjk.com

[O04] 定义异步函数并等待
来源：http://wzi.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://big.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://arn.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://bgn.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zbu.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xio.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xhh.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://wio.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://bcn.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://rwj.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://dqg.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://awd.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://dsb.cashguo.top

TS:   await Promise.all(tasks)
来源：http://vgw.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cjy.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gul.wangdashe.top

Ruby: threads.map(&:join)
来源：http://vsb.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://qiu.yuanzhike.top

[O06] 使用进程池
来源：http://fgu.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tkl.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hzx.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://knm.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://ujx.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bbt.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://abi.hfpthk.cn

Ruby: // fork 块
来源：http://tih.hesvh.cn

C#:   Parallel.For
来源：http://nso.zhiwuduotai.top

================================================================================
来源：http://zyu.uphjek.com

P. 常用工具函数
来源：http://djp.xziqi.cn

================================================================================
来源：http://rah.zdqjudy.top

[P01] 生成 UUID
来源：http://fbn.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://iqx.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tqf.vehdjk.com

JS:   crypto.randomUUID()
来源：http://wqj.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://zbf.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://knz.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://qhc.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://zjb.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://rfg.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://dui.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rxk.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bbm.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ses.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eob.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cvj.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xym.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yjf.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://avk.chenlongwang.top

[P03] 生成短随机字符串
来源：http://ypf.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ang.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bbi.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wal.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mri.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rsy.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ako.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vdf.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jbf.jyoumei.cn

[P04] 求长度
来源：http://lcf.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nqp.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gkp.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asf.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bvc.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://yaa.daria6918.cn

Go:   len(arr);  len(m)
来源：http://axg.gotoacloud.top

Ruby: x.length;  x.size
来源：http://wpr.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nya.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://bby.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://skl.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fim.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ksm.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lxz.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gmu.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://gig.hongshengwenyu.top

Ruby: a == b
来源：http://zdw.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zts.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yfr.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uki.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://ypn.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yyq.hcnkem.com

TS:   if (x == null) {}
来源：http://eyg.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ngk.nanxuanxn.top

Go:   if x == nil {}
来源：http://nto.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ldq.ydjk.org.cn

C#:   if (x is null) {}
来源：http://fso.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://rbe.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tco.cashguo.top

PHP:  // 手写时间戳比较
来源：http://txz.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://siu.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ojv.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ith.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qur.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://qnl.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://imt.fehbvm.com

[P08] 处理浮点精度问题
来源：http://pwe.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://duo.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tzb.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ydr.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wxd.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cho.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://izj.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yqb.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uih.chenlongwang.top

================================================================================
来源：http://yer.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://adt.yuxming.cn

================================================================================
来源：http://eqa.hywenlv.cn

[Q01] 创建表
来源：http://krv.xingfuxueyuan.xyz

CREATE TABLE users (
来源：http://ttu.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ydw.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://hek.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://xzm.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zmj.jinyuanbaomall.cn

);
来源：http://jfs.hcnkem.com

[Q02] 创建带外键的表
来源：http://szd.quarkkingdee.top

CREATE TABLE orders (
来源：http://fag.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvf.tianlin.xyz

user_id INT NOT NULL,
来源：http://ndi.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://dho.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rqu.zhijiandao.cn

);
来源：http://mvs.bbcook.cn

[Q03] 增加列
来源：http://ajs.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zzl.jqgufenzy.top

[Q04] 修改列类型
来源：http://vyu.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qnr.ehwqpu.com

[Q05] 重命名列
来源：http://zxz.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://spp.hfpthk.cn

[Q06] 删除列
来源：http://jin.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://lnw.yongpay.top

[Q07] 删除表
来源：http://yit.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://bsv.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://dwu.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://quy.yongpay.top

[Q09] 创建唯一索引
来源：http://zxd.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://igo.jyoumei.cn

[Q10] 插入单行
来源：http://xgg.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dhr.guannengcc.top

[Q11] 一次插入多行
来源：http://fyh.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://era.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://wik.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://cxg.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bpy.wangdashe.top

[Q13] 忽略重复插入
来源：http://wgt.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eak.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://lnu.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lcf.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hak.jinghuilouyu.cn

[Q15] 查询全部
来源：http://hkc.haohaochexian.top

SELECT * FROM users;
来源：http://tlf.zhixingplan.top

[Q16] 查询指定列
来源：http://kei.zhijiandao.cn

SELECT id, name FROM users;
来源：http://zjn.smart0.xyz

[Q17] 条件查询
来源：http://eih.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nnh.sweek.top

[Q18] 模糊匹配
来源：http://inc.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zob.yj20258888.top

[Q19] 范围查询
来源：http://edd.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ynj.yj20258888.top

[Q20] IN 列表
来源：http://nzt.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eqx.tanke756.top

[Q21] 空值判断
来源：http://ukg.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://blf.smart0.xyz

[Q22] 排序
来源：http://hah.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ntg.yangfankeji.com

[Q23] 分页
来源：http://khx.haohaochexian.top


<!-- 参考信息 -->