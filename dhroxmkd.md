代发 wailian999

Ruby: arr.sort
来源：http://uhk.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wpv.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://cmc.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://caz.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://dxf.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbt.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wmo.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rbl.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qcy.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mte.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://jgg.fktsv.cn

[N04] 斐波那契数列
来源：http://pnf.cdnleiting.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bdu.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sjg.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iup.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://smd.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzu.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lcw.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://obk.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ljb.vqdsnc.cn

[N05] 最大公约数
来源：http://zeb.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://wpe.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dqe.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wmr.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrt.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uhw.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avq.nwbrower.top

Ruby: a.gcd(b)
来源：http://kih.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gkw.ppjwa.cn

[N06] 判断回文字符串
来源：http://odd.tianlin.xyz

Py:   s == s[::-1]
来源：http://xku.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://fff.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://ujy.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://uay.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ear.hesvh.cn

Go:   // 双指针从两端比较
来源：http://gka.yueranfly.top

Ruby: s == s.reverse
来源：http://wzy.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lyu.cheryme.top

[N07] 两数之和（返回下标）
来源：http://avq.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ddi.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rlf.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jno.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://ybm.dashuyun.cn

Java: // 手写 HashMap
来源：http://csx.fehbvm.com

Go:   // 手写 map[int]int
来源：http://bap.yj202588.top

Ruby: // 手写 Hash
来源：http://uhn.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://pdk.iojbl.cn

[N08] 生成全排列
来源：http://nsx.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://eng.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://cju.zhixingplan.top

JS:   // 手写回溯递归
来源：http://lol.dashuyun.cn

TS:   // 手写回溯递归
来源：http://zhq.ybcxt.top

Java: // 手写回溯递归
来源：http://sml.9152youxi.cn

Go:   // 手写回溯递归
来源：http://gzh.yj20258.top

Ruby: arr.permutation.to_a
来源：http://rdt.yj20258888.top

C#:   // 手写回溯递归
来源：http://dvj.ivvv.top

[N09] 栈与队列
来源：http://yjz.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dtf.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vnt.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gij.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wuq.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mix.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vic.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xmd.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mbt.sjlbkw.cn

[N10] 链表节点定义
来源：http://ocs.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qkq.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mrh.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pjr.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kfc.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://ahk.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://qcx.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zfx.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ixr.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://wko.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fes.yuanzhike.top

PHP:  // 手写递归函数
来源：http://dyn.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ahy.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgb.jinqigfzy.top

Java: // 手写递归
来源：http://wyw.dashuyun.cn

Go:   // 手写递归
来源：http://iri.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ytw.havefunace.top

C#:   // 手写递归
来源：http://zrd.jqgufenzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jch.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tde.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygq.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://whm.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmx.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iiu.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://beq.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jmg.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zhr.yanxiufei.cn

================================================================================
来源：http://gai.nanxinkj.top

O. 并发与异步
来源：http://ysd.yangfankeji.com

================================================================================
来源：http://col.hongshengwenyu.top

[O01] 启动一个线程
来源：http://weh.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oma.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aid.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://afd.zhiwuduotai.top

TS:   // 同 JS
来源：http://ucj.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://rtm.tian-w.cn

Go:   go f()
来源：http://ceu.cashguo.top

Ruby: Thread.new { f }
来源：http://psx.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://dua.jiagoushi.top

[O02] 使用线程池
来源：http://ykc.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dpw.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xwi.redwolf501.top

JS:   // worker_threads 线程池
来源：http://ova.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://iyq.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dsh.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wic.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gyj.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dwv.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://exf.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://qtz.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://mkv.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ryu.nwbrower.top

TS:   // 同 JS
来源：http://xxe.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://myj.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bbi.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gtu.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://gfs.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://ycl.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://roo.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yvj.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://cqa.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gvv.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nww.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sle.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://npv.sweek.top

C#:   async Task F() { await G(); }
来源：http://esi.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://apw.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://wti.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ohi.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://idr.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://mdt.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://luq.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gdv.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://wrn.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://jnx.cdnleiting.top

[O06] 使用进程池
来源：http://gqc.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nfz.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ytx.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://pgs.ppjwa.cn

TS:   // child_process / cluster 模块
来源：http://ioi.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hqw.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wro.aizwys.cn

Ruby: // fork 块
来源：http://ekx.jinqigfzy.top

C#:   Parallel.For
来源：http://sxh.316326.xyz

================================================================================
来源：http://vmv.fanxiaobao.xyz

P. 常用工具函数
来源：http://hcp.zhixingplan.top

================================================================================
来源：http://vpf.andypj.xyz

[P01] 生成 UUID
来源：http://lcq.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://ojh.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ads.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://xll.jianghu66.top

TS:   crypto.randomUUID()
来源：http://eht.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://uwh.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://hlx.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://msq.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://ziq.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://tof.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qje.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rav.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://csq.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hqf.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zhv.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pfe.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vzo.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qbg.aibaodan.cn

[P03] 生成短随机字符串
来源：http://kyp.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rge.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bsg.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixz.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nnv.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://frw.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gsq.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rye.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kyl.cucudq.cn

[P04] 求长度
来源：http://rus.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fxx.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yfh.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvi.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsj.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://tka.daria6918.cn

Go:   len(arr);  len(m)
来源：http://vlj.yfazqb.com

Ruby: x.length;  x.size
来源：http://mxn.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pyk.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://bkd.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pwj.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qcv.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://skl.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sjl.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://smt.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://eer.daria6918.cn

Ruby: a == b
来源：http://ldd.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dew.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lth.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://inx.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://dnu.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ubx.zdqjudy.top

TS:   if (x == null) {}
来源：http://bdj.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vme.meibo888.top

Go:   if x == nil {}
来源：http://chr.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://opb.andypj.xyz

C#:   if (x is null) {}
来源：http://scm.vehdjk.com

[P07] 防抖与节流
来源：http://ern.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oeq.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://aii.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ial.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eop.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sgg.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://apk.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qyc.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ujs.bbcook.cn

[P08] 处理浮点精度问题
来源：http://izl.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xnw.nwbrower.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gpz.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://suf.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wgj.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uhk.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gin.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://byt.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oug.aibaodan.cn

================================================================================
来源：http://nya.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sdj.tanke756.top

================================================================================
来源：http://ufx.jinqigufen.top

[Q01] 创建表
来源：http://rqn.shzxlz.cn

CREATE TABLE users (
来源：http://oom.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://opy.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://iak.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://wca.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jkv.fanxiaobao.xyz

);
来源：http://qdz.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://acx.xziqi.cn

CREATE TABLE orders (
来源：http://nvu.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fag.ppjwa.cn

user_id INT NOT NULL,
来源：http://sdy.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://vxx.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vlc.yvedp.cn

);
来源：http://byf.sweek.top

[Q03] 增加列
来源：http://dxu.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vns.shzxlz.cn

[Q04] 修改列类型
来源：http://klj.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eix.cucudq.cn

[Q05] 重命名列
来源：http://zsz.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oci.gogol.net.cn

[Q06] 删除列
来源：http://zqc.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gbn.xuetiantiany.cn

[Q07] 删除表
来源：http://gvf.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://kth.hfpthk.cn

[Q08] 创建普通索引
来源：http://dfe.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gjb.redwolf501.top

[Q09] 创建唯一索引
来源：http://ees.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://npq.feifeiyinyue.top

[Q10] 插入单行
来源：http://mkr.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://brr.snrcjt.cn

[Q11] 一次插入多行
来源：http://mvu.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nuv.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://evm.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mxu.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://omf.svipenyu.cn

[Q13] 忽略重复插入
来源：http://xcx.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kjh.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://wpl.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mvm.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vqj.kuanghao11.cn

[Q15] 查询全部
来源：http://rni.shanyushiyangtech.top

SELECT * FROM users;
来源：http://kqv.nwbrower.top

[Q16] 查询指定列
来源：http://mvu.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://vkt.jianghu66.top

[Q17] 条件查询
来源：http://ykw.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dyg.ehwqpu.com

[Q18] 模糊匹配
来源：http://crm.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uvd.hysaishi.cn

[Q19] 范围查询
来源：http://nrx.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cbc.smart0.xyz

[Q20] IN 列表
来源：http://dvk.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://her.daria6918.cn

[Q21] 空值判断
来源：http://krh.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://tym.ywan-chungtsiang.top

[Q22] 排序
来源：http://nqi.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mxu.redwolf501.top

[Q23] 分页
来源：http://hwe.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gou.xziqi.cn

[Q24] 去重
来源：http://xem.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://tii.yvedp.cn

[Q25] 只取前 N 条
来源：http://nur.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vhy.jyoumei.cn

[Q26] 计数
来源：http://yha.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://wpk.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://bxw.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rbp.dianchejie.cn

[Q28] 求和与平均
来源：http://tej.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hrj.gzhubu.top

[Q29] 最大最小值
来源：http://sym.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bce.redwolf501.top

[Q30] 分组统计
来源：http://wij.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybg.nwbrower.top

[Q31] 分组后过滤
来源：http://bsd.zdqjudy.top


<!-- 参考信息 -->