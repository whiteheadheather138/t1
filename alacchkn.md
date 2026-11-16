代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://lar.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jpj.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xnq.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://agj.jlsjyb.cn

Ruby: arr.sort
来源：http://eir.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dej.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://cce.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ssb.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://zzb.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmk.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://odz.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ejp.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cbj.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vaq.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wvw.guowangkeji.top

[N04] 斐波那契数列
来源：http://idt.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ihj.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xhl.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hxp.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://khz.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzy.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eyj.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://elq.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xhl.ppjwa.cn

[N05] 最大公约数
来源：http://hkd.yfazqb.com

Py:   math.gcd(a, b)
来源：http://ste.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ipv.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kel.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aew.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lbg.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mst.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://kfn.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kgc.yueranfly.top

[N06] 判断回文字符串
来源：http://wfu.tian-w.cn

Py:   s == s[::-1]
来源：http://ypx.redwolf501.top

PHP:  $s === strrev($s);
来源：http://fxo.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://hxs.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://bzg.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yso.epnwcf.com

Go:   // 双指针从两端比较
来源：http://lcd.c1oappe.top

Ruby: s == s.reverse
来源：http://gtc.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gul.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://heg.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oii.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cqi.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wzb.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://jll.gotoacloud.top

Java: // 手写 HashMap
来源：http://wgl.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://yae.zdbjq.cn

Ruby: // 手写 Hash
来源：http://kkb.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://dql.haohaochexian.top

[N08] 生成全排列
来源：http://oye.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://scm.smart0.xyz

PHP:  // 手写递归交换
来源：http://psn.ehwqpu.com

JS:   // 手写回溯递归
来源：http://qxj.hammf.cn

TS:   // 手写回溯递归
来源：http://rpk.tarul.cn

Java: // 手写回溯递归
来源：http://ifv.hammf.cn

Go:   // 手写回溯递归
来源：http://qci.hammf.cn

Ruby: arr.permutation.to_a
来源：http://msz.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://xsl.hammf.cn

[N09] 栈与队列
来源：http://tvz.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wxb.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lbg.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mmr.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qhc.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uli.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://igk.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lex.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfi.feifeiyinyue.top

[N10] 链表节点定义
来源：http://svo.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uto.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://are.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yal.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqy.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://pul.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://rhr.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zdz.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ovx.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://rdm.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xmv.tarul.cn

PHP:  // 手写递归函数
来源：http://bev.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://exa.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kto.chenzaomai.com

Java: // 手写递归
来源：http://nps.meibo888.top

Go:   // 手写递归
来源：http://wkg.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lmf.shanyushiyangtech.top

C#:   // 手写递归
来源：http://sqd.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yud.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rza.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zrb.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvr.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pia.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://svz.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sza.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://duu.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nyu.xylfe.cn

================================================================================
来源：http://yrx.sysykeji.top

O. 并发与异步
来源：http://qlh.jqgufenzy.top

================================================================================
来源：http://vrp.xziqi.cn

[O01] 启动一个线程
来源：http://wmb.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tlg.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ndn.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xyf.jianghu66.top

TS:   // 同 JS
来源：http://ube.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://vdz.hywenlv.cn

Go:   go f()
来源：http://grp.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://dsb.xziqi.cn

C#:   Task.Run(() => F());
来源：http://jlr.0kj1m.cn

[O02] 使用线程池
来源：http://bpf.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lxs.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xfh.uphjek.com

JS:   // worker_threads 线程池
来源：http://rgt.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://mii.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://edy.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jvs.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eri.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kma.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://seo.mhx1999.top

Py:   with lock: shared += 1
来源：http://ver.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://ucl.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tko.pengpengdd.cyou

TS:   // 同 JS
来源：http://yaa.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://zwu.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://djc.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://vmr.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://txt.fengsongda.top

[O04] 定义异步函数并等待
来源：http://nrq.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://wom.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsw.ivvv.top

JS:   async function f() { await g(); }
来源：http://ypt.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://lwb.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://znb.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://awz.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://pwd.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://jwh.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://ejd.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://skt.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ywk.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://fmy.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://hjq.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xvn.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gem.hcnkem.com

Ruby: threads.map(&:join)
来源：http://kxq.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fne.epnwcf.com

[O06] 使用进程池
来源：http://ews.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vtu.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qqg.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://mpr.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://bqe.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hpf.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fyp.hnqzz.top

Ruby: // fork 块
来源：http://uwh.meibo888.top

C#:   Parallel.For
来源：http://vdm.shzxlz.cn

================================================================================
来源：http://ypq.dianchejie.cn

P. 常用工具函数
来源：http://xzn.sufxvd.cn

================================================================================
来源：http://uqe.sjlbkw.cn

[P01] 生成 UUID
来源：http://kjf.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://fop.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rug.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://hza.cheryme.top

TS:   crypto.randomUUID()
来源：http://eah.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://tnc.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://moi.316326.xyz

Ruby: SecureRandom.uuid
来源：http://nqp.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://ukr.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://tqf.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dfv.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zyr.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzf.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gwc.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://raj.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://znh.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lpq.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hlq.vehdjk.com

[P03] 生成短随机字符串
来源：http://atq.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jev.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://skb.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tvx.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hae.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ahl.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cat.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zel.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zja.shuidangran.top

[P04] 求长度
来源：http://nia.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qxo.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uth.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://njb.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dqe.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://cad.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://rrq.shuidangran.top

Ruby: x.length;  x.size
来源：http://rmj.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nio.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://zax.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ojh.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://are.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kxl.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjy.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dyl.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://faf.shanyushiyangkeji.top

Ruby: a == b
来源：http://qai.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bfu.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gcd.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cil.cashguo.top

PHP:  if (empty($x)) {}
来源：http://wpo.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kai.fktsv.cn

TS:   if (x == null) {}
来源：http://cgl.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://brk.mhx1999.top

Go:   if x == nil {}
来源：http://hgv.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ftc.yueranfly.top

C#:   if (x is null) {}
来源：http://bww.dashuyun.cn

[P07] 防抖与节流
来源：http://hta.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yhk.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://jux.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hun.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrz.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://onj.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oyk.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ngm.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fqo.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://dqx.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jvv.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oft.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://idg.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ici.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dyr.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fvf.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tju.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xnv.svipenyu.cn

================================================================================
来源：http://lxv.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qrk.xingfuxueyuan.xyz

================================================================================
来源：http://agw.ywan-chungtsiang.top

[Q01] 创建表
来源：http://fue.shangyingyoupin.top

CREATE TABLE users (
来源：http://sdx.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://onk.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://ndu.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://dbb.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://irx.yanxiufei.cn

);
来源：http://jyl.meibo888.top

[Q02] 创建带外键的表
来源：http://hye.wangshuangyany.cn

CREATE TABLE orders (
来源：http://aad.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yih.zdbjq.cn

user_id INT NOT NULL,
来源：http://ous.hcnkem.com

amount DECIMAL(10, 2),
来源：http://sdj.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ryp.zdqjudy.top

);
来源：http://oeg.hysaishi.cn

[Q03] 增加列
来源：http://hel.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://avv.xziqi.cn

[Q04] 修改列类型
来源：http://gpy.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ujm.hnxiangtu.top

[Q05] 重命名列
来源：http://poh.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ivp.wangshuangyany.cn

[Q06] 删除列
来源：http://sfb.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://ynd.jqgufenzy.top

[Q07] 删除表
来源：http://exe.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://pti.zhijiandao.cn

[Q08] 创建普通索引
来源：http://vdb.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nsb.nwbrower.top

[Q09] 创建唯一索引
来源：http://pct.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehm.andypj.xyz

[Q10] 插入单行
来源：http://opo.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://njv.tarul.cn

[Q11] 一次插入多行
来源：http://gcv.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rjy.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://tjo.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://adr.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pbk.guannengcc.top

[Q13] 忽略重复插入
来源：http://tmq.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sdz.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://smv.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ujs.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://odh.yangfankeji.com

[Q15] 查询全部
来源：http://wsp.sxryk.cn

SELECT * FROM users;
来源：http://fcj.xuanzx.com

[Q16] 查询指定列
来源：http://zxk.aizwys.cn

SELECT id, name FROM users;
来源：http://ena.ybcxt.top

[Q17] 条件查询
来源：http://lae.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rzv.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://iqu.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pds.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://knk.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kyp.chenzaomai.com

[Q20] IN 列表
来源：http://rxk.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hrx.cdnleiting.top

[Q21] 空值判断
来源：http://ozx.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yvd.ivvv.top

[Q22] 排序
来源：http://jsh.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oms.xylfe.cn

[Q23] 分页
来源：http://xqv.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sbp.ybcxt.top

[Q24] 去重
来源：http://njj.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://elo.yongpay.top

[Q25] 只取前 N 条
来源：http://exj.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqt.hcnkem.com

[Q26] 计数
来源：http://ggq.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://twf.chenjidiqi.icu

[Q27] 条件计数
来源：http://nvq.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpm.svipenyu.cn

[Q28] 求和与平均
来源：http://xja.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://swh.birdmap.top

[Q29] 最大最小值
来源：http://rml.jinqigfzy.top


<!-- 参考信息 -->