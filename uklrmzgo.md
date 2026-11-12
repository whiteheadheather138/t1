代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://fpz.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jhg.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cwo.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fvz.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tqc.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://apt.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ghl.svipenyu.cn

[N04] 斐波那契数列
来源：http://ewc.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kly.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipl.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mtk.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sgc.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sdj.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jmm.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jqs.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pgc.jqgufenzy.top

[N05] 最大公约数
来源：http://ngl.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://cbu.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://crv.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wqn.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rpb.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://byf.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pmk.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://blq.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yof.yangfankeji.com

[N06] 判断回文字符串
来源：http://dtp.sysykeji.top

Py:   s == s[::-1]
来源：http://gpa.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://mqp.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://bwc.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://eqf.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qnq.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://ilq.ctjpmb.com

Ruby: s == s.reverse
来源：http://kni.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://lzz.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://hax.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mwb.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qqc.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iup.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://zaj.gzhubu.top

Java: // 手写 HashMap
来源：http://jtf.andypj.xyz

Go:   // 手写 map[int]int
来源：http://qgv.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://sqm.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dws.feifeiyinyue.top

[N08] 生成全排列
来源：http://vxt.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://iof.pycfn.com

PHP:  // 手写递归交换
来源：http://lmo.fktsv.cn

JS:   // 手写回溯递归
来源：http://jkw.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://zbt.yanxiufei.cn

Java: // 手写回溯递归
来源：http://trm.chenlongwang.top

Go:   // 手写回溯递归
来源：http://gma.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://ujq.hnqzz.top

C#:   // 手写回溯递归
来源：http://gbb.yongpay.top

[N09] 栈与队列
来源：http://jhn.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://msh.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vcs.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://axr.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://peh.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sng.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rdg.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rai.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uyu.daxiang520.top

[N10] 链表节点定义
来源：http://moz.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://znn.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gmk.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://icu.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rya.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://qpr.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://leg.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ivf.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://awc.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://yus.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gob.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://pvm.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itp.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://svn.52xcode.cn

Java: // 手写递归
来源：http://ccd.316326.xyz

Go:   // 手写递归
来源：http://yna.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ixl.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://grk.yfazqb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vhx.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kpz.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hod.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://msp.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://frw.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://khf.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bby.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jla.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sas.jinyuanbaomall.cn

================================================================================
来源：http://aki.andypj.xyz

O. 并发与异步
来源：http://txd.pycfn.com

================================================================================
来源：http://fff.fzhhl.top

[O01] 启动一个线程
来源：http://pkb.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ipa.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uxt.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fui.wangdashe.top

TS:   // 同 JS
来源：http://mja.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://ips.wangdashe.top

Go:   go f()
来源：http://daf.snrcjt.cn

Ruby: Thread.new { f }
来源：http://dni.ydzc1.top

C#:   Task.Run(() => F());
来源：http://udm.gzhubu.top

[O02] 使用线程池
来源：http://biq.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vst.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cte.yj20258.top

JS:   // worker_threads 线程池
来源：http://hnl.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://vhv.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://amd.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lsf.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tvg.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tnd.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://heb.yongpay.top

Py:   with lock: shared += 1
来源：http://frh.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://tpd.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ian.yangfankeji.com

TS:   // 同 JS
来源：http://zbk.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://urp.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wwt.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xlt.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://tqx.yuxming.cn

[O04] 定义异步函数并等待
来源：http://bdh.pycfn.com

Py:   async def f():⏎    await g()
来源：http://jay.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zpf.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://vec.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://fww.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ego.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tnx.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://gcr.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://dzg.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://hka.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://hiv.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ddg.tarul.cn

JS:   await Promise.all(tasks)
来源：http://ytf.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://lrr.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jdp.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jbh.smart0.xyz

Ruby: threads.map(&:join)
来源：http://gji.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qre.hcnkem.com

[O06] 使用进程池
来源：http://dfv.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bhn.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://auw.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://vhw.yonumen.top

TS:   // child_process / cluster 模块
来源：http://rks.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xkm.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nrw.pengpengdd.cyou

Ruby: // fork 块
来源：http://oof.gzhubu.top

C#:   Parallel.For
来源：http://hsq.jinghuilouyu.cn

================================================================================
来源：http://efc.hesvh.cn

P. 常用工具函数
来源：http://vja.0kj1m.cn

================================================================================
来源：http://zxd.yj202588.top

[P01] 生成 UUID
来源：http://amt.tarul.cn

Py:   str(uuid.uuid4())
来源：http://vte.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tcc.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://yym.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://zus.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://chk.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://qeh.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://ovh.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://efb.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://cqf.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kxx.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://yro.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ytj.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nte.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vvs.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mai.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vgy.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jqx.uphjek.com

[P03] 生成短随机字符串
来源：http://wip.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qgd.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ekl.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jyc.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kyj.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gso.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lpz.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://owf.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://upf.ppjwa.cn

[P04] 求长度
来源：http://nea.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eso.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hvp.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgu.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tug.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://rlm.tarul.cn

Go:   len(arr);  len(m)
来源：http://cfl.daria6918.cn

Ruby: x.length;  x.size
来源：http://hil.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gqq.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://rhk.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://viw.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://anz.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://asa.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://veo.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vub.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gxn.jiagoushi.top

Ruby: a == b
来源：http://wci.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uyf.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hyh.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nsk.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://phb.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lrx.9152youxi.cn

TS:   if (x == null) {}
来源：http://prv.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lhr.ppjwa.cn

Go:   if x == nil {}
来源：http://ijo.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nyb.ehwqpu.com

C#:   if (x is null) {}
来源：http://oag.jinqigfzy.top

[P07] 防抖与节流
来源：http://jhw.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mne.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://pke.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jtn.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsy.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tze.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iyg.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://emm.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dbn.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://jyu.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hsk.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dtn.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cad.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tir.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ibt.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gvz.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uxh.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iyd.kuanghao11.cn

================================================================================
来源：http://ipq.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kop.jinqigfzy.top

================================================================================
来源：http://sld.fehbvm.com

[Q01] 创建表
来源：http://pnk.cheryme.top

CREATE TABLE users (
来源：http://sqx.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqh.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://srz.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://rso.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jll.xylfe.cn

);
来源：http://qwp.yongpay.top

[Q02] 创建带外键的表
来源：http://ahy.mhx1999.top

CREATE TABLE orders (
来源：http://vok.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yjn.epnwcf.com

user_id INT NOT NULL,
来源：http://ifl.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://qwk.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zsi.cqqwz.cn

);
来源：http://tcr.jlsjyb.cn

[Q03] 增加列
来源：http://ijd.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ruc.sysykeji.top

[Q04] 修改列类型
来源：http://kze.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://doi.jianghu66.top

[Q05] 重命名列
来源：http://ixf.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mrw.316326.xyz

[Q06] 删除列
来源：http://efc.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://orj.dianchejie.cn

[Q07] 删除表
来源：http://sto.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://vhg.yongpay.top

[Q08] 创建普通索引
来源：http://zqe.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ylv.andypj.xyz

[Q09] 创建唯一索引
来源：http://qjl.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oxq.dashuyun.cn

[Q10] 插入单行
来源：http://ngb.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mma.cheryme.top

[Q11] 一次插入多行
来源：http://lhu.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://odi.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://lxw.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://cta.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fte.daria6918.cn

[Q13] 忽略重复插入
来源：http://chs.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tbh.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://ohy.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pql.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ttc.jinghuilouyu.cn

[Q15] 查询全部
来源：http://cwe.birdmap.top

SELECT * FROM users;
来源：http://zwy.quarkkingdee.top

[Q16] 查询指定列
来源：http://ihp.quarkkingdee.top

SELECT id, name FROM users;
来源：http://qfs.shanyushiyangtech.top

[Q17] 条件查询
来源：http://ysk.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://isg.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://jtw.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tty.zdqjudy.top

[Q19] 范围查询
来源：http://rhp.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cty.mhx1999.top

[Q20] IN 列表
来源：http://sgi.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ybv.kuanghao11.cn

[Q21] 空值判断
来源：http://aur.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ynm.hongshengwenyu.top

[Q22] 排序
来源：http://xup.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://skh.sufxvd.cn

[Q23] 分页
来源：http://ngc.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://euv.pengpengdd.cyou

[Q24] 去重
来源：http://qpv.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://snt.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://hbg.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vnu.hnqzz.top

[Q26] 计数
来源：http://vph.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://yir.mhx1999.top

[Q27] 条件计数
来源：http://xlz.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wrf.yj202588.top

[Q28] 求和与平均
来源：http://hxa.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pic.hywenlv.cn

[Q29] 最大最小值
来源：http://ynk.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dtc.nanxinkj.top

[Q30] 分组统计
来源：http://caf.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tjk.havefunace.top

[Q31] 分组后过滤
来源：http://bqk.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rdy.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://ind.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ujs.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ijh.hesvh.cn


<!-- 参考信息 -->