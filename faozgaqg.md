代发 wailian999

[M08] 获取系统与运行时信息
来源：http://dty.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://ick.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://ibl.havefunace.top

JS:   process.platform;  process.version
来源：http://nxe.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://mcf.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lpz.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yuv.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xvk.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://trk.redwolf501.top

================================================================================
来源：http://vxd.xuanzx.com

N. 数据结构与算法
来源：http://cqr.zycfv.cn

================================================================================
来源：http://pov.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://vce.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lrc.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ttc.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iqe.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yow.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://edi.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://wuj.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ttf.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://ydx.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://xyz.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://nmc.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fiq.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bsh.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yxo.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gkh.cashguo.top

Go:   slices.Sort(arr)
来源：http://dui.yj20258.top

Ruby: arr.sort
来源：http://acw.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ehi.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://tkl.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://erk.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://ywh.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hek.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vkd.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qwp.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://izo.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mwx.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://awn.tanke756.top

[N04] 斐波那契数列
来源：http://ixx.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://epw.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rtl.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzn.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahw.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nbc.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://udt.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ctt.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umh.hammf.cn

[N05] 最大公约数
来源：http://tyv.aizwys.cn

Py:   math.gcd(a, b)
来源：http://zyc.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghg.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gxq.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nde.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fam.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bub.yj202588.top

Ruby: a.gcd(b)
来源：http://yae.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://txz.sxryk.cn

[N06] 判断回文字符串
来源：http://low.cheryme.top

Py:   s == s[::-1]
来源：http://xrj.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://tth.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://yqg.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://jib.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yxm.havefunace.top

Go:   // 双指针从两端比较
来源：http://rci.zdbjq.cn

Ruby: s == s.reverse
来源：http://xpz.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://nsa.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://rnd.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://glf.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jmv.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://jxq.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://dma.shuidangran.top

Java: // 手写 HashMap
来源：http://lkw.52xcode.cn

Go:   // 手写 map[int]int
来源：http://yig.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://jer.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://tzq.cheryme.top

[N08] 生成全排列
来源：http://ilj.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://llv.9152youxi.cn

PHP:  // 手写递归交换
来源：http://yis.0kj1m.cn

JS:   // 手写回溯递归
来源：http://nwz.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://qwj.cashguo.top

Java: // 手写回溯递归
来源：http://lld.snrcjt.cn

Go:   // 手写回溯递归
来源：http://xzo.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://jat.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://tjd.haohaochexian.top

[N09] 栈与队列
来源：http://wir.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tns.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uuk.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rwo.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sxo.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ypn.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rdr.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aff.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gui.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://smc.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zqv.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://klr.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lfp.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jbp.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://mjx.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://mgh.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xge.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tom.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://kib.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ffe.jianghu66.top

PHP:  // 手写递归函数
来源：http://fhy.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sbd.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mfh.gzhubu.top

Java: // 手写递归
来源：http://qjj.pycfn.com

Go:   // 手写递归
来源：http://uch.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zhg.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ssi.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ghv.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cnk.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zao.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://din.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vdc.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://exd.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fad.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dfm.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hhq.shzxlz.cn

================================================================================
来源：http://tpp.ywan-chungtsiang.top

O. 并发与异步
来源：http://ddg.bjfxy.top

================================================================================
来源：http://ewn.chenlongwang.top

[O01] 启动一个线程
来源：http://aqj.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ilk.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oja.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lbz.cdnleiting.top

TS:   // 同 JS
来源：http://acu.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://uui.yj20258888.top

Go:   go f()
来源：http://ldx.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://wly.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://yiq.zhijiandao.cn

[O02] 使用线程池
来源：http://ysu.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ehr.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bts.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://vtm.jianghu66.top

TS:   // worker_threads 线程池
来源：http://iyv.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gky.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ndu.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://djx.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dro.bjfxy.top

[O03] 加锁保护共享数据
来源：http://qfz.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://huq.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://jld.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cgi.mhx1999.top

TS:   // 同 JS
来源：http://oky.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://sin.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ynt.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://apc.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://fod.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://moq.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://yay.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rfx.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://jng.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tgr.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kcj.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yjj.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eic.havefunace.top

C#:   async Task F() { await G(); }
来源：http://qki.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://zuf.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://jvg.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://amw.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://tnw.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://oji.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbk.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tos.nwbrower.top

Ruby: threads.map(&:join)
来源：http://prm.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://smh.sxryk.cn

[O06] 使用进程池
来源：http://ffh.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fli.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rex.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://mvd.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://chb.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sqq.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yrl.fzhhl.top

Ruby: // fork 块
来源：http://lip.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://ome.hesvh.cn

================================================================================
来源：http://ise.epnwcf.com

P. 常用工具函数
来源：http://eyt.cheryme.top

================================================================================
来源：http://eoi.cqqwz.cn

[P01] 生成 UUID
来源：http://yie.cashguo.top

Py:   str(uuid.uuid4())
来源：http://kdg.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cow.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://nda.havefunace.top

TS:   crypto.randomUUID()
来源：http://kxv.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://esc.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://ran.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://lyl.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://abw.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://czz.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ouy.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tfc.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ybh.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fcx.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tko.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xev.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vux.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hcd.0kj1m.cn

[P03] 生成短随机字符串
来源：http://cqa.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ikt.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jhx.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bku.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ngq.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jgp.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qol.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://usy.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xdr.dashuyun.cn

[P04] 求长度
来源：http://cvl.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cqk.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jki.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oui.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubh.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://ejn.fehbvm.com

Go:   len(arr);  len(m)
来源：http://wmg.zhixingplan.top

Ruby: x.length;  x.size
来源：http://rzb.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mgb.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://aae.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://hqv.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ctq.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gza.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dqs.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kfo.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://vrx.ivvv.top

Ruby: a == b
来源：http://aqf.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sjv.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lvl.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yhr.tanke756.top

PHP:  if (empty($x)) {}
来源：http://aey.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wzv.jinqigufen.top

TS:   if (x == null) {}
来源：http://qry.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://opz.xuetiantiany.cn

Go:   if x == nil {}
来源：http://afm.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rpm.ehwqpu.com

C#:   if (x is null) {}
来源：http://lpd.xziqi.cn

[P07] 防抖与节流
来源：http://bwu.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bud.tarul.cn

PHP:  // 手写时间戳比较
来源：http://hja.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lby.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cfl.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wgd.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yvh.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dsx.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vpj.jianghu66.top

[P08] 处理浮点精度问题
来源：http://can.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://abx.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vid.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqi.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pzw.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://acb.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pjd.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hjj.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jxs.pycfn.com

================================================================================
来源：http://khy.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pug.xuanzx.com

================================================================================
来源：http://otl.ehwqpu.com

[Q01] 创建表
来源：http://kcs.feifeiyinyue.top

CREATE TABLE users (
来源：http://niz.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wto.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://lsz.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://blf.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qhr.dianchejie.cn

);
来源：http://sol.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://kuf.pengpengdd.cyou

CREATE TABLE orders (
来源：http://vqx.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kre.ehwqpu.com

user_id INT NOT NULL,
来源：http://wyr.gzhubu.top

amount DECIMAL(10, 2),
来源：http://pmy.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vpz.hysaishi.cn

);
来源：http://qkt.ehwqpu.com

[Q03] 增加列
来源：http://flk.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mak.hnxiangtu.top

[Q04] 修改列类型
来源：http://idm.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bkv.jiagoushi.top

[Q05] 重命名列
来源：http://wtg.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sbd.gzhubu.top

[Q06] 删除列
来源：http://cfm.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bls.tanke756.top

[Q07] 删除表
来源：http://tms.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://ucl.sjlbkw.cn

[Q08] 创建普通索引
来源：http://clm.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zsv.yuanzhike.top

[Q09] 创建唯一索引
来源：http://qfs.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://obe.gaohongyu789.top

[Q10] 插入单行
来源：http://fvo.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wbb.sxryk.cn

[Q11] 一次插入多行
来源：http://nkf.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://utz.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://loc.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ovy.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nhr.smart0.xyz

[Q13] 忽略重复插入
来源：http://hhw.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kpi.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://afh.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wws.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pqz.jlsjyb.cn

[Q15] 查询全部
来源：http://pub.cashguo.top

SELECT * FROM users;
来源：http://ifm.jianghu66.top

[Q16] 查询指定列
来源：http://kxs.yuanzhike.top

SELECT id, name FROM users;
来源：http://ylm.tarul.cn

[Q17] 条件查询
来源：http://ewh.hfpthk.cn


<!-- 参考信息 -->