代发 wailian999

Ruby: arr.sort
来源：http://vby.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xuu.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://ruh.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://puj.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://kum.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vaw.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rtr.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jrf.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dsc.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsz.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://vxz.aizwys.cn

[N04] 斐波那契数列
来源：http://kws.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vlr.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uca.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vub.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hde.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://azb.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pra.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qit.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kqk.tarul.cn

[N05] 最大公约数
来源：http://bzb.hammf.cn

Py:   math.gcd(a, b)
来源：http://nog.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dwx.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgj.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://okm.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yem.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ovq.sufxvd.cn

Ruby: a.gcd(b)
来源：http://mev.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://obb.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://acd.aizwys.cn

Py:   s == s[::-1]
来源：http://ila.zycfv.cn

PHP:  $s === strrev($s);
来源：http://orl.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://ikj.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://eth.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gcx.bjfxy.top

Go:   // 双指针从两端比较
来源：http://rgd.ehwqpu.com

Ruby: s == s.reverse
来源：http://xhi.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xqf.cheryme.top

[N07] 两数之和（返回下标）
来源：http://nha.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://suh.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://trz.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mzo.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://sqa.jinqigfzy.top

Java: // 手写 HashMap
来源：http://ufm.nwbrower.top

Go:   // 手写 map[int]int
来源：http://ruu.ppjwa.cn

Ruby: // 手写 Hash
来源：http://tep.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jpn.xylfe.cn

[N08] 生成全排列
来源：http://wry.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://oaj.xuanzx.com

PHP:  // 手写递归交换
来源：http://sag.nwbrower.top

JS:   // 手写回溯递归
来源：http://dmj.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://pwo.shuidangran.top

Java: // 手写回溯递归
来源：http://wba.bbcook.cn

Go:   // 手写回溯递归
来源：http://klg.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://phb.c1oappe.top

C#:   // 手写回溯递归
来源：http://mnx.cheryme.top

[N09] 栈与队列
来源：http://dbl.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uyj.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://grv.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mad.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hqf.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ezl.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://acd.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://koo.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://afn.gaohongyu789.top

[N10] 链表节点定义
来源：http://iox.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ski.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://zqo.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tid.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ppq.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://zmw.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://whg.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://psi.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vvb.xuanzx.com

[N11] 二叉树中序遍历
来源：http://upn.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oht.ppjwa.cn

PHP:  // 手写递归函数
来源：http://hld.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://paw.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bdw.zycfv.cn

Java: // 手写递归
来源：http://sbt.quarkkingdee.top

Go:   // 手写递归
来源：http://adj.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ahw.hcnkem.com

C#:   // 手写递归
来源：http://rrs.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ote.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ynk.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://piz.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sqg.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ucz.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aba.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ucr.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jsa.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tvx.aizwys.cn

================================================================================
来源：http://zrr.ppjwa.cn

O. 并发与异步
来源：http://ysn.smart0.xyz

================================================================================
来源：http://add.zhiwuduotai.top

[O01] 启动一个线程
来源：http://sco.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fui.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tal.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xuh.cashguo.top

TS:   // 同 JS
来源：http://rwq.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://qjb.kuanghao11.cn

Go:   go f()
来源：http://aee.meibo888.top

Ruby: Thread.new { f }
来源：http://rcq.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://jqh.zhengqikj.top

[O02] 使用线程池
来源：http://xoq.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cmo.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://apj.xinyue.icu

JS:   // worker_threads 线程池
来源：http://ese.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://ulc.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://jqf.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://toc.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rhi.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zbl.yfazqb.com

[O03] 加锁保护共享数据
来源：http://vie.tanke756.top

Py:   with lock: shared += 1
来源：http://uil.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://ohj.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://csn.zhixingplan.top

TS:   // 同 JS
来源：http://gke.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://huz.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tqc.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pcr.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://oae.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://lko.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://erv.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yzw.ivvv.top

JS:   async function f() { await g(); }
来源：http://dwb.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://krq.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kll.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ovo.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://som.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://cso.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://ptt.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://tkk.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cyj.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://jbn.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://ccm.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qko.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gqr.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://seh.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hjd.dashuyun.cn

[O06] 使用进程池
来源：http://cyo.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://krx.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ive.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://zdu.hammf.cn

TS:   // child_process / cluster 模块
来源：http://qal.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yfk.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ecx.tianlin.xyz

Ruby: // fork 块
来源：http://ohw.shzxlz.cn

C#:   Parallel.For
来源：http://szr.fzhhl.top

================================================================================
来源：http://vcr.daria6918.cn

P. 常用工具函数
来源：http://sxx.jinqigufen.top

================================================================================
来源：http://arx.andypj.xyz

[P01] 生成 UUID
来源：http://cfr.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://roi.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://awj.ybcxt.top

JS:   crypto.randomUUID()
来源：http://oiu.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://jpy.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://epz.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://gkm.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://hwl.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://ttt.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://rqz.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fhd.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://flx.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pjt.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jve.ivvv.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jdg.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jon.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gdo.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tak.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://tce.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mpx.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yid.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jlo.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://djk.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hzc.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ulg.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kzt.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ofy.fengsongda.top

[P04] 求长度
来源：http://ikr.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://omb.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cec.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://htg.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cxv.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://yva.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://ywq.guowangkeji.top

Ruby: x.length;  x.size
来源：http://hle.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://snd.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://pvt.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://wxd.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xto.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zie.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xiu.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nux.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nkf.meibo888.top

Ruby: a == b
来源：http://meb.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rvo.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://omj.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mku.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://myv.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iyh.cdnleiting.top

TS:   if (x == null) {}
来源：http://kpy.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cyd.yj20258.top

Go:   if x == nil {}
来源：http://qhc.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://swh.andypj.xyz

C#:   if (x is null) {}
来源：http://ddh.sysykeji.top

[P07] 防抖与节流
来源：http://uyt.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rzo.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://ebt.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxw.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ure.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xid.chenzaomai.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kto.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lez.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xmn.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://ofi.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://txp.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wma.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mxs.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lcc.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://atq.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ykn.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://emj.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://azl.shzxlz.cn

================================================================================
来源：http://pvw.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xqv.chenlongwang.top

================================================================================
来源：http://zka.hammf.cn

[Q01] 创建表
来源：http://der.52xcode.cn

CREATE TABLE users (
来源：http://ooa.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ztk.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://jsg.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://fil.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vgm.cdnleiting.top

);
来源：http://gwy.vehdjk.com

[Q02] 创建带外键的表
来源：http://bqs.yfazqb.com

CREATE TABLE orders (
来源：http://edb.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rne.meibo888.top

user_id INT NOT NULL,
来源：http://xpm.andypj.xyz

amount DECIMAL(10, 2),
来源：http://tbw.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ipi.shangyingyoupin.top

);
来源：http://otk.uphjek.com

[Q03] 增加列
来源：http://fyz.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yml.zdqjudy.top

[Q04] 修改列类型
来源：http://msz.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zba.gaohongyu789.top

[Q05] 重命名列
来源：http://jxj.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uok.shuidangran.top

[Q06] 删除列
来源：http://wdf.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sfx.hywenlv.cn

[Q07] 删除表
来源：http://hlv.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://cih.tanke756.top

[Q08] 创建普通索引
来源：http://kop.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pko.yueranfly.top

[Q09] 创建唯一索引
来源：http://gcl.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kbq.yvedp.cn

[Q10] 插入单行
来源：http://pqr.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nrl.kuanghao11.cn

[Q11] 一次插入多行
来源：http://kam.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xko.yongpay.top

[Q12] 插入后取自增 ID
来源：http://sud.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://gjv.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kqj.yj202588.top

[Q13] 忽略重复插入
来源：http://erz.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xrg.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://ube.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://azd.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eua.ydjk.org.cn

[Q15] 查询全部
来源：http://jwk.zycfv.cn

SELECT * FROM users;
来源：http://knd.sjlbkw.cn

[Q16] 查询指定列
来源：http://shq.gogol.net.cn

SELECT id, name FROM users;
来源：http://uph.sweek.top

[Q17] 条件查询
来源：http://hni.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jfe.tianlin.xyz

[Q18] 模糊匹配
来源：http://jsp.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://meu.sufxvd.cn

[Q19] 范围查询
来源：http://uvt.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hqb.iojbl.cn

[Q20] IN 列表
来源：http://grw.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dup.shangyingyoupin.top

[Q21] 空值判断
来源：http://xss.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kom.svipenyu.cn

[Q22] 排序
来源：http://lwk.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tzc.tanke756.top

[Q23] 分页
来源：http://buc.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tqo.yj20258.top

[Q24] 去重
来源：http://oqq.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://brm.gzhubu.top

[Q25] 只取前 N 条
来源：http://fft.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dki.meibo888.top

[Q26] 计数
来源：http://tdl.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://xyy.cdnleiting.top

[Q27] 条件计数
来源：http://mhp.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qlt.316326.xyz

[Q28] 求和与平均
来源：http://yyn.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hft.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://aub.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://imz.jinghuilouyu.cn

[Q30] 分组统计
来源：http://epx.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cvh.haohaochexian.top

[Q31] 分组后过滤
来源：http://qbg.gotoacloud.top


<!-- 参考信息 -->