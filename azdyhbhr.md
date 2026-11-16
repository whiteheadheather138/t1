代发 wailian999

Ruby: arr.sort
来源：http://cpy.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://zgc.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://bgr.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ynj.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://lhy.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pxz.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://har.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kxp.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zwu.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dio.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://hml.hfpthk.cn

[N04] 斐波那契数列
来源：http://war.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wpq.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cqq.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pxm.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmu.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vxl.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ekr.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://geu.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xne.zdqjudy.top

[N05] 最大公约数
来源：http://vcp.tanke756.top

Py:   math.gcd(a, b)
来源：http://kgv.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kjr.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ryu.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzb.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rod.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rkz.gotoacloud.top

Ruby: a.gcd(b)
来源：http://tmd.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ezo.kuanghao11.cn

[N06] 判断回文字符串
来源：http://lky.andypj.xyz

Py:   s == s[::-1]
来源：http://erh.daria6918.cn

PHP:  $s === strrev($s);
来源：http://wuw.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://lgu.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://huk.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cuy.fehbvm.com

Go:   // 双指针从两端比较
来源：http://dbg.daria6918.cn

Ruby: s == s.reverse
来源：http://vux.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qvl.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://elz.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bpf.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ejk.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uen.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://qbq.316326.xyz

Java: // 手写 HashMap
来源：http://ate.xylfe.cn

Go:   // 手写 map[int]int
来源：http://dvo.gzhubu.top

Ruby: // 手写 Hash
来源：http://ozv.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://enb.shzxlz.cn

[N08] 生成全排列
来源：http://udk.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://lnv.yfazqb.com

PHP:  // 手写递归交换
来源：http://xki.ydzc1.top

JS:   // 手写回溯递归
来源：http://dqd.xuanzx.com

TS:   // 手写回溯递归
来源：http://bgg.hnxiangtu.top

Java: // 手写回溯递归
来源：http://eqy.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://ywn.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://xea.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://von.yonumen.top

[N09] 栈与队列
来源：http://xjx.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jrb.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://elw.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ndx.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iob.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lwf.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://suh.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gng.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://irp.yonumen.top

[N10] 链表节点定义
来源：http://ptg.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eup.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eyr.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dyg.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zib.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://feb.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://xle.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://brf.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://icg.gzhubu.top

[N11] 二叉树中序遍历
来源：http://nhj.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gie.316326.xyz

PHP:  // 手写递归函数
来源：http://uxz.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kda.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tzq.zhaomingkeji.xyz

Java: // 手写递归
来源：http://jul.fzhhl.top

Go:   // 手写递归
来源：http://bef.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iki.zhoulong.xyz

C#:   // 手写递归
来源：http://gon.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://klx.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://csc.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://njb.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kno.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xzx.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jgn.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bje.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://afr.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eer.zhengqikj.top

================================================================================
来源：http://dkh.meibo888.top

O. 并发与异步
来源：http://xvo.sweek.top

================================================================================
来源：http://hkv.feifeiyinyue.top

[O01] 启动一个线程
来源：http://ofe.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ctw.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ihc.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zbs.meibo888.top

TS:   // 同 JS
来源：http://oeu.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://tvl.gotoacloud.top

Go:   go f()
来源：http://mer.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://yic.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://fdp.ivvv.top

[O02] 使用线程池
来源：http://wlh.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hzo.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xhu.tarul.cn

JS:   // worker_threads 线程池
来源：http://tgr.yvedp.cn

TS:   // worker_threads 线程池
来源：http://ulp.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://pfd.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zpe.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://byd.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oyy.tarul.cn

[O03] 加锁保护共享数据
来源：http://zkc.ppjwa.cn

Py:   with lock: shared += 1
来源：http://ruv.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://ska.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zqd.aizwys.cn

TS:   // 同 JS
来源：http://nzu.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://jhp.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://udn.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sbp.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://asa.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://sgo.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://yio.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xwb.uphjek.com

JS:   async function f() { await g(); }
来源：http://ilf.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mxb.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gnt.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xfv.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kee.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://bzu.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://ywq.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://ati.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zud.tarul.cn

JS:   await Promise.all(tasks)
来源：http://xfb.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://fwv.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wvp.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mpg.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://tsz.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rpg.hysaishi.cn

[O06] 使用进程池
来源：http://omf.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mor.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iwa.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://iuc.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://sbj.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jdb.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mfd.fktsv.cn

Ruby: // fork 块
来源：http://owx.bjfxy.top

C#:   Parallel.For
来源：http://kju.ctjpmb.com

================================================================================
来源：http://wfa.yfazqb.com

P. 常用工具函数
来源：http://upn.shanyushiyangkeji.top

================================================================================
来源：http://yag.zdbjq.cn

[P01] 生成 UUID
来源：http://nwd.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://thm.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yyp.iojbl.cn

JS:   crypto.randomUUID()
来源：http://zla.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://sdk.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://lbw.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://trk.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://agh.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://hjy.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://hsz.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckp.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iix.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lms.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ghj.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ipn.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qpl.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pkt.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ezi.nwbrower.top

[P03] 生成短随机字符串
来源：http://osa.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ybp.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pvp.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://quf.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://erd.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hoj.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uqu.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zbu.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vfx.hywenlv.cn

[P04] 求长度
来源：http://laj.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://twx.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwy.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgw.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ayt.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://oqi.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://fks.hesvh.cn

Ruby: x.length;  x.size
来源：http://iav.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://djy.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://zsd.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://njw.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wqp.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://syv.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gkh.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://evx.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://ofc.yfazqb.com

Ruby: a == b
来源：http://lae.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vmf.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ddl.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xly.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://tzk.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nos.jlsjyb.cn

TS:   if (x == null) {}
来源：http://igw.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://zxi.xziqi.cn

Go:   if x == nil {}
来源：http://iko.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rlx.jiagoushi.top

C#:   if (x is null) {}
来源：http://jqk.zycfv.cn

[P07] 防抖与节流
来源：http://dds.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fah.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://yja.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mkv.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hdm.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xtb.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hoy.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iyq.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jcw.fengsongda.top

[P08] 处理浮点精度问题
来源：http://bha.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qlo.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zek.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jor.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zig.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://exp.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iqs.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://foe.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dyf.zhijiandao.cn

================================================================================
来源：http://kkc.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lfb.tianlin.xyz

================================================================================
来源：http://ujh.andypj.xyz

[Q01] 创建表
来源：http://cfj.hcnkem.com

CREATE TABLE users (
来源：http://qfn.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkx.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://yxn.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://vda.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hkr.kuanghao11.cn

);
来源：http://arj.ivvv.top

[Q02] 创建带外键的表
来源：http://owi.kuanghao11.cn

CREATE TABLE orders (
来源：http://dps.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ugj.fktsv.cn

user_id INT NOT NULL,
来源：http://qat.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://nrg.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qri.yj20258.top

);
来源：http://tmz.shuidangran.top

[Q03] 增加列
来源：http://gwp.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hzq.zhongyouzk.top

[Q04] 修改列类型
来源：http://adn.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://poo.tianlin.xyz

[Q05] 重命名列
来源：http://die.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://san.fzhhl.top

[Q06] 删除列
来源：http://oft.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://otw.hnxiangtu.top

[Q07] 删除表
来源：http://ima.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://mlj.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://hsz.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mol.hesvh.cn

[Q09] 创建唯一索引
来源：http://fwt.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dex.haohaochexian.top

[Q10] 插入单行
来源：http://vhi.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aqo.cheryme.top

[Q11] 一次插入多行
来源：http://twp.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nxz.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://hkr.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://dnn.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hay.smart0.xyz

[Q13] 忽略重复插入
来源：http://rjf.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dna.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://rgf.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://okb.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mgp.316326.xyz

[Q15] 查询全部
来源：http://mwd.sweek.top

SELECT * FROM users;
来源：http://bkr.nanxinkj.top

[Q16] 查询指定列
来源：http://ift.kuanghao11.cn

SELECT id, name FROM users;
来源：http://ezj.sysykeji.top

[Q17] 条件查询
来源：http://jgm.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ceg.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://mmw.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zpx.hysaishi.cn

[Q19] 范围查询
来源：http://crc.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pze.pengpengdd.cyou

[Q20] IN 列表
来源：http://zxu.ivvv.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ybi.yuanzhike.top

[Q21] 空值判断
来源：http://mlt.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uty.havefunace.top

[Q22] 排序
来源：http://jse.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://svo.nanxuanxn.top

[Q23] 分页
来源：http://uij.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dge.snrcjt.cn

[Q24] 去重
来源：http://juf.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://cnk.cdnleiting.top

[Q25] 只取前 N 条
来源：http://xqw.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yrc.chenlongwang.top

[Q26] 计数
来源：http://evd.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://zav.cdnleiting.top

[Q27] 条件计数
来源：http://llt.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tbz.vehdjk.com

[Q28] 求和与平均
来源：http://ewk.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nyb.sufxvd.cn

[Q29] 最大最小值
来源：http://rnh.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://kek.nanxuanxn.top

[Q30] 分组统计
来源：http://yvx.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vzh.bbcook.cn

[Q31] 分组后过滤
来源：http://lrr.shuidangran.top


<!-- 参考信息 -->