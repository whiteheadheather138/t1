代发 wailian999

Ruby: arr.sort
来源：http://tbp.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uqy.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://mze.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ugg.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://ufr.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lqc.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kmz.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eza.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mnv.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://axt.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://omm.yj202588.top

[N04] 斐波那契数列
来源：http://vux.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hwi.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bfw.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aab.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mzi.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://alp.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baz.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oro.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kxb.xuetiantiany.cn

[N05] 最大公约数
来源：http://ysb.epnwcf.com

Py:   math.gcd(a, b)
来源：http://qre.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://izx.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgp.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqq.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://egl.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wqw.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://hsr.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://scv.yangfankeji.com

[N06] 判断回文字符串
来源：http://mek.dashuyun.cn

Py:   s == s[::-1]
来源：http://zfz.aizwys.cn

PHP:  $s === strrev($s);
来源：http://tiy.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://frl.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://emd.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rwj.shuidangran.top

Go:   // 双指针从两端比较
来源：http://asn.gaohongyu789.top

Ruby: s == s.reverse
来源：http://wlf.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hyy.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://qpq.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nff.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nfj.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://vyb.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://uoa.yuanzhike.top

Java: // 手写 HashMap
来源：http://hrp.hnqzz.top

Go:   // 手写 map[int]int
来源：http://bzs.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://xfg.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zuk.hammf.cn

[N08] 生成全排列
来源：http://ipy.yonumen.top

Py:   itertools.permutations(arr)
来源：http://rzo.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://wds.cdnleiting.top

JS:   // 手写回溯递归
来源：http://pwb.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://mtl.cdnleiting.top

Java: // 手写回溯递归
来源：http://dni.hesvh.cn

Go:   // 手写回溯递归
来源：http://dww.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://lnm.zycfv.cn

C#:   // 手写回溯递归
来源：http://kry.sufxvd.cn

[N09] 栈与队列
来源：http://xin.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ffv.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jbg.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://epf.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ifl.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jgj.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ybk.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dvx.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zgs.tian-w.cn

[N10] 链表节点定义
来源：http://ppe.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bba.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://vrk.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jfs.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kly.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://psy.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dpb.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://qdc.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bwv.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://hcm.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ikh.wangdashe.top

PHP:  // 手写递归函数
来源：http://kpk.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vzk.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrw.zhengqikj.top

Java: // 手写递归
来源：http://gfn.hesvh.cn

Go:   // 手写递归
来源：http://ywu.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ujg.tian-w.cn

C#:   // 手写递归
来源：http://ptu.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jbr.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lfx.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qbl.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjc.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://amc.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kip.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://spm.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wvs.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iec.gaohongyu789.top

================================================================================
来源：http://lpm.zdbjq.cn

O. 并发与异步
来源：http://kfb.haohaochexian.top

================================================================================
来源：http://fbd.redwolf501.top

[O01] 启动一个线程
来源：http://zos.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vzt.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vem.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qtt.hywenlv.cn

TS:   // 同 JS
来源：http://zun.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://igu.hysaishi.cn

Go:   go f()
来源：http://glj.guowangkeji.top

Ruby: Thread.new { f }
来源：http://aer.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://dkr.dianchejie.cn

[O02] 使用线程池
来源：http://zfb.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hdn.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vjx.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://lre.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://kml.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://tim.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://icj.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ofd.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fct.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://bjk.cashguo.top

Py:   with lock: shared += 1
来源：http://iep.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://ayg.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lxx.svipenyu.cn

TS:   // 同 JS
来源：http://gqn.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://yud.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qcs.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dyt.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://ftm.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://mvf.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://lod.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rxk.hesvh.cn

JS:   async function f() { await g(); }
来源：http://udc.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ihy.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tod.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vom.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://pgq.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://eee.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://coh.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://hcw.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wkn.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://zwz.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://mlk.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uni.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bpd.vehdjk.com

Ruby: threads.map(&:join)
来源：http://gew.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uvy.ybcxt.top

[O06] 使用进程池
来源：http://tze.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ssr.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xvw.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://tyv.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://dmq.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hff.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ohn.chenlongwang.top

Ruby: // fork 块
来源：http://loq.bjfxy.top

C#:   Parallel.For
来源：http://syf.316326.xyz

================================================================================
来源：http://hgz.sweek.top

P. 常用工具函数
来源：http://rwj.9152youxi.cn

================================================================================
来源：http://uwz.shuidangran.top

[P01] 生成 UUID
来源：http://tam.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://mgy.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aum.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://cgk.sysykeji.top

TS:   crypto.randomUUID()
来源：http://cxn.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://eht.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://dxs.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://pdg.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://aop.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://hyj.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dge.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://lbp.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zln.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fvu.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pdm.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://urr.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://krp.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sop.bjfxy.top

[P03] 生成短随机字符串
来源：http://uec.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xxe.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uye.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://afa.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://itj.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gbo.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upp.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ucd.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mgm.aizwys.cn

[P04] 求长度
来源：http://xhs.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qzn.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://swj.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gny.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pxr.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://nam.sweek.top

Go:   len(arr);  len(m)
来源：http://wkx.shzxlz.cn

Ruby: x.length;  x.size
来源：http://lyz.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://nmi.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://xeo.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zzo.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://unv.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://awz.pengpengdd.cyou

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adq.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rge.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tdo.9152youxi.cn

Ruby: a == b
来源：http://obt.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rdj.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cfq.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zlt.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://zov.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ulp.chenzaomai.com

TS:   if (x == null) {}
来源：http://kpp.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cox.ctjpmb.com

Go:   if x == nil {}
来源：http://mbb.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qoo.hesvh.cn

C#:   if (x is null) {}
来源：http://dah.yonumen.top

[P07] 防抖与节流
来源：http://bco.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qpp.tarul.cn

PHP:  // 手写时间戳比较
来源：http://zzp.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nyj.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pdn.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gti.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jjv.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://cgi.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ldo.havefunace.top

[P08] 处理浮点精度问题
来源：http://hdk.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pqu.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ppk.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rlo.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dlr.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dwb.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gqd.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wlw.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ann.yuanzhike.top

================================================================================
来源：http://vsw.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aew.zdqjudy.top

================================================================================
来源：http://ugp.jqgfzy.top

[Q01] 创建表
来源：http://etg.xziqi.cn

CREATE TABLE users (
来源：http://rjm.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyu.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://wfc.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://kov.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://anc.vqdsnc.cn

);
来源：http://fcw.cucudq.cn

[Q02] 创建带外键的表
来源：http://rpi.tianlin.xyz

CREATE TABLE orders (
来源：http://xvk.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqo.vqdsnc.cn

user_id INT NOT NULL,
来源：http://nus.xinyue.icu

amount DECIMAL(10, 2),
来源：http://cin.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ail.sxryk.cn

);
来源：http://dtz.smart0.xyz

[Q03] 增加列
来源：http://dwb.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pih.sjlbkw.cn

[Q04] 修改列类型
来源：http://ahb.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yso.yj202588.top

[Q05] 重命名列
来源：http://hof.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zhh.sufxvd.cn

[Q06] 删除列
来源：http://zgk.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://jlp.zhongyouzk.top

[Q07] 删除表
来源：http://llg.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://bmd.birdmap.top

[Q08] 创建普通索引
来源：http://udx.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ykj.zdqjudy.top

[Q09] 创建唯一索引
来源：http://qlz.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rca.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://fiu.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pss.snrcjt.cn

[Q11] 一次插入多行
来源：http://eew.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ixd.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://rhm.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://afq.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://erh.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://ppo.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rks.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://ibt.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dzs.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zfc.quarkkingdee.top

[Q15] 查询全部
来源：http://kla.nwbrower.top

SELECT * FROM users;
来源：http://atx.hongshengwenyu.top

[Q16] 查询指定列
来源：http://yzi.zhoulong.xyz

SELECT id, name FROM users;
来源：http://sbn.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://zxo.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ojp.gaohongyu789.top

[Q18] 模糊匹配
来源：http://kpc.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xtd.nanxuanxn.top

[Q19] 范围查询
来源：http://rcn.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rtp.iojbl.cn

[Q20] IN 列表
来源：http://vwr.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ojc.zhoulong.xyz

[Q21] 空值判断
来源：http://oss.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tew.hfpthk.cn

[Q22] 排序
来源：http://cds.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dcy.zhiwuduotai.top

[Q23] 分页
来源：http://vty.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsn.0kj1m.cn

[Q24] 去重
来源：http://jby.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://mks.52xcode.cn

[Q25] 只取前 N 条
来源：http://abb.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://agv.fanxiaobao.xyz

[Q26] 计数
来源：http://phc.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://zay.xinyue.icu

[Q27] 条件计数
来源：http://kvj.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://igh.daxiang520.top

[Q28] 求和与平均
来源：http://xcw.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://joi.chenjidiqi.icu

[Q29] 最大最小值
来源：http://quy.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhk.aibaodan.cn

[Q30] 分组统计
来源：http://aqt.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xco.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://wmc.xinyue.icu


<!-- 参考信息 -->