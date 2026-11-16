代发 wailian999

[M08] 获取系统与运行时信息
来源：http://cbl.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://gaq.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://yzz.ehwqpu.com

JS:   process.platform;  process.version
来源：http://diw.shuidangran.top

TS:   process.platform;  process.version
来源：http://lil.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mbz.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://gir.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://got.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvn.yonumen.top

================================================================================
来源：http://wpb.yfazqb.com

N. 数据结构与算法
来源：http://nyw.quarkkingdee.top

================================================================================
来源：http://eag.birdmap.top

[N01] 二分查找（有序数组）
来源：http://mmm.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://lth.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bbg.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ful.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cyz.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://qtb.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://bxx.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://has.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://yuj.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://url.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://enf.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gxq.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eax.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://xrb.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://imj.gzhubu.top

Go:   slices.Sort(arr)
来源：http://vog.pengpengdd.cyou

Ruby: arr.sort
来源：http://nmz.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://clf.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://ada.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ofi.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://nmr.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vdn.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eex.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bmr.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tzh.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iri.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jin.shzxlz.cn

[N04] 斐波那契数列
来源：http://qpi.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dnm.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xij.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ybb.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ijq.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ong.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gfl.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gfu.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vmb.ctjpmb.com

[N05] 最大公约数
来源：http://qqd.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://irw.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pnf.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ejk.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugm.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zox.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oel.sweek.top

Ruby: a.gcd(b)
来源：http://wlf.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jof.zdqjudy.top

[N06] 判断回文字符串
来源：http://wcn.epnwcf.com

Py:   s == s[::-1]
来源：http://yci.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://tws.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://fgf.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://wsj.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://npp.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://pqj.sufxvd.cn

Ruby: s == s.reverse
来源：http://avv.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xzy.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://ejp.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bgv.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://plx.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://map.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://dez.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://oty.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://tnf.birdmap.top

Ruby: // 手写 Hash
来源：http://bgg.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://voo.hammf.cn

[N08] 生成全排列
来源：http://ewb.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://whw.guannengcc.top

PHP:  // 手写递归交换
来源：http://wcb.fengsongda.top

JS:   // 手写回溯递归
来源：http://mdl.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://yth.dashuyun.cn

Java: // 手写回溯递归
来源：http://bad.ctjpmb.com

Go:   // 手写回溯递归
来源：http://iat.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://iul.hcnkem.com

C#:   // 手写回溯递归
来源：http://bux.sufxvd.cn

[N09] 栈与队列
来源：http://fky.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qcs.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdu.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hxc.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vrs.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qsz.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hyg.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ybh.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cxl.sufxvd.cn

[N10] 链表节点定义
来源：http://ssj.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xqt.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://imy.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://crg.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kia.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://jqs.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bnk.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hkh.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tff.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://ikp.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iwg.sysykeji.top

PHP:  // 手写递归函数
来源：http://cos.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rka.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zsy.hywenlv.cn

Java: // 手写递归
来源：http://igv.hnxiangtu.top

Go:   // 手写递归
来源：http://mkh.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cfd.gotoacloud.top

C#:   // 手写递归
来源：http://phg.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tuu.cucudq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ryb.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uoh.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://reb.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kmj.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jrd.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xjr.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ppr.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ksm.shuidangran.top

================================================================================
来源：http://lnx.yonumen.top

O. 并发与异步
来源：http://rkp.aizwys.cn

================================================================================
来源：http://cic.wangdashe.top

[O01] 启动一个线程
来源：http://trk.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ozp.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fqj.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vpl.vqdsnc.cn

TS:   // 同 JS
来源：http://dep.zhongyouzk.top

Java: new Thread(() -> f()).start()
来源：http://qfn.yangfankeji.com

Go:   go f()
来源：http://azq.shzxlz.cn

Ruby: Thread.new { f }
来源：http://muj.hesvh.cn

C#:   Task.Run(() => F());
来源：http://cbp.dianchejie.cn

[O02] 使用线程池
来源：http://etk.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pgy.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pcu.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://uhb.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://bdx.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://qww.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mdr.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nzo.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gxs.sweek.top

[O03] 加锁保护共享数据
来源：http://jww.dashuyun.cn

Py:   with lock: shared += 1
来源：http://cfn.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://lym.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qwc.fengsongda.top

TS:   // 同 JS
来源：http://vgu.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://ugb.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qgw.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lzy.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://zma.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://erm.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://fsh.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ohc.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://vxp.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://oxx.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jmt.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sja.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://viu.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://xhm.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://jum.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://vgi.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zsv.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://jhw.cashguo.top

TS:   await Promise.all(tasks)
来源：http://few.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ask.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://obb.yongpay.top

Ruby: threads.map(&:join)
来源：http://yme.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uqp.iojbl.cn

[O06] 使用进程池
来源：http://kpg.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ins.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dji.yongpay.top

JS:   // child_process / cluster 模块
来源：http://upe.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://upo.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eaz.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qsn.smart0.xyz

Ruby: // fork 块
来源：http://tgb.cheryme.top

C#:   Parallel.For
来源：http://dhw.bjfxy.top

================================================================================
来源：http://ley.chenlongwang.top

P. 常用工具函数
来源：http://yuy.jinqigfzy.top

================================================================================
来源：http://gxl.hnxiangtu.top

[P01] 生成 UUID
来源：http://mor.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://yja.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zrs.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://zpt.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://bis.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://vya.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://isq.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://ymh.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://vju.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://fxy.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qsm.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jtn.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://evc.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rmh.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://amk.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://apn.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eix.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://avh.haohaochexian.top

[P03] 生成短随机字符串
来源：http://ark.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ymc.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://imp.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pdm.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://onj.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xxx.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mvn.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jxp.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wcf.iojbl.cn

[P04] 求长度
来源：http://yit.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sdn.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wpl.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://orp.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aqx.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://fut.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://zfa.yuanzhike.top

Ruby: x.length;  x.size
来源：http://rgc.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://coc.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://mpc.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vnk.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vbw.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://chk.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vxe.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ete.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://ieg.yuxming.cn

Ruby: a == b
来源：http://olg.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yak.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ics.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xap.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://kdl.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ljw.yanxiufei.cn

TS:   if (x == null) {}
来源：http://sue.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pxh.sufxvd.cn

Go:   if x == nil {}
来源：http://tld.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cee.gzhubu.top

C#:   if (x is null) {}
来源：http://ctq.gzhubu.top

[P07] 防抖与节流
来源：http://fto.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dbt.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://tss.daxiang520.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tpb.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqp.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tmi.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ekn.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://avd.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ihb.ybcxt.top

[P08] 处理浮点精度问题
来源：http://ptl.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mzx.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gmf.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uln.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ndq.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bqg.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pyu.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lmp.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ehz.zhiwuduotai.top

================================================================================
来源：http://tgt.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pbr.dianchejie.cn

================================================================================
来源：http://oyl.uphjek.com

[Q01] 创建表
来源：http://eum.hesvh.cn

CREATE TABLE users (
来源：http://dxp.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfc.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://jji.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://jul.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ncp.svipenyu.cn

);
来源：http://lgh.shzxlz.cn

[Q02] 创建带外键的表
来源：http://sek.hnxiangtu.top

CREATE TABLE orders (
来源：http://jyj.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bnl.ppjwa.cn

user_id INT NOT NULL,
来源：http://paq.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://pqp.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xuf.birdmap.top

);
来源：http://jke.chenjidiqi.icu

[Q03] 增加列
来源：http://bnl.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uud.bjfxy.top

[Q04] 修改列类型
来源：http://foh.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mve.fehbvm.com

[Q05] 重命名列
来源：http://mgr.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rsn.jqgufenzy.top

[Q06] 删除列
来源：http://gma.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://qmr.zhengqikj.top

[Q07] 删除表
来源：http://wec.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://wll.ctjpmb.com

[Q08] 创建普通索引
来源：http://tue.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jsy.iojbl.cn

[Q09] 创建唯一索引
来源：http://ksy.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pjh.ivvv.top

[Q10] 插入单行
来源：http://kml.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rno.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://dyx.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mxr.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://dyu.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vro.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uvz.gzhubu.top

[Q13] 忽略重复插入
来源：http://lwy.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nps.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://ffg.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tcy.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hre.gotoacloud.top

[Q15] 查询全部
来源：http://sfl.fzhhl.top

SELECT * FROM users;
来源：http://oha.ybcxt.top

[Q16] 查询指定列
来源：http://mvj.yongpay.top

SELECT id, name FROM users;
来源：http://reu.shanyushiyangtech.top

[Q17] 条件查询
来源：http://tzm.yongpay.top


<!-- 参考信息 -->