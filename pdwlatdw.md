代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vxv.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fcn.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bmi.kuanghao11.cn

[N04] 斐波那契数列
来源：http://cca.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ppv.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://smo.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gsz.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgr.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eoy.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://imr.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ipi.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nwo.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://ihn.shuidangran.top

Py:   math.gcd(a, b)
来源：http://uxw.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rao.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://roa.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgo.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mvh.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uek.52xcode.cn

Ruby: a.gcd(b)
来源：http://hwa.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lvu.fzhhl.top

[N06] 判断回文字符串
来源：http://isb.bjfxy.top

Py:   s == s[::-1]
来源：http://gwv.daria6918.cn

PHP:  $s === strrev($s);
来源：http://zsw.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://tqg.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://rlb.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tra.fehbvm.com

Go:   // 双指针从两端比较
来源：http://vgt.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://xct.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fio.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://aic.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sff.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vbf.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cwi.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://iun.tanke756.top

Java: // 手写 HashMap
来源：http://kik.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://fgq.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://toa.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://nao.chenjidiqi.icu

[N08] 生成全排列
来源：http://ide.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://csg.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://kas.svipenyu.cn

JS:   // 手写回溯递归
来源：http://pyf.zhengqikj.top

TS:   // 手写回溯递归
来源：http://qyy.haohaochexian.top

Java: // 手写回溯递归
来源：http://oez.dashuyun.cn

Go:   // 手写回溯递归
来源：http://uzf.pycfn.com

Ruby: arr.permutation.to_a
来源：http://vjo.cheryme.top

C#:   // 手写回溯递归
来源：http://cqn.sufxvd.cn

[N09] 栈与队列
来源：http://hkk.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gwx.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://evo.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pes.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cyr.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://txe.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://smq.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wds.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tjv.feifeiyinyue.top

[N10] 链表节点定义
来源：http://rdt.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://btr.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dif.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qcj.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ipz.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://xbx.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://gsk.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qhy.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oup.havefunace.top

[N11] 二叉树中序遍历
来源：http://hbv.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ogn.zycfv.cn

PHP:  // 手写递归函数
来源：http://ckw.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qpx.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dvg.guowangkeji.top

Java: // 手写递归
来源：http://hcm.shangyingyoupin.top

Go:   // 手写递归
来源：http://mot.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ltr.sxryk.cn

C#:   // 手写递归
来源：http://gyh.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uws.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jfd.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eik.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kza.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcb.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iov.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hjl.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pzx.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://egv.yongpay.top

================================================================================
来源：http://fuf.chenlongwang.top

O. 并发与异步
来源：http://zoo.daria6918.cn

================================================================================
来源：http://qly.jlsjyb.cn

[O01] 启动一个线程
来源：http://xub.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nfb.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vtt.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://chw.cdnleiting.top

TS:   // 同 JS
来源：http://ncp.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://zcm.wangshuangyany.cn

Go:   go f()
来源：http://hhy.cheryme.top

Ruby: Thread.new { f }
来源：http://owm.shuidangran.top

C#:   Task.Run(() => F());
来源：http://qio.zhixingplan.top

[O02] 使用线程池
来源：http://dho.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nub.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://htf.smart0.xyz

JS:   // worker_threads 线程池
来源：http://czm.tarul.cn

TS:   // worker_threads 线程池
来源：http://jad.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ohr.cucudq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qnu.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cqm.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qqv.bjfxy.top

[O03] 加锁保护共享数据
来源：http://eac.vehdjk.com

Py:   with lock: shared += 1
来源：http://tga.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://cyn.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yxm.sxryk.cn

TS:   // 同 JS
来源：http://fro.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://iyv.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xxr.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tfz.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://ihr.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://nyy.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://vzj.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qrs.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://gnn.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bmi.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hsp.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dhv.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://ttq.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://jeq.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://icr.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://dhs.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lah.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://ghe.uphjek.com

TS:   await Promise.all(tasks)
来源：http://oxf.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wpe.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fyw.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://pcs.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://ypi.bjfxy.top

[O06] 使用进程池
来源：http://hhe.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uvn.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://grm.meibo888.top

JS:   // child_process / cluster 模块
来源：http://qsn.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://cmb.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zxc.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://upe.hesvh.cn

Ruby: // fork 块
来源：http://auj.shangyingyoupin.top

C#:   Parallel.For
来源：http://mml.smart0.xyz

================================================================================
来源：http://pwc.zhengqikj.top

P. 常用工具函数
来源：http://hts.gotoacloud.top

================================================================================
来源：http://wyt.gogol.net.cn

[P01] 生成 UUID
来源：http://cmd.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://wmb.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xkx.smart0.xyz

JS:   crypto.randomUUID()
来源：http://aek.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://joe.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://djt.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://wls.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://sec.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://heq.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://ezg.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mmn.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://cuj.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aey.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vvy.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ket.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://foo.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sfi.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://atc.316326.xyz

[P03] 生成短随机字符串
来源：http://hsh.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cnl.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ytb.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eym.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yll.yfazqb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bto.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mij.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rhv.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blj.jinghuilouyu.cn

[P04] 求长度
来源：http://mqm.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kml.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rlb.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fof.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wrd.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://tre.yonumen.top

Go:   len(arr);  len(m)
来源：http://iky.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://rad.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nnt.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://smg.daria6918.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jlp.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://npg.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yql.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://can.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yfl.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vey.cashguo.top

Ruby: a == b
来源：http://hgy.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://imd.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cct.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hbu.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://jsr.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hgs.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://hxh.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ngf.mhx1999.top

Go:   if x == nil {}
来源：http://esz.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lxm.ehwqpu.com

C#:   if (x is null) {}
来源：http://mqs.yangfankeji.com

[P07] 防抖与节流
来源：http://pla.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://chu.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://rsx.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://est.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wms.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lfl.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fra.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mql.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hjn.tanke756.top

[P08] 处理浮点精度问题
来源：http://rdz.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nap.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blg.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jcm.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lzv.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rct.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://svl.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fuv.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xcq.fehbvm.com

================================================================================
来源：http://ler.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gpr.tarul.cn

================================================================================
来源：http://uug.hammf.cn

[Q01] 创建表
来源：http://nni.jiagoushi.top

CREATE TABLE users (
来源：http://heu.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mxx.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://ibm.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://hhp.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jgk.wangshuangyany.cn

);
来源：http://lkt.bjfxy.top

[Q02] 创建带外键的表
来源：http://jbi.ivvv.top

CREATE TABLE orders (
来源：http://hdu.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dsp.fzhhl.top

user_id INT NOT NULL,
来源：http://xxg.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://kyt.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://apv.daxiang520.top

);
来源：http://cav.zhixingplan.top

[Q03] 增加列
来源：http://vmy.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ssm.sjlbkw.cn

[Q04] 修改列类型
来源：http://uwq.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hyv.kuanghao11.cn

[Q05] 重命名列
来源：http://cdf.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://clt.aizwys.cn

[Q06] 删除列
来源：http://knz.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://grx.shanyushiyangkeji.top

[Q07] 删除表
来源：http://gzg.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://mvn.dashuyun.cn

[Q08] 创建普通索引
来源：http://ffm.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tze.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://edx.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hjf.meibo888.top

[Q10] 插入单行
来源：http://aub.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://unf.iojbl.cn

[Q11] 一次插入多行
来源：http://xyg.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kkz.yongpay.top

[Q12] 插入后取自增 ID
来源：http://wsh.uphjek.com

INSERT INTO users (name) VALUES ('C');
来源：http://qod.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibe.bjfxy.top

[Q13] 忽略重复插入
来源：http://lnp.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xiu.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://rbo.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ovb.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ohi.xylfe.cn

[Q15] 查询全部
来源：http://iwa.pycfn.com

SELECT * FROM users;
来源：http://vtl.xinyue.icu

[Q16] 查询指定列
来源：http://otb.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://wil.redwolf501.top

[Q17] 条件查询
来源：http://ekn.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zwp.jinqigufen.top

[Q18] 模糊匹配
来源：http://sqs.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oxa.52xcode.cn

[Q19] 范围查询
来源：http://phl.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yur.sweek.top

[Q20] IN 列表
来源：http://iuh.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tbd.vehdjk.com

[Q21] 空值判断
来源：http://nbc.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xco.feifeiyinyue.top

[Q22] 排序
来源：http://zvz.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wqi.hcnkem.com

[Q23] 分页
来源：http://jmc.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jgr.9152youxi.cn

[Q24] 去重
来源：http://ssz.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://tih.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://pcc.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ifn.cucudq.cn

[Q26] 计数
来源：http://udr.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://wie.c1oappe.top

[Q27] 条件计数
来源：http://ygb.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ahl.cdnleiting.top

[Q28] 求和与平均
来源：http://xct.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pwu.ppjwa.cn

[Q29] 最大最小值
来源：http://exe.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://chz.wangshuangyany.cn

[Q30] 分组统计
来源：http://zkz.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://owl.daria6918.cn

[Q31] 分组后过滤
来源：http://gww.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xjg.sxryk.cn

[Q32] 分组拼接字符串
来源：http://axq.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://phf.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://znq.zhijiandao.cn

[Q33] 多列分组
来源：http://ijy.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vgy.hnxiangtu.top

[Q34] 每组取第一条
来源：http://hge.snrcjt.cn

SELECT * FROM (
来源：http://tme.jinghuilouyu.cn


<!-- 参考信息 -->