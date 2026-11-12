代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://jic.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yyp.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aba.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qnr.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pbf.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://asf.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://tqf.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://hrv.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bvv.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://byv.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npf.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rpt.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://idw.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://efq.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tam.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mii.sjlbkw.cn

[N05] 最大公约数
来源：http://mnt.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://oem.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://poe.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tqj.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfa.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://roy.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uan.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://orp.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kzq.uphjek.com

[N06] 判断回文字符串
来源：http://auk.jqgufenzy.top

Py:   s == s[::-1]
来源：http://btd.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://aum.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://wyq.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://hfq.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://whg.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://srs.cucudq.cn

Ruby: s == s.reverse
来源：http://rgm.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nll.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://kmy.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uwj.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ous.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kjp.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://bfa.ivvv.top

Java: // 手写 HashMap
来源：http://unx.tian-w.cn

Go:   // 手写 map[int]int
来源：http://myj.redwolf501.top

Ruby: // 手写 Hash
来源：http://ott.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gcm.bjfxy.top

[N08] 生成全排列
来源：http://ajy.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://jrd.yj20258.top

PHP:  // 手写递归交换
来源：http://fip.redwolf501.top

JS:   // 手写回溯递归
来源：http://nfw.birdmap.top

TS:   // 手写回溯递归
来源：http://vfu.gotoacloud.top

Java: // 手写回溯递归
来源：http://anb.hesvh.cn

Go:   // 手写回溯递归
来源：http://trq.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://don.iojbl.cn

C#:   // 手写回溯递归
来源：http://ijx.xuetiantiany.cn

[N09] 栈与队列
来源：http://tyi.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qcs.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wnz.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xch.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://swt.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ojg.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://azl.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ksn.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://igx.haohaochexian.top

[N10] 链表节点定义
来源：http://uzh.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cws.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lxw.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aix.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oaq.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://vnd.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sjs.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lpq.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jeg.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://cpt.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://twp.dashuyun.cn

PHP:  // 手写递归函数
来源：http://ngi.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwe.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mvl.quarkkingdee.top

Java: // 手写递归
来源：http://sve.xuetiantiany.cn

Go:   // 手写递归
来源：http://cgj.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ejp.vehdjk.com

C#:   // 手写递归
来源：http://fmb.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wdb.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gmq.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xqd.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rfm.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://asx.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dvr.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://omu.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xir.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wag.ivvv.top

================================================================================
来源：http://ewr.bbcook.cn

O. 并发与异步
来源：http://hqz.cashguo.top

================================================================================
来源：http://oty.smart0.xyz

[O01] 启动一个线程
来源：http://msa.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hmd.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://shg.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nqo.pycfn.com

TS:   // 同 JS
来源：http://ixq.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://dnq.ppjwa.cn

Go:   go f()
来源：http://ubb.ivvv.top

Ruby: Thread.new { f }
来源：http://esu.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://mjv.guowangkeji.top

[O02] 使用线程池
来源：http://dpz.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fik.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ili.jianghu66.top

JS:   // worker_threads 线程池
来源：http://uxw.andypj.xyz

TS:   // worker_threads 线程池
来源：http://haw.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gym.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bod.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zat.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mbo.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://onl.yangfankeji.com

Py:   with lock: shared += 1
来源：http://lzc.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://rwy.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wag.hnqzz.top

TS:   // 同 JS
来源：http://rtn.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://lnf.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yee.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://adi.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://igm.52xcode.cn

[O04] 定义异步函数并等待
来源：http://het.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://olu.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ffc.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://cye.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kcj.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ppo.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzi.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://iny.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://utp.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://isy.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://cdk.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fuz.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://leh.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://pod.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nxn.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xqn.xylfe.cn

Ruby: threads.map(&:join)
来源：http://sfn.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sye.vqdsnc.cn

[O06] 使用进程池
来源：http://fbv.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bvw.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://zsc.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://gpi.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://jff.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kjp.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xrq.yonumen.top

Ruby: // fork 块
来源：http://yoh.chenzaomai.com

C#:   Parallel.For
来源：http://opx.fehbvm.com

================================================================================
来源：http://thk.zhongyouzk.top

P. 常用工具函数
来源：http://hxa.gzhubu.top

================================================================================
来源：http://ctr.jyoumei.cn

[P01] 生成 UUID
来源：http://knd.yj202588.top

Py:   str(uuid.uuid4())
来源：http://mqy.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kga.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://ciz.hnqzz.top

TS:   crypto.randomUUID()
来源：http://ouw.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://auc.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://rlg.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://tpx.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://wyf.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://eru.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://efu.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mwn.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tto.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gcu.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fxf.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lcm.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://htm.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hsk.chenlongwang.top

[P03] 生成短随机字符串
来源：http://swq.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ujn.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ple.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uyc.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qtl.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pwz.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://slq.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lhx.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jek.ywan-chungtsiang.top

[P04] 求长度
来源：http://gqf.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uuc.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xdf.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bau.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://byt.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://woh.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://aoj.yj202588.top

Ruby: x.length;  x.size
来源：http://zmz.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xdi.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://byn.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zax.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://njy.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://svy.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fll.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rab.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://cym.zdqjudy.top

Ruby: a == b
来源：http://rwy.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lma.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bxj.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qyr.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://fqh.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ong.aizwys.cn

TS:   if (x == null) {}
来源：http://ljp.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qjx.zdbjq.cn

Go:   if x == nil {}
来源：http://qsl.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fba.fehbvm.com

C#:   if (x is null) {}
来源：http://vvr.316326.xyz

[P07] 防抖与节流
来源：http://mze.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nve.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://ewi.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lvc.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mmi.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cin.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zgn.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qhs.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nrf.shuidangran.top

[P08] 处理浮点精度问题
来源：http://hmn.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kzg.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kqv.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ohy.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ehf.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://biy.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oke.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lti.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://daq.hnxiangtu.top

================================================================================
来源：http://llx.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://agr.wangdashe.top

================================================================================
来源：http://ewl.zhixingplan.top

[Q01] 创建表
来源：http://idz.snrcjt.cn

CREATE TABLE users (
来源：http://ygm.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mdz.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://xyq.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://htv.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://asx.vqdsnc.cn

);
来源：http://uee.jinqigufen.top

[Q02] 创建带外键的表
来源：http://zrt.0kj1m.cn

CREATE TABLE orders (
来源：http://ten.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sek.aizwys.cn

user_id INT NOT NULL,
来源：http://qkm.yvedp.cn

amount DECIMAL(10, 2),
来源：http://qtm.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ebj.tanke756.top

);
来源：http://ufg.chenzaomai.com

[Q03] 增加列
来源：http://wiz.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://chn.tarul.cn

[Q04] 修改列类型
来源：http://yzq.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vvy.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://ewr.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hss.cdnleiting.top

[Q06] 删除列
来源：http://hca.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://ypt.shuidangran.top

[Q07] 删除表
来源：http://yhm.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://ljn.xziqi.cn

[Q08] 创建普通索引
来源：http://hde.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pqd.meibo888.top

[Q09] 创建唯一索引
来源：http://ase.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xru.zhijiandao.cn

[Q10] 插入单行
来源：http://eub.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://djq.sweek.top

[Q11] 一次插入多行
来源：http://jhd.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ugl.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://ena.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://ful.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pct.ydzc1.top

[Q13] 忽略重复插入
来源：http://hjp.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iky.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://chg.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xtk.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://umd.mhx1999.top

[Q15] 查询全部
来源：http://yhb.zhijiandao.cn

SELECT * FROM users;
来源：http://etv.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://krl.ybcxt.top

SELECT id, name FROM users;
来源：http://uhg.mhx1999.top

[Q17] 条件查询
来源：http://omh.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://daj.sxryk.cn

[Q18] 模糊匹配
来源：http://wtc.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oxz.daxiang520.top

[Q19] 范围查询
来源：http://krl.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uco.chenzaomai.com

[Q20] IN 列表
来源：http://hpe.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oin.epnwcf.com

[Q21] 空值判断
来源：http://abq.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://osm.316326.xyz

[Q22] 排序
来源：http://chu.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vgd.wangdashe.top

[Q23] 分页
来源：http://vcb.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vih.aizwys.cn

[Q24] 去重
来源：http://nkl.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://fad.52xcode.cn

[Q25] 只取前 N 条
来源：http://hih.bbcook.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qph.fanxiaobao.xyz

[Q26] 计数
来源：http://rrb.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://sds.vehdjk.com

[Q27] 条件计数
来源：http://jwj.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ofx.yuanzhike.top

[Q28] 求和与平均
来源：http://vtw.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zjc.jlsjyb.cn

[Q29] 最大最小值
来源：http://hxu.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pjq.c1oappe.top

[Q30] 分组统计
来源：http://ydi.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dqo.hysaishi.cn

[Q31] 分组后过滤
来源：http://xut.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://awl.yvedp.cn

[Q32] 分组拼接字符串
来源：http://mlg.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qoz.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pbp.yj20258.top


<!-- 参考信息 -->