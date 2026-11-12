代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://vhd.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xah.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jmy.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://vyz.jlsjyb.cn

Ruby: arr.sort
来源：http://hhj.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dod.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://zda.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ctn.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://lto.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxh.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vsc.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xoo.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://udj.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fcw.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://ibx.pycfn.com

[N04] 斐波那契数列
来源：http://rju.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jft.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xbe.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://icf.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uel.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sdm.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mip.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vjp.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ofn.mhx1999.top

[N05] 最大公约数
来源：http://cvh.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://vmc.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yoi.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://udr.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ymm.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eey.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://usl.jiagoushi.top

Ruby: a.gcd(b)
来源：http://tag.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dhh.epnwcf.com

[N06] 判断回文字符串
来源：http://whz.sysykeji.top

Py:   s == s[::-1]
来源：http://sld.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://sgt.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://ilf.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://rwf.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sqz.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://ftc.jqgfzy.top

Ruby: s == s.reverse
来源：http://rgh.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yhk.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://ppj.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uoh.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uuh.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gaj.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://wvv.zdqjudy.top

Java: // 手写 HashMap
来源：http://zdu.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://cxk.tanke756.top

Ruby: // 手写 Hash
来源：http://gsy.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rwa.guannengcc.top

[N08] 生成全排列
来源：http://ygp.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://hid.ydjk.org.cn

PHP:  // 手写递归交换
来源：http://nrv.fehbvm.com

JS:   // 手写回溯递归
来源：http://cmm.xuanzx.com

TS:   // 手写回溯递归
来源：http://ymv.fehbvm.com

Java: // 手写回溯递归
来源：http://gui.sufxvd.cn

Go:   // 手写回溯递归
来源：http://hgp.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://lqk.snrcjt.cn

C#:   // 手写回溯递归
来源：http://orz.zhijiandao.cn

[N09] 栈与队列
来源：http://idx.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qjy.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aql.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iel.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bsu.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eba.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://you.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ckf.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ehb.sjlbkw.cn

[N10] 链表节点定义
来源：http://wmv.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zhi.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eaw.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://paf.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hfh.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://icg.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://czh.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rni.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fck.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://ywc.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wbj.yvedp.cn

PHP:  // 手写递归函数
来源：http://kpf.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kmn.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fux.aibaodan.cn

Java: // 手写递归
来源：http://rqz.ydjk.org.cn

Go:   // 手写递归
来源：http://xdd.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ouo.zhengqikj.top

C#:   // 手写递归
来源：http://sou.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://caz.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vfu.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cem.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ced.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://njf.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rws.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jxv.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nec.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nez.pycfn.com

================================================================================
来源：http://ebs.cucudq.cn

O. 并发与异步
来源：http://xtm.wangshuangyany.cn

================================================================================
来源：http://cdz.daria6918.cn

[O01] 启动一个线程
来源：http://gcp.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://osv.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kaz.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wum.hesvh.cn

TS:   // 同 JS
来源：http://oxa.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://ebv.fengsongda.top

Go:   go f()
来源：http://lls.xziqi.cn

Ruby: Thread.new { f }
来源：http://iye.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://ewd.ydjk.org.cn

[O02] 使用线程池
来源：http://kdp.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tvl.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ypv.tanke756.top

JS:   // worker_threads 线程池
来源：http://fck.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://ksk.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nkg.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mzj.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wdc.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hly.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://dqc.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://hey.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://hxs.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hhu.xinyue.icu

TS:   // 同 JS
来源：http://lrf.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://hpq.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kvw.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hqg.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://ljc.iojbl.cn

[O04] 定义异步函数并等待
来源：http://jra.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://vrj.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oyp.xuanzx.com

JS:   async function f() { await g(); }
来源：http://hes.zdqjudy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zph.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ijd.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://atf.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vjc.birdmap.top

C#:   async Task F() { await G(); }
来源：http://qzf.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://lma.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://sey.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://see.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://mfa.yj202588.top

TS:   await Promise.all(tasks)
来源：http://yws.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fwf.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wlj.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://ign.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://slg.zhoulong.xyz

[O06] 使用进程池
来源：http://tol.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vnn.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://agy.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://cpz.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://afq.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nrm.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ucw.chenzaomai.com

Ruby: // fork 块
来源：http://nsl.snrcjt.cn

C#:   Parallel.For
来源：http://xzf.yuxming.cn

================================================================================
来源：http://qoc.zhoulong.xyz

P. 常用工具函数
来源：http://que.c1oappe.top

================================================================================
来源：http://fri.xziqi.cn

[P01] 生成 UUID
来源：http://cak.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://jah.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://obu.wangdashe.top

JS:   crypto.randomUUID()
来源：http://pku.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://ktp.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://gmx.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://ddm.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://lnj.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://gqf.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://vwz.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zlk.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rnk.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mgo.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ohp.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bsn.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qkd.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eup.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vsn.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://ybq.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qtz.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qyf.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uba.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xeu.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jil.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mcv.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://rwu.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uzx.feifeiyinyue.top

[P04] 求长度
来源：http://skm.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hrl.havefunace.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rgr.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jmr.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dpt.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://jpc.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://itz.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://ujo.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xrm.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://olk.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cka.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hiz.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wpb.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pua.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eju.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://cah.zhaomingkeji.xyz

Ruby: a == b
来源：http://fhj.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dye.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uov.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zaz.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://qhk.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tyf.shzxlz.cn

TS:   if (x == null) {}
来源：http://qha.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ynq.aizwys.cn

Go:   if x == nil {}
来源：http://fct.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tta.jlsjyb.cn

C#:   if (x is null) {}
来源：http://ebp.birdmap.top

[P07] 防抖与节流
来源：http://vye.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://trt.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://ykm.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kmg.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bzy.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wcp.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jxt.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rtw.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vdc.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://ssg.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cnw.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mst.guowangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jlv.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hlu.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yik.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xwq.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sha.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://krp.quarkkingdee.top

================================================================================
来源：http://tnu.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fhg.yj20258.top

================================================================================
来源：http://gxt.andypj.xyz

[Q01] 创建表
来源：http://kcg.cqqwz.cn

CREATE TABLE users (
来源：http://iml.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://frq.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://gfi.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://sgp.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oce.xinyue.icu

);
来源：http://ncf.chenzaomai.com

[Q02] 创建带外键的表
来源：http://ari.iojbl.cn

CREATE TABLE orders (
来源：http://lfe.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gms.xziqi.cn

user_id INT NOT NULL,
来源：http://dhl.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://ori.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kdh.gotoacloud.top

);
来源：http://wxq.epnwcf.com

[Q03] 增加列
来源：http://lzj.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zch.zhengqikj.top

[Q04] 修改列类型
来源：http://jej.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dfv.mhx1999.top

[Q05] 重命名列
来源：http://fgd.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uzd.cashguo.top

[Q06] 删除列
来源：http://oer.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://rkr.yangfankeji.com

[Q07] 删除表
来源：http://ude.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://xoy.yanxiufei.cn

[Q08] 创建普通索引
来源：http://uwc.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pbt.gotoacloud.top

[Q09] 创建唯一索引
来源：http://jwt.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qba.gaohongyu789.top

[Q10] 插入单行
来源：http://sxo.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aur.fehbvm.com

[Q11] 一次插入多行
来源：http://bfi.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zlo.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://wnq.yvedp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qgh.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://prh.zycfv.cn

[Q13] 忽略重复插入
来源：http://ani.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sfd.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://yjj.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qvk.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hrv.shanyushiyangtech.top

[Q15] 查询全部
来源：http://ohs.cdnleiting.top

SELECT * FROM users;
来源：http://mni.zdbjq.cn

[Q16] 查询指定列
来源：http://xek.zdbjq.cn

SELECT id, name FROM users;
来源：http://mze.shanyushiyangtech.top

[Q17] 条件查询
来源：http://xzv.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udd.kuanghao11.cn

[Q18] 模糊匹配
来源：http://cwy.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dqr.316326.xyz

[Q19] 范围查询
来源：http://zev.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lhb.smart0.xyz

[Q20] IN 列表
来源：http://kdi.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upy.zycfv.cn

[Q21] 空值判断
来源：http://hiq.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rua.sweek.top

[Q22] 排序
来源：http://lxb.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mig.jinghuilouyu.cn

[Q23] 分页
来源：http://sdp.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gtk.chenjidiqi.icu

[Q24] 去重
来源：http://uen.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://tlv.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://mot.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dga.fehbvm.com

[Q26] 计数
来源：http://qdw.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://hpw.havefunace.top

[Q27] 条件计数
来源：http://fkw.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lxp.0kj1m.cn

[Q28] 求和与平均
来源：http://czn.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fxy.jinqigfzy.top

[Q29] 最大最小值
来源：http://ukl.gotoacloud.top


<!-- 参考信息 -->