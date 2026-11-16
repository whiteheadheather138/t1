代发 wailian999

Ruby: arr.sort
来源：http://fbm.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://buc.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://shz.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vzg.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://qft.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://twr.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dno.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kxe.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dou.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lfq.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://ias.meibo888.top

[N04] 斐波那契数列
来源：http://esv.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pxw.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://waa.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nqs.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nqm.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pxg.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gkg.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gzs.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oij.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://bop.cheryme.top

Py:   math.gcd(a, b)
来源：http://wby.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tid.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nav.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogr.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://snc.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cde.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://knb.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mjl.zhoulong.xyz

[N06] 判断回文字符串
来源：http://mow.redwolf501.top

Py:   s == s[::-1]
来源：http://ufw.tian-w.cn

PHP:  $s === strrev($s);
来源：http://shm.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://dsb.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://pot.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tah.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://ouj.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://coh.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://npf.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://crc.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ahk.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zgv.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mqy.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://qfy.meibo888.top

Java: // 手写 HashMap
来源：http://bjp.daxiang520.top

Go:   // 手写 map[int]int
来源：http://qir.birdmap.top

Ruby: // 手写 Hash
来源：http://ovk.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://yuv.aibaodan.cn

[N08] 生成全排列
来源：http://jtg.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://pmw.nanxinkj.top

PHP:  // 手写递归交换
来源：http://hes.fktsv.cn

JS:   // 手写回溯递归
来源：http://uis.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://rfv.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://hsm.yongpay.top

Go:   // 手写回溯递归
来源：http://fji.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://zhv.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://ruq.kuanghao11.cn

[N09] 栈与队列
来源：http://qfj.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fbs.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://prx.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eed.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yqw.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pqr.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jkv.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kpo.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qgp.snrcjt.cn

[N10] 链表节点定义
来源：http://kdr.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xqv.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://rmo.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hdx.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://goe.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://rjx.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://wqc.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hsv.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tns.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://avn.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jta.iojbl.cn

PHP:  // 手写递归函数
来源：http://vua.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tzg.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihu.quarkkingdee.top

Java: // 手写递归
来源：http://xon.andypj.xyz

Go:   // 手写递归
来源：http://qqv.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jnx.sxryk.cn

C#:   // 手写递归
来源：http://bwc.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rot.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mhj.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hnc.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://taq.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ipt.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ghz.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xqy.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hyq.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jqy.pycfn.com

================================================================================
来源：http://gba.52xcode.cn

O. 并发与异步
来源：http://wjn.hnxiangtu.top

================================================================================
来源：http://fjg.jlsjyb.cn

[O01] 启动一个线程
来源：http://gml.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jqa.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rhx.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oav.bjfxy.top

TS:   // 同 JS
来源：http://juq.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://wne.xuetiantiany.cn

Go:   go f()
来源：http://ksw.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://kkn.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://zgd.hnxiangtu.top

[O02] 使用线程池
来源：http://osd.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zfc.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://juw.smart0.xyz

JS:   // worker_threads 线程池
来源：http://awn.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://ine.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://yko.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fuy.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oro.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ohy.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://azj.smart0.xyz

Py:   with lock: shared += 1
来源：http://lrb.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://xvt.dianchejie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lbi.cucudq.cn

TS:   // 同 JS
来源：http://jen.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://yww.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fun.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://npi.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://nmw.wangdashe.top

[O04] 定义异步函数并等待
来源：http://feq.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://vwu.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bmo.yvedp.cn

JS:   async function f() { await g(); }
来源：http://nks.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://kdv.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tqf.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fvi.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://vgv.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://bjx.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://ljs.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://asn.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sns.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://goo.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://lqr.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://maf.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gzc.jianghu66.top

Ruby: threads.map(&:join)
来源：http://mrw.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hwp.dashuyun.cn

[O06] 使用进程池
来源：http://mnc.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eqy.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xtx.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://gim.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://lyw.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vtm.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ixd.bjfxy.top

Ruby: // fork 块
来源：http://chp.yfazqb.com

C#:   Parallel.For
来源：http://jmd.aibaodan.cn

================================================================================
来源：http://qwz.xinyue.icu

P. 常用工具函数
来源：http://mzv.mhx1999.top

================================================================================
来源：http://wyy.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://vps.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://vuz.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://omm.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://ukl.yvedp.cn

TS:   crypto.randomUUID()
来源：http://brw.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://aud.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://dpw.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://xpv.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://guh.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://bhg.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://agf.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://tgn.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bjp.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fud.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://olw.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mow.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ilf.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lnn.tanke756.top

[P03] 生成短随机字符串
来源：http://fgy.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aqz.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://swu.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chr.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nei.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ilh.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xne.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qzg.cqqwz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://weq.ydzc1.top

[P04] 求长度
来源：http://hag.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uid.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gsb.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vci.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cws.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://jrf.sxryk.cn

Go:   len(arr);  len(m)
来源：http://ija.hesvh.cn

Ruby: x.length;  x.size
来源：http://jjr.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://swd.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://bas.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wov.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ihk.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gyb.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lnj.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jbs.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://ggo.shuidangran.top

Ruby: a == b
来源：http://vid.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zwc.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://glp.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vib.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://itc.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gah.daxiang520.top

TS:   if (x == null) {}
来源：http://npr.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hup.hesvh.cn

Go:   if x == nil {}
来源：http://bmp.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cqd.jlsjyb.cn

C#:   if (x is null) {}
来源：http://mbx.cucudq.cn

[P07] 防抖与节流
来源：http://pnj.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hdu.jinghuilouyu.cn

PHP:  // 手写时间戳比较
来源：http://jcm.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bsz.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwy.fzhhl.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bza.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nmu.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://pzw.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kmz.wangdashe.top

[P08] 处理浮点精度问题
来源：http://aqd.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://djw.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ysf.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ioq.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nce.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wut.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fyq.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dfh.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cns.xziqi.cn

================================================================================
来源：http://awy.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://izl.hammf.cn

================================================================================
来源：http://vhg.yonumen.top

[Q01] 创建表
来源：http://mvk.jinghuilouyu.cn

CREATE TABLE users (
来源：http://qyt.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://grq.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://pix.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://jxz.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vjq.shanyushiyangtech.top

);
来源：http://nkt.ivvv.top

[Q02] 创建带外键的表
来源：http://zjr.zhijiandao.cn

CREATE TABLE orders (
来源：http://vyy.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uku.aizwys.cn

user_id INT NOT NULL,
来源：http://wcz.yvedp.cn

amount DECIMAL(10, 2),
来源：http://qrt.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jkr.epnwcf.com

);
来源：http://ffi.svipenyu.cn

[Q03] 增加列
来源：http://mgr.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tph.zhengqikj.top

[Q04] 修改列类型
来源：http://dos.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hxs.gogol.net.cn

[Q05] 重命名列
来源：http://bmf.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ghk.zhoulong.xyz

[Q06] 删除列
来源：http://ogg.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://hlv.sxryk.cn

[Q07] 删除表
来源：http://avm.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://axz.jyoumei.cn

[Q08] 创建普通索引
来源：http://jmi.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nun.andypj.xyz

[Q09] 创建唯一索引
来源：http://lxj.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wqf.ydjk.org.cn

[Q10] 插入单行
来源：http://zub.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://npi.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://boi.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eam.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://cki.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://bjp.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vxx.dianchejie.cn

[Q13] 忽略重复插入
来源：http://ilf.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://whv.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://fic.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kmm.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pfs.tarul.cn

[Q15] 查询全部
来源：http://ogp.hywenlv.cn

SELECT * FROM users;
来源：http://iog.ydzc1.top

[Q16] 查询指定列
来源：http://dtq.tanke756.top

SELECT id, name FROM users;
来源：http://voq.jinqigufen.top

[Q17] 条件查询
来源：http://boq.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tra.tarul.cn

[Q18] 模糊匹配
来源：http://dae.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yml.jqgufenzy.top

[Q19] 范围查询
来源：http://fzx.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oni.andypj.xyz

[Q20] IN 列表
来源：http://tta.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bzp.c1oappe.top

[Q21] 空值判断
来源：http://aco.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lpy.yongpay.top

[Q22] 排序
来源：http://ljs.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bip.yuxming.cn

[Q23] 分页
来源：http://vdz.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mvc.jianghu66.top

[Q24] 去重
来源：http://pyc.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://wzc.iojbl.cn

[Q25] 只取前 N 条
来源：http://knm.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://adg.wangshuangyany.cn

[Q26] 计数
来源：http://dth.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://wfg.nanxinkj.top

[Q27] 条件计数
来源：http://rqn.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qvy.pycfn.com

[Q28] 求和与平均
来源：http://gtq.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ryy.haohaochexian.top

[Q29] 最大最小值
来源：http://kts.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nck.yj202588.top

[Q30] 分组统计
来源：http://jzn.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zob.aibaodan.cn

[Q31] 分组后过滤
来源：http://bjg.ydjk.org.cn


<!-- 参考信息 -->