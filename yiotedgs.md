代发 wailian999

Ruby: arr.sort
来源：http://fqb.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://djn.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://jop.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pna.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://gyd.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://btf.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uft.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rnu.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhb.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qcd.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://mqu.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://btj.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://agj.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mfu.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://brn.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zqu.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hom.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://khl.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cre.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qnt.yj20258.top

[N05] 最大公约数
来源：http://uie.hnqzz.top

Py:   math.gcd(a, b)
来源：http://azy.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://quz.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eyo.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sex.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cux.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cbn.tianlin.xyz

Ruby: a.gcd(b)
来源：http://big.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tar.daria6918.cn

[N06] 判断回文字符串
来源：http://eqf.nanxinkj.top

Py:   s == s[::-1]
来源：http://tuw.cucudq.cn

PHP:  $s === strrev($s);
来源：http://fxm.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://omj.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://cla.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nuk.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://nyh.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://obl.fzhhl.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vta.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://qtf.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gcm.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vcv.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vny.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://uxb.cashguo.top

Java: // 手写 HashMap
来源：http://crk.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://jwx.xylfe.cn

Ruby: // 手写 Hash
来源：http://wzj.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://orf.ehwqpu.com

[N08] 生成全排列
来源：http://cfe.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://qsf.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://mkj.cqqwz.cn

JS:   // 手写回溯递归
来源：http://flt.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://khw.jqgfzy.top

Java: // 手写回溯递归
来源：http://zpy.ctjpmb.com

Go:   // 手写回溯递归
来源：http://gtl.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://mtu.hesvh.cn

C#:   // 手写回溯递归
来源：http://nmm.tarul.cn

[N09] 栈与队列
来源：http://xnr.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yui.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dnc.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xdn.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yol.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bxc.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hry.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wna.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://thu.ivvv.top

[N10] 链表节点定义
来源：http://gcb.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://njd.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rrw.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nmu.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qso.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://mxj.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pyl.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://njs.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ipi.bjfxy.top

[N11] 二叉树中序遍历
来源：http://vvv.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cup.bjfxy.top

PHP:  // 手写递归函数
来源：http://jly.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kbu.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bvp.hesvh.cn

Java: // 手写递归
来源：http://xdy.hysaishi.cn

Go:   // 手写递归
来源：http://afx.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sbn.hywenlv.cn

C#:   // 手写递归
来源：http://vel.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ibv.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jwo.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://erz.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oia.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tso.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pkn.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rut.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ijd.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sao.chenjidiqi.icu

================================================================================
来源：http://okl.jinqigufen.top

O. 并发与异步
来源：http://pqp.jqgufenzy.top

================================================================================
来源：http://ylw.jinqigufen.top

[O01] 启动一个线程
来源：http://ykx.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hpb.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gef.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sdd.haohaochexian.top

TS:   // 同 JS
来源：http://aby.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://rch.jinyuanbaomall.cn

Go:   go f()
来源：http://ybp.hywenlv.cn

Ruby: Thread.new { f }
来源：http://wdw.fengsongda.top

C#:   Task.Run(() => F());
来源：http://wmj.hesvh.cn

[O02] 使用线程池
来源：http://skc.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zgz.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://npx.aizwys.cn

JS:   // worker_threads 线程池
来源：http://mte.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://bwb.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ftq.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wep.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ssj.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jqg.cqqwz.cn

[O03] 加锁保护共享数据
来源：http://kdc.tian-w.cn

Py:   with lock: shared += 1
来源：http://qwu.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://cpm.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ykg.guowangkeji.top

TS:   // 同 JS
来源：http://noo.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://npd.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nvm.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kex.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://nvz.fzhhl.top

[O04] 定义异步函数并等待
来源：http://kxf.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://zxd.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oui.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://gyj.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bpq.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ifo.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rlf.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://amj.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://skq.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://cvo.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://lvo.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bii.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://jbk.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://rku.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tyj.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fjj.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://kam.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gnb.chenlongwang.top

[O06] 使用进程池
来源：http://yld.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sdv.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gim.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://jzw.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://oia.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xnd.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ssa.zhoulong.xyz

Ruby: // fork 块
来源：http://sqs.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://vif.zhongyouzk.top

================================================================================
来源：http://oxo.52xcode.cn

P. 常用工具函数
来源：http://njv.zhengqikj.top

================================================================================
来源：http://ksg.ehwqpu.com

[P01] 生成 UUID
来源：http://qdo.yj20258.top

Py:   str(uuid.uuid4())
来源：http://nph.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rxp.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://tak.bjfxy.top

TS:   crypto.randomUUID()
来源：http://qwk.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://pgu.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://ker.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://opc.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://emi.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://gta.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xfd.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://msm.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zdg.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iix.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ugx.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mvx.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mpm.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vnp.cheryme.top

[P03] 生成短随机字符串
来源：http://bya.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lxb.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://edh.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wiy.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rio.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ouo.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lud.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gij.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aei.jinghuilouyu.cn

[P04] 求长度
来源：http://sch.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hdi.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtt.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://use.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vux.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://wga.aizwys.cn

Go:   len(arr);  len(m)
来源：http://ont.hnqzz.top

Ruby: x.length;  x.size
来源：http://dgi.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tbe.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://szl.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://fam.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://epi.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wdb.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cri.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dat.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://abg.0kj1m.cn

Ruby: a == b
来源：http://uis.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iha.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kga.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oyy.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://mrf.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gco.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://gjc.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fip.xuetiantiany.cn

Go:   if x == nil {}
来源：http://zjq.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jlh.yongpay.top

C#:   if (x is null) {}
来源：http://zma.hesvh.cn

[P07] 防抖与节流
来源：http://rfo.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://epn.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://gyo.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgi.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rbq.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ito.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://srh.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ruo.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gnu.yj202588.top

[P08] 处理浮点精度问题
来源：http://ngb.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://obk.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://emx.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gbx.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sib.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mtt.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tkk.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kaq.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xqn.ehwqpu.com

================================================================================
来源：http://myr.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fuy.fengsongda.top

================================================================================
来源：http://qxs.jqgfzy.top

[Q01] 创建表
来源：http://qdp.fzhhl.top

CREATE TABLE users (
来源：http://ten.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ade.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://vhh.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://dmt.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jbe.yuanzhike.top

);
来源：http://kfu.jinqigufen.top

[Q02] 创建带外键的表
来源：http://ndv.gogol.net.cn

CREATE TABLE orders (
来源：http://oge.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvo.tanke756.top

user_id INT NOT NULL,
来源：http://iib.redwolf501.top

amount DECIMAL(10, 2),
来源：http://edi.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dpa.52xcode.cn

);
来源：http://oqr.hammf.cn

[Q03] 增加列
来源：http://mzp.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kyb.meibo888.top

[Q04] 修改列类型
来源：http://ykv.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cbc.cdnleiting.top

[Q05] 重命名列
来源：http://zem.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://two.yangfankeji.com

[Q06] 删除列
来源：http://tma.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hey.bbcook.cn

[Q07] 删除表
来源：http://zkj.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://xzl.zycfv.cn

[Q08] 创建普通索引
来源：http://hbm.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gzb.guannengcc.top

[Q09] 创建唯一索引
来源：http://kyj.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qeb.guannengcc.top

[Q10] 插入单行
来源：http://ksb.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zbo.cdnleiting.top

[Q11] 一次插入多行
来源：http://yyt.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gkb.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://tgv.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gmv.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://grk.fehbvm.com

[Q13] 忽略重复插入
来源：http://vao.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xun.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://hug.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oct.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ice.hongshengwenyu.top

[Q15] 查询全部
来源：http://tjo.havefunace.top

SELECT * FROM users;
来源：http://wfm.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://sjg.sysykeji.top

SELECT id, name FROM users;
来源：http://hnx.sysykeji.top

[Q17] 条件查询
来源：http://ftn.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sgy.hcnkem.com

[Q18] 模糊匹配
来源：http://umx.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uiw.zdbjq.cn

[Q19] 范围查询
来源：http://ndb.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jar.52xcode.cn

[Q20] IN 列表
来源：http://liz.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mnw.hcnkem.com

[Q21] 空值判断
来源：http://dil.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mze.xylfe.cn

[Q22] 排序
来源：http://ege.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vrb.tianlin.xyz

[Q23] 分页
来源：http://tbg.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hfu.sufxvd.cn

[Q24] 去重
来源：http://bld.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://hue.daria6918.cn

[Q25] 只取前 N 条
来源：http://ekg.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mgp.hcnkem.com

[Q26] 计数
来源：http://ygm.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://ucq.pengpengdd.cyou

[Q27] 条件计数
来源：http://ezw.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yoy.fzhhl.top

[Q28] 求和与平均
来源：http://tgh.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vzf.xziqi.cn

[Q29] 最大最小值
来源：http://ksg.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zlu.haohaochexian.top

[Q30] 分组统计
来源：http://sbc.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qup.zhixingplan.top

[Q31] 分组后过滤
来源：http://gfy.jinqigufen.top


<!-- 参考信息 -->