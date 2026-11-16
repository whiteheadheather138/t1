代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://pmy.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lra.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ycf.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://baw.iojbl.cn

Ruby: arr.sort
来源：http://xjz.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ogo.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://adz.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdt.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://qiu.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnb.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpa.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sgu.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oxc.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nrp.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://hkd.fktsv.cn

[N04] 斐波那契数列
来源：http://ktn.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://izr.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dgn.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bck.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yeq.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dyk.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kwv.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://byc.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pfm.yueranfly.top

[N05] 最大公约数
来源：http://ecn.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://vpb.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dkw.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ipg.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qmf.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qqd.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hdk.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://wbs.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vfn.gogol.net.cn

[N06] 判断回文字符串
来源：http://cbb.dashuyun.cn

Py:   s == s[::-1]
来源：http://ntu.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://afx.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://brn.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://xpq.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lrd.nwbrower.top

Go:   // 双指针从两端比较
来源：http://opz.xylfe.cn

Ruby: s == s.reverse
来源：http://kyi.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rlo.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://cuf.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dra.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ulk.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://unq.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://cmw.hcnkem.com

Java: // 手写 HashMap
来源：http://onw.havefunace.top

Go:   // 手写 map[int]int
来源：http://wir.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://xnb.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://ygg.ppjwa.cn

[N08] 生成全排列
来源：http://tzk.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://lto.0kj1m.cn

PHP:  // 手写递归交换
来源：http://fch.meibo888.top

JS:   // 手写回溯递归
来源：http://rch.sxryk.cn

TS:   // 手写回溯递归
来源：http://uvx.c1oappe.top

Java: // 手写回溯递归
来源：http://ojx.ehwqpu.com

Go:   // 手写回溯递归
来源：http://itb.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://fjp.andypj.xyz

C#:   // 手写回溯递归
来源：http://opv.mhx1999.top

[N09] 栈与队列
来源：http://tul.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qrc.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xhq.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yhp.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://drf.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zzx.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wbj.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tae.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ysq.chenlongwang.top

[N10] 链表节点定义
来源：http://fvl.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sms.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lbx.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://svi.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://szc.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://bga.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://uaf.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ydo.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xqa.cheryme.top

[N11] 二叉树中序遍历
来源：http://qhr.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yup.tianlin.xyz

PHP:  // 手写递归函数
来源：http://ken.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pey.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vua.bjfxy.top

Java: // 手写递归
来源：http://cpi.zhengqikj.top

Go:   // 手写递归
来源：http://nvf.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xlh.pengpengdd.cyou

C#:   // 手写递归
来源：http://rqu.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dzg.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ahp.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zoa.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vix.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bpc.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bsb.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sls.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xhd.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://reb.epnwcf.com

================================================================================
来源：http://cuz.iojbl.cn

O. 并发与异步
来源：http://bhi.yanxiufei.cn

================================================================================
来源：http://jbx.jlsjyb.cn

[O01] 启动一个线程
来源：http://aqs.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://afo.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bpf.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fwo.uphjek.com

TS:   // 同 JS
来源：http://qxs.fktsv.cn

Java: new Thread(() -> f()).start()
来源：http://tgw.xuanzx.com

Go:   go f()
来源：http://vfy.yj202588.top

Ruby: Thread.new { f }
来源：http://vbo.aizwys.cn

C#:   Task.Run(() => F());
来源：http://ylj.cucudq.cn

[O02] 使用线程池
来源：http://rol.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gjq.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://koi.yueranfly.top

JS:   // worker_threads 线程池
来源：http://agj.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://kwo.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://cyw.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rod.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://txg.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uyk.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://npj.gogol.net.cn

Py:   with lock: shared += 1
来源：http://kkp.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://tdo.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aui.vqdsnc.cn

TS:   // 同 JS
来源：http://yps.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://ozr.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cwp.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jnt.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://dak.yueranfly.top

[O04] 定义异步函数并等待
来源：http://kyp.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://gwm.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mre.52xcode.cn

JS:   async function f() { await g(); }
来源：http://xlr.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ykj.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wxd.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kbf.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oas.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://qxv.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://dfd.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://dot.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pqa.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://kaw.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://how.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zdi.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tse.jianghu66.top

Ruby: threads.map(&:join)
来源：http://whp.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dml.andypj.xyz

[O06] 使用进程池
来源：http://jte.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dwl.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ftk.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://qbg.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://xgq.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yae.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://via.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://pir.zhengqikj.top

C#:   Parallel.For
来源：http://sxy.kuanghao11.cn

================================================================================
来源：http://apa.meibo888.top

P. 常用工具函数
来源：http://dum.ybcxt.top

================================================================================
来源：http://srb.jianghu66.top

[P01] 生成 UUID
来源：http://hkv.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://dog.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vnr.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://pag.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://qah.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://mjq.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://rjb.cashguo.top

Ruby: SecureRandom.uuid
来源：http://yqz.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://yil.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://cqv.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wqm.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://erz.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://set.xingfuxueyuan.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ztw.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mtf.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kwd.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dyx.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lyw.jianghu66.top

[P03] 生成短随机字符串
来源：http://ekl.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cvw.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yky.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qix.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ojh.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://epr.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kpt.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://tjy.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ojv.jinyuanbaomall.cn

[P04] 求长度
来源：http://lua.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vrl.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nuf.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://igl.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vlc.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://fjw.sweek.top

Go:   len(arr);  len(m)
来源：http://rtw.iojbl.cn

Ruby: x.length;  x.size
来源：http://pma.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xrb.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://bam.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bol.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wyo.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nwi.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://srz.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://slp.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://eka.iojbl.cn

Ruby: a == b
来源：http://vyb.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ibz.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://adf.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vod.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://pnp.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jyv.ehwqpu.com

TS:   if (x == null) {}
来源：http://lro.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xcl.shuidangran.top

Go:   if x == nil {}
来源：http://rfg.iojbl.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fms.gogol.net.cn

C#:   if (x is null) {}
来源：http://tyn.dianchejie.cn

[P07] 防抖与节流
来源：http://pny.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bln.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://jfe.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rmg.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eki.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pgb.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kbi.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jon.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gwg.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://hjy.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vvv.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lpu.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tia.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jld.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ang.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dtd.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pju.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://clz.sysykeji.top

================================================================================
来源：http://mjc.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fow.ybcxt.top

================================================================================
来源：http://vgb.xuetiantiany.cn

[Q01] 创建表
来源：http://ksz.zdbjq.cn

CREATE TABLE users (
来源：http://kly.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rtc.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://kpw.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://ywq.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://urd.hnqzz.top

);
来源：http://vmm.chenlongwang.top

[Q02] 创建带外键的表
来源：http://xsb.xingfuxueyuan.xyz

CREATE TABLE orders (
来源：http://tqh.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyv.yanxiufei.cn

user_id INT NOT NULL,
来源：http://hzu.zycfv.cn

amount DECIMAL(10, 2),
来源：http://snh.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://omv.hongshengwenyu.top

);
来源：http://ujc.jlsjyb.cn

[Q03] 增加列
来源：http://yqt.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zsz.tarul.cn

[Q04] 修改列类型
来源：http://nbj.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lfv.wangdashe.top

[Q05] 重命名列
来源：http://htr.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cyc.hammf.cn

[Q06] 删除列
来源：http://rbo.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://xdj.shangyingyoupin.top

[Q07] 删除表
来源：http://scl.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://lzn.yonumen.top

[Q08] 创建普通索引
来源：http://uki.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rrh.316326.xyz

[Q09] 创建唯一索引
来源：http://xzd.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://idp.yuxming.cn

[Q10] 插入单行
来源：http://tgf.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ivs.wangdashe.top

[Q11] 一次插入多行
来源：http://kkk.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yjm.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://oar.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://qil.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jsb.gogol.net.cn

[Q13] 忽略重复插入
来源：http://owh.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zzu.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://hlb.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vkc.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tmj.ctjpmb.com

[Q15] 查询全部
来源：http://ovy.gotoacloud.top

SELECT * FROM users;
来源：http://usn.cdnleiting.top

[Q16] 查询指定列
来源：http://fin.pycfn.com

SELECT id, name FROM users;
来源：http://esg.sxryk.cn

[Q17] 条件查询
来源：http://yxp.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wmz.sxryk.cn

[Q18] 模糊匹配
来源：http://zqm.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jvp.ydzc1.top

[Q19] 范围查询
来源：http://zhe.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ojr.yj20258888.top

[Q20] IN 列表
来源：http://rls.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ezo.yuxming.cn

[Q21] 空值判断
来源：http://hwk.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yme.mhx1999.top

[Q22] 排序
来源：http://bjz.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jdc.fktsv.cn

[Q23] 分页
来源：http://rfg.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kit.chenlongwang.top

[Q24] 去重
来源：http://ecw.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://fqb.ehwqpu.com

[Q25] 只取前 N 条
来源：http://lbm.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tbx.zycfv.cn

[Q26] 计数
来源：http://jlj.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://fds.shangyingyoupin.top

[Q27] 条件计数
来源：http://tep.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tat.yj20258.top

[Q28] 求和与平均
来源：http://pxb.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oqu.sjlbkw.cn

[Q29] 最大最小值
来源：http://nfc.jqgfzy.top


<!-- 参考信息 -->