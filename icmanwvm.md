代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://njt.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://guz.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ybb.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yil.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lzo.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://icq.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rer.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://ufw.yj202588.top

Ruby: arr.sort
来源：http://mtc.haohaochexian.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukr.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://net.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yuo.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://eim.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qda.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gyv.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mam.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xnr.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kqd.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://twq.pycfn.com

[N04] 斐波那契数列
来源：http://ang.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vos.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qqa.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ldv.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hvx.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rwg.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qli.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://prd.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yzo.feifeiyinyue.top

[N05] 最大公约数
来源：http://gqu.yuxming.cn

Py:   math.gcd(a, b)
来源：http://fag.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://inp.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bfc.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szv.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lcj.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://byl.yj20258888.top

Ruby: a.gcd(b)
来源：http://ifn.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hgi.zhixingplan.top

[N06] 判断回文字符串
来源：http://ipa.yj202588.top

Py:   s == s[::-1]
来源：http://qnn.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://rgk.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://mmt.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://ynq.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zwv.mhx1999.top

Go:   // 双指针从两端比较
来源：http://ciz.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://cht.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://roo.316326.xyz

[N07] 两数之和（返回下标）
来源：http://fbh.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mwy.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://spy.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tuq.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://lgb.quarkkingdee.top

Java: // 手写 HashMap
来源：http://klr.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://iai.tanke756.top

Ruby: // 手写 Hash
来源：http://chs.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ffc.gaohongyu789.top

[N08] 生成全排列
来源：http://kcb.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://zbs.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://ayi.gogol.net.cn

JS:   // 手写回溯递归
来源：http://mhy.cqqwz.cn

TS:   // 手写回溯递归
来源：http://ipu.aibaodan.cn

Java: // 手写回溯递归
来源：http://age.jyoumei.cn

Go:   // 手写回溯递归
来源：http://sce.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://ixj.xuanzx.com

C#:   // 手写回溯递归
来源：http://ubx.zycfv.cn

[N09] 栈与队列
来源：http://rkv.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eqa.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qbb.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ewl.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ilb.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zpi.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://giw.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fjp.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bad.jinqigfzy.top

[N10] 链表节点定义
来源：http://dza.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jsy.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hxa.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://keb.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oyh.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://emf.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ruf.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://prg.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://owx.fehbvm.com

[N11] 二叉树中序遍历
来源：http://rbr.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uxr.zycfv.cn

PHP:  // 手写递归函数
来源：http://mqc.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwc.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ejj.hfpthk.cn

Java: // 手写递归
来源：http://lkq.fzhhl.top

Go:   // 手写递归
来源：http://vip.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nqr.havefunace.top

C#:   // 手写递归
来源：http://hfm.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cix.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://swa.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://paf.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gvg.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjd.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lqi.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uom.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vrf.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ycl.gzhubu.top

================================================================================
来源：http://sgr.nanxuanxn.top

O. 并发与异步
来源：http://tdv.iojbl.cn

================================================================================
来源：http://zfu.xuetiantiany.cn

[O01] 启动一个线程
来源：http://zai.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjm.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ohx.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gyr.yuxming.cn

TS:   // 同 JS
来源：http://rvl.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://wjy.shanyushiyangtech.top

Go:   go f()
来源：http://rkz.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://pvn.hammf.cn

C#:   Task.Run(() => F());
来源：http://hno.jianghu66.top

[O02] 使用线程池
来源：http://ksc.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rtf.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wgn.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://swi.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://jzj.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://xup.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://adx.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sal.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://goi.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://vjp.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://akt.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://gxl.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oum.shangyingyoupin.top

TS:   // 同 JS
来源：http://jxa.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://fbv.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ksn.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xao.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://qbn.xylfe.cn

[O04] 定义异步函数并等待
来源：http://kkn.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://kna.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dym.cucudq.cn

JS:   async function f() { await g(); }
来源：http://dnh.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zzi.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vkl.redwolf501.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://laq.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lyr.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://zxr.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://bxt.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://pdo.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vdt.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://fna.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://axp.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ikp.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://egc.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://exj.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rjz.guowangkeji.top

[O06] 使用进程池
来源：http://tvd.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dbi.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://gku.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://lnc.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://atr.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cqm.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lhr.jlsjyb.cn

Ruby: // fork 块
来源：http://igp.hongshengwenyu.top

C#:   Parallel.For
来源：http://oih.jqgufenzy.top

================================================================================
来源：http://lsg.nanxinkj.top

P. 常用工具函数
来源：http://nuu.meibo888.top

================================================================================
来源：http://nag.jqgfzy.top

[P01] 生成 UUID
来源：http://nyx.pycfn.com

Py:   str(uuid.uuid4())
来源：http://hss.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://odo.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://gkg.yj20258.top

TS:   crypto.randomUUID()
来源：http://xpj.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://otj.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://gti.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://szu.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://mpw.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://lsl.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iem.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kzc.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pro.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qvj.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fcu.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lsh.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bfk.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tjm.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://tiy.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cer.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zen.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ing.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gux.ppjwa.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lit.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pqm.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qdk.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vpe.zhoulong.xyz

[P04] 求长度
来源：http://ltc.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xaj.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgv.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wen.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hrb.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://zsy.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://cqt.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://ana.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ird.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://frv.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qjd.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hig.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hin.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ful.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kek.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rxg.cashguo.top

Ruby: a == b
来源：http://vsd.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ckm.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ysi.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://icv.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://dfm.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ezc.daria6918.cn

TS:   if (x == null) {}
来源：http://ubo.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ijs.0kj1m.cn

Go:   if x == nil {}
来源：http://mcr.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sls.hnqzz.top

C#:   if (x is null) {}
来源：http://tkk.guannengcc.top

[P07] 防抖与节流
来源：http://inf.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hvj.vqdsnc.cn

PHP:  // 手写时间戳比较
来源：http://ojk.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxg.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nvw.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oky.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dti.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wki.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kam.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://san.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://slc.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iba.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xwx.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hnq.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://spj.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ouj.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tei.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vbw.xuetiantiany.cn

================================================================================
来源：http://ven.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mzk.yj20258888.top

================================================================================
来源：http://ipn.sjlbkw.cn

[Q01] 创建表
来源：http://fvp.birdmap.top

CREATE TABLE users (
来源：http://xbv.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bor.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://vil.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://dgw.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ujc.ehwqpu.com

);
来源：http://sdd.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://kye.ctjpmb.com

CREATE TABLE orders (
来源：http://rcd.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://niw.xuanzx.com

user_id INT NOT NULL,
来源：http://tha.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://vmn.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qkj.sxryk.cn

);
来源：http://gds.gzhubu.top

[Q03] 增加列
来源：http://xrl.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hpr.wangdashe.top

[Q04] 修改列类型
来源：http://bhb.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hrm.xuetiantiany.cn

[Q05] 重命名列
来源：http://wtj.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yye.9152youxi.cn

[Q06] 删除列
来源：http://ges.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://oor.jinqigfzy.top

[Q07] 删除表
来源：http://nlw.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://dta.yfazqb.com

[Q08] 创建普通索引
来源：http://uib.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jsk.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://pme.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mzg.gogol.net.cn

[Q10] 插入单行
来源：http://fow.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zzi.gogol.net.cn

[Q11] 一次插入多行
来源：http://mry.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rmc.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://raa.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://miw.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zek.hesvh.cn

[Q13] 忽略重复插入
来源：http://kta.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cpy.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://pel.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zbs.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qih.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://fwt.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://ave.shzxlz.cn

[Q16] 查询指定列
来源：http://thd.ctjpmb.com

SELECT id, name FROM users;
来源：http://xby.jinqigfzy.top

[Q17] 条件查询
来源：http://nbz.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mzq.jinqigfzy.top

[Q18] 模糊匹配
来源：http://jwx.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://haq.yj20258888.top

[Q19] 范围查询
来源：http://bhb.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mpj.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://gnn.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fyn.jinghuilouyu.cn

[Q21] 空值判断
来源：http://nsl.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://lqn.ppjwa.cn

[Q22] 排序
来源：http://zre.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fth.yanxiufei.cn

[Q23] 分页
来源：http://acl.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dzo.fengsongda.top

[Q24] 去重
来源：http://flx.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://ogs.chenzaomai.com

[Q25] 只取前 N 条
来源：http://ran.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qho.birdmap.top

[Q26] 计数
来源：http://mdv.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://mdf.dianchejie.cn

[Q27] 条件计数
来源：http://abd.svipenyu.cn


<!-- 参考信息 -->