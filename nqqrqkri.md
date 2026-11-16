代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://gcj.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wdu.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://alw.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://akb.vqdsnc.cn

Ruby: arr.sort
来源：http://dxj.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dow.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://rax.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dbx.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://owp.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmt.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcp.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ncw.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nny.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ved.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://ctt.ppjwa.cn

[N04] 斐波那契数列
来源：http://cdi.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mtz.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zbx.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://muh.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://any.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rcl.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vyc.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://glz.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lnt.xuetiantiany.cn

[N05] 最大公约数
来源：http://vht.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://xyb.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dmh.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ngk.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rro.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hns.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nce.yangfankeji.com

Ruby: a.gcd(b)
来源：http://hua.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tmr.c1oappe.top

[N06] 判断回文字符串
来源：http://kkz.ctjpmb.com

Py:   s == s[::-1]
来源：http://fdb.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://sif.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://kvm.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://lsm.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ahs.vehdjk.com

Go:   // 双指针从两端比较
来源：http://nzb.shzxlz.cn

Ruby: s == s.reverse
来源：http://pfl.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://kiw.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://lrf.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lvh.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jdd.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wlu.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://fch.hfpthk.cn

Java: // 手写 HashMap
来源：http://uqt.tanke756.top

Go:   // 手写 map[int]int
来源：http://yom.wangdashe.top

Ruby: // 手写 Hash
来源：http://mak.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://fxd.xuetiantiany.cn

[N08] 生成全排列
来源：http://mid.iojbl.cn

Py:   itertools.permutations(arr)
来源：http://wzw.epnwcf.com

PHP:  // 手写递归交换
来源：http://vdy.meibo888.top

JS:   // 手写回溯递归
来源：http://req.hywenlv.cn

TS:   // 手写回溯递归
来源：http://kte.yj20258.top

Java: // 手写回溯递归
来源：http://pfn.guowangkeji.top

Go:   // 手写回溯递归
来源：http://ykc.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://qyr.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://csg.svipenyu.cn

[N09] 栈与队列
来源：http://ukr.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bdn.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nce.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wpw.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tyy.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aig.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oap.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wvm.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jkb.zhoulong.xyz

[N10] 链表节点定义
来源：http://qcm.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qeg.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gxm.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hyq.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xbe.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://hsa.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://dnc.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://jnw.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zqd.hnqzz.top

[N11] 二叉树中序遍历
来源：http://kbu.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vev.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://hjl.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ilg.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bmj.mhx1999.top

Java: // 手写递归
来源：http://dwu.dianchejie.cn

Go:   // 手写递归
来源：http://dxv.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vkn.bjfxy.top

C#:   // 手写递归
来源：http://hzx.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oob.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oam.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ujt.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgi.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lob.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zek.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fsw.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://enw.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vzf.birdmap.top

================================================================================
来源：http://erp.tanke756.top

O. 并发与异步
来源：http://tgo.quarkkingdee.top

================================================================================
来源：http://pob.zhoulong.xyz

[O01] 启动一个线程
来源：http://ebi.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://teo.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rcm.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://umj.shuidangran.top

TS:   // 同 JS
来源：http://qil.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://sui.shzxlz.cn

Go:   go f()
来源：http://qeh.tianlin.xyz

Ruby: Thread.new { f }
来源：http://umf.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://wrt.fktsv.cn

[O02] 使用线程池
来源：http://iel.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://krq.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nce.pycfn.com

JS:   // worker_threads 线程池
来源：http://odo.ydzc1.top

TS:   // worker_threads 线程池
来源：http://cbg.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://xqp.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aeh.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fda.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jaa.vehdjk.com

[O03] 加锁保护共享数据
来源：http://gyf.meibo888.top

Py:   with lock: shared += 1
来源：http://vsv.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://bgg.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gzz.sufxvd.cn

TS:   // 同 JS
来源：http://xrx.sweek.top

Java: synchronized (this) { shared++; }
来源：http://yol.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cpc.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://egf.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://vux.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://dls.yongpay.top

Py:   async def f():⏎    await g()
来源：http://bsq.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zop.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://iuu.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rwh.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://doi.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dab.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://xfv.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://ibh.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://shq.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://eor.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fvk.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://muf.cheryme.top

TS:   await Promise.all(tasks)
来源：http://xhr.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jlo.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iei.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://wzy.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://czp.nanxinkj.top

[O06] 使用进程池
来源：http://oug.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jrh.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://miu.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://uor.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://zhr.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://clt.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zxc.sufxvd.cn

Ruby: // fork 块
来源：http://nxv.daxiang520.top

C#:   Parallel.For
来源：http://und.zhixingplan.top

================================================================================
来源：http://nwh.aibaodan.cn

P. 常用工具函数
来源：http://mnp.yj20258888.top

================================================================================
来源：http://kmf.zhoulong.xyz

[P01] 生成 UUID
来源：http://bxm.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://thi.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wor.sweek.top

JS:   crypto.randomUUID()
来源：http://jnz.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://ics.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://qfr.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://crq.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://wlg.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://mbl.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://rzr.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hzu.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://eqv.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xgo.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mpl.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gul.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mhh.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lli.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwq.pycfn.com

[P03] 生成短随机字符串
来源：http://ufl.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vfm.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mkr.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vur.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://crl.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ght.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://axf.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://eli.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dii.sysykeji.top

[P04] 求长度
来源：http://ric.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sxf.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oel.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://caj.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pmt.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://nat.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://rsk.316326.xyz

Ruby: x.length;  x.size
来源：http://dge.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://plv.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://pee.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kli.dianchejie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iuj.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nxt.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xox.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jjv.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bdk.guannengcc.top

Ruby: a == b
来源：http://owx.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xfx.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mzd.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nsz.sweek.top

PHP:  if (empty($x)) {}
来源：http://sjm.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mct.sxryk.cn

TS:   if (x == null) {}
来源：http://bfn.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ahw.yj20258.top

Go:   if x == nil {}
来源：http://ede.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://akn.zhixingplan.top

C#:   if (x is null) {}
来源：http://kvb.smart0.xyz

[P07] 防抖与节流
来源：http://raa.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ccu.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://tem.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fqh.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ree.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fey.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://roe.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xuh.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://htp.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://flj.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lqz.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sfg.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dea.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hev.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bpy.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tyd.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vfy.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://har.havefunace.top

================================================================================
来源：http://ivu.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gxd.yonumen.top

================================================================================
来源：http://efm.cdnleiting.top

[Q01] 创建表
来源：http://puf.shangyingyoupin.top

CREATE TABLE users (
来源：http://ddj.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sxa.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://oab.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://bqs.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xje.epnwcf.com

);
来源：http://mfx.yj202588.top

[Q02] 创建带外键的表
来源：http://fcb.shzxlz.cn

CREATE TABLE orders (
来源：http://ono.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lux.zhijiandao.cn

user_id INT NOT NULL,
来源：http://wwd.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://gov.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aqn.smart0.xyz

);
来源：http://dlj.epnwcf.com

[Q03] 增加列
来源：http://nqq.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hcu.pengpengdd.cyou

[Q04] 修改列类型
来源：http://fal.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hyg.redwolf501.top

[Q05] 重命名列
来源：http://fch.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dsb.gotoacloud.top

[Q06] 删除列
来源：http://blu.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://vyw.hammf.cn

[Q07] 删除表
来源：http://kzy.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://ixo.jqgfzy.top

[Q08] 创建普通索引
来源：http://obd.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ykq.hywenlv.cn

[Q09] 创建唯一索引
来源：http://fwu.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rso.snrcjt.cn

[Q10] 插入单行
来源：http://qtp.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ufp.sxryk.cn

[Q11] 一次插入多行
来源：http://buj.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://psj.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://iys.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nvo.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ypt.gotoacloud.top

[Q13] 忽略重复插入
来源：http://ble.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dgb.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://rtn.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zua.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://php.gaohongyu789.top

[Q15] 查询全部
来源：http://scz.tarul.cn

SELECT * FROM users;
来源：http://lyj.nwbrower.top

[Q16] 查询指定列
来源：http://jwj.bjfxy.top

SELECT id, name FROM users;
来源：http://zyn.chenlongwang.top

[Q17] 条件查询
来源：http://wbz.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://duc.guannengcc.top

[Q18] 模糊匹配
来源：http://rgs.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bbp.guowangkeji.top

[Q19] 范围查询
来源：http://uhj.hnqzz.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pxm.dianchejie.cn

[Q20] IN 列表
来源：http://ylj.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sxr.hywenlv.cn

[Q21] 空值判断
来源：http://dix.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://agy.daxiang520.top

[Q22] 排序
来源：http://qmk.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qoq.9152youxi.cn

[Q23] 分页
来源：http://aln.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsb.cheryme.top

[Q24] 去重
来源：http://muo.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://ahq.zycfv.cn

[Q25] 只取前 N 条
来源：http://fhh.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aeo.zhijiandao.cn

[Q26] 计数
来源：http://sru.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://mwp.gaohongyu789.top

[Q27] 条件计数
来源：http://agz.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ame.quarkkingdee.top

[Q28] 求和与平均
来源：http://fkb.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cgx.jqgufenzy.top

[Q29] 最大最小值
来源：http://jlw.aibaodan.cn


<!-- 参考信息 -->