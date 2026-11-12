代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://uau.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xzy.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://suc.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://caj.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iyj.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xcv.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://yrf.tianlin.xyz

[N04] 斐波那契数列
来源：http://xid.xinyue.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kcq.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cjr.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npm.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vjr.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mtg.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mkp.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dge.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://elj.fengsongda.top

[N05] 最大公约数
来源：http://buu.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://uim.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oog.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bnf.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ove.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ugj.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oxd.iojbl.cn

Ruby: a.gcd(b)
来源：http://vdz.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qda.cqqwz.cn

[N06] 判断回文字符串
来源：http://rxc.andypj.xyz

Py:   s == s[::-1]
来源：http://gnz.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://cyh.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://gws.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://gxm.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nbt.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://klj.tanke756.top

Ruby: s == s.reverse
来源：http://gkq.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ozv.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://tuo.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ynw.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://efp.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gdf.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://wir.hysaishi.cn

Java: // 手写 HashMap
来源：http://ain.cashguo.top

Go:   // 手写 map[int]int
来源：http://emb.yj20258.top

Ruby: // 手写 Hash
来源：http://lde.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://qen.quarkkingdee.top

[N08] 生成全排列
来源：http://jrn.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://frg.daria6918.cn

PHP:  // 手写递归交换
来源：http://xjv.fengsongda.top

JS:   // 手写回溯递归
来源：http://qaf.hywenlv.cn

TS:   // 手写回溯递归
来源：http://shz.zdqjudy.top

Java: // 手写回溯递归
来源：http://vco.yueranfly.top

Go:   // 手写回溯递归
来源：http://ydi.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://nbn.havefunace.top

C#:   // 手写回溯递归
来源：http://ggh.yj20258.top

[N09] 栈与队列
来源：http://xzx.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://grj.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bky.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pma.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jxz.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mwj.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lnn.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://efi.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bdl.tianlin.xyz

[N10] 链表节点定义
来源：http://rfu.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iph.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ayq.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ggw.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bju.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://trd.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qwl.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mtf.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ojp.yfazqb.com

[N11] 二叉树中序遍历
来源：http://gld.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://buu.wangdashe.top

PHP:  // 手写递归函数
来源：http://wuc.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xvl.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oot.ydjk.org.cn

Java: // 手写递归
来源：http://ekj.svipenyu.cn

Go:   // 手写递归
来源：http://hai.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kbo.ppjwa.cn

C#:   // 手写递归
来源：http://bad.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://owx.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kml.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fll.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hwz.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ypd.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nnz.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://umg.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hfh.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://loy.ppjwa.cn

================================================================================
来源：http://dux.52xcode.cn

O. 并发与异步
来源：http://hcq.feifeiyinyue.top

================================================================================
来源：http://qok.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://fbg.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cwo.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dyg.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kpv.tanke756.top

TS:   // 同 JS
来源：http://lhc.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://jkz.52xcode.cn

Go:   go f()
来源：http://ere.fehbvm.com

Ruby: Thread.new { f }
来源：http://bkt.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://tbc.chenzaomai.com

[O02] 使用线程池
来源：http://qqv.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://otu.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://phy.epnwcf.com

JS:   // worker_threads 线程池
来源：http://lzc.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://dio.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://amc.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rwa.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tof.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://azi.nwbrower.top

[O03] 加锁保护共享数据
来源：http://bcg.zhengqikj.top

Py:   with lock: shared += 1
来源：http://ryn.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://fgr.sysykeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mnb.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://ctg.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://akn.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qvw.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fbi.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://xfo.hcnkem.com

[O04] 定义异步函数并等待
来源：http://qos.zdbjq.cn

Py:   async def f():⏎    await g()
来源：http://yxp.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ccy.daria6918.cn

JS:   async function f() { await g(); }
来源：http://euh.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dim.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rhc.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lee.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ril.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://jjx.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://bdb.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://qfw.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xnw.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://pry.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://xvw.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwz.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pbd.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://fzr.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ddm.xylfe.cn

[O06] 使用进程池
来源：http://iwn.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hcw.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cvv.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://dxv.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://qyj.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hds.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fqi.daria6918.cn

Ruby: // fork 块
来源：http://syy.haohaochexian.top

C#:   Parallel.For
来源：http://wby.hywenlv.cn

================================================================================
来源：http://ftb.gaohongyu789.top

P. 常用工具函数
来源：http://jfx.xylfe.cn

================================================================================
来源：http://zfc.jiagoushi.top

[P01] 生成 UUID
来源：http://jtp.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://srx.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xhg.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://dsz.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://oxl.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://zph.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://jjd.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://vtm.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://aaa.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://zky.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygt.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wuf.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://inj.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rhi.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ype.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cco.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://znz.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cju.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://xgy.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slt.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jxg.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://giv.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqc.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bhc.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vff.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wqq.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://opp.dashuyun.cn

[P04] 求长度
来源：http://nrm.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://juh.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lfy.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://knd.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stl.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://uwc.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://vlm.dashuyun.cn

Ruby: x.length;  x.size
来源：http://tqc.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iys.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://uoa.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://ggh.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bbq.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://adn.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ixw.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dbv.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uki.fanxiaobao.xyz

Ruby: a == b
来源：http://kou.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gzx.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hfa.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mwv.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://cei.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xss.vqdsnc.cn

TS:   if (x == null) {}
来源：http://eza.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gjl.yuxming.cn

Go:   if x == nil {}
来源：http://gac.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://raz.epnwcf.com

C#:   if (x is null) {}
来源：http://jgc.0kj1m.cn

[P07] 防抖与节流
来源：http://mdx.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vbl.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://jzc.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odc.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkb.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zwh.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sbz.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://dcp.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dcs.hammf.cn

[P08] 处理浮点精度问题
来源：http://cdt.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gwu.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zxl.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gim.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vrh.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://noh.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cyn.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kfb.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://esb.wangshuangyany.cn

================================================================================
来源：http://ucl.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://szu.iojbl.cn

================================================================================
来源：http://uad.ydzc1.top

[Q01] 创建表
来源：http://mgc.yanxiufei.cn

CREATE TABLE users (
来源：http://ilr.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ory.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://ecf.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://hva.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aco.xziqi.cn

);
来源：http://ogl.fktsv.cn

[Q02] 创建带外键的表
来源：http://vjd.guannengcc.top

CREATE TABLE orders (
来源：http://psc.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nfb.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://bqd.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://sgr.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mka.fanxiaobao.xyz

);
来源：http://zzi.jqgufenzy.top

[Q03] 增加列
来源：http://xqb.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xbw.bjfxy.top

[Q04] 修改列类型
来源：http://ntz.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vgj.jiagoushi.top

[Q05] 重命名列
来源：http://kjy.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://odw.tian-w.cn

[Q06] 删除列
来源：http://xcl.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://wpv.shangyingyoupin.top

[Q07] 删除表
来源：http://nwt.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://xgg.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://asb.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xww.nanxinkj.top

[Q09] 创建唯一索引
来源：http://xvw.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hru.quarkkingdee.top

[Q10] 插入单行
来源：http://xnx.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lqs.redwolf501.top

[Q11] 一次插入多行
来源：http://llx.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hqo.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://jop.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://yyr.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fll.fzhhl.top

[Q13] 忽略重复插入
来源：http://gpv.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://syk.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://vgz.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://arm.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://idz.zhengqikj.top

[Q15] 查询全部
来源：http://mgv.daxiang520.top

SELECT * FROM users;
来源：http://jrg.xziqi.cn

[Q16] 查询指定列
来源：http://mad.tanke756.top

SELECT id, name FROM users;
来源：http://vyu.jianghu66.top

[Q17] 条件查询
来源：http://lcw.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gno.ppjwa.cn

[Q18] 模糊匹配
来源：http://gui.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oce.fanxiaobao.xyz

[Q19] 范围查询
来源：http://vnn.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qaf.hcnkem.com

[Q20] IN 列表
来源：http://ahx.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pgy.hcnkem.com

[Q21] 空值判断
来源：http://pwq.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ryv.daria6918.cn

[Q22] 排序
来源：http://ljn.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mhe.guannengcc.top

[Q23] 分页
来源：http://yix.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sas.yonumen.top

[Q24] 去重
来源：http://bgk.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://yok.iojbl.cn

[Q25] 只取前 N 条
来源：http://yda.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://doh.xuanzx.com

[Q26] 计数
来源：http://woi.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://nfd.yvedp.cn

[Q27] 条件计数
来源：http://itt.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uhd.sufxvd.cn

[Q28] 求和与平均
来源：http://vyg.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hwz.cheryme.top

[Q29] 最大最小值
来源：http://sft.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vfl.hesvh.cn

[Q30] 分组统计
来源：http://ekj.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kth.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://oeg.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vcm.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://pui.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ibg.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://thn.fktsv.cn


<!-- 参考信息 -->