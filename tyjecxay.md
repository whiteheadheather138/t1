代发 wailian999

Ruby: arr.sort
来源：http://rwz.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ohf.316326.xyz

[N03] 快速排序（分治示例）
来源：http://llt.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ims.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://jvz.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojb.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wnm.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jcn.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tva.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rqc.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://olx.zhengqikj.top

[N04] 斐波那契数列
来源：http://vey.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://drg.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bic.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqf.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mlm.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ffd.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uyg.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ibu.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fzm.jqgufenzy.top

[N05] 最大公约数
来源：http://yzb.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://yso.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dte.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hkb.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mrb.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://knl.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jzv.vehdjk.com

Ruby: a.gcd(b)
来源：http://gwe.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://egb.yueranfly.top

[N06] 判断回文字符串
来源：http://qsw.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://gfr.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://auz.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://opc.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://una.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hvr.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://efe.sufxvd.cn

Ruby: s == s.reverse
来源：http://vzg.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wzt.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://vku.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydp.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://amp.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vmp.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://czl.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://fed.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://lck.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://dpa.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yvk.sweek.top

[N08] 生成全排列
来源：http://hjx.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://kft.guannengcc.top

PHP:  // 手写递归交换
来源：http://vzm.yj20258888.top

JS:   // 手写回溯递归
来源：http://esu.yongpay.top

TS:   // 手写回溯递归
来源：http://arj.wangdashe.top

Java: // 手写回溯递归
来源：http://nrr.shzxlz.cn

Go:   // 手写回溯递归
来源：http://bzw.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://cmj.tian-w.cn

C#:   // 手写回溯递归
来源：http://fgx.yangfankeji.com

[N09] 栈与队列
来源：http://rjx.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sqk.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mbb.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://atf.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qdu.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hxk.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qyx.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fge.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vgh.ivvv.top

[N10] 链表节点定义
来源：http://pkg.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wvl.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qad.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qgs.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ciz.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://jbv.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://vrl.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://fei.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dmv.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://ehh.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mlp.jqgfzy.top

PHP:  // 手写递归函数
来源：http://lgx.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://afa.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gda.gaohongyu789.top

Java: // 手写递归
来源：http://msr.daria6918.cn

Go:   // 手写递归
来源：http://kud.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wga.cucudq.cn

C#:   // 手写递归
来源：http://euj.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dca.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hys.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hkm.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejn.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kxw.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://knr.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wew.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pic.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://car.jinyuanbaomall.cn

================================================================================
来源：http://utm.cucudq.cn

O. 并发与异步
来源：http://uvg.ydjk.org.cn

================================================================================
来源：http://qxq.cqqwz.cn

[O01] 启动一个线程
来源：http://hdg.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qvq.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xuz.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qez.xuanzx.com

TS:   // 同 JS
来源：http://uke.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://hte.nwbrower.top

Go:   go f()
来源：http://apq.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://wul.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://yuq.jlsjyb.cn

[O02] 使用线程池
来源：http://zni.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://enn.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mrn.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://mbm.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://yfp.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rnd.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kte.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avc.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hpv.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://dmv.cucudq.cn

Py:   with lock: shared += 1
来源：http://hzp.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://fsj.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uvb.yj202588.top

TS:   // 同 JS
来源：http://jif.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://xyx.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qag.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wqp.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://azp.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://ppn.316326.xyz

Py:   async def f():⏎    await g()
来源：http://npq.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uen.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://rzp.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ush.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yov.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zph.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cet.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://afp.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://tjx.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://pes.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pyt.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://fsy.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://bza.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iuj.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qyq.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://rqj.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pxq.xuetiantiany.cn

[O06] 使用进程池
来源：http://yfi.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qvw.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kjm.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://dqa.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://not.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rnm.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nyk.316326.xyz

Ruby: // fork 块
来源：http://ely.havefunace.top

C#:   Parallel.For
来源：http://fop.pycfn.com

================================================================================
来源：http://ama.zhijiandao.cn

P. 常用工具函数
来源：http://rva.yonumen.top

================================================================================
来源：http://aix.jinqigfzy.top

[P01] 生成 UUID
来源：http://wwr.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://zrl.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zvh.mhx1999.top

JS:   crypto.randomUUID()
来源：http://ctd.xuanzx.com

TS:   crypto.randomUUID()
来源：http://ygv.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://psb.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://ftj.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://lav.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://tlc.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://zwb.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cob.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uod.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iij.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nny.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://umx.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nzr.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kdt.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kdd.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://una.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zie.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lov.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nwf.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvb.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://umg.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nai.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cga.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nob.pengpengdd.cyou

[P04] 求长度
来源：http://vit.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://duw.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://twz.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubf.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://juf.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://pib.fzhhl.top

Go:   len(arr);  len(m)
来源：http://wpm.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://ser.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wzf.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://vnl.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uwc.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dyi.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uzd.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kkw.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yte.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://egn.nanxinkj.top

Ruby: a == b
来源：http://jts.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dgt.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vif.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qzc.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://cik.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aav.mhx1999.top

TS:   if (x == null) {}
来源：http://rtg.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mco.gotoacloud.top

Go:   if x == nil {}
来源：http://bbu.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rlg.andypj.xyz

C#:   if (x is null) {}
来源：http://zzc.yj202588.top

[P07] 防抖与节流
来源：http://aee.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qkc.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://fak.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vel.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yll.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bsi.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sqv.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bcr.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iwm.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://oyn.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hvk.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jpp.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zrk.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ppg.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cic.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wyn.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yja.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://elc.yanxiufei.cn

================================================================================
来源：http://moa.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gnh.ybcxt.top

================================================================================
来源：http://dpj.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://tvx.kuanghao11.cn

CREATE TABLE users (
来源：http://tig.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zib.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://bud.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://kns.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tcz.chenjidiqi.icu

);
来源：http://qfo.havefunace.top

[Q02] 创建带外键的表
来源：http://zwc.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://cow.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kkx.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://vao.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://vpk.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wmq.gotoacloud.top

);
来源：http://xhe.yj202588.top

[Q03] 增加列
来源：http://why.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ujx.gaohongyu789.top

[Q04] 修改列类型
来源：http://mkt.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cug.xuetiantiany.cn

[Q05] 重命名列
来源：http://cxi.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ndc.jiagoushi.top

[Q06] 删除列
来源：http://rfz.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yka.shzxlz.cn

[Q07] 删除表
来源：http://lmx.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://dqq.hywenlv.cn

[Q08] 创建普通索引
来源：http://kta.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fdv.daxiang520.top

[Q09] 创建唯一索引
来源：http://gpy.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jjs.yuanzhike.top

[Q10] 插入单行
来源：http://toc.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tcw.cdnleiting.top

[Q11] 一次插入多行
来源：http://vqn.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kut.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://ahr.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://pbo.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mib.epnwcf.com

[Q13] 忽略重复插入
来源：http://wsw.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nxy.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://kad.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://scp.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ldz.shzxlz.cn

[Q15] 查询全部
来源：http://xcs.zhiwuduotai.top

SELECT * FROM users;
来源：http://rtl.xziqi.cn

[Q16] 查询指定列
来源：http://wdz.yongpay.top

SELECT id, name FROM users;
来源：http://vvs.hongshengwenyu.top

[Q17] 条件查询
来源：http://yvi.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pad.xylfe.cn

[Q18] 模糊匹配
来源：http://krb.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lrj.yj20258888.top

[Q19] 范围查询
来源：http://sck.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ycu.sxryk.cn

[Q20] IN 列表
来源：http://asv.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jdh.yonumen.top

[Q21] 空值判断
来源：http://yzz.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://apf.9152youxi.cn

[Q22] 排序
来源：http://tvo.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xnh.hysaishi.cn

[Q23] 分页
来源：http://ojg.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zbj.hammf.cn

[Q24] 去重
来源：http://sgy.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://zqt.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://diq.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dno.hnxiangtu.top

[Q26] 计数
来源：http://fdd.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://ldu.jinqigufen.top

[Q27] 条件计数
来源：http://caa.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvk.haohaochexian.top

[Q28] 求和与平均
来源：http://xhd.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hoo.jyoumei.cn

[Q29] 最大最小值
来源：http://lkj.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tpx.ybcxt.top

[Q30] 分组统计
来源：http://czj.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pwr.ppjwa.cn

[Q31] 分组后过滤
来源：http://hyd.haohaochexian.top


<!-- 参考信息 -->