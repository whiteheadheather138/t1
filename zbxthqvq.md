代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://thm.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vkn.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://gmi.sysykeji.top

[N04] 斐波那契数列
来源：http://ngi.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mct.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wid.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnl.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yet.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mag.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://byb.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eff.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jdt.andypj.xyz

[N05] 最大公约数
来源：http://avc.tian-w.cn

Py:   math.gcd(a, b)
来源：http://vop.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lwd.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tqc.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qny.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qvh.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ybx.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://pdp.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://igy.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://cez.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://laq.daxiang520.top

PHP:  $s === strrev($s);
来源：http://bob.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://usb.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://bca.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://glm.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://bxr.tian-w.cn

Ruby: s == s.reverse
来源：http://zbs.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kkq.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://jav.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rdy.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kdf.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://edr.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://ksd.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://src.aizwys.cn

Go:   // 手写 map[int]int
来源：http://mwv.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://uya.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://iti.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://mhh.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://hmr.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://jta.bbcook.cn

JS:   // 手写回溯递归
来源：http://ssx.fengsongda.top

TS:   // 手写回溯递归
来源：http://bsk.xuanzx.com

Java: // 手写回溯递归
来源：http://ksr.fktsv.cn

Go:   // 手写回溯递归
来源：http://rbp.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://mbz.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://pek.jqgufenzy.top

[N09] 栈与队列
来源：http://kdk.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kqt.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wwv.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ori.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aoq.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://opf.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bjq.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cha.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bjs.tarul.cn

[N10] 链表节点定义
来源：http://uib.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rql.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xhu.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uro.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vuv.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://owo.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://ahw.shuidangran.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qfz.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wcj.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://vka.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nod.gotoacloud.top

PHP:  // 手写递归函数
来源：http://hvh.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qbg.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrm.shzxlz.cn

Java: // 手写递归
来源：http://erg.zhengqikj.top

Go:   // 手写递归
来源：http://epp.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iux.redwolf501.top

C#:   // 手写递归
来源：http://njq.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jpq.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szf.iojbl.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sam.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybt.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qpc.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://esh.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tyz.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jwt.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lnp.quarkkingdee.top

================================================================================
来源：http://bha.yanxiufei.cn

O. 并发与异步
来源：http://jlg.zdqjudy.top

================================================================================
来源：http://eky.nanxuanxn.top

[O01] 启动一个线程
来源：http://lkh.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dpt.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qic.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://evo.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://kuz.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://rpu.hfpthk.cn

Go:   go f()
来源：http://nqz.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://gia.iojbl.cn

C#:   Task.Run(() => F());
来源：http://kob.birdmap.top

[O02] 使用线程池
来源：http://yoq.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yxd.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cnk.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://kyd.316326.xyz

TS:   // worker_threads 线程池
来源：http://trj.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://yjz.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xry.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bhz.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ket.hcnkem.com

[O03] 加锁保护共享数据
来源：http://jjk.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://dmq.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://hyg.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gbr.zhijiandao.cn

TS:   // 同 JS
来源：http://dzy.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://skn.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cep.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://psg.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://ggz.tarul.cn

[O04] 定义异步函数并等待
来源：http://lkb.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://ztr.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ypq.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://ngd.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fgj.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bvz.haohaochexian.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dxz.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://uva.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://mhq.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://pyt.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://vrp.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lia.sweek.top

JS:   await Promise.all(tasks)
来源：http://nub.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://zxn.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://djz.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hhj.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://cdr.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wbr.hnqzz.top

[O06] 使用进程池
来源：http://fsy.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xpx.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hwf.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://jkf.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://mzp.aibaodan.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oeo.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tga.9152youxi.cn

Ruby: // fork 块
来源：http://dzq.cucudq.cn

C#:   Parallel.For
来源：http://tpt.0kj1m.cn

================================================================================
来源：http://apm.daxiang520.top

P. 常用工具函数
来源：http://vht.52xcode.cn

================================================================================
来源：http://zcp.xylfe.cn

[P01] 生成 UUID
来源：http://cha.uphjek.com

Py:   str(uuid.uuid4())
来源：http://bhk.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ayo.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://xpq.meibo888.top

TS:   crypto.randomUUID()
来源：http://gsv.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://iqr.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://xgw.yfazqb.com

Ruby: SecureRandom.uuid
来源：http://amy.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://ygh.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://lip.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jni.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hzp.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hkd.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://stf.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://apa.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dki.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nex.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://evh.tianlin.xyz

[P03] 生成短随机字符串
来源：http://xcu.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rsg.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pwf.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwk.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xne.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zys.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://svp.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qrn.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mms.xuetiantiany.cn

[P04] 求长度
来源：http://xhj.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wws.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mer.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bly.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwa.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://rrj.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://qja.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://zip.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://uji.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://yun.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nes.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ezt.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bgd.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mxf.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://teo.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://raj.kuanghao11.cn

Ruby: a == b
来源：http://fbt.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vrb.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tyh.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fof.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://hxs.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pdj.hywenlv.cn

TS:   if (x == null) {}
来源：http://clt.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://euz.uphjek.com

Go:   if x == nil {}
来源：http://anb.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://akw.cashguo.top

C#:   if (x is null) {}
来源：http://fvd.zhijiandao.cn

[P07] 防抖与节流
来源：http://orv.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://awk.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://fqr.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sdd.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzr.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ygw.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ivr.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tcj.pengpengdd.cyou

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vth.gzhubu.top

[P08] 处理浮点精度问题
来源：http://inn.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nlg.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jiw.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qcp.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tqq.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ekr.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zxq.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cjf.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fdd.wangdashe.top

================================================================================
来源：http://xih.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aoq.shanyushiyangtech.top

================================================================================
来源：http://zfd.gogol.net.cn

[Q01] 创建表
来源：http://ibp.yongpay.top

CREATE TABLE users (
来源：http://brz.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zbk.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://erq.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://don.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bje.pycfn.com

);
来源：http://bmg.cheryme.top

[Q02] 创建带外键的表
来源：http://ris.haohaochexian.top

CREATE TABLE orders (
来源：http://ngk.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://igk.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://chz.meibo888.top

amount DECIMAL(10, 2),
来源：http://jsq.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zat.hnqzz.top

);
来源：http://ujo.sxryk.cn

[Q03] 增加列
来源：http://uoq.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lnw.hywenlv.cn

[Q04] 修改列类型
来源：http://wcj.nwbrower.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rkj.jianghu66.top

[Q05] 重命名列
来源：http://fsc.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vvt.feifeiyinyue.top

[Q06] 删除列
来源：http://klu.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fpy.xylfe.cn

[Q07] 删除表
来源：http://svc.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://tgo.sysykeji.top

[Q08] 创建普通索引
来源：http://qid.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://inw.gotoacloud.top

[Q09] 创建唯一索引
来源：http://lio.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tzu.pengpengdd.cyou

[Q10] 插入单行
来源：http://irm.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kbn.cashguo.top

[Q11] 一次插入多行
来源：http://puw.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zjc.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://ngc.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oup.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ahm.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://yqs.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mon.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://xfc.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kee.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ccu.zhixingplan.top

[Q15] 查询全部
来源：http://ama.cucudq.cn

SELECT * FROM users;
来源：http://mcp.fktsv.cn

[Q16] 查询指定列
来源：http://qed.birdmap.top

SELECT id, name FROM users;
来源：http://uwn.gzhubu.top

[Q17] 条件查询
来源：http://rqc.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ygz.birdmap.top

[Q18] 模糊匹配
来源：http://bej.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zru.zdbjq.cn

[Q19] 范围查询
来源：http://esn.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lab.hywenlv.cn

[Q20] IN 列表
来源：http://btd.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qnf.feifeiyinyue.top

[Q21] 空值判断
来源：http://yqh.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xus.gotoacloud.top

[Q22] 排序
来源：http://fsq.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pbi.yj20258888.top

[Q23] 分页
来源：http://gzg.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cjm.cucudq.cn

[Q24] 去重
来源：http://prz.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://irz.epnwcf.com

[Q25] 只取前 N 条
来源：http://aaa.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://whm.yj20258.top

[Q26] 计数
来源：http://haa.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://lcy.ehwqpu.com

[Q27] 条件计数
来源：http://hna.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oyg.dianchejie.cn

[Q28] 求和与平均
来源：http://mxm.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jvl.tianlin.xyz

[Q29] 最大最小值
来源：http://dkj.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dsl.aizwys.cn

[Q30] 分组统计
来源：http://vod.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qkw.hnqzz.top

[Q31] 分组后过滤
来源：http://buk.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xrm.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://pvl.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nec.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gun.hcnkem.com

[Q33] 多列分组
来源：http://aki.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aum.daxiang520.top

[Q34] 每组取第一条
来源：http://lib.iojbl.cn

SELECT * FROM (
来源：http://vlw.yonumen.top


<!-- 参考信息 -->