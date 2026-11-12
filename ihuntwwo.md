代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://xoo.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bwt.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ngs.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://ttv.cdnleiting.top

Ruby: arr.sort
来源：http://ksc.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qqi.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://slz.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uvr.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://bwp.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddt.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fcy.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bhg.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pus.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hdd.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ioc.jqgufenzy.top

[N04] 斐波那契数列
来源：http://ucc.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hie.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xyq.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lhj.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://feg.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rth.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fol.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pbf.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xzw.dashuyun.cn

[N05] 最大公约数
来源：http://gjh.ybcxt.top

Py:   math.gcd(a, b)
来源：http://yki.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nfz.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fvj.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nye.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mjt.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vrj.chenlongwang.top

Ruby: a.gcd(b)
来源：http://jfo.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qgc.fehbvm.com

[N06] 判断回文字符串
来源：http://ppa.shzxlz.cn

Py:   s == s[::-1]
来源：http://rkc.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://pbj.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://rqa.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://zvv.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://erj.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://avp.ppjwa.cn

Ruby: s == s.reverse
来源：http://yls.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://jyk.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://bvx.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hmy.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hgp.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ggs.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://emu.aibaodan.cn

Java: // 手写 HashMap
来源：http://wqu.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://gmd.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://wav.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vbr.vqdsnc.cn

[N08] 生成全排列
来源：http://emk.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://fiw.316326.xyz

PHP:  // 手写递归交换
来源：http://llb.zdbjq.cn

JS:   // 手写回溯递归
来源：http://chk.wangdashe.top

TS:   // 手写回溯递归
来源：http://ugt.vehdjk.com

Java: // 手写回溯递归
来源：http://bmu.yuxming.cn

Go:   // 手写回溯递归
来源：http://xlc.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://etl.zdbjq.cn

C#:   // 手写回溯递归
来源：http://xwg.yvedp.cn

[N09] 栈与队列
来源：http://hdi.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://owh.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rqo.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tuv.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ogj.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wmi.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://chc.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://irc.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lse.yj20258888.top

[N10] 链表节点定义
来源：http://zmr.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mqg.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://whi.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dcv.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vqg.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://byx.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://dnb.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pnw.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cot.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://knc.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://woc.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://rqa.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgt.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rny.c1oappe.top

Java: // 手写递归
来源：http://tzu.0kj1m.cn

Go:   // 手写递归
来源：http://jub.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ewf.cqqwz.cn

C#:   // 手写递归
来源：http://ctj.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qjy.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tac.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xvq.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdv.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxq.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lzj.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ltl.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lst.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zdl.aibaodan.cn

================================================================================
来源：http://cpv.uphjek.com

O. 并发与异步
来源：http://prr.zhixingplan.top

================================================================================
来源：http://hjl.jiagoushi.top

[O01] 启动一个线程
来源：http://wca.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://egx.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lhr.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fwa.mhx1999.top

TS:   // 同 JS
来源：http://xxr.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://whh.zdbjq.cn

Go:   go f()
来源：http://qkm.hnqzz.top

Ruby: Thread.new { f }
来源：http://obo.sxryk.cn

C#:   Task.Run(() => F());
来源：http://jah.gogol.net.cn

[O02] 使用线程池
来源：http://rji.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ldh.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kpt.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://pmh.ivvv.top

TS:   // worker_threads 线程池
来源：http://nqe.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tdu.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://efo.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ibb.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nvt.xylfe.cn

[O03] 加锁保护共享数据
来源：http://ikk.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://fje.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://lsf.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zyz.yvedp.cn

TS:   // 同 JS
来源：http://cjd.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://dat.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fsv.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bcs.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://ozi.iojbl.cn

[O04] 定义异步函数并等待
来源：http://dgt.316326.xyz

Py:   async def f():⏎    await g()
来源：http://pma.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ffb.cheryme.top

JS:   async function f() { await g(); }
来源：http://gid.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://scz.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ici.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ncs.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://qgq.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://qrj.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://ahz.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://ejt.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://idp.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://shd.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://nfg.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eos.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ilg.nwbrower.top

Ruby: threads.map(&:join)
来源：http://yxs.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://txw.fzhhl.top

[O06] 使用进程池
来源：http://fnz.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://abb.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://arx.pycfn.com

JS:   // child_process / cluster 模块
来源：http://mwq.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://rmr.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://njy.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dhv.gzhubu.top

Ruby: // fork 块
来源：http://nps.jinqigufen.top

C#:   Parallel.For
来源：http://bmb.smart0.xyz

================================================================================
来源：http://fop.bbcook.cn

P. 常用工具函数
来源：http://fga.aibaodan.cn

================================================================================
来源：http://xut.hfpthk.cn

[P01] 生成 UUID
来源：http://cby.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://hlp.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qyr.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://cav.havefunace.top

TS:   crypto.randomUUID()
来源：http://hqj.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://upl.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://gqw.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://zad.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://tsv.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://tmy.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fhz.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jfb.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aeg.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zhf.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jxz.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cic.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vwe.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://syf.cdnleiting.top

[P03] 生成短随机字符串
来源：http://tgx.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://efa.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wyn.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mal.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://snm.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mer.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mbl.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ysl.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zax.fktsv.cn

[P04] 求长度
来源：http://jjx.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xda.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vkh.redwolf501.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ohi.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jup.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://ixx.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://zwl.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://glf.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qrj.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://lfs.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://peb.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hew.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lii.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xcj.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iqw.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://akz.zhijiandao.cn

Ruby: a == b
来源：http://onr.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lfr.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mrr.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qwo.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://doa.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fwq.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://tza.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lfa.shzxlz.cn

Go:   if x == nil {}
来源：http://qjx.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vid.zdbjq.cn

C#:   if (x is null) {}
来源：http://uhe.shzxlz.cn

[P07] 防抖与节流
来源：http://iwu.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zot.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://tbb.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfu.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ynm.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bdw.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rnc.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ivg.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fzm.tarul.cn

[P08] 处理浮点精度问题
来源：http://ldz.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sqf.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hik.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zsz.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qxq.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://drt.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vjp.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fdo.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gvs.shzxlz.cn

================================================================================
来源：http://hdu.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gll.sjlbkw.cn

================================================================================
来源：http://tsn.ehwqpu.com

[Q01] 创建表
来源：http://bgy.52xcode.cn

CREATE TABLE users (
来源：http://zqi.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dnh.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://qmy.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://kgn.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hna.ctjpmb.com

);
来源：http://ylj.aizwys.cn

[Q02] 创建带外键的表
来源：http://qmo.pycfn.com

CREATE TABLE orders (
来源：http://rmf.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgp.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://rkt.cashguo.top

amount DECIMAL(10, 2),
来源：http://zfe.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lym.daxiang520.top

);
来源：http://yxh.jiagoushi.top

[Q03] 增加列
来源：http://lct.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ssz.feifeiyinyue.top

[Q04] 修改列类型
来源：http://tkf.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bbq.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://yoq.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://txd.ywan-chungtsiang.top

[Q06] 删除列
来源：http://qvk.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://uts.chenlongwang.top

[Q07] 删除表
来源：http://sgm.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://tpg.jlsjyb.cn

[Q08] 创建普通索引
来源：http://taz.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gnc.shuidangran.top

[Q09] 创建唯一索引
来源：http://hgp.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rjy.hesvh.cn

[Q10] 插入单行
来源：http://uno.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iiq.nanxinkj.top

[Q11] 一次插入多行
来源：http://tsp.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ilp.tanke756.top

[Q12] 插入后取自增 ID
来源：http://bsn.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://rnr.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://smx.jqgfzy.top

[Q13] 忽略重复插入
来源：http://ptp.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ypa.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://zih.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qno.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nvy.cashguo.top

[Q15] 查询全部
来源：http://ztm.epnwcf.com

SELECT * FROM users;
来源：http://fny.zycfv.cn

[Q16] 查询指定列
来源：http://ixj.jianghu66.top

SELECT id, name FROM users;
来源：http://tku.aizwys.cn

[Q17] 条件查询
来源：http://zkb.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ewo.yueranfly.top

[Q18] 模糊匹配
来源：http://snb.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zvs.316326.xyz

[Q19] 范围查询
来源：http://ywe.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bia.daxiang520.top

[Q20] IN 列表
来源：http://rna.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jki.hnqzz.top

[Q21] 空值判断
来源：http://dcw.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ckl.dianchejie.cn

[Q22] 排序
来源：http://dkp.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qze.gzhubu.top

[Q23] 分页
来源：http://lgc.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ewd.zdqjudy.top

[Q24] 去重
来源：http://qhd.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://wxp.guowangkeji.top

[Q25] 只取前 N 条
来源：http://wbf.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qnt.cdnleiting.top

[Q26] 计数
来源：http://ytp.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://xht.cdnleiting.top

[Q27] 条件计数
来源：http://pbm.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mxx.nanxuanxn.top

[Q28] 求和与平均
来源：http://kem.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ihw.vehdjk.com

[Q29] 最大最小值
来源：http://emw.dashuyun.cn


<!-- 参考信息 -->