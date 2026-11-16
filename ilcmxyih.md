代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://rem.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mge.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ohm.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://vnz.yueranfly.top

Ruby: arr.sort
来源：http://cxu.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyy.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://qtc.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jbj.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://uxo.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://raf.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lkb.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xoq.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gep.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ddm.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oyd.yj20258888.top

[N04] 斐波那契数列
来源：http://vda.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mgh.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nuo.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cfs.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npc.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fww.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yzj.smart0.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rxt.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nad.ybcxt.top

[N05] 最大公约数
来源：http://oif.yonumen.top

Py:   math.gcd(a, b)
来源：http://zby.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ppn.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://djf.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ppm.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bow.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hor.hywenlv.cn

Ruby: a.gcd(b)
来源：http://thk.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpa.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://iwn.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://aei.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://vgr.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://vbx.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://drd.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kik.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://fkh.cdnleiting.top

Ruby: s == s.reverse
来源：http://wjb.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cke.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://vte.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gqj.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sfs.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vmp.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://qqn.chenzaomai.com

Java: // 手写 HashMap
来源：http://tne.tanke756.top

Go:   // 手写 map[int]int
来源：http://oql.cdnleiting.top

Ruby: // 手写 Hash
来源：http://sdj.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://vbc.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://mhz.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://cjm.daxiang520.top

PHP:  // 手写递归交换
来源：http://wck.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://fba.yonumen.top

TS:   // 手写回溯递归
来源：http://qwq.xuanzx.com

Java: // 手写回溯递归
来源：http://uxh.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://mse.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://etg.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://rfi.guowangkeji.top

[N09] 栈与队列
来源：http://lrt.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pme.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gwc.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aup.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bhg.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://toy.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wgi.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mds.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jqk.cheryme.top

[N10] 链表节点定义
来源：http://cgp.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yki.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fcs.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mub.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vex.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://bzq.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ioj.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zrk.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://vxt.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://ukl.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wuh.yj202588.top

PHP:  // 手写递归函数
来源：http://fhh.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zon.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlx.hongshengwenyu.top

Java: // 手写递归
来源：http://prx.jiagoushi.top

Go:   // 手写递归
来源：http://ztv.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bec.sweek.top

C#:   // 手写递归
来源：http://gjq.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vdp.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://axa.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pru.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://plx.ppjwa.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fhm.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://weo.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dls.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xvd.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://irw.yfazqb.com

================================================================================
来源：http://wct.xylfe.cn

O. 并发与异步
来源：http://gpi.kuanghao11.cn

================================================================================
来源：http://caw.hywenlv.cn

[O01] 启动一个线程
来源：http://fzi.ydzc1.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dbo.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://snl.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://epl.zhoulong.xyz

TS:   // 同 JS
来源：http://wuc.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://xii.shanyushiyangkeji.top

Go:   go f()
来源：http://ucc.svipenyu.cn

Ruby: Thread.new { f }
来源：http://bje.birdmap.top

C#:   Task.Run(() => F());
来源：http://ece.vqdsnc.cn

[O02] 使用线程池
来源：http://fix.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://duz.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ypt.cashguo.top

JS:   // worker_threads 线程池
来源：http://hvy.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://gfz.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://tqt.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://civ.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mmw.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bhh.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://gku.uphjek.com

Py:   with lock: shared += 1
来源：http://idm.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://phv.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wbd.nanxinkj.top

TS:   // 同 JS
来源：http://klg.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://cmh.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jvg.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ycs.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://hnb.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://wxm.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://hhe.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhl.cucudq.cn

JS:   async function f() { await g(); }
来源：http://zob.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tel.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qve.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qkv.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://vjo.meibo888.top

C#:   async Task F() { await G(); }
来源：http://wby.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://wsm.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://bcc.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ghw.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://sed.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://tyi.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vbc.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iaw.hnqzz.top

Ruby: threads.map(&:join)
来源：http://ndm.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dza.havefunace.top

[O06] 使用进程池
来源：http://bjg.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eol.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kbs.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://uoa.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://hda.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uie.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nwf.yuanzhike.top

Ruby: // fork 块
来源：http://ydf.aizwys.cn

C#:   Parallel.For
来源：http://xgn.sweek.top

================================================================================
来源：http://uhx.zhixingplan.top

P. 常用工具函数
来源：http://jgz.havefunace.top

================================================================================
来源：http://mku.yanxiufei.cn

[P01] 生成 UUID
来源：http://zaq.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://mzo.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pbf.gzhubu.top

JS:   crypto.randomUUID()
来源：http://vkn.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://ywn.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://gzc.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://glv.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://adc.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://chb.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://wmb.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hxy.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://omz.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qmj.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jyf.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kcz.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pwg.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pxi.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mur.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://cqv.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rxs.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vss.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xlw.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upg.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mtg.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wah.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fxm.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zhu.nanxuanxn.top

[P04] 求长度
来源：http://akg.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ffv.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbn.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pvd.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qyx.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://qgk.yuxming.cn

Go:   len(arr);  len(m)
来源：http://hlv.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://bjk.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://woh.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://fft.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://dhw.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kdt.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://taw.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qsl.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://egv.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yaq.shanyushiyangkeji.top

Ruby: a == b
来源：http://efk.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nyr.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vjl.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://spi.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://gxw.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pir.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://vog.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://miz.snrcjt.cn

Go:   if x == nil {}
来源：http://pko.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uya.dashuyun.cn

C#:   if (x is null) {}
来源：http://qtw.nwbrower.top

[P07] 防抖与节流
来源：http://tay.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lkh.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://ffl.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwh.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iro.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lwl.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ubc.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://duu.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zxe.epnwcf.com

[P08] 处理浮点精度问题
来源：http://ofc.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urd.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xtb.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wxy.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oop.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ktb.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kup.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ank.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ayg.hammf.cn

================================================================================
来源：http://ynn.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ohn.gaohongyu789.top

================================================================================
来源：http://qhy.shanyushiyangtech.top

[Q01] 创建表
来源：http://ccc.yanxiufei.cn

CREATE TABLE users (
来源：http://kqh.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://miq.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://tor.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://fyv.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pik.hywenlv.cn

);
来源：http://oek.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://aot.zycfv.cn

CREATE TABLE orders (
来源：http://otz.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://knf.tian-w.cn

user_id INT NOT NULL,
来源：http://ozf.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://khb.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fvt.yanxiufei.cn

);
来源：http://fxh.fengsongda.top

[Q03] 增加列
来源：http://pfc.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vfn.pengpengdd.cyou

[Q04] 修改列类型
来源：http://joa.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ash.sxryk.cn

[Q05] 重命名列
来源：http://puj.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yed.havefunace.top

[Q06] 删除列
来源：http://omf.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://glm.jinghuilouyu.cn

[Q07] 删除表
来源：http://tmt.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://fly.hysaishi.cn

[Q08] 创建普通索引
来源：http://ldv.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yoo.meibo888.top

[Q09] 创建唯一索引
来源：http://uwf.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mgf.uphjek.com

[Q10] 插入单行
来源：http://evz.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rsg.vqdsnc.cn

[Q11] 一次插入多行
来源：http://dlm.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uzd.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://bnc.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://fnc.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cbd.tanke756.top

[Q13] 忽略重复插入
来源：http://rut.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cvk.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://tjk.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iih.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://haz.yvedp.cn

[Q15] 查询全部
来源：http://jvq.sysykeji.top

SELECT * FROM users;
来源：http://bvd.fehbvm.com

[Q16] 查询指定列
来源：http://nao.zhoulong.xyz

SELECT id, name FROM users;
来源：http://upi.meibo888.top

[Q17] 条件查询
来源：http://slq.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ois.sysykeji.top

[Q18] 模糊匹配
来源：http://dlo.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vwd.fengsongda.top

[Q19] 范围查询
来源：http://vap.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kzl.zhijiandao.cn

[Q20] IN 列表
来源：http://gto.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mfj.havefunace.top

[Q21] 空值判断
来源：http://hfd.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ofs.fengsongda.top

[Q22] 排序
来源：http://rrs.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jiy.yueranfly.top

[Q23] 分页
来源：http://ddo.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eck.zhongyouzk.top

[Q24] 去重
来源：http://cfn.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://ajl.iojbl.cn

[Q25] 只取前 N 条
来源：http://cwf.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ooy.gogol.net.cn

[Q26] 计数
来源：http://tpm.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://jky.ctjpmb.com

[Q27] 条件计数
来源：http://lne.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dyg.cheryme.top

[Q28] 求和与平均
来源：http://mxr.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wtf.cashguo.top

[Q29] 最大最小值
来源：http://xhm.uphjek.com


<!-- 参考信息 -->