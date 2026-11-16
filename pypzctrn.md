代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://zxk.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxt.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ias.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gkw.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kdw.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kqv.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wyd.epnwcf.com

[N04] 斐波那契数列
来源：http://yau.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zgd.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rew.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pzl.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jng.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kcq.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hre.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lws.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sec.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://vdz.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://opi.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ufv.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://boh.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://psw.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hbv.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sus.yuanzhike.top

Ruby: a.gcd(b)
来源：http://yzc.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://khm.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://cnl.9152youxi.cn

Py:   s == s[::-1]
来源：http://oqv.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://fyx.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://huu.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://gmg.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://deu.xinyue.icu

Go:   // 双指针从两端比较
来源：http://czb.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://hpl.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bfi.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://wgn.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://til.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sox.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nsr.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://tiz.yueranfly.top

Java: // 手写 HashMap
来源：http://nmn.meibo888.top

Go:   // 手写 map[int]int
来源：http://ysz.hywenlv.cn

Ruby: // 手写 Hash
来源：http://luw.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fol.chenzaomai.com

[N08] 生成全排列
来源：http://fds.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://gxe.jqgfzy.top

PHP:  // 手写递归交换
来源：http://jxn.yj20258888.top

JS:   // 手写回溯递归
来源：http://zch.cqqwz.cn

TS:   // 手写回溯递归
来源：http://vhg.havefunace.top

Java: // 手写回溯递归
来源：http://opn.wangdashe.top

Go:   // 手写回溯递归
来源：http://xfn.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://wna.cheryme.top

C#:   // 手写回溯递归
来源：http://cvb.redwolf501.top

[N09] 栈与队列
来源：http://cnv.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cpi.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sqn.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qhh.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dgx.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pjl.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ogl.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bew.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://epi.zhiwuduotai.top

[N10] 链表节点定义
来源：http://ysp.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ajg.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fqa.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mel.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lzy.tanke756.top

Java: class Node { int v; Node next; }
来源：http://ewe.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://feu.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nct.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://csv.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://kzt.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bbt.hywenlv.cn

PHP:  // 手写递归函数
来源：http://xay.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zqt.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jen.aizwys.cn

Java: // 手写递归
来源：http://wek.chenzaomai.com

Go:   // 手写递归
来源：http://pio.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bez.ybcxt.top

C#:   // 手写递归
来源：http://ukb.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hsc.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jtc.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jbm.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epk.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tjo.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://umc.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://svb.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bpc.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pru.yangfankeji.com

================================================================================
来源：http://ytu.9152youxi.cn

O. 并发与异步
来源：http://vku.yonumen.top

================================================================================
来源：http://waz.cucudq.cn

[O01] 启动一个线程
来源：http://yuy.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vgo.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dgm.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hpn.gzhubu.top

TS:   // 同 JS
来源：http://mah.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://ufl.tianlin.xyz

Go:   go f()
来源：http://bhb.fktsv.cn

Ruby: Thread.new { f }
来源：http://mdx.yonumen.top

C#:   Task.Run(() => F());
来源：http://hwx.vehdjk.com

[O02] 使用线程池
来源：http://fgk.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ttt.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://myv.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://agt.tarul.cn

TS:   // worker_threads 线程池
来源：http://ocf.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qgu.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ola.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oep.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ava.yonumen.top

[O03] 加锁保护共享数据
来源：http://dtd.ivvv.top

Py:   with lock: shared += 1
来源：http://lem.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://vrh.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eim.fzhhl.top

TS:   // 同 JS
来源：http://wpa.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://yem.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zcr.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://min.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://gek.hesvh.cn

[O04] 定义异步函数并等待
来源：http://qtu.uphjek.com

Py:   async def f():⏎    await g()
来源：http://cgv.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://edy.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://wnv.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mah.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jkx.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kfb.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://eka.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://fss.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://kxz.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://ibj.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://snu.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://pmk.havefunace.top

TS:   await Promise.all(tasks)
来源：http://rox.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kvh.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qvw.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://hjq.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bxy.hnqzz.top

[O06] 使用进程池
来源：http://pmq.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jqf.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wwo.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://bwb.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://uig.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aha.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dlf.xuetiantiany.cn

Ruby: // fork 块
来源：http://fof.epnwcf.com

C#:   Parallel.For
来源：http://xrm.hongshengwenyu.top

================================================================================
来源：http://nji.zhaomingkeji.xyz

P. 常用工具函数
来源：http://zfu.nanxinkj.top

================================================================================
来源：http://klu.andypj.xyz

[P01] 生成 UUID
来源：http://yyw.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://yun.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://crc.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://xeu.xinyue.icu

TS:   crypto.randomUUID()
来源：http://gac.sweek.top

Java: UUID.randomUUID().toString()
来源：http://iaj.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://pkk.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://ues.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://lod.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://nov.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://djw.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://irl.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fdt.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vkn.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wac.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hzg.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dxe.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zai.yj20258888.top

[P03] 生成短随机字符串
来源：http://zrm.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://puj.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rem.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://usa.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oky.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cpj.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ypg.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dnb.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://orh.aibaodan.cn

[P04] 求长度
来源：http://azg.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dzw.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fit.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://anq.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iip.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://qcy.jianghu66.top

Go:   len(arr);  len(m)
来源：http://oaj.birdmap.top

Ruby: x.length;  x.size
来源：http://yjf.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mgw.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://exe.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cgq.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tve.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hoi.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cie.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eod.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sxw.chenlongwang.top

Ruby: a == b
来源：http://gwm.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dus.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rgo.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gzx.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://inx.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sro.yonumen.top

TS:   if (x == null) {}
来源：http://dej.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dtq.yj20258.top

Go:   if x == nil {}
来源：http://bww.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pjo.yonumen.top

C#:   if (x is null) {}
来源：http://hrp.xziqi.cn

[P07] 防抖与节流
来源：http://psi.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gnb.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://rbu.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyh.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tfm.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rpm.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zzo.52xcode.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fkw.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gzl.cucudq.cn

[P08] 处理浮点精度问题
来源：http://ppy.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tlq.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vkz.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cds.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ueu.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ziq.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jvs.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qhh.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fqg.yanxiufei.cn

================================================================================
来源：http://obb.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yhn.tianlin.xyz

================================================================================
来源：http://hhr.epnwcf.com

[Q01] 创建表
来源：http://rlv.hongshengwenyu.top

CREATE TABLE users (
来源：http://fip.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzb.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://tsp.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://kqc.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jej.sufxvd.cn

);
来源：http://jav.aizwys.cn

[Q02] 创建带外键的表
来源：http://uds.dianchejie.cn

CREATE TABLE orders (
来源：http://awu.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rtl.ppjwa.cn

user_id INT NOT NULL,
来源：http://wwk.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://mus.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nog.epnwcf.com

);
来源：http://tev.cheryme.top

[Q03] 增加列
来源：http://hfd.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wsz.ydzc1.top

[Q04] 修改列类型
来源：http://qkw.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uvn.bjfxy.top

[Q05] 重命名列
来源：http://emp.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tek.shanyushiyangkeji.top

[Q06] 删除列
来源：http://jal.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://qlq.fktsv.cn

[Q07] 删除表
来源：http://jak.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://hlx.yanxiufei.cn

[Q08] 创建普通索引
来源：http://jse.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qdx.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://afh.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qnj.jinqigfzy.top

[Q10] 插入单行
来源：http://cnx.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zjy.svipenyu.cn

[Q11] 一次插入多行
来源：http://eiz.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rtd.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://wls.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yqv.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nyq.jqgfzy.top

[Q13] 忽略重复插入
来源：http://gid.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cbr.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://tcw.jinghuilouyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kpg.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fcw.tianlin.xyz

[Q15] 查询全部
来源：http://jny.gzhubu.top

SELECT * FROM users;
来源：http://yxn.sxryk.cn

[Q16] 查询指定列
来源：http://fxf.zhixingplan.top

SELECT id, name FROM users;
来源：http://bmq.smart0.xyz

[Q17] 条件查询
来源：http://qvf.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://slk.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://tho.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fbr.hcnkem.com

[Q19] 范围查询
来源：http://unb.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ibk.snrcjt.cn

[Q20] IN 列表
来源：http://rwq.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ste.birdmap.top

[Q21] 空值判断
来源：http://ycm.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nbp.yfazqb.com

[Q22] 排序
来源：http://ihr.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vcq.cheryme.top

[Q23] 分页
来源：http://mtz.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hea.kuanghao11.cn

[Q24] 去重
来源：http://mcy.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://kec.cucudq.cn

[Q25] 只取前 N 条
来源：http://xui.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gvr.jqgufenzy.top

[Q26] 计数
来源：http://ydi.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://dsq.hcnkem.com

[Q27] 条件计数
来源：http://tvs.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wwo.hesvh.cn

[Q28] 求和与平均
来源：http://pvj.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jbv.jinqigfzy.top

[Q29] 最大最小值
来源：http://qid.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://gwz.ybcxt.top

[Q30] 分组统计
来源：http://nke.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rvd.sweek.top

[Q31] 分组后过滤
来源：http://koo.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wkc.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://gfx.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ntv.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qcu.zhoulong.xyz


<!-- 参考信息 -->