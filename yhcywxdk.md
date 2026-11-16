代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mdr.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wnf.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ksc.svipenyu.cn

[N04] 斐波那契数列
来源：http://tmt.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ufx.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sxx.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymz.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ocd.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fqc.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pzs.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kdf.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xdr.ydzc1.top

[N05] 最大公约数
来源：http://fep.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://xqz.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vdq.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xho.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kmq.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://spa.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mtm.ehwqpu.com

Ruby: a.gcd(b)
来源：http://iba.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yqb.0kj1m.cn

[N06] 判断回文字符串
来源：http://fxa.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://ban.mhx1999.top

PHP:  $s === strrev($s);
来源：http://joz.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://dho.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://yer.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pxa.iojbl.cn

Go:   // 双指针从两端比较
来源：http://ubi.birdmap.top

Ruby: s == s.reverse
来源：http://kkg.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://reo.316326.xyz

[N07] 两数之和（返回下标）
来源：http://bmq.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdi.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bed.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://oph.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://kgb.hywenlv.cn

Java: // 手写 HashMap
来源：http://vom.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://pzy.haohaochexian.top

Ruby: // 手写 Hash
来源：http://uwv.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://ejl.zdbjq.cn

[N08] 生成全排列
来源：http://tec.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://ohe.daria6918.cn

PHP:  // 手写递归交换
来源：http://oov.jinqigufen.top

JS:   // 手写回溯递归
来源：http://zuu.cqqwz.cn

TS:   // 手写回溯递归
来源：http://cit.quarkkingdee.top

Java: // 手写回溯递归
来源：http://oks.zdqjudy.top

Go:   // 手写回溯递归
来源：http://xun.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://vrn.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://gpw.meibo888.top

[N09] 栈与队列
来源：http://hyq.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ocl.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fbu.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iah.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ali.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fer.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dob.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qxu.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bdn.guowangkeji.top

[N10] 链表节点定义
来源：http://onv.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nkr.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sao.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hgr.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afl.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://fpm.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://dul.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lvs.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://aqk.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://huw.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bhl.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://pvw.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihj.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zzp.jinqigufen.top

Java: // 手写递归
来源：http://wid.zhixingplan.top

Go:   // 手写递归
来源：http://fpa.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oug.yfazqb.com

C#:   // 手写递归
来源：http://vex.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://obt.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oys.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://abb.jqgfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jju.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cda.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ywx.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lgt.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eyc.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hvy.smart0.xyz

================================================================================
来源：http://uhq.snrcjt.cn

O. 并发与异步
来源：http://uxz.yj20258888.top

================================================================================
来源：http://hrb.havefunace.top

[O01] 启动一个线程
来源：http://fop.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sia.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tjp.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ihb.jqgufenzy.top

TS:   // 同 JS
来源：http://suo.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://zfk.zhiwuduotai.top

Go:   go f()
来源：http://yad.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://ghh.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://lzq.shanyushiyangtech.top

[O02] 使用线程池
来源：http://dxu.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bwt.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jkv.yonumen.top

JS:   // worker_threads 线程池
来源：http://soj.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://nkn.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://syn.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nne.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rbk.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yys.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://wkx.yvedp.cn

Py:   with lock: shared += 1
来源：http://bso.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://jws.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kxc.aibaodan.cn

TS:   // 同 JS
来源：http://jde.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://usr.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vyc.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jnf.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://iel.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://mtl.cashguo.top

Py:   async def f():⏎    await g()
来源：http://muz.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oco.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://qcp.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pay.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mon.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qwe.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://mis.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://xbi.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://vxw.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://hxl.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cal.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://qkq.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://sre.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://son.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ikf.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://wnp.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://zmw.zdbjq.cn

[O06] 使用进程池
来源：http://ipn.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://all.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iyw.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://vga.meibo888.top

TS:   // child_process / cluster 模块
来源：http://yaq.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://soz.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xtm.hywenlv.cn

Ruby: // fork 块
来源：http://uoz.0kj1m.cn

C#:   Parallel.For
来源：http://esl.tanke756.top

================================================================================
来源：http://vze.pycfn.com

P. 常用工具函数
来源：http://dyc.ehwqpu.com

================================================================================
来源：http://bso.zycfv.cn

[P01] 生成 UUID
来源：http://aae.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://vum.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bsq.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://hrt.smart0.xyz

TS:   crypto.randomUUID()
来源：http://smq.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://mqj.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://ecb.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://mii.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://dtb.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://zxu.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://coy.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://evv.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xsi.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gje.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jrc.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aaz.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://taw.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vmo.wangdashe.top

[P03] 生成短随机字符串
来源：http://vuf.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bra.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aaz.zhongyouzk.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xwu.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dct.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qiz.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qja.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tjg.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ote.ybcxt.top

[P04] 求长度
来源：http://qet.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nih.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ack.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fzb.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lzt.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://wcl.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://aes.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://psm.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pat.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://yvz.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://loh.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zpo.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fcn.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mws.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cmz.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vle.zdbjq.cn

Ruby: a == b
来源：http://uqc.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mpg.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mtf.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ect.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://ncm.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://okz.cdnleiting.top

TS:   if (x == null) {}
来源：http://vks.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gse.pengpengdd.cyou

Go:   if x == nil {}
来源：http://kjp.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rfp.316326.xyz

C#:   if (x is null) {}
来源：http://jtb.hnxiangtu.top

[P07] 防抖与节流
来源：http://xlt.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sjj.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://xgj.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgg.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdb.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dcg.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://njl.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hbu.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fhj.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://rem.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://snc.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ugb.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://czp.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://muo.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uip.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jok.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gaw.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mgv.snrcjt.cn

================================================================================
来源：http://kgw.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kld.sxryk.cn

================================================================================
来源：http://ocp.zdqjudy.top

[Q01] 创建表
来源：http://ssp.zhengqikj.top

CREATE TABLE users (
来源：http://wbf.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ojo.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://bpn.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://xvo.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jlt.quarkkingdee.top

);
来源：http://wwl.sxryk.cn

[Q02] 创建带外键的表
来源：http://rxq.zhijiandao.cn

CREATE TABLE orders (
来源：http://rhc.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbj.guannengcc.top

user_id INT NOT NULL,
来源：http://pku.iojbl.cn

amount DECIMAL(10, 2),
来源：http://ccl.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qws.hesvh.cn

);
来源：http://yqt.52xcode.cn

[Q03] 增加列
来源：http://nms.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ydq.chenzaomai.com

[Q04] 修改列类型
来源：http://ily.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fhq.tarul.cn

[Q05] 重命名列
来源：http://ttn.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nav.sweek.top

[Q06] 删除列
来源：http://vxo.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://rnn.yuxming.cn

[Q07] 删除表
来源：http://uks.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://cfh.jinqigufen.top

[Q08] 创建普通索引
来源：http://tyf.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tah.fzhhl.top

[Q09] 创建唯一索引
来源：http://dop.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qjs.smart0.xyz

[Q10] 插入单行
来源：http://dik.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://grn.52xcode.cn

[Q11] 一次插入多行
来源：http://ora.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://umg.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://swp.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://whr.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iee.yongpay.top

[Q13] 忽略重复插入
来源：http://ohf.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nxb.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://eaa.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kot.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qdj.ybcxt.top

[Q15] 查询全部
来源：http://qtp.aizwys.cn

SELECT * FROM users;
来源：http://kcu.hfpthk.cn

[Q16] 查询指定列
来源：http://xfi.hnqzz.top

SELECT id, name FROM users;
来源：http://brl.fktsv.cn

[Q17] 条件查询
来源：http://sfs.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uxw.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://wnp.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://orr.shuidangran.top

[Q19] 范围查询
来源：http://ewm.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xiy.jqgfzy.top

[Q20] IN 列表
来源：http://xbi.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wcv.sufxvd.cn

[Q21] 空值判断
来源：http://oyf.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jlg.hesvh.cn

[Q22] 排序
来源：http://cqy.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://etr.yueranfly.top

[Q23] 分页
来源：http://hve.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eqe.sufxvd.cn

[Q24] 去重
来源：http://dws.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://zze.nwbrower.top

[Q25] 只取前 N 条
来源：http://rcv.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ppf.ppjwa.cn

[Q26] 计数
来源：http://ydf.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://waq.ivvv.top

[Q27] 条件计数
来源：http://umk.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yxm.havefunace.top

[Q28] 求和与平均
来源：http://vsn.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aju.sxryk.cn

[Q29] 最大最小值
来源：http://tbc.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://pqv.9152youxi.cn

[Q30] 分组统计
来源：http://sbj.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vky.xylfe.cn

[Q31] 分组后过滤
来源：http://pvu.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tpz.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://abq.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rms.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vkt.yvedp.cn

[Q33] 多列分组
来源：http://pxy.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bwp.yj20258888.top

[Q34] 每组取第一条
来源：http://nkh.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://wmc.daria6918.cn


<!-- 参考信息 -->