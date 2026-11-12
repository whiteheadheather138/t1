代发 wailian999

Ruby: arr.sort
来源：http://ryy.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ieu.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://iew.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bsm.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://pzj.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cnd.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zwd.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nyy.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhd.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://edz.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://frk.epnwcf.com

[N04] 斐波那契数列
来源：http://oua.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cas.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dvd.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sca.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ryp.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pjt.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fns.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ymx.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aqv.svipenyu.cn

[N05] 最大公约数
来源：http://eod.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://mue.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hdi.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aah.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zys.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kvt.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dpp.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://vlm.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fjg.aizwys.cn

[N06] 判断回文字符串
来源：http://qhp.zdbjq.cn

Py:   s == s[::-1]
来源：http://uqy.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://mtm.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://gdb.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://dwh.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://klr.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://qxk.epnwcf.com

Ruby: s == s.reverse
来源：http://jfl.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xhn.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://vfi.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hzk.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nrs.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://aqp.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://sfs.daxiang520.top

Java: // 手写 HashMap
来源：http://sge.uphjek.com

Go:   // 手写 map[int]int
来源：http://rcc.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://zrb.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://jgl.316326.xyz

[N08] 生成全排列
来源：http://uos.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://vhv.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://bkr.ctjpmb.com

JS:   // 手写回溯递归
来源：http://geh.cqqwz.cn

TS:   // 手写回溯递归
来源：http://rgs.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://hzc.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://zcu.yonumen.top

Ruby: arr.permutation.to_a
来源：http://xpk.jyoumei.cn

C#:   // 手写回溯递归
来源：http://rwb.shzxlz.cn

[N09] 栈与队列
来源：http://hcx.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://meb.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ycg.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ayb.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oqe.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qrq.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fqp.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qud.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fim.aibaodan.cn

[N10] 链表节点定义
来源：http://zak.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tqj.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://igv.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qsz.yj202588.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ajc.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://iov.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://gjj.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cga.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kfp.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://qpd.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bjt.cdnleiting.top

PHP:  // 手写递归函数
来源：http://hwk.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awv.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlj.gotoacloud.top

Java: // 手写递归
来源：http://nag.xinyue.icu

Go:   // 手写递归
来源：http://gcb.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cwq.yangfankeji.com

C#:   // 手写递归
来源：http://ipk.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dbz.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vhn.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wtz.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mvn.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cip.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zjf.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dsk.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vlt.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://elm.tianlin.xyz

================================================================================
来源：http://our.ehwqpu.com

O. 并发与异步
来源：http://imm.feifeiyinyue.top

================================================================================
来源：http://wkr.hcnkem.com

[O01] 启动一个线程
来源：http://sta.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jjb.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gdu.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pmi.ehwqpu.com

TS:   // 同 JS
来源：http://llp.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://cde.pengpengdd.cyou

Go:   go f()
来源：http://nwo.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://eyf.andypj.xyz

C#:   Task.Run(() => F());
来源：http://jva.fktsv.cn

[O02] 使用线程池
来源：http://sdi.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mok.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dmu.guannengcc.top

JS:   // worker_threads 线程池
来源：http://bft.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://fjd.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://qbi.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://efm.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lbr.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qjd.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://qvw.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://ory.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://jdz.hfpthk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qbk.guannengcc.top

TS:   // 同 JS
来源：http://ydb.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://clk.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lhg.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vke.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://ois.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://rps.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://pno.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ktl.meibo888.top

JS:   async function f() { await g(); }
来源：http://afe.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vkf.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dto.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ata.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://nri.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://uem.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://igp.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://izs.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://unr.yongpay.top

JS:   await Promise.all(tasks)
来源：http://pdv.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://nwp.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vzm.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uyt.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://pmg.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bom.sjlbkw.cn

[O06] 使用进程池
来源：http://uhj.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mjw.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://idc.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://aln.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://cab.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pfk.jyoumei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qsl.shangyingyoupin.top

Ruby: // fork 块
来源：http://wno.shuidangran.top

C#:   Parallel.For
来源：http://ssl.yanxiufei.cn

================================================================================
来源：http://ymz.fzhhl.top

P. 常用工具函数
来源：http://fng.316326.xyz

================================================================================
来源：http://oxv.yongpay.top

[P01] 生成 UUID
来源：http://wqi.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://ycu.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dnq.uphjek.com

JS:   crypto.randomUUID()
来源：http://kcb.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://dit.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://mol.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://woi.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://tyb.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://ayp.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://qag.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cmm.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qoi.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fci.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rwk.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mau.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fch.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xgt.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zpo.yj20258888.top

[P03] 生成短随机字符串
来源：http://lpq.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rhn.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kkw.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vho.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owf.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://upw.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://awb.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zfs.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mao.pengpengdd.cyou

[P04] 求长度
来源：http://rip.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oel.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dad.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://anh.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kgc.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://suq.birdmap.top

Go:   len(arr);  len(m)
来源：http://lcs.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://ojz.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hcl.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://meb.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qug.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yjp.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hhl.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aml.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://txb.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://amp.nwbrower.top

Ruby: a == b
来源：http://uyp.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fwc.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dsj.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aiy.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://vng.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bin.cashguo.top

TS:   if (x == null) {}
来源：http://bhr.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://avl.jqgufenzy.top

Go:   if x == nil {}
来源：http://uzd.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nyt.xuanzx.com

C#:   if (x is null) {}
来源：http://auz.jqgfzy.top

[P07] 防抖与节流
来源：http://fbz.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mtn.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://ile.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dns.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://roy.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uck.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uic.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dgw.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nzb.uphjek.com

[P08] 处理浮点精度问题
来源：http://zkg.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kbd.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgw.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xac.ydjk.org.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ydk.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eky.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yqr.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dzi.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mks.mhx1999.top

================================================================================
来源：http://epw.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dhb.hongshengwenyu.top

================================================================================
来源：http://opd.sjlbkw.cn

[Q01] 创建表
来源：http://bpt.316326.xyz

CREATE TABLE users (
来源：http://uwc.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpo.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://lor.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://dpe.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pfv.sufxvd.cn

);
来源：http://ooq.cashguo.top

[Q02] 创建带外键的表
来源：http://zxe.cqqwz.cn

CREATE TABLE orders (
来源：http://hqy.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://twv.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://npo.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://lle.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://awa.jiagoushi.top

);
来源：http://zpt.yj202588.top

[Q03] 增加列
来源：http://xzk.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ebn.zhoulong.xyz

[Q04] 修改列类型
来源：http://vxh.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ruc.hysaishi.cn

[Q05] 重命名列
来源：http://hlx.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqz.cashguo.top

[Q06] 删除列
来源：http://jgy.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://khy.dianchejie.cn

[Q07] 删除表
来源：http://onw.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://nev.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://orw.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tqg.guowangkeji.top

[Q09] 创建唯一索引
来源：http://rke.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fhi.zhiwuduotai.top

[Q10] 插入单行
来源：http://vvq.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fdy.fktsv.cn

[Q11] 一次插入多行
来源：http://jja.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gpt.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://esz.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hhx.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iuz.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://yrs.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kig.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://tns.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rep.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gdi.zdbjq.cn

[Q15] 查询全部
来源：http://wcy.tarul.cn

SELECT * FROM users;
来源：http://bwu.hnqzz.top

[Q16] 查询指定列
来源：http://brw.zhijiandao.cn

SELECT id, name FROM users;
来源：http://xon.fehbvm.com

[Q17] 条件查询
来源：http://oat.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aad.sweek.top

[Q18] 模糊匹配
来源：http://twy.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ulu.xuanzx.com

[Q19] 范围查询
来源：http://fbv.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cnd.316326.xyz

[Q20] IN 列表
来源：http://awu.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://btq.ppjwa.cn

[Q21] 空值判断
来源：http://mdi.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qqg.nanxuanxn.top

[Q22] 排序
来源：http://oei.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://del.redwolf501.top

[Q23] 分页
来源：http://qgi.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hid.ybcxt.top

[Q24] 去重
来源：http://xrf.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://nuk.gotoacloud.top

[Q25] 只取前 N 条
来源：http://ddc.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fgy.wangdashe.top

[Q26] 计数
来源：http://uax.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://tno.daxiang520.top

[Q27] 条件计数
来源：http://lbp.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dej.gotoacloud.top

[Q28] 求和与平均
来源：http://vrj.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://moy.yvedp.cn

[Q29] 最大最小值
来源：http://sgk.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://orv.9152youxi.cn

[Q30] 分组统计
来源：http://gog.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vtj.andypj.xyz

[Q31] 分组后过滤
来源：http://szz.ppjwa.cn


<!-- 参考信息 -->