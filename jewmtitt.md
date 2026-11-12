代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ioh.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://xrc.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://ryx.0kj1m.cn

JS:   process.platform;  process.version
来源：http://ink.316326.xyz

TS:   process.platform;  process.version
来源：http://nfz.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xyx.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yqi.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gma.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gea.sxryk.cn

================================================================================
来源：http://tei.chenlongwang.top

N. 数据结构与算法
来源：http://lyx.tian-w.cn

================================================================================
来源：http://qwn.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://zdj.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://mlt.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pgs.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mzu.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gst.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uys.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://wqb.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ulq.gaohongyu789.top

C#:   Array.BinarySearch(arr, x)
来源：http://uyv.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://kxx.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://gvf.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hap.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nuj.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cbi.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cqn.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://ngg.tanke756.top

Ruby: arr.sort
来源：http://ste.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sbv.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://fio.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://etm.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://omo.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ehm.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gop.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uxf.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hig.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ijo.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://mvf.zdqjudy.top

[N04] 斐波那契数列
来源：http://lqa.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wkw.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fyu.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://klc.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ssk.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rli.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dnx.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hnl.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rkb.0kj1m.cn

[N05] 最大公约数
来源：http://puv.xinyue.icu

Py:   math.gcd(a, b)
来源：http://xbe.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jhv.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://chv.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wni.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://csa.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ltb.jqgfzy.top

Ruby: a.gcd(b)
来源：http://qil.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vap.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://gnc.hammf.cn

Py:   s == s[::-1]
来源：http://sly.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://ltd.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://ytn.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://eji.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mtf.xuanzx.com

Go:   // 双指针从两端比较
来源：http://nkb.zhijiandao.cn

Ruby: s == s.reverse
来源：http://aki.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://rgz.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://gkh.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lah.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://slw.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oiw.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://lkk.cashguo.top

Java: // 手写 HashMap
来源：http://xet.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://fga.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://xto.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qhc.vqdsnc.cn

[N08] 生成全排列
来源：http://czq.hammf.cn

Py:   itertools.permutations(arr)
来源：http://nwk.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://wrk.guannengcc.top

JS:   // 手写回溯递归
来源：http://ybm.yuanzhike.top

TS:   // 手写回溯递归
来源：http://kuo.zdbjq.cn

Java: // 手写回溯递归
来源：http://hkx.chenzaomai.com

Go:   // 手写回溯递归
来源：http://lzp.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://fjx.fengsongda.top

C#:   // 手写回溯递归
来源：http://edc.xuetiantiany.cn

[N09] 栈与队列
来源：http://ysj.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rcg.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nbw.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vls.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://omz.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nqy.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wkt.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pnj.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dhk.xuetiantiany.cn

[N10] 链表节点定义
来源：http://qua.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wpq.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eoh.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://usq.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lhz.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://wit.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://vxv.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iqg.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://unc.fktsv.cn

[N11] 二叉树中序遍历
来源：http://xnx.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ptz.hammf.cn

PHP:  // 手写递归函数
来源：http://shx.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fuh.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fgn.yangfankeji.com

Java: // 手写递归
来源：http://xxl.bbcook.cn

Go:   // 手写递归
来源：http://zno.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sdg.yj20258888.top

C#:   // 手写递归
来源：http://xpn.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lxd.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zkl.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qrd.cqqwz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qoa.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gnt.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bja.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cpz.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zzx.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://auv.snrcjt.cn

================================================================================
来源：http://vxa.cheryme.top

O. 并发与异步
来源：http://gqa.xuanzx.com

================================================================================
来源：http://gxe.smart0.xyz

[O01] 启动一个线程
来源：http://wnm.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ymx.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uxu.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mfl.tian-w.cn

TS:   // 同 JS
来源：http://sna.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://pxs.hywenlv.cn

Go:   go f()
来源：http://zsz.cucudq.cn

Ruby: Thread.new { f }
来源：http://bfz.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://hqm.fengsongda.top

[O02] 使用线程池
来源：http://awb.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jdk.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hlr.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://xnn.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://bgp.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://llc.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xcz.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vvf.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dix.ydzc1.top

[O03] 加锁保护共享数据
来源：http://zhs.haohaochexian.top

Py:   with lock: shared += 1
来源：http://rxw.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://uvr.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pkd.hysaishi.cn

TS:   // 同 JS
来源：http://fdp.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://rpg.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mgi.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://elz.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://rwz.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://iiu.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://rmp.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vop.meibo888.top

JS:   async function f() { await g(); }
来源：http://urv.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pot.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://efq.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://whb.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://ioj.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://ter.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://kva.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://nht.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fao.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://lwj.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://zqo.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lrn.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fcu.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://qea.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nhv.tanke756.top

[O06] 使用进程池
来源：http://pph.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oqe.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://inv.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://lif.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://sfv.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cgk.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://flz.bbcook.cn

Ruby: // fork 块
来源：http://iel.jqgufenzy.top

C#:   Parallel.For
来源：http://zqo.ppjwa.cn

================================================================================
来源：http://uak.fehbvm.com

P. 常用工具函数
来源：http://wau.xylfe.cn

================================================================================
来源：http://qyz.chenjidiqi.icu

[P01] 生成 UUID
来源：http://xun.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://fgh.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pvf.yj20258888.top

JS:   crypto.randomUUID()
来源：http://nwb.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://qwx.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://srn.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://syc.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://cjc.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://uqx.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://mvn.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hjm.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://guv.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ozk.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qfd.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qwm.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tzd.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sft.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rtr.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://tkn.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mou.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ggr.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yll.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfj.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfi.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ojp.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ydf.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mjx.quarkkingdee.top

[P04] 求长度
来源：http://ung.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tau.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snn.zhongyouzk.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yji.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qpn.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://fzk.daxiang520.top

Go:   len(arr);  len(m)
来源：http://xht.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://otc.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kev.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://kop.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vkn.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eku.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tle.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mjn.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wni.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://dsd.yangfankeji.com

Ruby: a == b
来源：http://vnc.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xxs.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ehh.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mhd.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://weh.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zum.sweek.top

TS:   if (x == null) {}
来源：http://klv.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xey.shzxlz.cn

Go:   if x == nil {}
来源：http://nqi.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iks.gotoacloud.top

C#:   if (x is null) {}
来源：http://alg.ybcxt.top

[P07] 防抖与节流
来源：http://hcj.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://inn.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://ekh.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ayl.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mll.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gyw.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eld.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hac.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lah.gzhubu.top

[P08] 处理浮点精度问题
来源：http://tox.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://csq.nwbrower.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cmo.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aem.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gvr.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hyk.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gya.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zzu.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lxa.9152youxi.cn

================================================================================
来源：http://fxo.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jyv.hnxiangtu.top

================================================================================
来源：http://vgp.vqdsnc.cn

[Q01] 创建表
来源：http://yhi.shangyingyoupin.top

CREATE TABLE users (
来源：http://yxk.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kaw.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://mlm.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://wex.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kqj.hammf.cn

);
来源：http://baa.xinyue.icu

[Q02] 创建带外键的表
来源：http://jel.tian-w.cn

CREATE TABLE orders (
来源：http://bxu.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pok.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://ndd.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://xkr.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hgj.cheryme.top

);
来源：http://fsp.svipenyu.cn

[Q03] 增加列
来源：http://apw.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://okk.shzxlz.cn

[Q04] 修改列类型
来源：http://ybc.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tzx.shzxlz.cn

[Q05] 重命名列
来源：http://knh.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://afj.ehwqpu.com

[Q06] 删除列
来源：http://vsg.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://ngz.xuanzx.com

[Q07] 删除表
来源：http://lcs.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://oeh.jinqigfzy.top

[Q08] 创建普通索引
来源：http://uup.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://syx.ydzc1.top

[Q09] 创建唯一索引
来源：http://xgc.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gtg.pycfn.com

[Q10] 插入单行
来源：http://oxj.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eau.dianchejie.cn

[Q11] 一次插入多行
来源：http://myx.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tnr.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://fdo.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bcg.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qtd.ctjpmb.com

[Q13] 忽略重复插入
来源：http://svt.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bbd.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://ozv.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ycq.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://apq.daxiang520.top

[Q15] 查询全部
来源：http://nqz.chenlongwang.top

SELECT * FROM users;
来源：http://uro.zhijiandao.cn

[Q16] 查询指定列
来源：http://ssw.chenlongwang.top

SELECT id, name FROM users;
来源：http://sbu.gzhubu.top

[Q17] 条件查询
来源：http://yez.cashguo.top


<!-- 参考信息 -->