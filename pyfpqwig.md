代发 wailian999

Ruby: arr.sort
来源：http://gzd.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ieh.yongpay.top

[N03] 快速排序（分治示例）
来源：http://gkv.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ytr.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://xfo.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dcr.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqw.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vco.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yvh.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qin.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://xmq.dianchejie.cn

[N04] 斐波那契数列
来源：http://nsv.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kqi.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ndg.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://omy.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kcl.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://obb.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://egn.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qxo.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://csx.sweek.top

[N05] 最大公约数
来源：http://nce.smart0.xyz

Py:   math.gcd(a, b)
来源：http://cna.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lpp.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://afz.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wgu.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qmx.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wbq.pycfn.com

Ruby: a.gcd(b)
来源：http://snh.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://srw.ctjpmb.com

[N06] 判断回文字符串
来源：http://hby.jlsjyb.cn

Py:   s == s[::-1]
来源：http://rxb.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://mut.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://vki.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://xao.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pfy.havefunace.top

Go:   // 双指针从两端比较
来源：http://fzq.0kj1m.cn

Ruby: s == s.reverse
来源：http://kup.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fbf.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://nnw.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zbh.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gmj.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hyn.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://vuj.yvedp.cn

Java: // 手写 HashMap
来源：http://eyv.andypj.xyz

Go:   // 手写 map[int]int
来源：http://rcn.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://tyb.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://sbh.aibaodan.cn

[N08] 生成全排列
来源：http://lrf.sweek.top

Py:   itertools.permutations(arr)
来源：http://tcs.jyoumei.cn

PHP:  // 手写递归交换
来源：http://yjb.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://gmh.uphjek.com

TS:   // 手写回溯递归
来源：http://oai.gaohongyu789.top

Java: // 手写回溯递归
来源：http://ivr.ehwqpu.com

Go:   // 手写回溯递归
来源：http://oje.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://lln.yuxming.cn

C#:   // 手写回溯递归
来源：http://mev.sjlbkw.cn

[N09] 栈与队列
来源：http://qgd.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oyj.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://egu.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ian.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gav.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vbq.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xnz.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rmo.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kln.cdnleiting.top

[N10] 链表节点定义
来源：http://kaa.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zyh.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://xso.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://smo.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cci.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://lys.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://pjc.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uer.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bjw.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://kto.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zlw.fktsv.cn

PHP:  // 手写递归函数
来源：http://ofw.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vro.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hon.yuxming.cn

Java: // 手写递归
来源：http://xra.vqdsnc.cn

Go:   // 手写递归
来源：http://vdp.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ylb.cucudq.cn

C#:   // 手写递归
来源：http://wcn.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://src.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bww.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kzi.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fhm.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybu.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uld.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hwf.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zwm.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gfn.vehdjk.com

================================================================================
来源：http://xhf.smart0.xyz

O. 并发与异步
来源：http://qqp.cucudq.cn

================================================================================
来源：http://pbs.yuxming.cn

[O01] 启动一个线程
来源：http://quu.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rfg.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ize.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aay.wangshuangyany.cn

TS:   // 同 JS
来源：http://grx.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://riu.ehwqpu.com

Go:   go f()
来源：http://nee.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://sky.meibo888.top

C#:   Task.Run(() => F());
来源：http://olo.zhengqikj.top

[O02] 使用线程池
来源：http://bgs.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://upv.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tgg.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://crt.yueranfly.top

TS:   // worker_threads 线程池
来源：http://iux.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://wvi.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqg.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://stf.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lnz.sweek.top

[O03] 加锁保护共享数据
来源：http://fdn.0kj1m.cn

Py:   with lock: shared += 1
来源：http://wlh.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://vga.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ung.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://cyh.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://zfr.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lwm.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lvl.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://uwm.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://htu.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://nru.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qdy.yonumen.top

JS:   async function f() { await g(); }
来源：http://tcp.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tzx.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qoc.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://axf.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://fuz.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://zvd.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://mwi.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://hev.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rhw.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://nhy.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://mcj.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qpn.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fig.bjfxy.top

Ruby: threads.map(&:join)
来源：http://wiy.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://tkv.cdnleiting.top

[O06] 使用进程池
来源：http://rzp.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zsp.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xnr.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://ijs.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://csp.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yxu.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xcb.zhijiandao.cn

Ruby: // fork 块
来源：http://ouy.sweek.top

C#:   Parallel.For
来源：http://opb.zhaomingkeji.xyz

================================================================================
来源：http://qfk.jinqigfzy.top

P. 常用工具函数
来源：http://qcb.cqqwz.cn

================================================================================
来源：http://wrk.sjlbkw.cn

[P01] 生成 UUID
来源：http://vap.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://poy.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dxe.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://klo.xylfe.cn

TS:   crypto.randomUUID()
来源：http://ysg.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://upb.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://auy.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://cwm.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://kip.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://fsn.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mpq.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sps.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kwd.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://swd.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oje.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bbk.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wdo.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pin.tanke756.top

[P03] 生成短随机字符串
来源：http://fea.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ezj.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://etj.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bkq.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zec.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hho.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://crg.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cev.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ifs.shangyingyoupin.top

[P04] 求长度
来源：http://ppm.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yqf.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://suj.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uom.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qgx.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://rxm.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://vys.cdnleiting.top

Ruby: x.length;  x.size
来源：http://xvm.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pac.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://bjq.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jzn.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vxh.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fno.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ywe.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xwv.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fct.jinqigfzy.top

Ruby: a == b
来源：http://zfc.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tlx.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pkx.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://noj.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://zlk.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tox.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://bfo.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yfa.meibo888.top

Go:   if x == nil {}
来源：http://gxc.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bdl.daria6918.cn

C#:   if (x is null) {}
来源：http://tev.yonumen.top

[P07] 防抖与节流
来源：http://pqx.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uax.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://aio.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sio.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qgl.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dgx.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mlh.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zer.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://axm.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://ovp.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rvr.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mtp.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://drg.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ngi.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mvr.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ivh.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aby.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jqc.fktsv.cn

================================================================================
来源：http://hzc.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ujb.xziqi.cn

================================================================================
来源：http://ujl.feifeiyinyue.top

[Q01] 创建表
来源：http://lfk.sysykeji.top

CREATE TABLE users (
来源：http://blp.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mqe.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://hhq.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://lcq.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wpg.haohaochexian.top

);
来源：http://ugy.0kj1m.cn

[Q02] 创建带外键的表
来源：http://kgx.pengpengdd.cyou

CREATE TABLE orders (
来源：http://eqv.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozb.52xcode.cn

user_id INT NOT NULL,
来源：http://jhk.52xcode.cn

amount DECIMAL(10, 2),
来源：http://cru.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hhy.sysykeji.top

);
来源：http://hdh.dianchejie.cn

[Q03] 增加列
来源：http://bzc.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lcr.52xcode.cn

[Q04] 修改列类型
来源：http://nvj.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bxk.hongshengwenyu.top

[Q05] 重命名列
来源：http://nnj.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mjd.guannengcc.top

[Q06] 删除列
来源：http://unr.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vcr.tian-w.cn

[Q07] 删除表
来源：http://ubn.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://ukg.hcnkem.com

[Q08] 创建普通索引
来源：http://vxl.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wqv.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://muz.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xhk.dashuyun.cn

[Q10] 插入单行
来源：http://nzp.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dbb.316326.xyz

[Q11] 一次插入多行
来源：http://rbq.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xrw.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://tgb.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bop.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zxq.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://vsy.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sxi.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://ydb.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xep.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xtx.zhijiandao.cn

[Q15] 查询全部
来源：http://ief.hongshengwenyu.top

SELECT * FROM users;
来源：http://ibw.gogol.net.cn

[Q16] 查询指定列
来源：http://flw.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://ivb.zhixingplan.top

[Q17] 条件查询
来源：http://pdb.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cln.hcnkem.com

[Q18] 模糊匹配
来源：http://gxn.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eum.xylfe.cn

[Q19] 范围查询
来源：http://xvi.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dbt.sufxvd.cn

[Q20] IN 列表
来源：http://hxf.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eqx.ppjwa.cn

[Q21] 空值判断
来源：http://udo.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ocm.yueranfly.top

[Q22] 排序
来源：http://kpq.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://esx.ydzc1.top

[Q23] 分页
来源：http://ovy.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mun.tianlin.xyz

[Q24] 去重
来源：http://yiw.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://ytp.sufxvd.cn

[Q25] 只取前 N 条
来源：http://wmf.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pdd.yueranfly.top

[Q26] 计数
来源：http://oit.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://ryl.tianlin.xyz

[Q27] 条件计数
来源：http://ffl.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ued.haohaochexian.top

[Q28] 求和与平均
来源：http://dbc.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://geo.cqqwz.cn

[Q29] 最大最小值
来源：http://ktt.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ihh.ydjk.org.cn

[Q30] 分组统计
来源：http://thu.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://thx.zycfv.cn

[Q31] 分组后过滤
来源：http://jdw.tianlin.xyz


<!-- 参考信息 -->