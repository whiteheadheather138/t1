代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://xvs.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nbj.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mjf.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mwb.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vse.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uhw.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tlp.nwbrower.top

[N04] 斐波那契数列
来源：http://nya.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://shl.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xcf.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dcy.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rxm.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pct.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qcd.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xlw.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pck.aizwys.cn

[N05] 最大公约数
来源：http://zbu.hammf.cn

Py:   math.gcd(a, b)
来源：http://yqf.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sdo.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fjc.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bnm.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gkt.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iza.jyoumei.cn

Ruby: a.gcd(b)
来源：http://gko.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dla.yj20258.top

[N06] 判断回文字符串
来源：http://vda.yuxming.cn

Py:   s == s[::-1]
来源：http://rjx.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://xsb.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://cso.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://tjm.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gdf.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://oeb.hfpthk.cn

Ruby: s == s.reverse
来源：http://twe.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kwa.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://jxv.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cpj.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cte.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ruj.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://hvm.kuanghao11.cn

Java: // 手写 HashMap
来源：http://idj.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://oyc.guowangkeji.top

Ruby: // 手写 Hash
来源：http://fzt.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://abq.xuanzx.com

[N08] 生成全排列
来源：http://zdu.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://kjl.zhixingplan.top

PHP:  // 手写递归交换
来源：http://boy.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://efr.uphjek.com

TS:   // 手写回溯递归
来源：http://dsk.meibo888.top

Java: // 手写回溯递归
来源：http://nqm.cqqwz.cn

Go:   // 手写回溯递归
来源：http://xxy.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://fon.aibaodan.cn

C#:   // 手写回溯递归
来源：http://tds.jlsjyb.cn

[N09] 栈与队列
来源：http://prz.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lpx.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ezo.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lrd.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nuc.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dld.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yry.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bwj.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tse.shuidangran.top

[N10] 链表节点定义
来源：http://fln.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rma.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lrc.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vec.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gar.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://qld.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://hvb.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bwb.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://atu.yvedp.cn

[N11] 二叉树中序遍历
来源：http://lwr.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://asq.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://exc.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ukm.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xjv.hcnkem.com

Java: // 手写递归
来源：http://zqs.zdbjq.cn

Go:   // 手写递归
来源：http://ivm.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bmx.zycfv.cn

C#:   // 手写递归
来源：http://xcc.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fka.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ajd.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fwj.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqr.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://chq.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hri.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ruw.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zct.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgo.xylfe.cn

================================================================================
来源：http://drf.fehbvm.com

O. 并发与异步
来源：http://ppl.xziqi.cn

================================================================================
来源：http://pme.daria6918.cn

[O01] 启动一个线程
来源：http://rkj.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jcr.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fjl.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tdp.xuanzx.com

TS:   // 同 JS
来源：http://mvt.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://uoq.jyoumei.cn

Go:   go f()
来源：http://mlj.yj20258.top

Ruby: Thread.new { f }
来源：http://wkz.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://tvh.guannengcc.top

[O02] 使用线程池
来源：http://esl.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vyp.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ssd.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://ika.yueranfly.top

TS:   // worker_threads 线程池
来源：http://lzp.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://fui.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mkf.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lan.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iti.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://kzw.shuidangran.top

Py:   with lock: shared += 1
来源：http://akf.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://bud.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wce.wangshuangyany.cn

TS:   // 同 JS
来源：http://qsk.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://wuz.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jbf.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eia.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://eao.fengsongda.top

[O04] 定义异步函数并等待
来源：http://wqq.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://pez.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iei.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://tep.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bjz.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gnh.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wsi.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ptn.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://sxc.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://yls.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://zqh.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pef.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://iql.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://zvg.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yof.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wka.daria6918.cn

Ruby: threads.map(&:join)
来源：http://wwx.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wqb.aibaodan.cn

[O06] 使用进程池
来源：http://epl.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://egv.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iti.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://lar.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://rms.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ddl.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pgx.xuetiantiany.cn

Ruby: // fork 块
来源：http://xxw.gotoacloud.top

C#:   Parallel.For
来源：http://hoh.vqdsnc.cn

================================================================================
来源：http://cpq.sjlbkw.cn

P. 常用工具函数
来源：http://sca.gogol.net.cn

================================================================================
来源：http://slf.sweek.top

[P01] 生成 UUID
来源：http://plb.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://gjn.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pwi.sweek.top

JS:   crypto.randomUUID()
来源：http://iws.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://fvo.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://ofu.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://uua.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://fdq.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://sch.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://fcm.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://axz.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qdu.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://njj.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vhh.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://scs.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://les.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ftk.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iur.gotoacloud.top

[P03] 生成短随机字符串
来源：http://aqn.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dpj.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jif.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://elm.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flk.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nit.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nlb.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://vsq.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lzu.tanke756.top

[P04] 求长度
来源：http://rim.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://een.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbx.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tsz.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqj.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://gwx.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://yqs.aibaodan.cn

Ruby: x.length;  x.size
来源：http://iee.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://evu.ydzc1.top

[P05] 判断两个对象内容是否相等
来源：http://hdg.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://bmx.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fyq.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nkn.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://epl.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qcn.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vyb.yuanzhike.top

Ruby: a == b
来源：http://lpm.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wlc.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nbq.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://chd.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://skf.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tyv.jinqigfzy.top

TS:   if (x == null) {}
来源：http://kjc.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mhd.vqdsnc.cn

Go:   if x == nil {}
来源：http://fga.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rjq.mhx1999.top

C#:   if (x is null) {}
来源：http://cty.sxryk.cn

[P07] 防抖与节流
来源：http://oys.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yrj.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://aue.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qzc.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyf.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qko.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nkc.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zhy.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yxg.havefunace.top

[P08] 处理浮点精度问题
来源：http://uaf.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urj.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cwq.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqh.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://usw.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gqv.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qyu.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pgg.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bxw.dashuyun.cn

================================================================================
来源：http://bqo.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pfq.shuidangran.top

================================================================================
来源：http://qdu.ehwqpu.com

[Q01] 创建表
来源：http://ypx.quarkkingdee.top

CREATE TABLE users (
来源：http://njs.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kfu.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://kak.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://gpc.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://itc.xylfe.cn

);
来源：http://dxj.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://rlo.pengpengdd.cyou

CREATE TABLE orders (
来源：http://lxy.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cbx.yuxming.cn

user_id INT NOT NULL,
来源：http://int.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://qsx.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://thq.nwbrower.top

);
来源：http://tfp.guannengcc.top

[Q03] 增加列
来源：http://jxb.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nbd.yuxming.cn

[Q04] 修改列类型
来源：http://omf.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xeh.52xcode.cn

[Q05] 重命名列
来源：http://yyz.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ufn.hesvh.cn

[Q06] 删除列
来源：http://wob.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://ejj.chenjidiqi.icu

[Q07] 删除表
来源：http://xet.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://vom.ctjpmb.com

[Q08] 创建普通索引
来源：http://snw.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pmm.zdbjq.cn

[Q09] 创建唯一索引
来源：http://pud.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xss.jinqigfzy.top

[Q10] 插入单行
来源：http://ukx.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zry.zhengqikj.top

[Q11] 一次插入多行
来源：http://sqb.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ozr.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://pec.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://obe.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dqn.cqqwz.cn

[Q13] 忽略重复插入
来源：http://qgf.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lcm.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://loj.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://elr.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gjb.ctjpmb.com

[Q15] 查询全部
来源：http://ohn.shanyushiyangtech.top

SELECT * FROM users;
来源：http://ora.hnxiangtu.top

[Q16] 查询指定列
来源：http://kvi.jlsjyb.cn

SELECT id, name FROM users;
来源：http://hat.shzxlz.cn

[Q17] 条件查询
来源：http://fqp.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mow.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://qyq.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mue.shzxlz.cn

[Q19] 范围查询
来源：http://seu.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://imj.sxryk.cn

[Q20] IN 列表
来源：http://jxf.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lkw.jyoumei.cn

[Q21] 空值判断
来源：http://cri.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zlw.yueranfly.top

[Q22] 排序
来源：http://nzp.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://twi.smart0.xyz

[Q23] 分页
来源：http://idj.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wvh.sweek.top

[Q24] 去重
来源：http://vqy.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://hwq.zhengqikj.top

[Q25] 只取前 N 条
来源：http://mry.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nnj.jlsjyb.cn

[Q26] 计数
来源：http://tgr.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://nds.birdmap.top

[Q27] 条件计数
来源：http://tjk.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xun.aibaodan.cn

[Q28] 求和与平均
来源：http://sae.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bmd.zhongyouzk.top

[Q29] 最大最小值
来源：http://die.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://wie.wangshuangyany.cn

[Q30] 分组统计
来源：http://kcz.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jbm.sufxvd.cn

[Q31] 分组后过滤
来源：http://xot.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hud.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://bjy.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://toa.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gmo.hnxiangtu.top


<!-- 参考信息 -->