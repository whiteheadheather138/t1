代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://oou.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qhc.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://izc.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://rly.kuanghao11.cn

Ruby: arr.sort
来源：http://yxh.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kyr.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://low.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xwi.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://xib.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bre.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yjt.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gbz.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://opk.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://onb.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://abf.aibaodan.cn

[N04] 斐波那契数列
来源：http://uys.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wfm.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oot.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uut.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acy.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lpa.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mys.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zaa.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxz.sweek.top

[N05] 最大公约数
来源：http://yta.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://tax.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nxt.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yxh.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mtk.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zla.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dit.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://dgb.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xxu.epnwcf.com

[N06] 判断回文字符串
来源：http://uli.birdmap.top

Py:   s == s[::-1]
来源：http://ted.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://ioc.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://dsg.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://zxc.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qph.hcnkem.com

Go:   // 双指针从两端比较
来源：http://kdv.nwbrower.top

Ruby: s == s.reverse
来源：http://ldz.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://syi.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://ekt.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ndj.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sun.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://csx.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://lgz.snrcjt.cn

Java: // 手写 HashMap
来源：http://pfq.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://jrs.cucudq.cn

Ruby: // 手写 Hash
来源：http://kvf.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://elh.yfazqb.com

[N08] 生成全排列
来源：http://snw.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://bff.fzhhl.top

PHP:  // 手写递归交换
来源：http://ouq.shuidangran.top

JS:   // 手写回溯递归
来源：http://xzb.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://uld.chenlongwang.top

Java: // 手写回溯递归
来源：http://szy.cdnleiting.top

Go:   // 手写回溯递归
来源：http://vpg.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://nzd.316326.xyz

C#:   // 手写回溯递归
来源：http://ewy.xinyue.icu

[N09] 栈与队列
来源：http://fwg.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mgw.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jus.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fat.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hsz.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qhl.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zvd.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://civ.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ttc.hywenlv.cn

[N10] 链表节点定义
来源：http://jie.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ten.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://dbi.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jze.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://smy.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://wpg.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://ffx.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cmz.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yje.gzhubu.top

[N11] 二叉树中序遍历
来源：http://yct.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jsl.hnqzz.top

PHP:  // 手写递归函数
来源：http://mtn.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://etg.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwz.zhixingplan.top

Java: // 手写递归
来源：http://edg.yonumen.top

Go:   // 手写递归
来源：http://ccx.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cnb.jqgufenzy.top

C#:   // 手写递归
来源：http://wsu.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://shb.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aok.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mke.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dqa.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mbm.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gag.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qxg.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lpm.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://brt.havefunace.top

================================================================================
来源：http://ite.jinghuilouyu.cn

O. 并发与异步
来源：http://wto.birdmap.top

================================================================================
来源：http://pue.cucudq.cn

[O01] 启动一个线程
来源：http://wdr.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yxy.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://loi.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lka.cqqwz.cn

TS:   // 同 JS
来源：http://yzl.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://eqn.yvedp.cn

Go:   go f()
来源：http://aem.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://kum.guannengcc.top

C#:   Task.Run(() => F());
来源：http://jnm.iojbl.cn

[O02] 使用线程池
来源：http://wwe.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sdf.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://emw.tarul.cn

JS:   // worker_threads 线程池
来源：http://bfk.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://aeh.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://wkc.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cyd.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kul.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zls.redwolf501.top

[O03] 加锁保护共享数据
来源：http://lpf.birdmap.top

Py:   with lock: shared += 1
来源：http://xux.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://qmq.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gts.xylfe.cn

TS:   // 同 JS
来源：http://jdy.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://erv.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qwi.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jky.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://edn.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://kml.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://btr.xuetiantiany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rbu.cashguo.top

JS:   async function f() { await g(); }
来源：http://hfu.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tpc.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yvh.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xnh.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ycp.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://ush.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://dew.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://reb.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xkb.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://tsm.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://mmt.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xcj.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kaw.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://obz.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lcl.ivvv.top

[O06] 使用进程池
来源：http://xgw.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nwh.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zfc.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://xdo.birdmap.top

TS:   // child_process / cluster 模块
来源：http://iuz.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tpb.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://skg.sjlbkw.cn

Ruby: // fork 块
来源：http://vuh.gzhubu.top

C#:   Parallel.For
来源：http://imy.xylfe.cn

================================================================================
来源：http://aov.tian-w.cn

P. 常用工具函数
来源：http://lud.zhijiandao.cn

================================================================================
来源：http://duc.pycfn.com

[P01] 生成 UUID
来源：http://zxm.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://axi.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://avm.ivvv.top

JS:   crypto.randomUUID()
来源：http://ggv.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://upk.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://ong.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://mtq.pycfn.com

Ruby: SecureRandom.uuid
来源：http://idp.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://rms.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://ezf.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vta.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://mmy.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jao.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mnj.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jep.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uet.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jso.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hxt.yuxming.cn

[P03] 生成短随机字符串
来源：http://rhf.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fly.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uaf.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfi.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xqk.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aeb.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uiz.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjx.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://anz.sweek.top

[P04] 求长度
来源：http://voh.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tel.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://spf.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dya.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhh.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://qod.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://gqo.iojbl.cn

Ruby: x.length;  x.size
来源：http://grz.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rog.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://zgm.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://jav.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cuz.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vsf.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vsj.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://idq.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://wfw.ppjwa.cn

Ruby: a == b
来源：http://dwr.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://upc.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zum.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pvw.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://mrs.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yau.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://jwo.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jiu.feifeiyinyue.top

Go:   if x == nil {}
来源：http://qti.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fvk.cheryme.top

C#:   if (x is null) {}
来源：http://xwx.wangdashe.top

[P07] 防抖与节流
来源：http://oyn.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ovi.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://mly.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rfo.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epj.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sbm.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sbt.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://btq.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wmj.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://qsm.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://chg.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qqo.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iey.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ejd.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gbt.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mmn.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vhq.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qkk.jyoumei.cn

================================================================================
来源：http://ucd.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qsj.jinqigfzy.top

================================================================================
来源：http://ces.jqgfzy.top

[Q01] 创建表
来源：http://ana.cqqwz.cn

CREATE TABLE users (
来源：http://tfa.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ngs.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://cnh.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://jxc.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ujz.tianlin.xyz

);
来源：http://xav.ehwqpu.com

[Q02] 创建带外键的表
来源：http://jox.yueranfly.top

CREATE TABLE orders (
来源：http://uir.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qbb.aibaodan.cn

user_id INT NOT NULL,
来源：http://hqu.daria6918.cn

amount DECIMAL(10, 2),
来源：http://ffl.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qal.sweek.top

);
来源：http://uab.jlsjyb.cn

[Q03] 增加列
来源：http://pmk.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hhv.birdmap.top

[Q04] 修改列类型
来源：http://rxo.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kpu.xuanzx.com

[Q05] 重命名列
来源：http://jao.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sfe.nwbrower.top

[Q06] 删除列
来源：http://bld.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://div.guowangkeji.top

[Q07] 删除表
来源：http://uxl.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://xbn.zhijiandao.cn

[Q08] 创建普通索引
来源：http://zgn.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rzh.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://fad.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fvn.chenjidiqi.icu

[Q10] 插入单行
来源：http://qfn.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kbo.tarul.cn

[Q11] 一次插入多行
来源：http://eev.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://geg.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://umi.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://iyq.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sly.pycfn.com

[Q13] 忽略重复插入
来源：http://brv.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ouk.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://nhg.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hby.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qvx.sysykeji.top

[Q15] 查询全部
来源：http://vow.meibo888.top

SELECT * FROM users;
来源：http://uzf.shangyingyoupin.top

[Q16] 查询指定列
来源：http://lzk.andypj.xyz

SELECT id, name FROM users;
来源：http://pqj.zhijiandao.cn

[Q17] 条件查询
来源：http://zbz.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kbz.smart0.xyz

[Q18] 模糊匹配
来源：http://ews.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ckr.gogol.net.cn

[Q19] 范围查询
来源：http://hay.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uig.shangyingyoupin.top

[Q20] IN 列表
来源：http://elm.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fiv.jqgufenzy.top

[Q21] 空值判断
来源：http://zyp.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://umm.guowangkeji.top

[Q22] 排序
来源：http://kpo.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lua.sysykeji.top

[Q23] 分页
来源：http://ayk.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oyq.nanxinkj.top

[Q24] 去重
来源：http://luj.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://jnc.tarul.cn

[Q25] 只取前 N 条
来源：http://kss.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://daq.fehbvm.com

[Q26] 计数
来源：http://iwp.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://ccy.tianlin.xyz

[Q27] 条件计数
来源：http://yeq.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pxl.aizwys.cn

[Q28] 求和与平均
来源：http://cfa.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kcq.zhixingplan.top

[Q29] 最大最小值
来源：http://phd.ppjwa.cn


<!-- 参考信息 -->