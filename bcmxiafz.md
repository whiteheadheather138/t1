代发 wailian999

Ruby: arr.sort
来源：http://jgm.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ihw.sysykeji.top

[N03] 快速排序（分治示例）
来源：http://lwa.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yrl.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://wwl.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqn.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://owe.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jdj.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pqg.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://trw.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://ufu.yj20258.top

[N04] 斐波那契数列
来源：http://rrg.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://umb.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uhy.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wam.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ptm.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fuc.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yig.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://evr.fktsv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hky.shanyushiyangtech.top

[N05] 最大公约数
来源：http://isk.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://snj.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ntf.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://izp.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vdg.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://waj.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ndz.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://onv.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wia.zycfv.cn

[N06] 判断回文字符串
来源：http://bnx.daria6918.cn

Py:   s == s[::-1]
来源：http://hwv.bjfxy.top

PHP:  $s === strrev($s);
来源：http://are.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://asa.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://bgg.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://len.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://jed.bbcook.cn

Ruby: s == s.reverse
来源：http://lye.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ikx.tarul.cn

[N07] 两数之和（返回下标）
来源：http://nun.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ths.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cpt.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kbr.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://tuu.yanxiufei.cn

Java: // 手写 HashMap
来源：http://qid.uphjek.com

Go:   // 手写 map[int]int
来源：http://bic.fktsv.cn

Ruby: // 手写 Hash
来源：http://kzj.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://eyr.chenjidiqi.icu

[N08] 生成全排列
来源：http://ysp.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://pdd.hfpthk.cn

PHP:  // 手写递归交换
来源：http://lqa.hnqzz.top

JS:   // 手写回溯递归
来源：http://wsp.shzxlz.cn

TS:   // 手写回溯递归
来源：http://fkt.andypj.xyz

Java: // 手写回溯递归
来源：http://kiw.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://gjo.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://wiz.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://ape.hywenlv.cn

[N09] 栈与队列
来源：http://pvi.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bei.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rle.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yme.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yfs.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://frh.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://atw.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ros.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://puu.ydzc1.top

[N10] 链表节点定义
来源：http://cmi.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sxu.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pdq.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imt.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://akv.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://oap.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://esr.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cse.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xum.sysykeji.top

[N11] 二叉树中序遍历
来源：http://exg.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jgr.jianghu66.top

PHP:  // 手写递归函数
来源：http://ypw.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yqf.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xci.jinghuilouyu.cn

Java: // 手写递归
来源：http://frs.hcnkem.com

Go:   // 手写递归
来源：http://zqj.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mza.0kj1m.cn

C#:   // 手写递归
来源：http://mti.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gff.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sgi.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ehg.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekv.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dey.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bfp.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lxg.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ehp.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nkh.snrcjt.cn

================================================================================
来源：http://xhq.hongshengwenyu.top

O. 并发与异步
来源：http://oux.pycfn.com

================================================================================
来源：http://kmm.zhengqikj.top

[O01] 启动一个线程
来源：http://mjb.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ihc.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tjb.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dee.sjlbkw.cn

TS:   // 同 JS
来源：http://fzm.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://jil.yj20258888.top

Go:   go f()
来源：http://yzd.yuanzhike.top

Ruby: Thread.new { f }
来源：http://fjy.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://mif.iojbl.cn

[O02] 使用线程池
来源：http://efb.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yvf.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uev.andypj.xyz

JS:   // worker_threads 线程池
来源：http://vxw.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://lad.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tji.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wyv.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://daw.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ehs.jianghu66.top

[O03] 加锁保护共享数据
来源：http://hvw.smart0.xyz

Py:   with lock: shared += 1
来源：http://kob.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://qmh.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rsn.ctjpmb.com

TS:   // 同 JS
来源：http://utf.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://aju.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rxj.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sej.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://ndf.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://ase.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://twr.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rzw.tian-w.cn

JS:   async function f() { await g(); }
来源：http://zcf.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ksr.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syw.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kuw.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://fsy.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://xpv.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://hhd.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://mqy.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vjl.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://dlj.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://xmo.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oaa.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tmc.cucudq.cn

Ruby: threads.map(&:join)
来源：http://dsa.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qfh.hesvh.cn

[O06] 使用进程池
来源：http://jva.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://heb.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yfl.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://tzv.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://zla.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pje.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pjt.chenzaomai.com

Ruby: // fork 块
来源：http://jbt.yuanzhike.top

C#:   Parallel.For
来源：http://znz.havefunace.top

================================================================================
来源：http://req.fanxiaobao.xyz

P. 常用工具函数
来源：http://xic.nanxinkj.top

================================================================================
来源：http://rsr.chenjidiqi.icu

[P01] 生成 UUID
来源：http://nlc.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://wyp.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vai.jianghu66.top

JS:   crypto.randomUUID()
来源：http://zuw.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://pvv.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://imu.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://cmj.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://bqd.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://hoo.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://tau.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mzj.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mmg.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fiq.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xtx.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://plp.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rqz.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sta.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kno.hywenlv.cn

[P03] 生成短随机字符串
来源：http://sec.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gtl.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mfa.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svd.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://opu.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kyd.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bzh.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://czo.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vgf.hywenlv.cn

[P04] 求长度
来源：http://txt.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zml.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://alz.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dhb.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://naf.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://cgp.mhx1999.top

Go:   len(arr);  len(m)
来源：http://lbn.zdbjq.cn

Ruby: x.length;  x.size
来源：http://lsg.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://rbn.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://whl.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sxc.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fov.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://emu.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uqj.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ltb.fehbvm.com

Go:   reflect.DeepEqual(a, b)
来源：http://fex.meibo888.top

Ruby: a == b
来源：http://rvy.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zxn.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mpa.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wvd.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://exu.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hnv.fengsongda.top

TS:   if (x == null) {}
来源：http://gwg.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xzj.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://lbf.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eam.jyoumei.cn

C#:   if (x is null) {}
来源：http://uji.tianlin.xyz

[P07] 防抖与节流
来源：http://mby.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tyi.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://qdf.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://noq.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wvj.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://evx.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tbk.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://tjh.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hxl.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://drk.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ond.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://moa.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://clu.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://evg.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xrh.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ekr.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cyr.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tzz.snrcjt.cn

================================================================================
来源：http://clv.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qpa.andypj.xyz

================================================================================
来源：http://ilj.nanxuanxn.top

[Q01] 创建表
来源：http://avd.hnqzz.top

CREATE TABLE users (
来源：http://mtj.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://miu.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://wep.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://duh.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rbc.quarkkingdee.top

);
来源：http://dci.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://szb.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://vwf.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pfv.yongpay.top

user_id INT NOT NULL,
来源：http://rzi.316326.xyz

amount DECIMAL(10, 2),
来源：http://dne.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://crb.jqgufenzy.top

);
来源：http://cms.jinyuanbaomall.cn

[Q03] 增加列
来源：http://mnu.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hfm.yvedp.cn

[Q04] 修改列类型
来源：http://nus.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qis.yuxming.cn

[Q05] 重命名列
来源：http://dlk.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ngr.dianchejie.cn

[Q06] 删除列
来源：http://fve.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://zli.jinghuilouyu.cn

[Q07] 删除表
来源：http://ecd.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://teb.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://xdf.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gnu.cdnleiting.top

[Q09] 创建唯一索引
来源：http://enq.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zjl.daria6918.cn

[Q10] 插入单行
来源：http://lne.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://haa.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://thr.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tat.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://fcy.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://vmq.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lhu.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://ycp.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mlv.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://zrb.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eay.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nwv.ivvv.top

[Q15] 查询全部
来源：http://yqd.hammf.cn

SELECT * FROM users;
来源：http://jtz.ppjwa.cn

[Q16] 查询指定列
来源：http://kzn.gzhubu.top

SELECT id, name FROM users;
来源：http://ouu.0kj1m.cn

[Q17] 条件查询
来源：http://gov.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rcj.yanxiufei.cn

[Q18] 模糊匹配
来源：http://zwu.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tgk.aibaodan.cn

[Q19] 范围查询
来源：http://vru.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mzh.fehbvm.com

[Q20] IN 列表
来源：http://qjw.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jif.cdnleiting.top

[Q21] 空值判断
来源：http://bdk.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ghe.xuetiantiany.cn

[Q22] 排序
来源：http://ugc.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vfn.hfpthk.cn

[Q23] 分页
来源：http://mkl.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cub.yvedp.cn

[Q24] 去重
来源：http://rgc.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://lku.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://rii.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jfs.zhijiandao.cn

[Q26] 计数
来源：http://orz.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://mcp.fehbvm.com

[Q27] 条件计数
来源：http://byq.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gsk.cashguo.top

[Q28] 求和与平均
来源：http://paq.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vje.pengpengdd.cyou

[Q29] 最大最小值
来源：http://dpv.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://azw.hammf.cn

[Q30] 分组统计
来源：http://chq.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://khy.yuxming.cn

[Q31] 分组后过滤
来源：http://xse.9152youxi.cn


<!-- 参考信息 -->