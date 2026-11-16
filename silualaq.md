代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://wvs.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sgs.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wsu.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fja.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yhz.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yri.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nfd.ctjpmb.com

[N04] 斐波那契数列
来源：http://wpj.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dec.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pay.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rbe.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bfc.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cxn.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xzs.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://urq.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lpc.jqgufenzy.top

[N05] 最大公约数
来源：http://sgg.bjfxy.top

Py:   math.gcd(a, b)
来源：http://qyl.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://byu.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbi.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gmo.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iml.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oko.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://ldk.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dpj.yj20258888.top

[N06] 判断回文字符串
来源：http://yqy.epnwcf.com

Py:   s == s[::-1]
来源：http://qjm.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://jve.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://abl.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://rqt.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aah.xuanzx.com

Go:   // 双指针从两端比较
来源：http://qtx.yj20258888.top

Ruby: s == s.reverse
来源：http://mbt.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sws.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://hfx.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xuh.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uvg.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tuz.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://acy.hammf.cn

Java: // 手写 HashMap
来源：http://jrs.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://liw.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://uye.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://rmi.chenjidiqi.icu

[N08] 生成全排列
来源：http://pnj.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://vnb.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://fxh.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://gma.hcnkem.com

TS:   // 手写回溯递归
来源：http://jbk.zhoulong.xyz

Java: // 手写回溯递归
来源：http://liw.haohaochexian.top

Go:   // 手写回溯递归
来源：http://jdx.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://mrq.shzxlz.cn

C#:   // 手写回溯递归
来源：http://gla.hesvh.cn

[N09] 栈与队列
来源：http://fzh.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ijc.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wcd.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tbe.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pqj.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yml.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xtz.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ner.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gcd.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://ynn.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rvo.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gcz.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://szm.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nii.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://yvi.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fsp.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yvz.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tea.ydzc1.top

[N11] 二叉树中序遍历
来源：http://jbh.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rji.cqqwz.cn

PHP:  // 手写递归函数
来源：http://cbp.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qhs.sjlbkw.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdh.0kj1m.cn

Java: // 手写递归
来源：http://muz.sysykeji.top

Go:   // 手写递归
来源：http://cwl.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://noa.hcnkem.com

C#:   // 手写递归
来源：http://uyy.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://npq.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://daz.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mvq.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozk.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fas.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aru.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zeq.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sql.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hfy.tarul.cn

================================================================================
来源：http://eol.zhongyouzk.top

O. 并发与异步
来源：http://ycx.bbcook.cn

================================================================================
来源：http://vaf.jqgufenzy.top

[O01] 启动一个线程
来源：http://yft.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gjm.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vgc.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pps.fktsv.cn

TS:   // 同 JS
来源：http://htt.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://bla.jinyuanbaomall.cn

Go:   go f()
来源：http://eiw.yongpay.top

Ruby: Thread.new { f }
来源：http://oys.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://cts.yuxming.cn

[O02] 使用线程池
来源：http://rgl.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xcw.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lmw.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://ttp.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://eqs.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://xdt.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fjh.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iub.yuxming.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ska.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://mhi.ydzc1.top

Py:   with lock: shared += 1
来源：http://brx.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://wqz.dianchejie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qxn.fzhhl.top

TS:   // 同 JS
来源：http://mkz.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://rln.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rdr.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://frk.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://yfn.tarul.cn

[O04] 定义异步函数并等待
来源：http://jwr.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://sdz.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dcm.xziqi.cn

JS:   async function f() { await g(); }
来源：http://djf.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ssy.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qqs.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gus.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://elu.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://qqt.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://yhp.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://fcu.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sqp.316326.xyz

JS:   await Promise.all(tasks)
来源：http://wbp.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://zhr.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pfn.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xkp.wangdashe.top

Ruby: threads.map(&:join)
来源：http://zwl.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sap.kuanghao11.cn

[O06] 使用进程池
来源：http://kjx.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ixx.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kma.uphjek.com

JS:   // child_process / cluster 模块
来源：http://ahn.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://cfq.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rka.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wva.wangshuangyany.cn

Ruby: // fork 块
来源：http://bnz.yonumen.top

C#:   Parallel.For
来源：http://khm.jinghuilouyu.cn

================================================================================
来源：http://hfi.hywenlv.cn

P. 常用工具函数
来源：http://lra.sysykeji.top

================================================================================
来源：http://vjc.gogol.net.cn

[P01] 生成 UUID
来源：http://yql.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://etw.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qbe.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://gyc.daria6918.cn

TS:   crypto.randomUUID()
来源：http://nxy.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://yeu.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://wra.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://uzs.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://ndy.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://arh.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yyo.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://civ.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cud.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cyd.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fgt.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gcd.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://znw.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qlb.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://zwv.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bko.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wuh.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsp.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iot.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cft.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sxt.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xfl.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ypi.yj202588.top

[P04] 求长度
来源：http://fkk.yongpay.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iyh.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sxm.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uea.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ocz.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://izs.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://nxb.hcnkem.com

Ruby: x.length;  x.size
来源：http://zvw.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gjm.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://tch.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vtw.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pay.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aud.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aia.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hkx.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://odf.xuanzx.com

Ruby: a == b
来源：http://bfw.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cos.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qzs.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ubh.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://oyx.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ewk.c1oappe.top

TS:   if (x == null) {}
来源：http://xdr.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bfm.kuanghao11.cn

Go:   if x == nil {}
来源：http://poi.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mys.sweek.top

C#:   if (x is null) {}
来源：http://rxa.yanxiufei.cn

[P07] 防抖与节流
来源：http://wgk.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pmv.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://xmg.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxi.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgf.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bzq.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://plk.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hnj.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bsn.cucudq.cn

[P08] 处理浮点精度问题
来源：http://vsd.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tgy.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://osz.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zcl.xuetiantiany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xah.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ioq.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://evw.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wkx.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zip.jiagoushi.top

================================================================================
来源：http://hbg.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pkm.fzhhl.top

================================================================================
来源：http://evx.pycfn.com

[Q01] 创建表
来源：http://woq.yuanzhike.top

CREATE TABLE users (
来源：http://enc.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pwv.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://sre.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://yef.ctjpmb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gps.xinyue.icu

);
来源：http://tgd.daria6918.cn

[Q02] 创建带外键的表
来源：http://pjz.chenlongwang.top

CREATE TABLE orders (
来源：http://dsc.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zbp.316326.xyz

user_id INT NOT NULL,
来源：http://xpe.tarul.cn

amount DECIMAL(10, 2),
来源：http://nyx.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oro.shanyushiyangtech.top

);
来源：http://yke.zhixingplan.top

[Q03] 增加列
来源：http://rav.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qyn.hfpthk.cn

[Q04] 修改列类型
来源：http://iqo.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pvv.mhx1999.top

[Q05] 重命名列
来源：http://anu.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dim.andypj.xyz

[Q06] 删除列
来源：http://twr.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://onz.yvedp.cn

[Q07] 删除表
来源：http://jow.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://jxq.wangdashe.top

[Q08] 创建普通索引
来源：http://psh.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rhc.havefunace.top

[Q09] 创建唯一索引
来源：http://mcr.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lvv.ctjpmb.com

[Q10] 插入单行
来源：http://bmt.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nyq.hysaishi.cn

[Q11] 一次插入多行
来源：http://irx.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hip.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://tey.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ywc.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fmg.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://sng.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pnf.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://bus.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kof.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yqj.hnqzz.top

[Q15] 查询全部
来源：http://mjx.cashguo.top

SELECT * FROM users;
来源：http://nhx.hfpthk.cn

[Q16] 查询指定列
来源：http://nvh.fehbvm.com

SELECT id, name FROM users;
来源：http://iom.jinqigufen.top

[Q17] 条件查询
来源：http://uzn.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jmg.zycfv.cn

[Q18] 模糊匹配
来源：http://plo.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xca.fengsongda.top

[Q19] 范围查询
来源：http://zjz.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ewk.jyoumei.cn

[Q20] IN 列表
来源：http://iyj.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jsr.chenjidiqi.icu

[Q21] 空值判断
来源：http://dbo.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jzw.pycfn.com

[Q22] 排序
来源：http://kzq.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iwc.jinghuilouyu.cn

[Q23] 分页
来源：http://pby.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vuo.jiagoushi.top

[Q24] 去重
来源：http://wwv.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://ccl.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://lex.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uur.yj20258888.top

[Q26] 计数
来源：http://uef.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://iqm.shanyushiyangtech.top

[Q27] 条件计数
来源：http://ump.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bmp.jyoumei.cn

[Q28] 求和与平均
来源：http://rrh.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dyo.chenzaomai.com

[Q29] 最大最小值
来源：http://amh.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://rkf.jinqigfzy.top

[Q30] 分组统计
来源：http://dsk.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://idb.aizwys.cn

[Q31] 分组后过滤
来源：http://ypy.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qfh.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://hlm.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hbg.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ayf.yvedp.cn


<!-- 参考信息 -->