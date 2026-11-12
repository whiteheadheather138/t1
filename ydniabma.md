代发 wailian999

[N01] 二分查找（有序数组）
来源：http://ira.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gxg.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sob.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgn.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xue.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://dch.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://cnu.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yhv.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fln.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://jmt.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://glv.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vrx.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hss.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lzh.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xli.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://kua.aibaodan.cn

Ruby: arr.sort
来源：http://zdo.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lxx.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://owg.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fkw.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://pzi.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbf.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqm.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lfr.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://piv.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://afz.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://pho.hnxiangtu.top

[N04] 斐波那契数列
来源：http://iyl.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qto.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pvh.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://geo.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkn.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://npn.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ypa.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owz.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ymo.aibaodan.cn

[N05] 最大公约数
来源：http://fio.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://cav.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aiy.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jmy.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbt.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ace.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://icu.xinyue.icu

Ruby: a.gcd(b)
来源：http://vot.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dkq.fzhhl.top

[N06] 判断回文字符串
来源：http://vyg.xinyue.icu

Py:   s == s[::-1]
来源：http://pfp.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://uyo.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://qjf.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://btu.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gmp.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://cyu.nanxuanxn.top

Ruby: s == s.reverse
来源：http://ixx.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://csu.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://czb.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nen.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ylp.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dev.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://wmu.hnxiangtu.top

Java: // 手写 HashMap
来源：http://frq.c1oappe.top

Go:   // 手写 map[int]int
来源：http://vqn.daxiang520.top

Ruby: // 手写 Hash
来源：http://mjq.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://esz.cashguo.top

[N08] 生成全排列
来源：http://ptg.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://qff.tanke756.top

PHP:  // 手写递归交换
来源：http://syk.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://koh.fehbvm.com

TS:   // 手写回溯递归
来源：http://ugg.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://cwh.sufxvd.cn

Go:   // 手写回溯递归
来源：http://quq.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://exx.fzhhl.top

C#:   // 手写回溯递归
来源：http://mfs.shzxlz.cn

[N09] 栈与队列
来源：http://tkt.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rmy.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xjb.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qfa.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jzt.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xon.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ebo.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bos.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bty.cheryme.top

[N10] 链表节点定义
来源：http://wwn.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://obx.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ehv.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ubh.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bmi.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://tpy.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://nmj.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ual.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://crc.xziqi.cn

[N11] 二叉树中序遍历
来源：http://eqw.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bpq.bbcook.cn

PHP:  // 手写递归函数
来源：http://nkf.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tkv.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kov.dianchejie.cn

Java: // 手写递归
来源：http://aqg.yj202588.top

Go:   // 手写递归
来源：http://aqh.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ltm.c1oappe.top

C#:   // 手写递归
来源：http://gnh.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rzg.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sqh.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ekl.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zbm.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blz.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dbn.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qbd.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ymf.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xxr.zdbjq.cn

================================================================================
来源：http://iaz.yueranfly.top

O. 并发与异步
来源：http://jyt.yuxming.cn

================================================================================
来源：http://dop.yonumen.top

[O01] 启动一个线程
来源：http://axn.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lcm.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wpv.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hve.sweek.top

TS:   // 同 JS
来源：http://kct.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://frn.zdqjudy.top

Go:   go f()
来源：http://okg.tianlin.xyz

Ruby: Thread.new { f }
来源：http://fss.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://uwm.quarkkingdee.top

[O02] 使用线程池
来源：http://qkp.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bth.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bjd.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://pkz.xuanzx.com

TS:   // worker_threads 线程池
来源：http://dcy.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://drb.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gvd.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oaf.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dkg.xziqi.cn

[O03] 加锁保护共享数据
来源：http://xnm.jinqigufen.top

Py:   with lock: shared += 1
来源：http://rhm.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://vso.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oth.zhiwuduotai.top

TS:   // 同 JS
来源：http://tdo.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://bff.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rmj.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uab.zdqjudy.top

C#:   lock (gate) { shared++; }
来源：http://aco.pycfn.com

[O04] 定义异步函数并等待
来源：http://tcz.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://qnl.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://axc.bjfxy.top

JS:   async function f() { await g(); }
来源：http://mur.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ght.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wes.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://azy.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://jjm.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://wwz.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://hfx.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://zfj.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xon.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://wpi.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://rdh.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bim.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hoy.daxiang520.top

Ruby: threads.map(&:join)
来源：http://bax.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nnv.feifeiyinyue.top

[O06] 使用进程池
来源：http://nwy.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sdi.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ilz.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://pvc.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://cwy.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hgw.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zbe.tianlin.xyz

Ruby: // fork 块
来源：http://yev.ydzc1.top

C#:   Parallel.For
来源：http://zbd.ydzc1.top

================================================================================
来源：http://cff.xylfe.cn

P. 常用工具函数
来源：http://rdn.ydzc1.top

================================================================================
来源：http://jau.redwolf501.top

[P01] 生成 UUID
来源：http://abj.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://rlz.quarkkingdee.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ljv.hesvh.cn

JS:   crypto.randomUUID()
来源：http://iwj.smart0.xyz

TS:   crypto.randomUUID()
来源：http://wyh.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://ite.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://xtn.uphjek.com

Ruby: SecureRandom.uuid
来源：http://fdm.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://pbf.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://iwe.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fon.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xhw.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nly.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hzn.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uhi.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fmt.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mnx.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sks.cqqwz.cn

[P03] 生成短随机字符串
来源：http://qjf.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vwi.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vrw.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rnf.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://srk.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://opl.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ypv.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzm.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gcj.dianchejie.cn

[P04] 求长度
来源：http://yxy.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vom.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jkg.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lqi.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lpe.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://thp.nwbrower.top

Go:   len(arr);  len(m)
来源：http://ijl.aibaodan.cn

Ruby: x.length;  x.size
来源：http://bgo.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ahs.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://dzg.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cdi.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zef.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cmu.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ssb.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dvs.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://fqm.aizwys.cn

Ruby: a == b
来源：http://cfw.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rll.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jxm.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ful.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://kte.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ezx.chenlongwang.top

TS:   if (x == null) {}
来源：http://vqe.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lym.hywenlv.cn

Go:   if x == nil {}
来源：http://zpy.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qtp.yuxming.cn

C#:   if (x is null) {}
来源：http://gyh.yfazqb.com

[P07] 防抖与节流
来源：http://yxn.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pdc.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://mbe.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryj.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvr.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://svy.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pgl.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fzt.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uin.epnwcf.com

[P08] 处理浮点精度问题
来源：http://bnf.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tab.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rgc.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wtr.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://phx.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oda.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wyn.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rnj.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://haq.fehbvm.com

================================================================================
来源：http://mmd.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://agh.tanke756.top

================================================================================
来源：http://ldq.hnqzz.top

[Q01] 创建表
来源：http://gxt.daxiang520.top

CREATE TABLE users (
来源：http://ptb.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lam.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://rdo.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://ywr.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nfy.pengpengdd.cyou

);
来源：http://tnm.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://wyk.haohaochexian.top

CREATE TABLE orders (
来源：http://dgz.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zcx.jlsjyb.cn

user_id INT NOT NULL,
来源：http://sdo.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://jis.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mqz.shangyingyoupin.top

);
来源：http://wqd.tianlin.xyz

[Q03] 增加列
来源：http://miy.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ber.316326.xyz

[Q04] 修改列类型
来源：http://xfg.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jjq.jinqigufen.top

[Q05] 重命名列
来源：http://gjj.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vrc.yj20258888.top

[Q06] 删除列
来源：http://yyi.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://wlc.guowangkeji.top

[Q07] 删除表
来源：http://xet.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://mwf.chenlongwang.top

[Q08] 创建普通索引
来源：http://ooa.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://boh.aibaodan.cn

[Q09] 创建唯一索引
来源：http://kak.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iko.jqgfzy.top

[Q10] 插入单行
来源：http://fym.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cii.xinyue.icu

[Q11] 一次插入多行
来源：http://opa.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rok.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://nvq.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ydo.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://drb.nanxinkj.top

[Q13] 忽略重复插入
来源：http://com.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dpm.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://abq.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dey.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jxw.yanxiufei.cn

[Q15] 查询全部
来源：http://ahj.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://iby.yongpay.top

[Q16] 查询指定列
来源：http://ked.gogol.net.cn

SELECT id, name FROM users;
来源：http://omu.zdbjq.cn

[Q17] 条件查询
来源：http://ekk.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rdi.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://nyv.yfazqb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gxf.dianchejie.cn

[Q19] 范围查询
来源：http://rea.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iio.jinghuilouyu.cn

[Q20] IN 列表
来源：http://iky.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rtm.vqdsnc.cn

[Q21] 空值判断
来源：http://wes.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qmr.redwolf501.top

[Q22] 排序
来源：http://bio.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ocz.jinqigfzy.top

[Q23] 分页
来源：http://udg.meibo888.top


<!-- 参考信息 -->