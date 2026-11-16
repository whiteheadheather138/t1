代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://kyf.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xmu.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sjp.fzhhl.top

Go:   slices.Sort(arr)
来源：http://igd.cqqwz.cn

Ruby: arr.sort
来源：http://var.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kge.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://fqz.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jaq.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://fvp.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ixw.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xhn.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pdp.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jya.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aiq.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dvu.nanxinkj.top

[N04] 斐波那契数列
来源：http://njj.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vgr.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aam.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://skr.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://olb.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vob.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lxg.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cxg.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lrt.jqgufenzy.top

[N05] 最大公约数
来源：http://yqr.yj20258888.top

Py:   math.gcd(a, b)
来源：http://ody.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qut.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gue.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zdm.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tsi.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kye.ctjpmb.com

Ruby: a.gcd(b)
来源：http://wnn.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gxh.9152youxi.cn

[N06] 判断回文字符串
来源：http://pcm.yanxiufei.cn

Py:   s == s[::-1]
来源：http://age.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://uar.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://jqh.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://pae.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ldi.yfazqb.com

Go:   // 双指针从两端比较
来源：http://dyz.zhongyouzk.top

Ruby: s == s.reverse
来源：http://hql.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ezp.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://gfl.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pjf.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ufe.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qvx.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://bvf.quarkkingdee.top

Java: // 手写 HashMap
来源：http://jxn.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://ofh.sxryk.cn

Ruby: // 手写 Hash
来源：http://dzc.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jot.52xcode.cn

[N08] 生成全排列
来源：http://ahb.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://lya.c1oappe.top

PHP:  // 手写递归交换
来源：http://svs.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://tcd.iojbl.cn

TS:   // 手写回溯递归
来源：http://fwy.kuanghao11.cn

Java: // 手写回溯递归
来源：http://ssk.hysaishi.cn

Go:   // 手写回溯递归
来源：http://hli.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://jkt.c1oappe.top

C#:   // 手写回溯递归
来源：http://nzt.jlsjyb.cn

[N09] 栈与队列
来源：http://wzs.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zdu.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vhi.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yqz.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xte.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://asw.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vkl.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ypi.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ted.0kj1m.cn

[N10] 链表节点定义
来源：http://hmg.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wul.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uom.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lpv.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sku.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://ovp.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://vfk.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uhe.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wrz.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://hne.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vkb.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://env.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbt.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://neu.gotoacloud.top

Java: // 手写递归
来源：http://ndn.fengsongda.top

Go:   // 手写递归
来源：http://wjx.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ggq.ivvv.top

C#:   // 手写递归
来源：http://ool.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tuc.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://myn.pengpengdd.cyou

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iuv.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dta.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzm.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ziz.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cun.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xll.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wuk.tanke756.top

================================================================================
来源：http://wyh.dashuyun.cn

O. 并发与异步
来源：http://ced.zycfv.cn

================================================================================
来源：http://dru.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://kwf.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fze.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://abz.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bpd.yj202588.top

TS:   // 同 JS
来源：http://eyf.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://yqr.guowangkeji.top

Go:   go f()
来源：http://bsw.nwbrower.top

Ruby: Thread.new { f }
来源：http://wjk.pengpengdd.cyou

C#:   Task.Run(() => F());
来源：http://vve.wangdashe.top

[O02] 使用线程池
来源：http://mrr.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rrk.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mvo.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://qsz.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://dov.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://jlg.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vkw.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fzm.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uig.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://ypu.bbcook.cn

Py:   with lock: shared += 1
来源：http://epk.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://ckq.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ihx.yuanzhike.top

TS:   // 同 JS
来源：http://mhh.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://cqy.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://saf.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://afh.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://oxc.yueranfly.top

[O04] 定义异步函数并等待
来源：http://gvo.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://yed.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ivy.xylfe.cn

JS:   async function f() { await g(); }
来源：http://xau.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://qzb.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dzo.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vey.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jfk.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://lci.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://evl.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://qjo.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aya.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://vxx.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://nzm.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vva.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rlt.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://pxc.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://suk.cheryme.top

[O06] 使用进程池
来源：http://aav.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xrw.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gio.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://qal.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://eqg.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://frg.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ddx.jiagoushi.top

Ruby: // fork 块
来源：http://exx.ybcxt.top

C#:   Parallel.For
来源：http://jdx.nanxinkj.top

================================================================================
来源：http://xgj.zdqjudy.top

P. 常用工具函数
来源：http://rot.shzxlz.cn

================================================================================
来源：http://kec.bjfxy.top

[P01] 生成 UUID
来源：http://pqz.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://hrw.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zro.xinyue.icu

JS:   crypto.randomUUID()
来源：http://uvj.yj20258888.top

TS:   crypto.randomUUID()
来源：http://lmo.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://xbl.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://vnm.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://gfo.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://vbn.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://eej.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://upw.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vai.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wjl.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cxl.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wqa.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zxb.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ymt.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fxn.guowangkeji.top

[P03] 生成短随机字符串
来源：http://mco.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cyy.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://htv.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jti.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyp.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tmu.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ofp.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://sfj.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://srs.hysaishi.cn

[P04] 求长度
来源：http://qps.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nvg.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qwa.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vyu.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nyl.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://yjs.smart0.xyz

Go:   len(arr);  len(m)
来源：http://wtk.sweek.top

Ruby: x.length;  x.size
来源：http://hbz.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://vdg.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://mhu.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kem.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://apb.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ucx.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xhw.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nbg.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://mkq.jqgfzy.top

Ruby: a == b
来源：http://iuw.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zwb.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tjp.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cqx.tanke756.top

PHP:  if (empty($x)) {}
来源：http://mob.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hhh.zhongyouzk.top

TS:   if (x == null) {}
来源：http://rmb.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vbg.quarkkingdee.top

Go:   if x == nil {}
来源：http://qyt.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://llq.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://rwh.ydzc1.top

[P07] 防抖与节流
来源：http://tpj.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bur.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://jem.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyr.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://die.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dsv.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bqs.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://awp.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://map.birdmap.top

[P08] 处理浮点精度问题
来源：http://hdh.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://euf.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lag.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://flp.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jox.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bcc.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ilf.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ilu.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gyt.gotoacloud.top

================================================================================
来源：http://wzw.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://phc.xylfe.cn

================================================================================
来源：http://akp.fengsongda.top

[Q01] 创建表
来源：http://mzv.yj20258888.top

CREATE TABLE users (
来源：http://cic.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://byq.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://fhc.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://sxj.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vro.quarkkingdee.top

);
来源：http://wpi.fengsongda.top

[Q02] 创建带外键的表
来源：http://nnw.zhoulong.xyz

CREATE TABLE orders (
来源：http://kpj.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lyz.yvedp.cn

user_id INT NOT NULL,
来源：http://yoy.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://bnp.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://foi.ppjwa.cn

);
来源：http://obg.haohaochexian.top

[Q03] 增加列
来源：http://phk.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dbe.jqgfzy.top

[Q04] 修改列类型
来源：http://dex.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jgn.pycfn.com

[Q05] 重命名列
来源：http://eyy.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cdd.nanxinkj.top

[Q06] 删除列
来源：http://qgf.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://owb.ivvv.top

[Q07] 删除表
来源：http://zae.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://ymt.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://evz.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kdn.9152youxi.cn

[Q09] 创建唯一索引
来源：http://bqt.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://msy.0kj1m.cn

[Q10] 插入单行
来源：http://dem.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blu.nwbrower.top

[Q11] 一次插入多行
来源：http://jty.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dtv.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://bkx.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ekq.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://waw.9152youxi.cn

[Q13] 忽略重复插入
来源：http://msf.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pnr.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://ych.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hur.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://woc.quarkkingdee.top

[Q15] 查询全部
来源：http://vgt.pengpengdd.cyou

SELECT * FROM users;
来源：http://tiu.sysykeji.top

[Q16] 查询指定列
来源：http://xmm.yongpay.top

SELECT id, name FROM users;
来源：http://vuy.cashguo.top

[Q17] 条件查询
来源：http://zjx.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fnq.wangdashe.top

[Q18] 模糊匹配
来源：http://vay.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ska.hnxiangtu.top

[Q19] 范围查询
来源：http://vws.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pvg.cucudq.cn

[Q20] IN 列表
来源：http://kel.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uto.jinqigfzy.top

[Q21] 空值判断
来源：http://qyz.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mgz.vehdjk.com

[Q22] 排序
来源：http://hfu.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vsb.pycfn.com

[Q23] 分页
来源：http://ema.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://moj.316326.xyz

[Q24] 去重
来源：http://ofr.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://roe.ctjpmb.com

[Q25] 只取前 N 条
来源：http://tlp.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eze.vehdjk.com

[Q26] 计数
来源：http://pml.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://vkc.ybcxt.top

[Q27] 条件计数
来源：http://ehy.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rbr.hywenlv.cn

[Q28] 求和与平均
来源：http://xuh.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ccn.daxiang520.top

[Q29] 最大最小值
来源：http://mfn.aizwys.cn


<!-- 参考信息 -->