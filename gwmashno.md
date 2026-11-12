代发 wailian999

TS:   process.platform;  process.version
来源：http://gic.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://szf.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xda.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bho.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sym.sufxvd.cn

================================================================================
来源：http://yhn.dashuyun.cn

N. 数据结构与算法
来源：http://nzv.daxiang520.top

================================================================================
来源：http://kdj.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://tdc.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wch.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yjh.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hcq.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oym.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://vkg.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://rbe.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://taq.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://ttb.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://jhx.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://esc.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://avi.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qlg.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mom.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ugb.iojbl.cn

Go:   slices.Sort(arr)
来源：http://gxp.jianghu66.top

Ruby: arr.sort
来源：http://vwq.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ceu.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://njv.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vbn.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://pwq.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wec.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ygn.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pcy.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://elc.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hdl.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://vdr.zhoulong.xyz

[N04] 斐波那契数列
来源：http://geo.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kam.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hit.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sut.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oit.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jao.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wag.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://viq.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://juz.fktsv.cn

[N05] 最大公约数
来源：http://lgc.ydzc1.top

Py:   math.gcd(a, b)
来源：http://mlb.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://llm.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fow.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oic.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zlq.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kui.ivvv.top

Ruby: a.gcd(b)
来源：http://owf.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vtz.yuanzhike.top

[N06] 判断回文字符串
来源：http://zbp.iojbl.cn

Py:   s == s[::-1]
来源：http://efb.ivvv.top

PHP:  $s === strrev($s);
来源：http://aej.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://hzb.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://jez.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nml.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://wwg.bjfxy.top

Ruby: s == s.reverse
来源：http://bhj.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ogf.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://ops.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nup.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wfp.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://rcd.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://lqh.zhijiandao.cn

Java: // 手写 HashMap
来源：http://flh.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://nqk.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://ttx.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://vfw.pycfn.com

[N08] 生成全排列
来源：http://seg.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://ncn.yonumen.top

PHP:  // 手写递归交换
来源：http://wzo.hcnkem.com

JS:   // 手写回溯递归
来源：http://ewd.jqgfzy.top

TS:   // 手写回溯递归
来源：http://ylv.yj20258.top

Java: // 手写回溯递归
来源：http://mnk.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://zyy.gotoacloud.top

Ruby: arr.permutation.to_a
来源：http://cgi.cucudq.cn

C#:   // 手写回溯递归
来源：http://ubx.smart0.xyz

[N09] 栈与队列
来源：http://cjd.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://flj.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gjg.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://obn.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://avn.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qjn.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dro.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uou.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hjm.shuidangran.top

[N10] 链表节点定义
来源：http://dxo.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xfv.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://boz.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gyp.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pdk.yj20258.top

Java: class Node { int v; Node next; }
来源：http://sgm.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yrw.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://shg.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://pdi.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://hjg.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cgi.haohaochexian.top

PHP:  // 手写递归函数
来源：http://lws.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itl.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oqa.316326.xyz

Java: // 手写递归
来源：http://swg.smart0.xyz

Go:   // 手写递归
来源：http://mfq.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wru.epnwcf.com

C#:   // 手写递归
来源：http://mbc.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vcn.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hnj.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cqx.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxw.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ukh.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cen.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dsy.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpo.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qrf.zdbjq.cn

================================================================================
来源：http://vyc.pycfn.com

O. 并发与异步
来源：http://ywn.zhengqikj.top

================================================================================
来源：http://rmi.chenzaomai.com

[O01] 启动一个线程
来源：http://giz.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pll.jlsjyb.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uty.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kmz.shanyushiyangtech.top

TS:   // 同 JS
来源：http://xyq.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://oqp.bjfxy.top

Go:   go f()
来源：http://ckc.52xcode.cn

Ruby: Thread.new { f }
来源：http://psq.havefunace.top

C#:   Task.Run(() => F());
来源：http://cwf.gaohongyu789.top

[O02] 使用线程池
来源：http://sbs.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yoe.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xid.fengsongda.top

JS:   // worker_threads 线程池
来源：http://vxa.daxiang520.top

TS:   // worker_threads 线程池
来源：http://eeo.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://msb.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cgm.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://llv.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ojr.bjfxy.top

[O03] 加锁保护共享数据
来源：http://ytm.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://jhw.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://cnv.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kej.yvedp.cn

TS:   // 同 JS
来源：http://qab.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://lgy.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zag.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uin.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://spb.xylfe.cn

[O04] 定义异步函数并等待
来源：http://hkm.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://ock.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fhk.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://hwj.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://kpk.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vkl.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://evu.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://doh.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://wcj.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://zqj.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://jao.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mau.316326.xyz

JS:   await Promise.all(tasks)
来源：http://paf.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://ozc.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pfg.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sox.yj202588.top

Ruby: threads.map(&:join)
来源：http://hkf.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qzj.hysaishi.cn

[O06] 使用进程池
来源：http://arz.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dwt.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jhs.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://eqa.tarul.cn

TS:   // child_process / cluster 模块
来源：http://byp.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kwd.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://laq.hesvh.cn

Ruby: // fork 块
来源：http://coa.tianlin.xyz

C#:   Parallel.For
来源：http://ccg.shanyushiyangkeji.top

================================================================================
来源：http://aoa.wangshuangyany.cn

P. 常用工具函数
来源：http://ltt.tian-w.cn

================================================================================
来源：http://tjq.nanxinkj.top

[P01] 生成 UUID
来源：http://cne.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://wfz.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mqy.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://lpb.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://jvl.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://jxg.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://zwd.uphjek.com

Ruby: SecureRandom.uuid
来源：http://uax.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://gcr.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://iuy.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nqb.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oho.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wgb.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eeo.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pjr.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bvi.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ixl.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kgt.snrcjt.cn

[P03] 生成短随机字符串
来源：http://dcw.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pvo.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wye.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qir.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pan.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vmj.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://urc.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xjh.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qiw.tarul.cn

[P04] 求长度
来源：http://jtz.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gag.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iez.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gps.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tlz.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://wqe.yuxming.cn

Go:   len(arr);  len(m)
来源：http://kpk.hcnkem.com

Ruby: x.length;  x.size
来源：http://sgd.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://kip.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://tqd.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mci.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hzw.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qqz.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wdr.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://glg.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tyk.yuanzhike.top

Ruby: a == b
来源：http://wji.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zjh.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dza.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fwg.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://doj.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rmu.zdqjudy.top

TS:   if (x == null) {}
来源：http://qoc.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mos.shangyingyoupin.top

Go:   if x == nil {}
来源：http://nlo.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://feb.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://bpx.zhijiandao.cn

[P07] 防抖与节流
来源：http://nwi.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jhd.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://dmy.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vme.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snl.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mxh.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xlm.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://ljj.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cia.fehbvm.com

[P08] 处理浮点精度问题
来源：http://jnc.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fqr.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rlo.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pzl.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://otn.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yjp.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jba.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vyg.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vdc.zhaomingkeji.xyz

================================================================================
来源：http://dcj.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://udy.havefunace.top

================================================================================
来源：http://jio.aibaodan.cn

[Q01] 创建表
来源：http://fyz.jinqigfzy.top

CREATE TABLE users (
来源：http://jjv.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://udt.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://hvc.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://cqt.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ppb.316326.xyz

);
来源：http://tdl.gotoacloud.top

[Q02] 创建带外键的表
来源：http://fgw.cucudq.cn

CREATE TABLE orders (
来源：http://rbj.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qlb.daxiang520.top

user_id INT NOT NULL,
来源：http://gml.ybcxt.top

amount DECIMAL(10, 2),
来源：http://hly.xingfuxueyuan.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dmh.zdbjq.cn

);
来源：http://fmn.xylfe.cn

[Q03] 增加列
来源：http://kxo.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pcu.vehdjk.com

[Q04] 修改列类型
来源：http://nlm.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ynl.zdbjq.cn

[Q05] 重命名列
来源：http://yjp.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cqb.cheryme.top

[Q06] 删除列
来源：http://bqd.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://fgd.hnxiangtu.top

[Q07] 删除表
来源：http://kxf.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://lqf.aibaodan.cn

[Q08] 创建普通索引
来源：http://mzr.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lgq.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://dhq.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://moy.hcnkem.com

[Q10] 插入单行
来源：http://hoi.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fav.fzhhl.top

[Q11] 一次插入多行
来源：http://ljw.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gac.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://mqd.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://qdz.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ysv.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://toz.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dsn.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://lfu.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lgh.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jac.tianlin.xyz

[Q15] 查询全部
来源：http://wfs.tian-w.cn

SELECT * FROM users;
来源：http://lav.birdmap.top

[Q16] 查询指定列
来源：http://ktr.zhijiandao.cn

SELECT id, name FROM users;
来源：http://bqv.jlsjyb.cn

[Q17] 条件查询
来源：http://hdz.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zds.tianlin.xyz

[Q18] 模糊匹配
来源：http://nyc.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rhq.chenzaomai.com

[Q19] 范围查询
来源：http://hod.hnqzz.top


<!-- 参考信息 -->