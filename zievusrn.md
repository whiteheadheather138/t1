代发 wailian999

Ruby: arr.sort
来源：http://wcq.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kkh.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://rlt.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://von.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://kkb.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cso.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vuo.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eze.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rpb.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://edq.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://inl.snrcjt.cn

[N04] 斐波那契数列
来源：http://cbk.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qiz.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mvt.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ili.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ttc.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xsc.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tnv.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mvz.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://han.hnxiangtu.top

[N05] 最大公约数
来源：http://jtf.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://rwj.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vqq.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zxd.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hmd.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qqp.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ybw.zhengqikj.top

Ruby: a.gcd(b)
来源：http://tvc.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mae.iojbl.cn

[N06] 判断回文字符串
来源：http://tnb.yueranfly.top

Py:   s == s[::-1]
来源：http://qmy.hammf.cn

PHP:  $s === strrev($s);
来源：http://hfa.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://byy.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://kwk.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oat.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://lta.havefunace.top

Ruby: s == s.reverse
来源：http://ywr.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pce.yj20258.top

[N07] 两数之和（返回下标）
来源：http://rru.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oct.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cyj.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cdq.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://sam.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://wnr.yj20258.top

Go:   // 手写 map[int]int
来源：http://jyw.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://rbw.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://fxm.vehdjk.com

[N08] 生成全排列
来源：http://pwf.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://sye.hammf.cn

PHP:  // 手写递归交换
来源：http://tms.chenlongwang.top

JS:   // 手写回溯递归
来源：http://zzs.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://gym.hnxiangtu.top

Java: // 手写回溯递归
来源：http://bwt.tianlin.xyz

Go:   // 手写回溯递归
来源：http://eqh.sweek.top

Ruby: arr.permutation.to_a
来源：http://cwr.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://ota.shuidangran.top

[N09] 栈与队列
来源：http://fug.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ist.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://erc.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ois.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vjw.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ixd.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wbn.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ymr.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vki.dashuyun.cn

[N10] 链表节点定义
来源：http://ien.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gjf.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://opw.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ffk.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yes.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://ydo.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://hyl.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hpn.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ppp.aizwys.cn

[N11] 二叉树中序遍历
来源：http://jyf.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mnd.xinyue.icu

PHP:  // 手写递归函数
来源：http://htn.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jvj.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://brn.andypj.xyz

Java: // 手写递归
来源：http://smr.chenjidiqi.icu

Go:   // 手写递归
来源：http://qyy.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eiu.yj202588.top

C#:   // 手写递归
来源：http://tyu.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dfq.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qhn.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sbm.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ygt.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lee.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ljz.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://whk.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zmf.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sxl.shangyingyoupin.top

================================================================================
来源：http://zwd.wangdashe.top

O. 并发与异步
来源：http://zsc.yfazqb.com

================================================================================
来源：http://ewg.tarul.cn

[O01] 启动一个线程
来源：http://yfe.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uht.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pww.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ogn.mhx1999.top

TS:   // 同 JS
来源：http://seh.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://soa.chenlongwang.top

Go:   go f()
来源：http://glo.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://rjz.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://vpq.hnqzz.top

[O02] 使用线程池
来源：http://izl.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qaw.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzs.smart0.xyz

JS:   // worker_threads 线程池
来源：http://hfa.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://emz.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tsz.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gkw.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ofp.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://joj.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://ozr.cashguo.top

Py:   with lock: shared += 1
来源：http://eeu.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://lyu.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yue.sxryk.cn

TS:   // 同 JS
来源：http://hoq.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://ncd.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uxu.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://btw.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://rmm.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://lpr.sysykeji.top

Py:   async def f():⏎    await g()
来源：http://hzx.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yxc.sweek.top

JS:   async function f() { await g(); }
来源：http://hcj.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yty.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yrg.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xyf.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dzn.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://mxa.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://lbk.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://waa.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kde.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://onj.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://cae.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pvf.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://spv.hcnkem.com

Ruby: threads.map(&:join)
来源：http://bqh.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ijh.haohaochexian.top

[O06] 使用进程池
来源：http://rpe.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kvd.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://pkb.316326.xyz

JS:   // child_process / cluster 模块
来源：http://oul.tanke756.top

TS:   // child_process / cluster 模块
来源：http://wcs.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tdr.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nqf.cucudq.cn

Ruby: // fork 块
来源：http://dum.xziqi.cn

C#:   Parallel.For
来源：http://yvc.52xcode.cn

================================================================================
来源：http://fma.guannengcc.top

P. 常用工具函数
来源：http://ych.hammf.cn

================================================================================
来源：http://vit.chenlongwang.top

[P01] 生成 UUID
来源：http://crz.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://dox.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hru.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://iii.aizwys.cn

TS:   crypto.randomUUID()
来源：http://uzd.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://iew.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://znj.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://wen.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://ulv.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://xvm.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vdy.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sgw.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fwq.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vla.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zss.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fwd.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pup.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eqj.snrcjt.cn

[P03] 生成短随机字符串
来源：http://wmn.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cje.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zfa.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rmv.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvd.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ctb.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pqr.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rta.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://moo.hammf.cn

[P04] 求长度
来源：http://aes.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ocr.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vao.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://flt.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rry.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://fje.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://kcs.cucudq.cn

Ruby: x.length;  x.size
来源：http://nmm.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tmi.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://hrt.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://tvk.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qpq.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wxy.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xwz.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rbh.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://emh.uphjek.com

Ruby: a == b
来源：http://kwm.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zrg.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rnt.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hhf.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://vjp.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://prm.tarul.cn

TS:   if (x == null) {}
来源：http://zyx.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ixg.0kj1m.cn

Go:   if x == nil {}
来源：http://wmj.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wpa.gaohongyu789.top

C#:   if (x is null) {}
来源：http://thm.yangfankeji.com

[P07] 防抖与节流
来源：http://ivt.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zgq.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://esx.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txz.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cbw.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fub.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jgf.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ulk.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://equ.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://qca.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fiz.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://heb.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ixb.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wog.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://avk.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mem.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jqk.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://orh.316326.xyz

================================================================================
来源：http://plb.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wlq.hywenlv.cn

================================================================================
来源：http://wva.epnwcf.com

[Q01] 创建表
来源：http://dek.hcnkem.com

CREATE TABLE users (
来源：http://eqe.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://upz.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://nke.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://iog.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jnc.shangyingyoupin.top

);
来源：http://pzu.yueranfly.top

[Q02] 创建带外键的表
来源：http://meg.yuanzhike.top

CREATE TABLE orders (
来源：http://yzd.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ast.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://dzr.jianghu66.top

amount DECIMAL(10, 2),
来源：http://szz.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sfh.shangyingyoupin.top

);
来源：http://vik.pengpengdd.cyou

[Q03] 增加列
来源：http://vgu.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lxm.daria6918.cn

[Q04] 修改列类型
来源：http://epx.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fqf.havefunace.top

[Q05] 重命名列
来源：http://ddd.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xrx.hywenlv.cn

[Q06] 删除列
来源：http://gxn.ybcxt.top

ALTER TABLE users DROP COLUMN age;
来源：http://pph.shanyushiyangkeji.top

[Q07] 删除表
来源：http://uge.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://ull.bbcook.cn

[Q08] 创建普通索引
来源：http://ixe.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://stz.xuanzx.com

[Q09] 创建唯一索引
来源：http://ndf.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wyk.snrcjt.cn

[Q10] 插入单行
来源：http://iwa.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://slz.xuanzx.com

[Q11] 一次插入多行
来源：http://edp.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cdx.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://cdp.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://ezt.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bwq.dianchejie.cn

[Q13] 忽略重复插入
来源：http://uje.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hfw.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://tcm.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gjv.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tmd.chenjidiqi.icu

[Q15] 查询全部
来源：http://rbz.jinghuilouyu.cn

SELECT * FROM users;
来源：http://drd.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://raz.daria6918.cn

SELECT id, name FROM users;
来源：http://vyp.cdnleiting.top

[Q17] 条件查询
来源：http://ohj.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ini.9152youxi.cn

[Q18] 模糊匹配
来源：http://tpo.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rmu.guowangkeji.top

[Q19] 范围查询
来源：http://jwi.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zqy.dianchejie.cn

[Q20] IN 列表
来源：http://jzs.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qyi.ctjpmb.com

[Q21] 空值判断
来源：http://htw.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://als.jyoumei.cn

[Q22] 排序
来源：http://evc.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fan.bbcook.cn

[Q23] 分页
来源：http://rjx.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zns.zhiwuduotai.top

[Q24] 去重
来源：http://xzf.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://xah.uphjek.com

[Q25] 只取前 N 条
来源：http://xqc.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jen.yuanzhike.top

[Q26] 计数
来源：http://rwe.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://ucy.chenjidiqi.icu

[Q27] 条件计数
来源：http://fba.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tja.xylfe.cn

[Q28] 求和与平均
来源：http://jdg.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jbp.ivvv.top

[Q29] 最大最小值
来源：http://qau.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://btn.hongshengwenyu.top

[Q30] 分组统计
来源：http://xnc.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mtl.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://hzu.jqgufenzy.top


<!-- 参考信息 -->