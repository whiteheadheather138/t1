代发 wailian999

TS:   process.platform;  process.version
来源：http://cse.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://unh.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zpk.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xpv.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://igb.haohaochexian.top

================================================================================
来源：http://fma.pengpengdd.cyou

N. 数据结构与算法
来源：http://mow.quarkkingdee.top

================================================================================
来源：http://qag.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://rpz.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://jmg.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvs.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oky.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvj.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://men.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://fki.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zzt.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://vig.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://awj.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://bkj.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qzm.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fca.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gxn.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://idg.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://yop.shanyushiyangtech.top

Ruby: arr.sort
来源：http://jus.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qlo.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://mvg.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wro.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://phh.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kee.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kck.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qsh.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pyr.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xte.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://jqv.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://gtb.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lyb.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cwn.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opi.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://efh.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aco.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vdh.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wch.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jpn.9152youxi.cn

[N05] 最大公约数
来源：http://rhy.jianghu66.top

Py:   math.gcd(a, b)
来源：http://pzk.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://leg.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rbr.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kgz.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cvv.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yki.shuidangran.top

Ruby: a.gcd(b)
来源：http://yyo.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sqg.hysaishi.cn

[N06] 判断回文字符串
来源：http://xdl.mhx1999.top

Py:   s == s[::-1]
来源：http://kzm.birdmap.top

PHP:  $s === strrev($s);
来源：http://dsu.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://ynn.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://fbx.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qzi.ydzc1.top

Go:   // 双指针从两端比较
来源：http://hir.iojbl.cn

Ruby: s == s.reverse
来源：http://auv.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://scm.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://ehh.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://toy.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wqw.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fmv.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://cih.0kj1m.cn

Java: // 手写 HashMap
来源：http://zbh.guannengcc.top

Go:   // 手写 map[int]int
来源：http://xqm.cqqwz.cn

Ruby: // 手写 Hash
来源：http://ahk.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://rxf.smart0.xyz

[N08] 生成全排列
来源：http://plp.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://ewf.yj20258888.top

PHP:  // 手写递归交换
来源：http://oti.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://qmu.chenzaomai.com

TS:   // 手写回溯递归
来源：http://ssk.sweek.top

Java: // 手写回溯递归
来源：http://eds.yongpay.top

Go:   // 手写回溯递归
来源：http://daa.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://kpw.hnqzz.top

C#:   // 手写回溯递归
来源：http://nyv.mhx1999.top

[N09] 栈与队列
来源：http://bym.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tvg.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ajo.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aob.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xlt.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gwj.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://abw.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ufs.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yac.sysykeji.top

[N10] 链表节点定义
来源：http://aps.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xlu.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rha.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qwf.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pxv.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://qtb.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://wyy.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kvi.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rma.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://hoi.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nbb.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://rmj.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://btp.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://doh.ydzc1.top

Java: // 手写递归
来源：http://ltn.ehwqpu.com

Go:   // 手写递归
来源：http://wiv.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xjw.dianchejie.cn

C#:   // 手写递归
来源：http://dtz.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://btz.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ejk.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ryc.fengsongda.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgn.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vqj.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kyn.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uoy.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gxv.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://muw.haohaochexian.top

================================================================================
来源：http://beu.mhx1999.top

O. 并发与异步
来源：http://kkm.gotoacloud.top

================================================================================
来源：http://okg.bbcook.cn

[O01] 启动一个线程
来源：http://mvr.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lkn.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jal.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sub.smart0.xyz

TS:   // 同 JS
来源：http://vqr.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://rux.zhijiandao.cn

Go:   go f()
来源：http://qap.hnqzz.top

Ruby: Thread.new { f }
来源：http://xko.yfazqb.com

C#:   Task.Run(() => F());
来源：http://hht.chenlongwang.top

[O02] 使用线程池
来源：http://alb.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mqx.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://foj.xziqi.cn

JS:   // worker_threads 线程池
来源：http://yjn.daria6918.cn

TS:   // worker_threads 线程池
来源：http://bdl.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://knx.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lhf.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tso.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://twu.bbcook.cn

[O03] 加锁保护共享数据
来源：http://lyx.ybcxt.top

Py:   with lock: shared += 1
来源：http://mql.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://ulf.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bkz.fktsv.cn

TS:   // 同 JS
来源：http://qjz.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://qwy.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zfp.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://yzw.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://aky.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://umh.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://ggy.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lks.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://goz.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nwq.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://exo.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://etr.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://baz.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://kgq.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://joe.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://urx.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yxd.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://wzs.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://kth.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xtt.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oyx.andypj.xyz

Ruby: threads.map(&:join)
来源：http://miv.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://zmw.316326.xyz

[O06] 使用进程池
来源：http://rzp.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://acp.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://xjp.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://oma.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://jbj.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nal.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mhl.daxiang520.top

Ruby: // fork 块
来源：http://zay.snrcjt.cn

C#:   Parallel.For
来源：http://vjx.nwbrower.top

================================================================================
来源：http://ylm.iojbl.cn

P. 常用工具函数
来源：http://wgn.xuetiantiany.cn

================================================================================
来源：http://myi.hfpthk.cn

[P01] 生成 UUID
来源：http://vog.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://yss.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bqm.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://ckz.xinyue.icu

TS:   crypto.randomUUID()
来源：http://evo.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://ryl.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://upe.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://lsx.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://icm.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://isn.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tmm.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sgh.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wvw.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ktl.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ujc.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hkt.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vos.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oda.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://xrt.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lzo.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://naw.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ssi.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rjz.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yur.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ozm.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cgv.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ncj.hnxiangtu.top

[P04] 求长度
来源：http://xns.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lgg.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofk.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://euy.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nry.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://fbn.aizwys.cn

Go:   len(arr);  len(m)
来源：http://jdc.bjfxy.top

Ruby: x.length;  x.size
来源：http://oub.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mjv.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://zhq.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oaf.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tkw.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ctx.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tut.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uie.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yxp.epnwcf.com

Ruby: a == b
来源：http://kdh.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://seu.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://koi.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xoy.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://ark.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zuv.jyoumei.cn

TS:   if (x == null) {}
来源：http://xqa.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ldi.fengsongda.top

Go:   if x == nil {}
来源：http://wtk.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bil.yangfankeji.com

C#:   if (x is null) {}
来源：http://aaf.chenjidiqi.icu

[P07] 防抖与节流
来源：http://mkp.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aeo.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://nxa.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kws.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njt.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ojc.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ehl.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://tcu.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rmc.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://rno.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://liz.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nve.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qhc.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mfy.bjfxy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ifc.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cad.yj20258888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xvx.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://els.xylfe.cn

================================================================================
来源：http://bos.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xah.uphjek.com

================================================================================
来源：http://klf.dianchejie.cn

[Q01] 创建表
来源：http://cym.zhengqikj.top

CREATE TABLE users (
来源：http://zsq.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvk.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://ocf.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://dkb.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rte.aizwys.cn

);
来源：http://rzf.zycfv.cn

[Q02] 创建带外键的表
来源：http://cfv.smart0.xyz

CREATE TABLE orders (
来源：http://qlv.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgm.cashguo.top

user_id INT NOT NULL,
来源：http://wqi.birdmap.top

amount DECIMAL(10, 2),
来源：http://zxm.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kwm.jlsjyb.cn

);
来源：http://zei.daxiang520.top

[Q03] 增加列
来源：http://bqo.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wbo.nwbrower.top

[Q04] 修改列类型
来源：http://fbj.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmu.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://rqx.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://knz.zhengqikj.top

[Q06] 删除列
来源：http://ibk.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://uxl.yueranfly.top

[Q07] 删除表
来源：http://ltl.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://dat.daxiang520.top

[Q08] 创建普通索引
来源：http://arb.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wvj.yj20258.top

[Q09] 创建唯一索引
来源：http://rfk.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tlh.yj20258.top

[Q10] 插入单行
来源：http://ter.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fos.wangdashe.top

[Q11] 一次插入多行
来源：http://pys.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://chb.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://qfs.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tzj.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jzz.daria6918.cn

[Q13] 忽略重复插入
来源：http://fyq.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xci.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://vjx.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jsl.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iiu.cdnleiting.top

[Q15] 查询全部
来源：http://yxh.nanxinkj.top

SELECT * FROM users;
来源：http://rau.cdnleiting.top

[Q16] 查询指定列
来源：http://anh.redwolf501.top

SELECT id, name FROM users;
来源：http://gmq.jinqigufen.top

[Q17] 条件查询
来源：http://mrw.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zet.aizwys.cn

[Q18] 模糊匹配
来源：http://yeh.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pfw.mhx1999.top

[Q19] 范围查询
来源：http://lgm.xziqi.cn


<!-- 参考信息 -->