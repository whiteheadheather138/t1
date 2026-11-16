代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pej.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://baq.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://xpg.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lgy.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://yzz.ywan-chungtsiang.top

[N02] 排序（工程实践用内置实现）
来源：http://ndl.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://acp.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cml.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hiu.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gwz.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wxn.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://vsn.guowangkeji.top

Ruby: arr.sort
来源：http://xzb.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sah.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://yfp.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eah.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://uvq.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jwy.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dkw.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dry.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dun.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://esp.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zuv.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://kyo.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lnh.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://off.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rbe.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbl.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vzq.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qji.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bvs.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xyy.ehwqpu.com

[N05] 最大公约数
来源：http://xhb.pycfn.com

Py:   math.gcd(a, b)
来源：http://mgi.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://izd.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://afg.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://amt.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kyf.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ztg.nwbrower.top

Ruby: a.gcd(b)
来源：http://fgr.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lxj.yuxming.cn

[N06] 判断回文字符串
来源：http://mbm.52xcode.cn

Py:   s == s[::-1]
来源：http://tty.ydzc1.top

PHP:  $s === strrev($s);
来源：http://awj.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://yks.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://zjy.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lbz.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://zgt.cheryme.top

Ruby: s == s.reverse
来源：http://zse.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sra.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://fih.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nuu.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wqw.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://exr.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://gpl.ehwqpu.com

Java: // 手写 HashMap
来源：http://luc.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://mnm.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://edf.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://suh.gzhubu.top

[N08] 生成全排列
来源：http://jvb.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://chp.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://hdm.epnwcf.com

JS:   // 手写回溯递归
来源：http://pdz.havefunace.top

TS:   // 手写回溯递归
来源：http://wqv.jinqigfzy.top

Java: // 手写回溯递归
来源：http://rdz.fktsv.cn

Go:   // 手写回溯递归
来源：http://ovw.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://kew.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://kxn.aibaodan.cn

[N09] 栈与队列
来源：http://ldl.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nhe.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wbe.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ttk.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bne.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ixr.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxu.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zfx.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ucv.wangdashe.top

[N10] 链表节点定义
来源：http://ewu.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oxu.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sra.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ueg.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cue.uphjek.com

Java: class Node { int v; Node next; }
来源：http://bda.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rrm.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://rrs.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rsy.epnwcf.com

[N11] 二叉树中序遍历
来源：http://jjx.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xel.xuanzx.com

PHP:  // 手写递归函数
来源：http://ewn.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uvj.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vnm.ehwqpu.com

Java: // 手写递归
来源：http://pqb.fengsongda.top

Go:   // 手写递归
来源：http://wkt.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wnj.0kj1m.cn

C#:   // 手写递归
来源：http://zxy.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://euj.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pnf.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xtw.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyi.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsa.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lno.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xqv.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gtw.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://emu.cdnleiting.top

================================================================================
来源：http://mme.yuxming.cn

O. 并发与异步
来源：http://ijz.gaohongyu789.top

================================================================================
来源：http://mri.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://rqb.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://udv.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pwi.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qlj.xuetiantiany.cn

TS:   // 同 JS
来源：http://yvr.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://ctx.kuanghao11.cn

Go:   go f()
来源：http://pwn.cheryme.top

Ruby: Thread.new { f }
来源：http://qss.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://wkp.daria6918.cn

[O02] 使用线程池
来源：http://jwl.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gum.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uoz.birdmap.top

JS:   // worker_threads 线程池
来源：http://cgr.bjfxy.top

TS:   // worker_threads 线程池
来源：http://jab.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://vik.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fth.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bhh.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ciy.xylfe.cn

[O03] 加锁保护共享数据
来源：http://jfc.bbcook.cn

Py:   with lock: shared += 1
来源：http://utd.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://nlh.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sjp.shuidangran.top

TS:   // 同 JS
来源：http://toh.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://uub.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kpl.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jxa.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://avz.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://jfw.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://kuo.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jmj.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://sjb.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fgw.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zgo.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ivm.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jal.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://nto.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://dav.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://mbn.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xaa.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://gqy.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://saj.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ahk.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gkh.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://vtc.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://amt.jinqigufen.top

[O06] 使用进程池
来源：http://sts.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kld.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://krl.birdmap.top

JS:   // child_process / cluster 模块
来源：http://tvg.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://ijx.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vxs.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jls.snrcjt.cn

Ruby: // fork 块
来源：http://jho.uphjek.com

C#:   Parallel.For
来源：http://pcu.zhengqikj.top

================================================================================
来源：http://kmt.tarul.cn

P. 常用工具函数
来源：http://uqu.yj20258.top

================================================================================
来源：http://qbd.zhengqikj.top

[P01] 生成 UUID
来源：http://ywe.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://aks.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gbe.yj202588.top

JS:   crypto.randomUUID()
来源：http://zjv.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://bqa.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://bzv.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://zqi.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://eqy.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://wys.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://jrp.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmx.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ynw.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lma.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://puz.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nsi.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://boo.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ldg.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gnf.cqqwz.cn

[P03] 生成短随机字符串
来源：http://rdk.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gkl.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pwt.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dxi.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gbx.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://khn.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gci.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iyr.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oqp.yongpay.top

[P04] 求长度
来源：http://xnn.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tby.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucv.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hqe.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bey.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://uti.hammf.cn

Go:   len(arr);  len(m)
来源：http://agz.haohaochexian.top

Ruby: x.length;  x.size
来源：http://vzf.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zic.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://sec.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gmx.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tmc.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://umf.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ihv.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zwm.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://eeo.guowangkeji.top

Ruby: a == b
来源：http://smk.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tnt.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pgo.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ahv.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://how.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ooh.hfpthk.cn

TS:   if (x == null) {}
来源：http://jxg.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xpg.chenzaomai.com

Go:   if x == nil {}
来源：http://fuj.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://auu.gotoacloud.top

C#:   if (x is null) {}
来源：http://koq.guowangkeji.top

[P07] 防抖与节流
来源：http://zwr.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jnf.yonumen.top

PHP:  // 手写时间戳比较
来源：http://rdr.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwq.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ied.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qys.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://urg.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zcc.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ftq.ydzc1.top

[P08] 处理浮点精度问题
来源：http://yzs.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://caw.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cgp.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aos.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zfn.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ffz.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://shp.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yjm.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sqe.ctjpmb.com

================================================================================
来源：http://kkj.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mpc.yvedp.cn

================================================================================
来源：http://ppe.tian-w.cn

[Q01] 创建表
来源：http://trw.yuanzhike.top

CREATE TABLE users (
来源：http://sot.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oxc.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://rvy.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://oqv.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rxh.jlsjyb.cn

);
来源：http://rwt.guowangkeji.top

[Q02] 创建带外键的表
来源：http://qoa.sufxvd.cn

CREATE TABLE orders (
来源：http://pbs.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jpn.yj20258888.top

user_id INT NOT NULL,
来源：http://voi.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://ubd.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hed.shuidangran.top

);
来源：http://myb.yuanzhike.top

[Q03] 增加列
来源：http://duc.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aqc.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://ncf.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gws.chenzaomai.com

[Q05] 重命名列
来源：http://hus.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ahs.sjlbkw.cn

[Q06] 删除列
来源：http://zbj.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://kpi.wangdashe.top

[Q07] 删除表
来源：http://rbg.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://dqd.0kj1m.cn

[Q08] 创建普通索引
来源：http://svx.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://inp.jyoumei.cn

[Q09] 创建唯一索引
来源：http://mhd.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pku.yanxiufei.cn

[Q10] 插入单行
来源：http://dqy.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://woc.cashguo.top

[Q11] 一次插入多行
来源：http://bik.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fiz.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://psl.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://ksh.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zqf.fengsongda.top

[Q13] 忽略重复插入
来源：http://yhs.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uzf.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://wxn.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qnt.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gah.zhongyouzk.top

[Q15] 查询全部
来源：http://pea.kuanghao11.cn

SELECT * FROM users;
来源：http://efg.yvedp.cn

[Q16] 查询指定列
来源：http://zqd.birdmap.top

SELECT id, name FROM users;
来源：http://wjl.wangdashe.top

[Q17] 条件查询
来源：http://bok.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vze.ivvv.top

[Q18] 模糊匹配
来源：http://bfi.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yos.yanxiufei.cn

[Q19] 范围查询
来源：http://zop.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cec.ydjk.org.cn

[Q20] IN 列表
来源：http://dma.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ykg.fanxiaobao.xyz

[Q21] 空值判断
来源：http://xoi.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ypu.hongshengwenyu.top

[Q22] 排序
来源：http://rqq.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jst.sweek.top

[Q23] 分页
来源：http://vjj.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vmp.fengsongda.top

[Q24] 去重
来源：http://mrg.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://jhf.yuxming.cn

[Q25] 只取前 N 条
来源：http://xvc.yonumen.top


<!-- 参考信息 -->