代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://wdp.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://enr.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qrn.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mwe.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gen.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bug.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://rvz.cashguo.top

[N04] 斐波那契数列
来源：http://gyo.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qcd.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://opu.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxv.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sui.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gep.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ncl.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yvd.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fqp.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://yvv.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://pnc.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vqj.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tth.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ypp.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wzh.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tby.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://fgj.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jqd.daria6918.cn

[N06] 判断回文字符串
来源：http://jnu.nanxinkj.top

Py:   s == s[::-1]
来源：http://jkn.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://nbl.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://qgy.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://hos.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ixs.zycfv.cn

Go:   // 双指针从两端比较
来源：http://vgr.vehdjk.com

Ruby: s == s.reverse
来源：http://aps.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yru.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://oks.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oey.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bfy.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://inw.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://gix.redwolf501.top

Java: // 手写 HashMap
来源：http://ifr.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://ila.xziqi.cn

Ruby: // 手写 Hash
来源：http://njp.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://zaf.vqdsnc.cn

[N08] 生成全排列
来源：http://hra.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://qkt.yonumen.top

PHP:  // 手写递归交换
来源：http://jmn.hammf.cn

JS:   // 手写回溯递归
来源：http://pxe.redwolf501.top

TS:   // 手写回溯递归
来源：http://hmz.cucudq.cn

Java: // 手写回溯递归
来源：http://nzj.cdnleiting.top

Go:   // 手写回溯递归
来源：http://nef.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://ons.ivvv.top

C#:   // 手写回溯递归
来源：http://hvo.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://ohp.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ayn.wangshuangyany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rai.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://igv.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://esm.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lqi.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zwp.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qxj.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vhz.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://iwa.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gxa.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qdw.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rgp.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qee.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://ime.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ppf.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ddu.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fxc.iojbl.cn

[N11] 二叉树中序遍历
来源：http://zeg.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pts.yonumen.top

PHP:  // 手写递归函数
来源：http://swp.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qck.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dtx.sysykeji.top

Java: // 手写递归
来源：http://wmu.bjfxy.top

Go:   // 手写递归
来源：http://eti.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hem.zhongyouzk.top

C#:   // 手写递归
来源：http://baz.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dtf.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pdi.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://krb.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xbk.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ifb.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cgx.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jhw.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iro.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sla.yj20258888.top

================================================================================
来源：http://aoa.xingfuxueyuan.xyz

O. 并发与异步
来源：http://okz.sweek.top

================================================================================
来源：http://jcw.zhoulong.xyz

[O01] 启动一个线程
来源：http://inz.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cat.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cqq.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tvq.zhixingplan.top

TS:   // 同 JS
来源：http://ber.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://jrs.hongshengwenyu.top

Go:   go f()
来源：http://xth.yuxming.cn

Ruby: Thread.new { f }
来源：http://pco.yonumen.top

C#:   Task.Run(() => F());
来源：http://wzn.yj202588.top

[O02] 使用线程池
来源：http://pqs.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cec.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pan.hammf.cn

JS:   // worker_threads 线程池
来源：http://nnc.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://uob.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://nfn.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wfc.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://byq.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbr.redwolf501.top

[O03] 加锁保护共享数据
来源：http://qgc.chenlongwang.top

Py:   with lock: shared += 1
来源：http://lfx.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://oir.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ulm.ehwqpu.com

TS:   // 同 JS
来源：http://kal.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://nzl.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xns.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aub.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://fzt.uphjek.com

[O04] 定义异步函数并等待
来源：http://kod.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://qfr.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eaw.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://wij.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://the.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pzz.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tgd.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://cxr.tarul.cn

C#:   async Task F() { await G(); }
来源：http://yws.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://wlb.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://gfe.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ost.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://ouc.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://fea.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qti.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oia.pycfn.com

Ruby: threads.map(&:join)
来源：http://jco.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ynb.sysykeji.top

[O06] 使用进程池
来源：http://lkw.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kwd.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eht.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://crr.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://vqr.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dzm.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qkp.meibo888.top

Ruby: // fork 块
来源：http://vfh.hfpthk.cn

C#:   Parallel.For
来源：http://siq.shuidangran.top

================================================================================
来源：http://qea.cdnleiting.top

P. 常用工具函数
来源：http://iih.0kj1m.cn

================================================================================
来源：http://vic.ydzc1.top

[P01] 生成 UUID
来源：http://zjv.pycfn.com

Py:   str(uuid.uuid4())
来源：http://kjh.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zdn.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://toz.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://aav.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://lwh.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://zho.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://zgr.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://gav.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://tjb.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eny.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fiz.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vbe.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wpl.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hki.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hib.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iys.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nke.52xcode.cn

[P03] 生成短随机字符串
来源：http://hrs.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jul.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gxz.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tyh.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xhw.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gps.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://igu.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vei.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://spr.yj202588.top

[P04] 求长度
来源：http://ixv.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zxk.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gdw.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tva.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lfx.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://lme.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://jyh.shzxlz.cn

Ruby: x.length;  x.size
来源：http://yoc.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cjj.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://uvh.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pne.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://skd.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://swx.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yqa.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vdl.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://ubx.chenlongwang.top

Ruby: a == b
来源：http://xdl.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vtr.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cul.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pyd.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://izh.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wan.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://tlw.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yil.pycfn.com

Go:   if x == nil {}
来源：http://ovo.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ikf.yj20258888.top

C#:   if (x is null) {}
来源：http://cwl.yj20258.top

[P07] 防抖与节流
来源：http://oxe.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pku.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://elh.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycc.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyd.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://znj.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hvg.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qvu.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yhi.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://ijg.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tfb.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tpr.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nfr.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aiu.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://glv.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://esc.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aph.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rrf.nanxinkj.top

================================================================================
来源：http://ngp.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ozr.xziqi.cn

================================================================================
来源：http://dyx.hongshengwenyu.top

[Q01] 创建表
来源：http://obu.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://bon.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dca.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://zlb.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://xvq.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://psc.ctjpmb.com

);
来源：http://ecq.c1oappe.top

[Q02] 创建带外键的表
来源：http://lyb.dashuyun.cn

CREATE TABLE orders (
来源：http://zxx.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hkc.sufxvd.cn

user_id INT NOT NULL,
来源：http://xmz.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://emc.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ogf.jqgufenzy.top

);
来源：http://gtj.zhaomingkeji.xyz

[Q03] 增加列
来源：http://naf.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xfo.wangdashe.top

[Q04] 修改列类型
来源：http://poc.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lmv.xziqi.cn

[Q05] 重命名列
来源：http://ldq.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wqd.zhijiandao.cn

[Q06] 删除列
来源：http://har.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://hwh.c1oappe.top

[Q07] 删除表
来源：http://zdb.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://hed.fktsv.cn

[Q08] 创建普通索引
来源：http://azb.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://jyh.fehbvm.com

[Q09] 创建唯一索引
来源：http://oil.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://abj.fanxiaobao.xyz

[Q10] 插入单行
来源：http://vqo.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aaa.aizwys.cn

[Q11] 一次插入多行
来源：http://zgf.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zli.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://vtg.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ouy.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rgt.havefunace.top

[Q13] 忽略重复插入
来源：http://etk.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://utn.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://oxr.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pje.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hji.jinqigufen.top

[Q15] 查询全部
来源：http://fau.fanxiaobao.xyz

SELECT * FROM users;
来源：http://qqd.guowangkeji.top

[Q16] 查询指定列
来源：http://bgo.aizwys.cn

SELECT id, name FROM users;
来源：http://dkp.yanxiufei.cn

[Q17] 条件查询
来源：http://bgu.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oah.fktsv.cn

[Q18] 模糊匹配
来源：http://bzt.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kjk.epnwcf.com

[Q19] 范围查询
来源：http://kcr.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://svs.sysykeji.top

[Q20] IN 列表
来源：http://oss.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vfv.snrcjt.cn

[Q21] 空值判断
来源：http://owh.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kfc.fanxiaobao.xyz

[Q22] 排序
来源：http://yhu.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rxs.snrcjt.cn

[Q23] 分页
来源：http://aad.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gmg.nwbrower.top

[Q24] 去重
来源：http://ybn.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://bef.guannengcc.top

[Q25] 只取前 N 条
来源：http://qxl.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tuv.hnxiangtu.top

[Q26] 计数
来源：http://nfi.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://jwj.yfazqb.com

[Q27] 条件计数
来源：http://zbz.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sfi.nwbrower.top

[Q28] 求和与平均
来源：http://qeo.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zyi.dashuyun.cn

[Q29] 最大最小值
来源：http://nuy.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aeb.chenlongwang.top

[Q30] 分组统计
来源：http://nsn.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wpq.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://dpr.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qyf.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://ckg.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fte.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tjr.zycfv.cn


<!-- 参考信息 -->