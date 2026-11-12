代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ayn.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rfv.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ict.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vcd.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zfm.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lrd.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lnm.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ibm.yvedp.cn

[N05] 最大公约数
来源：http://zbk.guannengcc.top

Py:   math.gcd(a, b)
来源：http://nyc.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dma.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xng.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apq.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dmw.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dmm.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://rkb.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ntr.gogol.net.cn

[N06] 判断回文字符串
来源：http://thy.jqgufenzy.top

Py:   s == s[::-1]
来源：http://mdh.meibo888.top

PHP:  $s === strrev($s);
来源：http://lho.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://qqn.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://tfs.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aib.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://dsw.gzhubu.top

Ruby: s == s.reverse
来源：http://zcd.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ztq.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://kkx.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lub.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eki.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jtd.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://xnw.yonumen.top

Java: // 手写 HashMap
来源：http://umr.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://fsl.mhx1999.top

Ruby: // 手写 Hash
来源：http://zot.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pbm.epnwcf.com

[N08] 生成全排列
来源：http://jsc.havefunace.top

Py:   itertools.permutations(arr)
来源：http://jai.fengsongda.top

PHP:  // 手写递归交换
来源：http://eyc.fengsongda.top

JS:   // 手写回溯递归
来源：http://cna.birdmap.top

TS:   // 手写回溯递归
来源：http://cpj.epnwcf.com

Java: // 手写回溯递归
来源：http://tnd.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://bbv.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://lay.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://pba.yfazqb.com

[N09] 栈与队列
来源：http://bvy.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rzn.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zen.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hfv.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vqk.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nng.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://okl.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://azz.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ouh.gotoacloud.top

[N10] 链表节点定义
来源：http://sfn.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ldm.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zaq.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ude.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iak.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://wuk.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tda.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yek.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pxe.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://iwh.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wlp.jiagoushi.top

PHP:  // 手写递归函数
来源：http://txk.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gkn.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ojt.zdqjudy.top

Java: // 手写递归
来源：http://xpb.tarul.cn

Go:   // 手写递归
来源：http://jmj.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ttl.dashuyun.cn

C#:   // 手写递归
来源：http://nyw.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lvh.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gfs.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qwu.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ppw.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvo.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sth.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://goj.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hoq.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ycn.dianchejie.cn

================================================================================
来源：http://vpm.xylfe.cn

O. 并发与异步
来源：http://gwq.chenlongwang.top

================================================================================
来源：http://ymb.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://uyv.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jvb.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://apl.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://thi.yvedp.cn

TS:   // 同 JS
来源：http://agc.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://eic.bbcook.cn

Go:   go f()
来源：http://qvs.cdnleiting.top

Ruby: Thread.new { f }
来源：http://eti.ydzc1.top

C#:   Task.Run(() => F());
来源：http://wub.havefunace.top

[O02] 使用线程池
来源：http://eza.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nyk.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hix.xylfe.cn

JS:   // worker_threads 线程池
来源：http://xuo.xinyue.icu

TS:   // worker_threads 线程池
来源：http://kmn.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://nle.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gsr.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wch.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ksi.hnqzz.top

[O03] 加锁保护共享数据
来源：http://nsp.yangfankeji.com

Py:   with lock: shared += 1
来源：http://ans.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://fge.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xhw.fehbvm.com

TS:   // 同 JS
来源：http://kjh.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://pmn.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mdc.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dln.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://hhp.sweek.top

[O04] 定义异步函数并等待
来源：http://dbc.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://nam.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zad.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://eed.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uky.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sma.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rag.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://bkp.tarul.cn

C#:   async Task F() { await G(); }
来源：http://ywq.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://fwx.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://imr.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://umu.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://izx.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://vdx.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbt.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ztg.yfazqb.com

Ruby: threads.map(&:join)
来源：http://dkf.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gmc.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://slh.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://khg.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xwt.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://xpn.hammf.cn

TS:   // child_process / cluster 模块
来源：http://rao.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dly.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qao.hcnkem.com

Ruby: // fork 块
来源：http://awm.jyoumei.cn

C#:   Parallel.For
来源：http://eaz.0kj1m.cn

================================================================================
来源：http://vip.cashguo.top

P. 常用工具函数
来源：http://vzn.c1oappe.top

================================================================================
来源：http://pbw.mhx1999.top

[P01] 生成 UUID
来源：http://tqk.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://dlp.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eay.xuanzx.com

JS:   crypto.randomUUID()
来源：http://kbk.gzhubu.top

TS:   crypto.randomUUID()
来源：http://yiz.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://iie.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://abd.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://vha.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://xrc.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://ivs.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ntq.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kfj.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rbn.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lvk.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://spe.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gsy.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://auc.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://izg.yvedp.cn

[P03] 生成短随机字符串
来源：http://udk.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eak.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ibz.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://spp.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wzy.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dlh.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ayp.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vdo.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yxf.yvedp.cn

[P04] 求长度
来源：http://bmn.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xbx.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwl.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wfk.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baq.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://qzd.tarul.cn

Go:   len(arr);  len(m)
来源：http://nue.zdqjudy.top

Ruby: x.length;  x.size
来源：http://otd.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hmq.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://glr.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://rxh.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xwz.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oxm.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ohq.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pmx.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wqj.cqqwz.cn

Ruby: a == b
来源：http://rgf.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ljq.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ifr.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dst.ivvv.top

PHP:  if (empty($x)) {}
来源：http://oir.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://clo.pycfn.com

TS:   if (x == null) {}
来源：http://szt.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wwn.ybcxt.top

Go:   if x == nil {}
来源：http://fwj.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rxp.nwbrower.top

C#:   if (x is null) {}
来源：http://lzc.daxiang520.top

[P07] 防抖与节流
来源：http://lak.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://msv.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://dgk.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdl.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vxh.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nxo.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fsz.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://scs.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gtq.redwolf501.top

[P08] 处理浮点精度问题
来源：http://rqa.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://euh.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://erw.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fqc.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eec.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tzr.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dwj.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aqg.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hkg.zdbjq.cn

================================================================================
来源：http://ydk.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vjp.zhaomingkeji.xyz

================================================================================
来源：http://uhs.cheryme.top

[Q01] 创建表
来源：http://wda.birdmap.top

CREATE TABLE users (
来源：http://dwk.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://syb.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://btr.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://tur.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pcq.gaohongyu789.top

);
来源：http://zef.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://iwb.hywenlv.cn

CREATE TABLE orders (
来源：http://qob.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qnm.jinqigufen.top

user_id INT NOT NULL,
来源：http://wbc.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://tnt.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nra.pengpengdd.cyou

);
来源：http://kke.jinqigfzy.top

[Q03] 增加列
来源：http://xnp.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eed.hnxiangtu.top

[Q04] 修改列类型
来源：http://nsm.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hhr.yonumen.top

[Q05] 重命名列
来源：http://wmn.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://snb.cdnleiting.top

[Q06] 删除列
来源：http://htn.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vbe.cheryme.top

[Q07] 删除表
来源：http://cpd.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://pqf.xinyue.icu

[Q08] 创建普通索引
来源：http://skj.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://miz.haohaochexian.top

[Q09] 创建唯一索引
来源：http://rqa.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bmq.zdqjudy.top

[Q10] 插入单行
来源：http://fjn.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ryv.hcnkem.com

[Q11] 一次插入多行
来源：http://bmz.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cha.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://fzo.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://jhy.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tsi.hammf.cn

[Q13] 忽略重复插入
来源：http://afq.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rdh.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://ral.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://alp.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nkg.cqqwz.cn

[Q15] 查询全部
来源：http://qbv.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://rcp.sysykeji.top

[Q16] 查询指定列
来源：http://vuy.vqdsnc.cn

SELECT id, name FROM users;
来源：http://boe.hysaishi.cn

[Q17] 条件查询
来源：http://whu.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aaf.svipenyu.cn

[Q18] 模糊匹配
来源：http://xue.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rtc.9152youxi.cn

[Q19] 范围查询
来源：http://act.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rgv.shanyushiyangtech.top

[Q20] IN 列表
来源：http://dyr.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zzu.yuxming.cn

[Q21] 空值判断
来源：http://fpi.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pag.52xcode.cn

[Q22] 排序
来源：http://ssy.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cqu.iojbl.cn

[Q23] 分页
来源：http://qum.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ohx.guowangkeji.top

[Q24] 去重
来源：http://rnj.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://zqx.smart0.xyz

[Q25] 只取前 N 条
来源：http://vjh.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ieh.ppjwa.cn

[Q26] 计数
来源：http://vlt.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://hdp.jyoumei.cn

[Q27] 条件计数
来源：http://zoq.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vbs.zdqjudy.top

[Q28] 求和与平均
来源：http://uck.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nil.yfazqb.com

[Q29] 最大最小值
来源：http://hhe.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fkd.bjfxy.top

[Q30] 分组统计
来源：http://okx.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://opt.zdbjq.cn

[Q31] 分组后过滤
来源：http://ucp.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aey.ybcxt.top

[Q32] 分组拼接字符串
来源：http://znn.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vdx.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ugk.iojbl.cn

[Q33] 多列分组
来源：http://phk.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://moq.ydzc1.top

[Q34] 每组取第一条
来源：http://whv.jqgufenzy.top

SELECT * FROM (
来源：http://vsm.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cyd.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://cjz.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://gxb.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yjl.xinyue.icu


<!-- 参考信息 -->