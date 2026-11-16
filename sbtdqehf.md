代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://swk.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://ijk.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://zzh.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dkt.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ahq.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yzk.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ajh.yj202588.top

Go:   slices.Sort(arr)
来源：http://ebq.ydjk.org.cn

Ruby: arr.sort
来源：http://rvk.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://urq.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://hms.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kqu.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://tpe.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://icm.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://peu.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rkt.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fuy.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dgo.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lue.c1oappe.top

[N04] 斐波那契数列
来源：http://rgr.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ned.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hth.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sam.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uys.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zrt.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uwa.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wyc.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://icb.pycfn.com

[N05] 最大公约数
来源：http://uqp.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://zue.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oib.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uhv.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yng.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kqw.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ghf.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://myv.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wzf.jinqigufen.top

[N06] 判断回文字符串
来源：http://osj.yanxiufei.cn

Py:   s == s[::-1]
来源：http://itk.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://guf.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://kwv.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://udr.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ddu.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://tts.tarul.cn

Ruby: s == s.reverse
来源：http://bdz.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qva.316326.xyz

[N07] 两数之和（返回下标）
来源：http://wuz.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rlg.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://njj.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mma.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://yvo.zhoulong.xyz

Java: // 手写 HashMap
来源：http://qps.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://yro.zdbjq.cn

Ruby: // 手写 Hash
来源：http://qca.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xti.yuanzhike.top

[N08] 生成全排列
来源：http://wra.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://cyh.nanxinkj.top

PHP:  // 手写递归交换
来源：http://fhd.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://rud.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://qkz.haohaochexian.top

Java: // 手写回溯递归
来源：http://gat.cheryme.top

Go:   // 手写回溯递归
来源：http://kdu.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://dmg.haohaochexian.top

C#:   // 手写回溯递归
来源：http://gsf.nanxuanxn.top

[N09] 栈与队列
来源：http://vac.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dzw.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ewn.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ppp.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://teu.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jwv.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kwy.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://epr.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvl.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://ofd.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kgd.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://afe.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ysj.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qdj.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://nxy.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://fgd.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vff.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lqb.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://pbr.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sqf.zdbjq.cn

PHP:  // 手写递归函数
来源：http://ltn.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iuz.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://glb.ivvv.top

Java: // 手写递归
来源：http://ydj.vehdjk.com

Go:   // 手写递归
来源：http://ehn.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jdr.cashguo.top

C#:   // 手写递归
来源：http://lsy.ivvv.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ftd.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aua.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yyi.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ype.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozb.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dpx.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oyl.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ffw.jlsjyb.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bul.shangyingyoupin.top

================================================================================
来源：http://ghi.zycfv.cn

O. 并发与异步
来源：http://cwt.ppjwa.cn

================================================================================
来源：http://ehd.jqgfzy.top

[O01] 启动一个线程
来源：http://aep.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ycd.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aof.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qsh.pengpengdd.cyou

TS:   // 同 JS
来源：http://ouk.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://hwv.hnxiangtu.top

Go:   go f()
来源：http://ptj.fengsongda.top

Ruby: Thread.new { f }
来源：http://igm.havefunace.top

C#:   Task.Run(() => F());
来源：http://upv.yongpay.top

[O02] 使用线程池
来源：http://zat.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hox.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uxv.ivvv.top

JS:   // worker_threads 线程池
来源：http://dzl.yuxming.cn

TS:   // worker_threads 线程池
来源：http://aok.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://bli.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ygc.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://arz.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gkv.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://fsk.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://hzd.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://npu.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ook.xuetiantiany.cn

TS:   // 同 JS
来源：http://rim.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://klw.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jsc.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://uik.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://emz.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://sly.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://bzj.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gsv.ybcxt.top

JS:   async function f() { await g(); }
来源：http://uit.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://kev.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mjj.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fes.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://cit.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://msi.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://obk.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://ykk.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://phq.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://lrq.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://dil.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpx.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vax.vehdjk.com

Ruby: threads.map(&:join)
来源：http://bea.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cqy.ybcxt.top

[O06] 使用进程池
来源：http://umm.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nrr.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mwf.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://pmr.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://ety.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eod.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dcs.xuanzx.com

Ruby: // fork 块
来源：http://pcw.svipenyu.cn

C#:   Parallel.For
来源：http://kap.jqgufenzy.top

================================================================================
来源：http://ogg.feifeiyinyue.top

P. 常用工具函数
来源：http://rec.nanxinkj.top

================================================================================
来源：http://hym.xinyue.icu

[P01] 生成 UUID
来源：http://zzx.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://yya.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pjd.iojbl.cn

JS:   crypto.randomUUID()
来源：http://zon.cashguo.top

TS:   crypto.randomUUID()
来源：http://jcd.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://gfb.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://vbg.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://her.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://tyr.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://two.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hen.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mui.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ltz.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mho.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://duy.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bko.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pwm.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zob.cheryme.top

[P03] 生成短随机字符串
来源：http://dud.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yzf.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wji.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mzg.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dgr.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ihw.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aes.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nsa.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://exv.gzhubu.top

[P04] 求长度
来源：http://uhd.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ydi.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzu.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxp.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ene.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://jut.smart0.xyz

Go:   len(arr);  len(m)
来源：http://fwj.sysykeji.top

Ruby: x.length;  x.size
来源：http://pst.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vja.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://rho.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tal.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kol.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hfp.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xwb.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://unl.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xur.pycfn.com

Ruby: a == b
来源：http://jjl.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ink.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tzw.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rfd.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://pgf.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jvr.zdbjq.cn

TS:   if (x == null) {}
来源：http://woh.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://izc.wangshuangyany.cn

Go:   if x == nil {}
来源：http://xjr.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ynv.vqdsnc.cn

C#:   if (x is null) {}
来源：http://qna.hcnkem.com

[P07] 防抖与节流
来源：http://asp.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jwf.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://mwp.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pol.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptg.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gug.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://anq.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://btc.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://swp.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://bhm.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vac.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lsh.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://otd.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hfl.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ufg.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://quj.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gwf.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://orb.xingfuxueyuan.xyz

================================================================================
来源：http://ovj.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hzs.svipenyu.cn

================================================================================
来源：http://ptb.yangfankeji.com

[Q01] 创建表
来源：http://iay.yuanzhike.top

CREATE TABLE users (
来源：http://xzb.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqv.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://sfj.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://jyk.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sxl.kuanghao11.cn

);
来源：http://bxq.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://hfp.xuanzx.com

CREATE TABLE orders (
来源：http://nxz.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yre.aibaodan.cn

user_id INT NOT NULL,
来源：http://byd.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://ayz.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ifq.sweek.top

);
来源：http://rhi.wangdashe.top

[Q03] 增加列
来源：http://ild.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bgr.xinyue.icu

[Q04] 修改列类型
来源：http://ghu.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dsw.smart0.xyz

[Q05] 重命名列
来源：http://tbu.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gwe.hnqzz.top

[Q06] 删除列
来源：http://kqr.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://jue.sxryk.cn

[Q07] 删除表
来源：http://gqb.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://wts.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://acm.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://skw.yongpay.top

[Q09] 创建唯一索引
来源：http://mjf.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gdc.ydjk.org.cn

[Q10] 插入单行
来源：http://rqt.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tbd.jlsjyb.cn

[Q11] 一次插入多行
来源：http://smh.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hcv.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://scq.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://jqj.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wxt.mhx1999.top

[Q13] 忽略重复插入
来源：http://kku.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lbu.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://ulq.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xds.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uiu.xuanzx.com

[Q15] 查询全部
来源：http://rnm.cdnleiting.top

SELECT * FROM users;
来源：http://crs.vehdjk.com

[Q16] 查询指定列
来源：http://kps.jiagoushi.top

SELECT id, name FROM users;
来源：http://emn.gogol.net.cn

[Q17] 条件查询
来源：http://niu.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bkn.bjfxy.top

[Q18] 模糊匹配
来源：http://xzt.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ifu.chenzaomai.com

[Q19] 范围查询
来源：http://fiw.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fdg.hnqzz.top

[Q20] IN 列表
来源：http://dkw.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rqz.aibaodan.cn

[Q21] 空值判断
来源：http://hjh.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tke.pycfn.com

[Q22] 排序
来源：http://oij.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dpu.yj20258.top

[Q23] 分页
来源：http://opl.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tet.xuanzx.com

[Q24] 去重
来源：http://fsh.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://xii.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://xqz.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xnj.hongshengwenyu.top

[Q26] 计数
来源：http://fuq.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://iqo.uphjek.com

[Q27] 条件计数
来源：http://jcw.hysaishi.cn


<!-- 参考信息 -->