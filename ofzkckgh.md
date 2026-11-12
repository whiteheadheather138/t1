代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://ilz.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cvo.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rks.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://ncg.zycfv.cn

Ruby: arr.sort
来源：http://cdj.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lwm.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://lmq.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qtc.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://cik.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://euz.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://veh.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xwd.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qil.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xdj.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://orj.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://cqv.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ufa.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vkh.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pcu.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dms.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jio.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xok.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cjl.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aqp.snrcjt.cn

[N05] 最大公约数
来源：http://jgf.meibo888.top

Py:   math.gcd(a, b)
来源：http://vui.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wze.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://trp.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avt.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ufr.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://daq.nwbrower.top

Ruby: a.gcd(b)
来源：http://dze.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qgt.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://cka.cdnleiting.top

Py:   s == s[::-1]
来源：http://vle.meibo888.top

PHP:  $s === strrev($s);
来源：http://hkc.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://wfr.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://tja.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bjf.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://wdh.quarkkingdee.top

Ruby: s == s.reverse
来源：http://abg.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://osm.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://kjd.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wyq.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iey.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zel.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://dlj.cheryme.top

Java: // 手写 HashMap
来源：http://ptm.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://eya.bbcook.cn

Ruby: // 手写 Hash
来源：http://ibd.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://iti.yj20258.top

[N08] 生成全排列
来源：http://qxi.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://bye.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://tyw.jinqigufen.top

JS:   // 手写回溯递归
来源：http://vdr.aizwys.cn

TS:   // 手写回溯递归
来源：http://ojh.chenzaomai.com

Java: // 手写回溯递归
来源：http://lkc.fktsv.cn

Go:   // 手写回溯递归
来源：http://gme.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://tuh.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://qcu.yonumen.top

[N09] 栈与队列
来源：http://rdv.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aaw.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://scd.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qcc.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zzo.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://loi.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tpj.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vva.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dlp.nwbrower.top

[N10] 链表节点定义
来源：http://gri.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fdm.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://lvr.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ykx.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pad.tarul.cn

Java: class Node { int v; Node next; }
来源：http://kbn.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://rvt.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zlz.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xbz.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://juw.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://amr.sweek.top

PHP:  // 手写递归函数
来源：http://vkb.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ujv.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uma.yangfankeji.com

Java: // 手写递归
来源：http://ion.shzxlz.cn

Go:   // 手写递归
来源：http://hhp.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://exm.aibaodan.cn

C#:   // 手写递归
来源：http://myu.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lwf.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kcr.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xgq.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oju.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mrs.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rtc.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rwd.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ncg.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yme.jinqigfzy.top

================================================================================
来源：http://jie.ydzc1.top

O. 并发与异步
来源：http://ndq.ydjk.org.cn

================================================================================
来源：http://zvp.xuetiantiany.cn

[O01] 启动一个线程
来源：http://yye.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yhg.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kkg.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rhl.dianchejie.cn

TS:   // 同 JS
来源：http://btz.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://qzu.ybcxt.top

Go:   go f()
来源：http://uln.yj202588.top

Ruby: Thread.new { f }
来源：http://rqc.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://jeh.zycfv.cn

[O02] 使用线程池
来源：http://pvl.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://brz.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lzj.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://bvd.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://lfv.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://wdw.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qyu.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vmm.yj20258888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ecq.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://lkt.chenzaomai.com

Py:   with lock: shared += 1
来源：http://lis.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://rkx.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fes.fengsongda.top

TS:   // 同 JS
来源：http://lrp.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://ibj.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://smr.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pcs.dianchejie.cn

C#:   lock (gate) { shared++; }
来源：http://fpv.yvedp.cn

[O04] 定义异步函数并等待
来源：http://xgq.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://zzu.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://plx.vehdjk.com

JS:   async function f() { await g(); }
来源：http://clk.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://itt.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jcm.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wce.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://sxw.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://pyn.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://ope.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://ros.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ocu.meibo888.top

JS:   await Promise.all(tasks)
来源：http://nmq.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://imb.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ney.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vhd.cucudq.cn

Ruby: threads.map(&:join)
来源：http://efu.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lst.fengsongda.top

[O06] 使用进程池
来源：http://yal.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://evu.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://are.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://flk.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://crl.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fck.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ujn.yfazqb.com

Ruby: // fork 块
来源：http://guw.tanke756.top

C#:   Parallel.For
来源：http://cfg.jianghu66.top

================================================================================
来源：http://pdy.hesvh.cn

P. 常用工具函数
来源：http://zqq.vqdsnc.cn

================================================================================
来源：http://hvh.zycfv.cn

[P01] 生成 UUID
来源：http://mrk.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://mwk.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bcu.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://jwx.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://laa.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://slq.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://zqb.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://tyz.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://uil.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://zbs.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dsy.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ogr.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://stn.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ybc.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ktz.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hxt.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://byk.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vyw.ppjwa.cn

[P03] 生成短随机字符串
来源：http://xnl.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhl.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://znu.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://phu.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hct.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qof.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zuo.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ded.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kcj.sxryk.cn

[P04] 求长度
来源：http://auw.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cpw.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nth.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bjg.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://esf.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://uru.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://lgt.hywenlv.cn

Ruby: x.length;  x.size
来源：http://xsp.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nko.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://dkw.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://idy.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nwk.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kxt.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hwr.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mlx.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lry.jlsjyb.cn

Ruby: a == b
来源：http://elf.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nrc.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dtq.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qck.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://kid.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dhh.yvedp.cn

TS:   if (x == null) {}
来源：http://gpm.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gcw.sxryk.cn

Go:   if x == nil {}
来源：http://std.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cat.gogol.net.cn

C#:   if (x is null) {}
来源：http://byx.dianchejie.cn

[P07] 防抖与节流
来源：http://apt.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xor.ivvv.top

PHP:  // 手写时间戳比较
来源：http://wcr.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gro.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xvy.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zcn.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gxv.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eha.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bow.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://use.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://obr.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vit.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qgl.ydjk.org.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pwn.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://udc.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pla.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oou.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wuy.hesvh.cn

================================================================================
来源：http://ieh.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ctb.bjfxy.top

================================================================================
来源：http://tmu.mhx1999.top

[Q01] 创建表
来源：http://pdu.ydzc1.top

CREATE TABLE users (
来源：http://ggp.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rjj.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://bpz.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://kru.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fta.xuetiantiany.cn

);
来源：http://hjv.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://scs.dashuyun.cn

CREATE TABLE orders (
来源：http://fzb.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cvi.vehdjk.com

user_id INT NOT NULL,
来源：http://rra.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://ysb.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fre.birdmap.top

);
来源：http://qkk.yuxming.cn

[Q03] 增加列
来源：http://kvd.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tal.xuetiantiany.cn

[Q04] 修改列类型
来源：http://tiv.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cti.ehwqpu.com

[Q05] 重命名列
来源：http://oen.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pnu.sjlbkw.cn

[Q06] 删除列
来源：http://akj.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://yil.jinyuanbaomall.cn

[Q07] 删除表
来源：http://qsx.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://lpw.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://agd.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yxy.yuanzhike.top

[Q09] 创建唯一索引
来源：http://xyc.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://obk.dianchejie.cn

[Q10] 插入单行
来源：http://qvq.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jiq.zhixingplan.top

[Q11] 一次插入多行
来源：http://jog.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wyb.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://dam.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://nwk.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hnv.ehwqpu.com

[Q13] 忽略重复插入
来源：http://nkt.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pnt.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://tzh.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tlj.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bos.chenzaomai.com

[Q15] 查询全部
来源：http://eux.pengpengdd.cyou

SELECT * FROM users;
来源：http://bvu.jlsjyb.cn

[Q16] 查询指定列
来源：http://asr.jyoumei.cn

SELECT id, name FROM users;
来源：http://etx.snrcjt.cn

[Q17] 条件查询
来源：http://wvn.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nup.wangdashe.top

[Q18] 模糊匹配
来源：http://twm.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gen.zhongyouzk.top

[Q19] 范围查询
来源：http://yvt.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fnr.jiagoushi.top

[Q20] IN 列表
来源：http://lkc.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pxz.cheryme.top

[Q21] 空值判断
来源：http://eip.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yxo.nanxinkj.top

[Q22] 排序
来源：http://ymb.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://whz.yuxming.cn

[Q23] 分页
来源：http://nkf.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ulq.jiagoushi.top

[Q24] 去重
来源：http://hkm.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://khy.yvedp.cn

[Q25] 只取前 N 条
来源：http://lww.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://has.quarkkingdee.top

[Q26] 计数
来源：http://fje.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://bsz.zhoulong.xyz

[Q27] 条件计数
来源：http://yty.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yvl.vqdsnc.cn

[Q28] 求和与平均
来源：http://wyl.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://abu.mhx1999.top

[Q29] 最大最小值
来源：http://gag.yueranfly.top


<!-- 参考信息 -->