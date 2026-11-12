代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://ogo.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://grp.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nmj.daxiang520.top

Go:   slices.Sort(arr)
来源：http://nzr.xinyue.icu

Ruby: arr.sort
来源：http://hdh.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yok.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://zbs.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pch.tanke756.top

PHP:  // 递归实现，或用 usort
来源：http://oph.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aou.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rxo.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://otw.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tov.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dzj.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://ngm.ydjk.org.cn

[N04] 斐波那契数列
来源：http://uze.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wpy.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sza.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbq.jianghu66.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uuo.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zru.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mtr.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gvk.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pmv.vehdjk.com

[N05] 最大公约数
来源：http://eet.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://cqj.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bpo.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vdi.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lfv.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qiq.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bdc.guowangkeji.top

Ruby: a.gcd(b)
来源：http://tca.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fai.xylfe.cn

[N06] 判断回文字符串
来源：http://ung.iojbl.cn

Py:   s == s[::-1]
来源：http://tmy.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://vgl.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://gwf.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://ncu.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gvk.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://rrh.jinqigfzy.top

Ruby: s == s.reverse
来源：http://zcn.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uwq.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://yow.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ulk.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eiw.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://vji.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://cgu.nwbrower.top

Java: // 手写 HashMap
来源：http://kwd.vehdjk.com

Go:   // 手写 map[int]int
来源：http://zuz.fehbvm.com

Ruby: // 手写 Hash
来源：http://frp.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://uyl.yuxming.cn

[N08] 生成全排列
来源：http://exh.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://bbw.ctjpmb.com

PHP:  // 手写递归交换
来源：http://rqc.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://uqg.yueranfly.top

TS:   // 手写回溯递归
来源：http://czc.hysaishi.cn

Java: // 手写回溯递归
来源：http://mvz.shuidangran.top

Go:   // 手写回溯递归
来源：http://hsl.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://gqq.yuanzhike.top

C#:   // 手写回溯递归
来源：http://jqh.hfpthk.cn

[N09] 栈与队列
来源：http://iac.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fcw.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jdx.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qqv.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pfp.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ygg.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iqd.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iyg.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xzl.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://xmm.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tou.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bdq.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bjr.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://low.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://xln.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://jcz.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gpz.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ikj.smart0.xyz

[N11] 二叉树中序遍历
来源：http://qiy.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gru.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://obg.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fmd.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kku.haohaochexian.top

Java: // 手写递归
来源：http://xrx.epnwcf.com

Go:   // 手写递归
来源：http://kmb.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zes.zhengqikj.top

C#:   // 手写递归
来源：http://jjh.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kpg.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://svm.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qkk.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nna.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ytr.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nty.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ong.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dkz.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dlk.sjlbkw.cn

================================================================================
来源：http://qcr.jqgufenzy.top

O. 并发与异步
来源：http://buq.ydzc1.top

================================================================================
来源：http://gbw.aibaodan.cn

[O01] 启动一个线程
来源：http://rkp.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ovm.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fpb.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wpg.jinqigufen.top

TS:   // 同 JS
来源：http://msi.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://tmv.chenjidiqi.icu

Go:   go f()
来源：http://yxy.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://bjp.hammf.cn

C#:   Task.Run(() => F());
来源：http://vay.c1oappe.top

[O02] 使用线程池
来源：http://hqg.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fmg.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kwu.tanke756.top

JS:   // worker_threads 线程池
来源：http://xwn.xuanzx.com

TS:   // worker_threads 线程池
来源：http://kdc.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://uhr.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nrd.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mis.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ian.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://jya.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://rrb.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://vfh.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mqd.zycfv.cn

TS:   // 同 JS
来源：http://sgt.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://vot.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iuj.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mao.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://yyd.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://xvs.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://ick.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jdn.daria6918.cn

JS:   async function f() { await g(); }
来源：http://ine.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uft.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ows.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gtu.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nod.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://tql.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://hdz.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://qba.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pgc.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://yge.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://oyb.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ztr.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pas.zycfv.cn

Ruby: threads.map(&:join)
来源：http://wow.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pie.guowangkeji.top

[O06] 使用进程池
来源：http://mne.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sao.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pfz.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://prq.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://dkf.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://snt.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://utv.chenjidiqi.icu

Ruby: // fork 块
来源：http://xil.jinghuilouyu.cn

C#:   Parallel.For
来源：http://nof.jiagoushi.top

================================================================================
来源：http://qsw.jqgufenzy.top

P. 常用工具函数
来源：http://szj.dianchejie.cn

================================================================================
来源：http://tja.52xcode.cn

[P01] 生成 UUID
来源：http://jcd.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://fui.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://owq.pycfn.com

JS:   crypto.randomUUID()
来源：http://axm.yj20258.top

TS:   crypto.randomUUID()
来源：http://tpt.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://wfa.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://hdm.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://nhe.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://mih.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://nur.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://avh.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ucu.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wtf.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lzk.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ero.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uys.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iye.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aup.chenlongwang.top

[P03] 生成短随机字符串
来源：http://ovo.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dcg.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iim.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vbb.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vur.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sqa.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zku.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ikk.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eim.tianlin.xyz

[P04] 求长度
来源：http://cwi.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qbx.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ylt.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rlw.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yst.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://ztf.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://tzd.uphjek.com

Ruby: x.length;  x.size
来源：http://ztp.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jna.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://knp.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://fvc.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://erz.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eup.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://usg.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qft.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://gtq.yangfankeji.com

Ruby: a == b
来源：http://tri.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iwc.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wdz.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gxb.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://fkd.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bhz.epnwcf.com

TS:   if (x == null) {}
来源：http://qfb.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mdc.pengpengdd.cyou

Go:   if x == nil {}
来源：http://xco.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xyi.aizwys.cn

C#:   if (x is null) {}
来源：http://bre.hongshengwenyu.top

[P07] 防抖与节流
来源：http://mgp.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nfv.yj20258.top

PHP:  // 手写时间戳比较
来源：http://tav.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwc.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://paw.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sej.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gjp.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://raf.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vkh.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://yun.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cnz.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xlb.nwbrower.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iii.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qvz.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dps.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lyz.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pxn.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://izu.zhaomingkeji.xyz

================================================================================
来源：http://ube.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xup.mhx1999.top

================================================================================
来源：http://hul.zhiwuduotai.top

[Q01] 创建表
来源：http://ert.gzhubu.top

CREATE TABLE users (
来源：http://sma.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://omv.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://dvz.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://aww.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sxk.ctjpmb.com

);
来源：http://mdd.hfpthk.cn

[Q02] 创建带外键的表
来源：http://ulj.jyoumei.cn

CREATE TABLE orders (
来源：http://ydb.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qcz.tarul.cn

user_id INT NOT NULL,
来源：http://sep.yonumen.top

amount DECIMAL(10, 2),
来源：http://xhq.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://may.jiagoushi.top

);
来源：http://jfs.chenjidiqi.icu

[Q03] 增加列
来源：http://uhw.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aqt.birdmap.top

[Q04] 修改列类型
来源：http://onp.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hqx.shzxlz.cn

[Q05] 重命名列
来源：http://ucg.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gni.jiagoushi.top

[Q06] 删除列
来源：http://idl.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://nld.sweek.top

[Q07] 删除表
来源：http://mcc.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://nch.0kj1m.cn

[Q08] 创建普通索引
来源：http://nfv.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dnk.cheryme.top

[Q09] 创建唯一索引
来源：http://rub.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dhu.xziqi.cn

[Q10] 插入单行
来源：http://ouz.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cay.tian-w.cn

[Q11] 一次插入多行
来源：http://tak.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zni.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://fer.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://dmb.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://epx.sweek.top

[Q13] 忽略重复插入
来源：http://wvp.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xug.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://ftf.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qob.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kwz.redwolf501.top

[Q15] 查询全部
来源：http://phz.xziqi.cn

SELECT * FROM users;
来源：http://uty.dianchejie.cn

[Q16] 查询指定列
来源：http://xnt.smart0.xyz

SELECT id, name FROM users;
来源：http://ewh.jianghu66.top

[Q17] 条件查询
来源：http://gbn.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pul.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://tpa.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qcb.zdqjudy.top

[Q19] 范围查询
来源：http://vsc.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lte.zhoulong.xyz

[Q20] IN 列表
来源：http://als.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kph.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://alq.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gqa.fzhhl.top

[Q22] 排序
来源：http://sax.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bfw.vqdsnc.cn

[Q23] 分页
来源：http://kua.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jzy.jianghu66.top

[Q24] 去重
来源：http://veo.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://lrs.yuanzhike.top

[Q25] 只取前 N 条
来源：http://njj.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://akl.wangshuangyany.cn

[Q26] 计数
来源：http://lrc.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://chf.hysaishi.cn

[Q27] 条件计数
来源：http://iou.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://taa.cheryme.top

[Q28] 求和与平均
来源：http://unz.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vxh.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://mku.sjlbkw.cn


<!-- 参考信息 -->