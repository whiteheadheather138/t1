代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hgm.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rnl.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uhg.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pru.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zpp.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://rbl.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://znh.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dis.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fuc.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://uto.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://gcx.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zfw.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pjr.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dkr.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://joo.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://grm.nanxuanxn.top

Ruby: arr.sort
来源：http://zqw.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://jve.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://hnq.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fon.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://ium.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://luy.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pvv.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nep.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vdx.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kij.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://edu.gzhubu.top

[N04] 斐波那契数列
来源：http://wyx.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wgo.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yyv.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxh.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jsl.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aem.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kdi.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zam.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kze.tian-w.cn

[N05] 最大公约数
来源：http://aph.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://ceh.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gnh.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://grr.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwp.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jfw.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://moe.xylfe.cn

Ruby: a.gcd(b)
来源：http://bel.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ekk.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://rts.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://euz.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://xxp.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://mxk.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://hcf.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hsp.yfazqb.com

Go:   // 双指针从两端比较
来源：http://gbo.guowangkeji.top

Ruby: s == s.reverse
来源：http://our.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://phd.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://wqs.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ynl.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zaf.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eir.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://ism.xuanzx.com

Java: // 手写 HashMap
来源：http://iuq.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://mly.chenlongwang.top

Ruby: // 手写 Hash
来源：http://rcg.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://xqw.hammf.cn

[N08] 生成全排列
来源：http://odd.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://nxp.epnwcf.com

PHP:  // 手写递归交换
来源：http://hfe.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://lam.cucudq.cn

TS:   // 手写回溯递归
来源：http://dkb.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://qjq.yj20258888.top

Go:   // 手写回溯递归
来源：http://cnv.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://kcw.xylfe.cn

C#:   // 手写回溯递归
来源：http://ncc.birdmap.top

[N09] 栈与队列
来源：http://jah.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oho.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ibh.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ruy.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uwz.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://evb.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bvv.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://otq.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://njx.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://mbe.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dql.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bgu.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://twm.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lnv.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://bqy.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://qch.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cgu.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://coh.c1oappe.top

[N11] 二叉树中序遍历
来源：http://epi.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jio.yfazqb.com

PHP:  // 手写递归函数
来源：http://wdh.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tkv.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ozh.meibo888.top

Java: // 手写递归
来源：http://wgx.hesvh.cn

Go:   // 手写递归
来源：http://imm.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://djw.yfazqb.com

C#:   // 手写递归
来源：http://niz.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vpw.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tzg.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://shv.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://loi.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwj.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ati.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gxo.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://syc.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ugg.jinghuilouyu.cn

================================================================================
来源：http://uxt.sysykeji.top

O. 并发与异步
来源：http://veg.shanyushiyangkeji.top

================================================================================
来源：http://sad.jinqigufen.top

[O01] 启动一个线程
来源：http://jna.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://scj.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nob.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://agp.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://bok.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://lbg.chenlongwang.top

Go:   go f()
来源：http://iic.yuxming.cn

Ruby: Thread.new { f }
来源：http://olr.tanke756.top

C#:   Task.Run(() => F());
来源：http://mut.jinqigufen.top

[O02] 使用线程池
来源：http://yft.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pyd.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tcp.fengsongda.top

JS:   // worker_threads 线程池
来源：http://evw.jianghu66.top

TS:   // worker_threads 线程池
来源：http://orx.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://bih.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://suo.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://itk.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lvj.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://mtz.nwbrower.top

Py:   with lock: shared += 1
来源：http://yzy.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://qqs.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tyo.fanxiaobao.xyz

TS:   // 同 JS
来源：http://hla.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://hne.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hiw.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tng.tarul.cn

C#:   lock (gate) { shared++; }
来源：http://kzp.zycfv.cn

[O04] 定义异步函数并等待
来源：http://bvf.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://xcw.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://myx.shuidangran.top

JS:   async function f() { await g(); }
来源：http://mvd.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rsg.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fny.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eem.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nsp.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://jzz.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://rqv.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://cgc.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oax.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://war.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://edz.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://via.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gnh.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://vzv.yonumen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lnl.sufxvd.cn

[O06] 使用进程池
来源：http://zng.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jco.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://kdc.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://chr.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://oyt.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cln.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yvz.xylfe.cn

Ruby: // fork 块
来源：http://wdy.bbcook.cn

C#:   Parallel.For
来源：http://nlw.smart0.xyz

================================================================================
来源：http://lpq.zdqjudy.top

P. 常用工具函数
来源：http://rir.yueranfly.top

================================================================================
来源：http://iqu.vehdjk.com

[P01] 生成 UUID
来源：http://jnd.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://tob.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ibo.havefunace.top

JS:   crypto.randomUUID()
来源：http://unv.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://sbr.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://cqo.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://byq.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://fyc.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://kuc.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://ykt.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nvw.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tlm.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fvz.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://udj.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ppw.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cnh.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yrj.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tkt.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://qnc.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://epb.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vuk.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rtv.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upl.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ivb.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lii.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kfz.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qoj.jianghu66.top

[P04] 求长度
来源：http://ggv.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mga.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxd.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ell.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tye.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://jvz.iojbl.cn

Go:   len(arr);  len(m)
来源：http://jln.ehwqpu.com

Ruby: x.length;  x.size
来源：http://cve.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://okr.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://bgr.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://sgu.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fpo.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sqk.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ima.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ioy.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://lkl.quarkkingdee.top

Ruby: a == b
来源：http://cwa.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://llo.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ayg.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dwf.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://eld.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cvj.hnxiangtu.top

TS:   if (x == null) {}
来源：http://afd.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://phg.jqgfzy.top

Go:   if x == nil {}
来源：http://hgq.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pyb.zhongyouzk.top

C#:   if (x is null) {}
来源：http://ktz.yanxiufei.cn

[P07] 防抖与节流
来源：http://zbh.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ein.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://cbt.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euj.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyq.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://smd.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://miy.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ghp.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kyk.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://bqr.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pjw.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://htq.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dnv.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pbt.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://noz.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xsu.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qjc.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ntb.yj20258.top

================================================================================
来源：http://rmh.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vgx.jiagoushi.top

================================================================================
来源：http://zwo.uphjek.com

[Q01] 创建表
来源：http://ivg.jlsjyb.cn

CREATE TABLE users (
来源：http://gce.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozn.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://yvk.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://uzr.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sbj.aizwys.cn

);
来源：http://amd.yangfankeji.com

[Q02] 创建带外键的表
来源：http://ymh.guowangkeji.top

CREATE TABLE orders (
来源：http://jyc.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gpq.hnqzz.top

user_id INT NOT NULL,
来源：http://kiq.c1oappe.top

amount DECIMAL(10, 2),
来源：http://ujd.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tze.yonumen.top

);
来源：http://ruq.wangdashe.top

[Q03] 增加列
来源：http://ecv.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dhu.chenzaomai.com

[Q04] 修改列类型
来源：http://ttl.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://otf.iojbl.cn

[Q05] 重命名列
来源：http://bbq.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fsx.cheryme.top

[Q06] 删除列
来源：http://pgd.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cmt.shanyushiyangkeji.top

[Q07] 删除表
来源：http://azy.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://eoi.andypj.xyz

[Q08] 创建普通索引
来源：http://pkb.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hov.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://iqk.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qmi.tarul.cn

[Q10] 插入单行
来源：http://dny.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ldo.iojbl.cn

[Q11] 一次插入多行
来源：http://ynb.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gjt.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://wtu.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://xun.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rhi.gotoacloud.top

[Q13] 忽略重复插入
来源：http://xdd.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://muq.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://jed.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://afs.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gbi.yvedp.cn

[Q15] 查询全部
来源：http://bwm.dashuyun.cn

SELECT * FROM users;
来源：http://tas.sxryk.cn

[Q16] 查询指定列
来源：http://hbv.9152youxi.cn

SELECT id, name FROM users;
来源：http://ult.sweek.top

[Q17] 条件查询
来源：http://cdn.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://feb.cqqwz.cn

[Q18] 模糊匹配
来源：http://ffm.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uxk.9152youxi.cn

[Q19] 范围查询
来源：http://vom.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://anc.sjlbkw.cn

[Q20] IN 列表
来源：http://iuk.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lij.shangyingyoupin.top

[Q21] 空值判断
来源：http://qyk.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://rfy.sjlbkw.cn

[Q22] 排序
来源：http://rqy.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jhn.jqgufenzy.top

[Q23] 分页
来源：http://quu.ydjk.org.cn


<!-- 参考信息 -->