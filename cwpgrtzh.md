代发 wailian999

Ruby: arr.sort
来源：http://qxm.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://imv.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://oyd.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ejc.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://udj.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tor.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tak.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rzy.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kkg.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kvg.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://qzt.hesvh.cn

[N04] 斐波那契数列
来源：http://erx.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tlk.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vpp.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zbp.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ljc.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jpx.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hnb.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gpe.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ull.bbcook.cn

[N05] 最大公约数
来源：http://zko.pycfn.com

Py:   math.gcd(a, b)
来源：http://hnl.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhj.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpp.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://phc.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vbb.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kld.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://fhk.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tyf.meibo888.top

[N06] 判断回文字符串
来源：http://csk.xylfe.cn

Py:   s == s[::-1]
来源：http://cmw.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://dss.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://otx.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://hgf.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ujd.c1oappe.top

Go:   // 双指针从两端比较
来源：http://rqb.cqqwz.cn

Ruby: s == s.reverse
来源：http://gdx.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://uri.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://nua.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aru.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fyf.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oqv.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://yha.hysaishi.cn

Java: // 手写 HashMap
来源：http://oms.hnqzz.top

Go:   // 手写 map[int]int
来源：http://dlc.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://mss.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://vjh.hfpthk.cn

[N08] 生成全排列
来源：http://rrf.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://frl.yueranfly.top

PHP:  // 手写递归交换
来源：http://fsf.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://ixr.nwbrower.top

TS:   // 手写回溯递归
来源：http://ppp.tarul.cn

Java: // 手写回溯递归
来源：http://nfq.yj20258.top

Go:   // 手写回溯递归
来源：http://qrq.tarul.cn

Ruby: arr.permutation.to_a
来源：http://zez.dianchejie.cn

C#:   // 手写回溯递归
来源：http://eva.xziqi.cn

[N09] 栈与队列
来源：http://njz.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hoa.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pgn.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nns.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://etv.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://okx.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rnj.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fsn.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sqt.zhengqikj.top

[N10] 链表节点定义
来源：http://zwl.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yhs.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://grr.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dit.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bvh.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://boe.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://tgs.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tpf.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uyy.bbcook.cn

[N11] 二叉树中序遍历
来源：http://wle.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pjv.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://vci.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oul.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nsh.sxryk.cn

Java: // 手写递归
来源：http://dkg.iojbl.cn

Go:   // 手写递归
来源：http://yqw.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lzd.jyoumei.cn

C#:   // 手写递归
来源：http://dys.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ifx.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qmz.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://erh.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hcr.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lza.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://olu.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eyj.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gqm.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://euc.xingfuxueyuan.xyz

================================================================================
来源：http://ckq.gogol.net.cn

O. 并发与异步
来源：http://pie.jianghu66.top

================================================================================
来源：http://rmt.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://gzj.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ayg.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ycj.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://akk.fzhhl.top

TS:   // 同 JS
来源：http://puc.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://svy.shuidangran.top

Go:   go f()
来源：http://qnt.nanxinkj.top

Ruby: Thread.new { f }
来源：http://fzv.sweek.top

C#:   Task.Run(() => F());
来源：http://nga.ehwqpu.com

[O02] 使用线程池
来源：http://scm.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rvp.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sqc.tian-w.cn

JS:   // worker_threads 线程池
来源：http://jda.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://nti.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://drp.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oox.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wjv.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nla.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://pod.daxiang520.top

Py:   with lock: shared += 1
来源：http://fuk.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://ial.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tcq.hnxiangtu.top

TS:   // 同 JS
来源：http://xqf.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://jqi.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://phh.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lvk.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://qod.cheryme.top

[O04] 定义异步函数并等待
来源：http://urq.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://iqm.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ayv.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://fkt.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bdj.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xpx.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qoa.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://waw.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://mkr.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://gnn.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://ghq.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://muk.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://tnm.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://oea.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ewh.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wjx.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://sxr.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kry.zdqjudy.top

[O06] 使用进程池
来源：http://wtp.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gbu.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ozp.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://aib.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://dbe.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ilb.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yhp.pycfn.com

Ruby: // fork 块
来源：http://shl.daria6918.cn

C#:   Parallel.For
来源：http://tbd.jiagoushi.top

================================================================================
来源：http://rum.iojbl.cn

P. 常用工具函数
来源：http://eoi.yueranfly.top

================================================================================
来源：http://lsn.guowangkeji.top

[P01] 生成 UUID
来源：http://zzq.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://hmg.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uec.daxiang520.top

JS:   crypto.randomUUID()
来源：http://iva.gzhubu.top

TS:   crypto.randomUUID()
来源：http://dtd.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://mbj.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://pxi.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://omc.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://lmq.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://diz.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fwm.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kdz.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dtq.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ojy.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fml.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kfq.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tqr.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wlj.tian-w.cn

[P03] 生成短随机字符串
来源：http://fnk.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ldp.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wzo.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sws.yvedp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://smc.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mfs.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nff.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bgl.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vkn.yongpay.top

[P04] 求长度
来源：http://aqi.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rlt.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cla.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qea.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kdx.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://lmk.tarul.cn

Go:   len(arr);  len(m)
来源：http://yoa.fehbvm.com

Ruby: x.length;  x.size
来源：http://kum.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mmw.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://pbg.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vpk.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fut.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xlh.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bzt.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rfm.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://imn.cqqwz.cn

Ruby: a == b
来源：http://aoj.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ukq.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hjd.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://djf.316326.xyz

PHP:  if (empty($x)) {}
来源：http://bhk.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rgt.hywenlv.cn

TS:   if (x == null) {}
来源：http://ggc.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://fuh.yfazqb.com

Go:   if x == nil {}
来源：http://dfx.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lkc.dianchejie.cn

C#:   if (x is null) {}
来源：http://yzs.fzhhl.top

[P07] 防抖与节流
来源：http://jju.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://orm.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://enw.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://avs.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwj.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pej.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cnz.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://smg.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ifj.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://gly.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sgj.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pjd.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tkh.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cav.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ezc.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kfu.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mcd.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bqb.guowangkeji.top

================================================================================
来源：http://nre.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bch.hammf.cn

================================================================================
来源：http://pim.epnwcf.com

[Q01] 创建表
来源：http://zsg.yueranfly.top

CREATE TABLE users (
来源：http://fkr.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aix.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://bjk.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://ynh.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gox.quarkkingdee.top

);
来源：http://hbk.316326.xyz

[Q02] 创建带外键的表
来源：http://iat.vehdjk.com

CREATE TABLE orders (
来源：http://vfd.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bih.fengsongda.top

user_id INT NOT NULL,
来源：http://mwt.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://eil.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iyv.chenlongwang.top

);
来源：http://jgq.ywan-chungtsiang.top

[Q03] 增加列
来源：http://mxf.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qqf.sxryk.cn

[Q04] 修改列类型
来源：http://uky.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wpl.yangfankeji.com

[Q05] 重命名列
来源：http://xsm.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://weg.nanxinkj.top

[Q06] 删除列
来源：http://oia.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://nbn.ivvv.top

[Q07] 删除表
来源：http://cde.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://smw.dashuyun.cn

[Q08] 创建普通索引
来源：http://fps.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://olm.yj20258.top

[Q09] 创建唯一索引
来源：http://ght.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iyi.pengpengdd.cyou

[Q10] 插入单行
来源：http://kcx.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dmj.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://iqe.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dkz.316326.xyz

[Q12] 插入后取自增 ID
来源：http://xmn.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://dhy.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qen.fehbvm.com

[Q13] 忽略重复插入
来源：http://bxa.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wxh.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://nea.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qzj.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kwy.zdbjq.cn

[Q15] 查询全部
来源：http://fib.cashguo.top

SELECT * FROM users;
来源：http://zsk.dianchejie.cn

[Q16] 查询指定列
来源：http://qpe.dianchejie.cn

SELECT id, name FROM users;
来源：http://gdq.shanyushiyangtech.top

[Q17] 条件查询
来源：http://fwk.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jev.zdbjq.cn

[Q18] 模糊匹配
来源：http://qtr.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zyq.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://yrd.tarul.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mxr.zdbjq.cn

[Q20] IN 列表
来源：http://kze.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lso.sysykeji.top

[Q21] 空值判断
来源：http://idx.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://zhg.fktsv.cn

[Q22] 排序
来源：http://qlm.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ugk.vehdjk.com

[Q23] 分页
来源：http://xyr.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xpf.chenzaomai.com

[Q24] 去重
来源：http://vlo.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://rqc.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://uow.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://plz.ctjpmb.com

[Q26] 计数
来源：http://cqq.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://pot.nanxinkj.top

[Q27] 条件计数
来源：http://oha.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dlm.cucudq.cn

[Q28] 求和与平均
来源：http://dnq.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lgh.jinqigufen.top

[Q29] 最大最小值
来源：http://mro.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rhz.jinqigfzy.top

[Q30] 分组统计
来源：http://ujw.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lif.gzhubu.top

[Q31] 分组后过滤
来源：http://fqo.fehbvm.com


<!-- 参考信息 -->