代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbh.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://heh.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://nla.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://zje.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://asb.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://vzl.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://bml.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://byi.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://naz.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qxt.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mfj.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://jsu.yj20258.top

Ruby: arr.sort
来源：http://hrd.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aiz.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://roa.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rgg.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://njw.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gac.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://enw.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gmt.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bcn.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://umb.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jxc.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://emo.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wot.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://apq.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jgb.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyk.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://itl.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vcp.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ulw.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mtt.chenlongwang.top

[N05] 最大公约数
来源：http://ncl.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://evz.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dgu.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zpw.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wie.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ljl.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wyq.hysaishi.cn

Ruby: a.gcd(b)
来源：http://ptz.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nbh.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://pja.cdnleiting.top

Py:   s == s[::-1]
来源：http://xkm.cucudq.cn

PHP:  $s === strrev($s);
来源：http://cqs.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://yxp.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://srp.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fps.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://gsz.svipenyu.cn

Ruby: s == s.reverse
来源：http://fsg.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://lzl.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://fxu.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cbg.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bwk.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zfu.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://xif.fzhhl.top

Java: // 手写 HashMap
来源：http://ptg.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://jfm.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://gci.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://huo.zhijiandao.cn

[N08] 生成全排列
来源：http://vam.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://lgy.fengsongda.top

PHP:  // 手写递归交换
来源：http://ggv.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://exw.hesvh.cn

TS:   // 手写回溯递归
来源：http://ksh.ehwqpu.com

Java: // 手写回溯递归
来源：http://auv.meibo888.top

Go:   // 手写回溯递归
来源：http://vif.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://yhh.52xcode.cn

C#:   // 手写回溯递归
来源：http://aag.gaohongyu789.top

[N09] 栈与队列
来源：http://oga.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zma.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cfi.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ahk.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oiq.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pwa.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwd.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hxt.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iqm.sufxvd.cn

[N10] 链表节点定义
来源：http://jwf.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hxy.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://puz.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://arz.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://apr.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://xqt.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uph.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rzw.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://mwc.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://tym.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oig.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://qip.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jjm.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://emf.svipenyu.cn

Java: // 手写递归
来源：http://uec.hammf.cn

Go:   // 手写递归
来源：http://mxw.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ayp.wangshuangyany.cn

C#:   // 手写递归
来源：http://bga.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xfz.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eeo.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tuf.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uik.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bre.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lmy.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jlf.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://srb.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qcw.daxiang520.top

================================================================================
来源：http://rtd.yanxiufei.cn

O. 并发与异步
来源：http://umc.jinghuilouyu.cn

================================================================================
来源：http://lvq.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://nus.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qaf.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rzo.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lhh.xinyue.icu

TS:   // 同 JS
来源：http://fgm.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://pnq.wangdashe.top

Go:   go f()
来源：http://jpk.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://cun.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://lbs.shangyingyoupin.top

[O02] 使用线程池
来源：http://pay.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oad.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ycd.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://zgr.yvedp.cn

TS:   // worker_threads 线程池
来源：http://xdy.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://qxd.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cml.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eoq.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kol.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://efi.yj20258.top

Py:   with lock: shared += 1
来源：http://xmm.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://cpg.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kxe.hywenlv.cn

TS:   // 同 JS
来源：http://pwt.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://jvh.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://okd.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sgz.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://smw.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://bml.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://iys.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mze.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://vlv.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fpz.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mrg.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vxy.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://xvx.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://gft.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://ami.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://mex.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jci.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://pzy.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://doh.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xqo.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://prt.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://vjx.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bbx.redwolf501.top

[O06] 使用进程池
来源：http://gzm.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xdt.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uxu.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://fuq.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://lxh.ydzc1.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dxn.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zck.ydzc1.top

Ruby: // fork 块
来源：http://bsn.nanxuanxn.top

C#:   Parallel.For
来源：http://iwi.c1oappe.top

================================================================================
来源：http://kab.pycfn.com

P. 常用工具函数
来源：http://nny.uphjek.com

================================================================================
来源：http://rpn.cucudq.cn

[P01] 生成 UUID
来源：http://sun.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://dht.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ufb.uphjek.com

JS:   crypto.randomUUID()
来源：http://oqu.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://bsm.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://gds.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://kls.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://gwl.hfpthk.cn

C#:   Guid.NewGuid().ToString()
来源：http://rac.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://fwn.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tre.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ilk.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ouy.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iem.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fds.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oza.aizwys.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mkh.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rza.yuxming.cn

[P03] 生成短随机字符串
来源：http://pbs.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mhe.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://emx.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tjg.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gak.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://smy.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wws.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mmo.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://czx.hysaishi.cn

[P04] 求长度
来源：http://rmn.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uff.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://whp.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yve.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ied.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://rul.cheryme.top

Go:   len(arr);  len(m)
来源：http://slv.yj20258888.top

Ruby: x.length;  x.size
来源：http://mxj.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ieq.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://all.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qrp.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tzy.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vqn.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://khw.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lev.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pnr.hesvh.cn

Ruby: a == b
来源：http://fqh.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jry.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bil.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ctz.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://wqc.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ttd.yongpay.top

TS:   if (x == null) {}
来源：http://uwh.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ddp.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://zbu.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://skl.zdqjudy.top

C#:   if (x is null) {}
来源：http://tsa.bbcook.cn

[P07] 防抖与节流
来源：http://cpy.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iaq.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://nkd.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dce.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfp.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kzf.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://scz.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ntl.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://idm.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://cuw.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eck.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jqk.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oar.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dhu.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ood.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yfw.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ldh.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rtt.aibaodan.cn

================================================================================
来源：http://seq.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rzz.wangdashe.top

================================================================================
来源：http://pys.jinghuilouyu.cn

[Q01] 创建表
来源：http://dfc.shuidangran.top

CREATE TABLE users (
来源：http://qrk.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mqj.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://tiw.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://gqj.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nwq.svipenyu.cn

);
来源：http://qev.fktsv.cn

[Q02] 创建带外键的表
来源：http://ree.fktsv.cn

CREATE TABLE orders (
来源：http://afh.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hev.yuanzhike.top

user_id INT NOT NULL,
来源：http://ejl.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://okr.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xyf.cdnleiting.top

);
来源：http://vfr.sjlbkw.cn

[Q03] 增加列
来源：http://fgc.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ooe.cqqwz.cn

[Q04] 修改列类型
来源：http://zeq.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nma.pycfn.com

[Q05] 重命名列
来源：http://uen.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oei.shanyushiyangkeji.top

[Q06] 删除列
来源：http://xtk.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://irt.jiagoushi.top

[Q07] 删除表
来源：http://yxg.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://vou.xuanzx.com

[Q08] 创建普通索引
来源：http://ktc.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://svm.jianghu66.top

[Q09] 创建唯一索引
来源：http://wod.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ojj.zdqjudy.top

[Q10] 插入单行
来源：http://uqm.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pvr.haohaochexian.top

[Q11] 一次插入多行
来源：http://lue.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://edf.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://qnz.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://kex.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xmg.zycfv.cn

[Q13] 忽略重复插入
来源：http://wch.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yxi.sweek.top

[Q14] 存在则更新（upsert）
来源：http://csu.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://twy.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dii.hesvh.cn

[Q15] 查询全部
来源：http://nnb.hnqzz.top

SELECT * FROM users;
来源：http://nap.hywenlv.cn

[Q16] 查询指定列
来源：http://yvx.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://jep.hywenlv.cn

[Q17] 条件查询
来源：http://yup.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sat.jqgufenzy.top

[Q18] 模糊匹配
来源：http://ouz.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pzr.pengpengdd.cyou

[Q19] 范围查询
来源：http://fyy.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ofg.zdqjudy.top

[Q20] IN 列表
来源：http://max.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xmy.zycfv.cn

[Q21] 空值判断
来源：http://ysv.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://dye.nanxinkj.top

[Q22] 排序
来源：http://cpg.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dkn.c1oappe.top

[Q23] 分页
来源：http://gln.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zqp.vqdsnc.cn

[Q24] 去重
来源：http://hew.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://ifa.tarul.cn

[Q25] 只取前 N 条
来源：http://zht.ctjpmb.com


<!-- 参考信息 -->