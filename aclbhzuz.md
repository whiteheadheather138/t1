代发 wailian999

TS:   process.platform;  process.version
来源：http://pch.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lvr.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://efr.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://als.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kaq.dashuyun.cn

================================================================================
来源：http://yon.bbcook.cn

N. 数据结构与算法
来源：http://ude.sjlbkw.cn

================================================================================
来源：http://jjn.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://qnq.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://kfb.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jtz.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dja.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbx.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://csw.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://cam.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mkc.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kde.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://ftt.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://sde.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nqi.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://edd.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://spw.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ckh.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://hdk.fanxiaobao.xyz

Ruby: arr.sort
来源：http://npr.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rlj.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://mrr.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tmi.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://pgm.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qve.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wum.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pjh.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dxp.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wlz.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ihc.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://zew.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nmd.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qvr.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ljq.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djz.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uin.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://msk.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://idf.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://chr.svipenyu.cn

[N05] 最大公约数
来源：http://xgy.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://wev.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mhk.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzy.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cyb.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bqb.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ngx.9152youxi.cn

Ruby: a.gcd(b)
来源：http://gue.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pot.xylfe.cn

[N06] 判断回文字符串
来源：http://nzc.bjfxy.top

Py:   s == s[::-1]
来源：http://msj.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://vsq.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://eiw.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://znx.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://asf.zycfv.cn

Go:   // 双指针从两端比较
来源：http://kpu.dianchejie.cn

Ruby: s == s.reverse
来源：http://xut.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nbx.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://mon.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wvr.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qlf.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bqt.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://unc.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://wpe.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://nby.gotoacloud.top

Ruby: // 手写 Hash
来源：http://prq.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tmi.chenlongwang.top

[N08] 生成全排列
来源：http://sct.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://ior.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://iyu.hesvh.cn

JS:   // 手写回溯递归
来源：http://ktx.dashuyun.cn

TS:   // 手写回溯递归
来源：http://udi.yangfankeji.com

Java: // 手写回溯递归
来源：http://amc.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://zbu.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://erm.tianlin.xyz

C#:   // 手写回溯递归
来源：http://qrv.zhoulong.xyz

[N09] 栈与队列
来源：http://emv.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uwm.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wsk.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oea.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uwr.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ejd.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hcw.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uuf.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xhn.9152youxi.cn

[N10] 链表节点定义
来源：http://woi.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hlh.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bmd.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zav.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xyv.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://ysj.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://knx.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://psg.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mum.jianghu66.top

[N11] 二叉树中序遍历
来源：http://lmq.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bok.epnwcf.com

PHP:  // 手写递归函数
来源：http://yzs.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udf.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqf.xinyue.icu

Java: // 手写递归
来源：http://wih.zhongyouzk.top

Go:   // 手写递归
来源：http://vnm.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://osc.sxryk.cn

C#:   // 手写递归
来源：http://zhh.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jhs.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wcv.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fql.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://znv.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knq.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://icr.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vuk.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mrg.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hjw.snrcjt.cn

================================================================================
来源：http://mws.xuetiantiany.cn

O. 并发与异步
来源：http://osf.cdnleiting.top

================================================================================
来源：http://ham.feifeiyinyue.top

[O01] 启动一个线程
来源：http://cgn.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jbw.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kac.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ffl.316326.xyz

TS:   // 同 JS
来源：http://dsd.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://rwz.hnqzz.top

Go:   go f()
来源：http://hne.jqgfzy.top

Ruby: Thread.new { f }
来源：http://qwj.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://htv.shuidangran.top

[O02] 使用线程池
来源：http://vrt.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dns.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lfr.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://kfs.aizwys.cn

TS:   // worker_threads 线程池
来源：http://gmt.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://isj.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nkx.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://woj.yfazqb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rjl.andypj.xyz

[O03] 加锁保护共享数据
来源：http://tob.jqgfzy.top

Py:   with lock: shared += 1
来源：http://vus.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://cso.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ksg.hfpthk.cn

TS:   // 同 JS
来源：http://nom.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://cqs.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rzn.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lhi.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://rlf.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://hkm.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://dav.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sbg.xziqi.cn

JS:   async function f() { await g(); }
来源：http://tnh.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bwx.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qvz.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rci.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://len.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://cdu.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://pwk.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://hbw.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xxc.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://pft.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://xhc.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zyv.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vsn.daria6918.cn

Ruby: threads.map(&:join)
来源：http://xol.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xxd.zhixingplan.top

[O06] 使用进程池
来源：http://mmn.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mag.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vmx.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://ikc.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://nzr.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rgg.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lzy.hysaishi.cn

Ruby: // fork 块
来源：http://exq.ydjk.org.cn

C#:   Parallel.For
来源：http://mdn.jqgfzy.top

================================================================================
来源：http://vvz.shangyingyoupin.top

P. 常用工具函数
来源：http://kzh.daxiang520.top

================================================================================
来源：http://ehy.jqgfzy.top

[P01] 生成 UUID
来源：http://eub.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://qou.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oym.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://ebu.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://ist.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://mtl.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://jzd.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://erj.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://hbr.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://jju.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eeq.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ccl.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mvh.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eru.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hqb.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pnv.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vox.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ycy.sxryk.cn

[P03] 生成短随机字符串
来源：http://xfa.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fxm.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rrk.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://caf.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vcl.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fta.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gew.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://voq.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ajx.yj20258.top

[P04] 求长度
来源：http://ehs.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rob.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lsa.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://thj.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pau.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://dyy.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://xjb.zhengqikj.top

Ruby: x.length;  x.size
来源：http://ezv.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gnc.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://xrt.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gzd.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bjn.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tbr.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ggy.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mwc.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://tho.yongpay.top

Ruby: a == b
来源：http://afo.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dbl.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bxs.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://khq.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://jzs.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpl.havefunace.top

TS:   if (x == null) {}
来源：http://wmw.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://rma.tanke756.top

Go:   if x == nil {}
来源：http://kut.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bih.zhengqikj.top

C#:   if (x is null) {}
来源：http://nsy.jlsjyb.cn

[P07] 防抖与节流
来源：http://nht.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ipo.tarul.cn

PHP:  // 手写时间戳比较
来源：http://qgx.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvd.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpj.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vew.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gjj.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kqa.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gdm.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://rcp.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dbs.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jhn.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://evw.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ipi.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wjk.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zqv.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mlj.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://prb.gogol.net.cn

================================================================================
来源：http://iwk.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hwr.haohaochexian.top

================================================================================
来源：http://pew.hnqzz.top

[Q01] 创建表
来源：http://ghq.yvedp.cn

CREATE TABLE users (
来源：http://sgx.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yrp.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://nzy.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://xwk.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rvw.jqgufenzy.top

);
来源：http://tit.tanke756.top

[Q02] 创建带外键的表
来源：http://xef.yangfankeji.com

CREATE TABLE orders (
来源：http://aie.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqq.hcnkem.com

user_id INT NOT NULL,
来源：http://ffa.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://uly.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ewo.hammf.cn

);
来源：http://jyh.jqgfzy.top

[Q03] 增加列
来源：http://yul.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uwk.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://elw.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ati.zhongyouzk.top

[Q05] 重命名列
来源：http://zpj.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mif.dianchejie.cn

[Q06] 删除列
来源：http://wdb.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://sps.316326.xyz

[Q07] 删除表
来源：http://eun.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://xyn.sweek.top

[Q08] 创建普通索引
来源：http://nxr.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yxk.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://xrw.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://anh.hfpthk.cn

[Q10] 插入单行
来源：http://jum.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwc.tianlin.xyz

[Q11] 一次插入多行
来源：http://olg.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eld.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://ckf.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kte.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sdb.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://ybw.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mjj.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://kvu.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xhz.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ffo.vehdjk.com

[Q15] 查询全部
来源：http://dhg.hesvh.cn

SELECT * FROM users;
来源：http://prt.c1oappe.top

[Q16] 查询指定列
来源：http://swn.zhengqikj.top

SELECT id, name FROM users;
来源：http://epg.feifeiyinyue.top

[Q17] 条件查询
来源：http://qbi.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rog.sxryk.cn

[Q18] 模糊匹配
来源：http://vtj.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://the.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://jgd.fengsongda.top


<!-- 参考信息 -->