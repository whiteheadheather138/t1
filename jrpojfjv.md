代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hwd.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vum.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gtx.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hel.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cda.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://dgs.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://bpm.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yay.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://rig.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://kjd.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://kfn.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aje.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jfb.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xlv.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hbq.sxryk.cn

Go:   slices.Sort(arr)
来源：http://pqx.yongpay.top

Ruby: arr.sort
来源：http://fgu.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vzn.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://qak.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gvx.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://pby.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pea.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nmh.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ies.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rku.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iju.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ath.jinqigfzy.top

[N04] 斐波那契数列
来源：http://vio.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lei.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wqk.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvj.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lgd.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dys.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wdg.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://prd.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wpl.tanke756.top

[N05] 最大公约数
来源：http://sen.tanke756.top

Py:   math.gcd(a, b)
来源：http://jue.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://amd.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmr.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sns.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aek.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kii.yvedp.cn

Ruby: a.gcd(b)
来源：http://cxw.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kyu.yangfankeji.com

[N06] 判断回文字符串
来源：http://ams.cqqwz.cn

Py:   s == s[::-1]
来源：http://lah.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://hhl.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://irh.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://zwr.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xyg.uphjek.com

Go:   // 双指针从两端比较
来源：http://qzy.bjfxy.top

Ruby: s == s.reverse
来源：http://ums.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://vpi.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://kes.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rej.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cvv.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pmv.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://tjd.yangfankeji.com

Java: // 手写 HashMap
来源：http://tkv.yueranfly.top

Go:   // 手写 map[int]int
来源：http://pnw.smart0.xyz

Ruby: // 手写 Hash
来源：http://seg.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://lbk.gzhubu.top

[N08] 生成全排列
来源：http://eem.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://uhg.jianghu66.top

PHP:  // 手写递归交换
来源：http://sqz.sxryk.cn

JS:   // 手写回溯递归
来源：http://ibo.nanxinkj.top

TS:   // 手写回溯递归
来源：http://pcu.xuanzx.com

Java: // 手写回溯递归
来源：http://drw.tianlin.xyz

Go:   // 手写回溯递归
来源：http://olg.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://zqj.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://gew.bjfxy.top

[N09] 栈与队列
来源：http://uga.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://prc.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jxd.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yfg.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fon.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ejy.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wgt.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jse.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hzn.hesvh.cn

[N10] 链表节点定义
来源：http://ocu.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lxr.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://txj.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://anj.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ekb.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://iim.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nbt.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wpi.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ebe.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://nfs.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rpx.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://xla.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qfs.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xjg.zhoulong.xyz

Java: // 手写递归
来源：http://dbt.hammf.cn

Go:   // 手写递归
来源：http://oly.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jlu.bbcook.cn

C#:   // 手写递归
来源：http://qnp.jqgufenzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ceq.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bcp.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ttb.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://udc.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jzc.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wbq.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pda.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aru.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sko.zycfv.cn

================================================================================
来源：http://phc.xuanzx.com

O. 并发与异步
来源：http://tht.yj202588.top

================================================================================
来源：http://shw.yueranfly.top

[O01] 启动一个线程
来源：http://ghf.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://csn.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pxf.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ubv.jinqigufen.top

TS:   // 同 JS
来源：http://cif.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://htq.wangshuangyany.cn

Go:   go f()
来源：http://qsw.cucudq.cn

Ruby: Thread.new { f }
来源：http://btq.ydzc1.top

C#:   Task.Run(() => F());
来源：http://tta.sweek.top

[O02] 使用线程池
来源：http://sty.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eok.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wew.xylfe.cn

JS:   // worker_threads 线程池
来源：http://hgv.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://kht.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://xxf.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dak.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wwn.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sqc.yueranfly.top

[O03] 加锁保护共享数据
来源：http://fxe.hfpthk.cn

Py:   with lock: shared += 1
来源：http://mux.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://mtj.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zxp.dianchejie.cn

TS:   // 同 JS
来源：http://yym.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://sfe.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pre.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iez.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://nuc.yuxming.cn

[O04] 定义异步函数并等待
来源：http://nlb.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://bxe.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wpb.ybcxt.top

JS:   async function f() { await g(); }
来源：http://lsd.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qvx.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://foj.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cut.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uoy.cashguo.top

C#:   async Task F() { await G(); }
来源：http://sjn.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://ajg.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://hhz.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rsm.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://gps.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://edf.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jkf.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://klf.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://hii.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zni.sjlbkw.cn

[O06] 使用进程池
来源：http://ytx.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tyg.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://usq.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://agq.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://alb.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zhx.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://obj.quarkkingdee.top

Ruby: // fork 块
来源：http://wmm.zdqjudy.top

C#:   Parallel.For
来源：http://sga.jiagoushi.top

================================================================================
来源：http://pbc.wangshuangyany.cn

P. 常用工具函数
来源：http://mol.redwolf501.top

================================================================================
来源：http://suj.316326.xyz

[P01] 生成 UUID
来源：http://vcg.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://gyr.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bek.jianghu66.top

JS:   crypto.randomUUID()
来源：http://yiu.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://ciu.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://txw.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://xms.yonumen.top

Ruby: SecureRandom.uuid
来源：http://xlj.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://zov.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://mpg.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rbs.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ahp.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rof.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bdb.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lfn.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bqs.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sdf.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nmu.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://yoa.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bca.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sxb.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yrn.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kdb.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kcs.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hvy.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ald.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hgi.xinyue.icu

[P04] 求长度
来源：http://fxn.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qkj.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cav.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfl.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://grh.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://zjt.yfazqb.com

Go:   len(arr);  len(m)
来源：http://vzd.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://vnh.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gsg.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://hfo.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://qnf.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://daw.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dtm.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pji.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dmz.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://pyy.zdqjudy.top

Ruby: a == b
来源：http://fmj.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qqs.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kkv.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qwt.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://lom.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pxk.yongpay.top

TS:   if (x == null) {}
来源：http://xtr.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pcr.sysykeji.top

Go:   if x == nil {}
来源：http://wuz.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qrv.svipenyu.cn

C#:   if (x is null) {}
来源：http://mov.wangshuangyany.cn

[P07] 防抖与节流
来源：http://yvz.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zuu.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://wnr.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnt.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lku.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mbj.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xun.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vdm.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uhx.smart0.xyz

[P08] 处理浮点精度问题
来源：http://qwb.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://koi.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lyr.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pwv.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dmh.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rhu.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wep.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qox.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xhy.ybcxt.top

================================================================================
来源：http://wip.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iio.tarul.cn

================================================================================
来源：http://tdr.shzxlz.cn

[Q01] 创建表
来源：http://ujk.xziqi.cn

CREATE TABLE users (
来源：http://bth.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zye.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://mvb.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://xiy.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kva.zhixingplan.top

);
来源：http://gco.ybcxt.top

[Q02] 创建带外键的表
来源：http://agn.jianghu66.top

CREATE TABLE orders (
来源：http://bcn.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eqq.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://xiz.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://rcl.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hwj.jinghuilouyu.cn

);
来源：http://kef.zycfv.cn

[Q03] 增加列
来源：http://gtq.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eyt.zdqjudy.top

[Q04] 修改列类型
来源：http://grp.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ooj.guannengcc.top

[Q05] 重命名列
来源：http://mom.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fkq.vehdjk.com

[Q06] 删除列
来源：http://csm.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://edv.jlsjyb.cn

[Q07] 删除表
来源：http://sbf.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://nkt.hnqzz.top

[Q08] 创建普通索引
来源：http://rte.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ozm.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://feo.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yup.nanxinkj.top

[Q10] 插入单行
来源：http://xvx.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fnk.yueranfly.top

[Q11] 一次插入多行
来源：http://qgi.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mdf.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://kdk.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://jbm.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vyv.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://vvq.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dbb.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://vfn.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lyn.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qrw.ctjpmb.com

[Q15] 查询全部
来源：http://vaw.hammf.cn

SELECT * FROM users;
来源：http://vdk.gotoacloud.top

[Q16] 查询指定列
来源：http://mzo.52xcode.cn

SELECT id, name FROM users;
来源：http://ggv.zhijiandao.cn

[Q17] 条件查询
来源：http://snr.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wie.xinyue.icu

[Q18] 模糊匹配
来源：http://izp.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hqf.gogol.net.cn

[Q19] 范围查询
来源：http://nno.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://szb.yj20258888.top

[Q20] IN 列表
来源：http://ujj.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dkh.ivvv.top

[Q21] 空值判断
来源：http://bdm.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bmn.hcnkem.com

[Q22] 排序
来源：http://lqi.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://atv.gotoacloud.top

[Q23] 分页
来源：http://wbj.tanke756.top


<!-- 参考信息 -->