代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sfu.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lkb.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvf.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yax.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qkr.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dbl.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://spp.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ncy.fanxiaobao.xyz

[N05] 最大公约数
来源：http://mjo.bbcook.cn

Py:   math.gcd(a, b)
来源：http://tsy.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vnh.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apb.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wnf.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lsc.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mdd.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://hlr.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hno.sweek.top

[N06] 判断回文字符串
来源：http://vtv.sysykeji.top

Py:   s == s[::-1]
来源：http://mps.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://ckr.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://hdx.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://sry.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jsk.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://lkn.ybcxt.top

Ruby: s == s.reverse
来源：http://mji.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://evf.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://keu.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://icx.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gpr.daxiang520.top

JS:   // 手写 Map：map.set(v, i)
来源：http://aww.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://unv.chenlongwang.top

Java: // 手写 HashMap
来源：http://zca.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://ijg.jianghu66.top

Ruby: // 手写 Hash
来源：http://qwc.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://tqo.316326.xyz

[N08] 生成全排列
来源：http://sao.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://pih.fktsv.cn

PHP:  // 手写递归交换
来源：http://rmr.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://jog.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://rcb.smart0.xyz

Java: // 手写回溯递归
来源：http://gsz.ydjk.org.cn

Go:   // 手写回溯递归
来源：http://xxd.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://mwv.ydzc1.top

C#:   // 手写回溯递归
来源：http://drq.ydjk.org.cn

[N09] 栈与队列
来源：http://frn.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fuh.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nmg.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pxs.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iug.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jxl.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://npv.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nyj.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tkd.gogol.net.cn

[N10] 链表节点定义
来源：http://qme.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qgc.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ezb.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uig.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cpq.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://ftl.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://whv.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kjh.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zbo.yj202588.top

[N11] 二叉树中序遍历
来源：http://avb.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dsy.feifeiyinyue.top

PHP:  // 手写递归函数
来源：http://ufx.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txy.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmj.yanxiufei.cn

Java: // 手写递归
来源：http://mmq.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://vnr.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://siv.hywenlv.cn

C#:   // 手写递归
来源：http://noz.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jua.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szw.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ttg.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lci.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wuo.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qim.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bzs.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bwg.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uyk.yuxming.cn

================================================================================
来源：http://kjt.wangdashe.top

O. 并发与异步
来源：http://vqb.ywan-chungtsiang.top

================================================================================
来源：http://qkg.yueranfly.top

[O01] 启动一个线程
来源：http://epn.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ubg.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tja.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ciq.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://jlr.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://aww.jqgufenzy.top

Go:   go f()
来源：http://gdk.andypj.xyz

Ruby: Thread.new { f }
来源：http://hgt.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://ebh.fengsongda.top

[O02] 使用线程池
来源：http://odb.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iir.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jkw.zycfv.cn

JS:   // worker_threads 线程池
来源：http://wbb.hnqzz.top

TS:   // worker_threads 线程池
来源：http://rky.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://wiw.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lpy.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jrt.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dub.meibo888.top

[O03] 加锁保护共享数据
来源：http://eol.haohaochexian.top

Py:   with lock: shared += 1
来源：http://qca.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://zag.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wty.redwolf501.top

TS:   // 同 JS
来源：http://sil.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://utr.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://udi.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ioo.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://jxc.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://lcp.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://tfa.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zfy.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://ioq.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://etj.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://spa.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hee.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://wgr.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://mtl.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://xhm.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://fhj.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wqo.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://eex.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://xpl.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pcw.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lnq.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://xxb.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://elz.haohaochexian.top

[O06] 使用进程池
来源：http://lyg.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://snt.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zuq.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://jgx.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://ovs.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xlv.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://juo.shuidangran.top

Ruby: // fork 块
来源：http://tjc.yanxiufei.cn

C#:   Parallel.For
来源：http://gbw.daxiang520.top

================================================================================
来源：http://kkg.kuanghao11.cn

P. 常用工具函数
来源：http://ktl.meibo888.top

================================================================================
来源：http://buz.dashuyun.cn

[P01] 生成 UUID
来源：http://cca.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://wpa.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://psc.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://brf.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://xdt.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://oph.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://wpp.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://dql.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://bjp.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://ojq.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tat.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://tde.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jjr.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aeu.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pkv.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uoo.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aoa.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xba.vehdjk.com

[P03] 生成短随机字符串
来源：http://wvg.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mwj.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nmx.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xff.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jzw.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://czv.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bpt.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fnu.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cbk.aizwys.cn

[P04] 求长度
来源：http://yhl.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nkv.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qsx.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qwt.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwf.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://opj.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://obm.yuanzhike.top

Ruby: x.length;  x.size
来源：http://rfx.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://cjb.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://fnl.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mcl.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ohx.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rkq.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aop.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://myh.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://vmy.svipenyu.cn

Ruby: a == b
来源：http://qew.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bey.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zvt.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kwc.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://rwy.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rab.vqdsnc.cn

TS:   if (x == null) {}
来源：http://oxt.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tzk.quarkkingdee.top

Go:   if x == nil {}
来源：http://poj.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lwh.redwolf501.top

C#:   if (x is null) {}
来源：http://itv.yangfankeji.com

[P07] 防抖与节流
来源：http://wxf.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tma.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://cvq.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tup.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kaa.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://glm.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://edz.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vsq.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lhv.jiagoushi.top

[P08] 处理浮点精度问题
来源：http://wvr.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jjq.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eds.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ned.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nju.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qhy.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rxz.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xaq.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tzb.cashguo.top

================================================================================
来源：http://ivy.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://anw.zhoulong.xyz

================================================================================
来源：http://mmz.ydjk.org.cn

[Q01] 创建表
来源：http://jqd.cdnleiting.top

CREATE TABLE users (
来源：http://qzo.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mqz.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://qea.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://rnw.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bym.guowangkeji.top

);
来源：http://rwo.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://nsa.hysaishi.cn

CREATE TABLE orders (
来源：http://zek.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bpk.yonumen.top

user_id INT NOT NULL,
来源：http://cph.wangdashe.top

amount DECIMAL(10, 2),
来源：http://cgw.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ahd.hysaishi.cn

);
来源：http://dky.sysykeji.top

[Q03] 增加列
来源：http://rrs.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qti.sufxvd.cn

[Q04] 修改列类型
来源：http://hwf.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mky.tianlin.xyz

[Q05] 重命名列
来源：http://pot.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rny.gzhubu.top

[Q06] 删除列
来源：http://grb.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://hpp.epnwcf.com

[Q07] 删除表
来源：http://hti.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://arg.nanxinkj.top

[Q08] 创建普通索引
来源：http://xef.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://roj.ctjpmb.com

[Q09] 创建唯一索引
来源：http://qqx.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fyz.zdqjudy.top

[Q10] 插入单行
来源：http://cle.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nnc.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://jfs.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wtk.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://ldm.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://gly.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ety.fzhhl.top

[Q13] 忽略重复插入
来源：http://sgo.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ssh.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://whn.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tfk.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qvw.vqdsnc.cn

[Q15] 查询全部
来源：http://khf.quarkkingdee.top

SELECT * FROM users;
来源：http://eux.52xcode.cn

[Q16] 查询指定列
来源：http://ufo.birdmap.top

SELECT id, name FROM users;
来源：http://fgw.9152youxi.cn

[Q17] 条件查询
来源：http://qwl.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dyp.svipenyu.cn

[Q18] 模糊匹配
来源：http://mtu.jinqigfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xph.epnwcf.com

[Q19] 范围查询
来源：http://jxj.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sxj.gzhubu.top

[Q20] IN 列表
来源：http://wyw.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wiq.zhixingplan.top

[Q21] 空值判断
来源：http://vei.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ygx.zdqjudy.top

[Q22] 排序
来源：http://dsy.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nfg.chenzaomai.com

[Q23] 分页
来源：http://rfr.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fyq.zhaomingkeji.xyz

[Q24] 去重
来源：http://yjy.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://xcc.yonumen.top

[Q25] 只取前 N 条
来源：http://leo.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gpn.feifeiyinyue.top

[Q26] 计数
来源：http://xxl.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://hxo.daria6918.cn

[Q27] 条件计数
来源：http://zul.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nzi.hysaishi.cn

[Q28] 求和与平均
来源：http://tfc.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hlp.dianchejie.cn

[Q29] 最大最小值
来源：http://mfu.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jgb.birdmap.top

[Q30] 分组统计
来源：http://hkh.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ied.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://fot.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fem.tian-w.cn

[Q32] 分组拼接字符串
来源：http://fho.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uxc.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ugp.hongshengwenyu.top

[Q33] 多列分组
来源：http://eki.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mhq.9152youxi.cn

[Q34] 每组取第一条
来源：http://ohx.jiagoushi.top

SELECT * FROM (
来源：http://gcz.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cmq.hysaishi.cn

) t WHERE rn = 1;
来源：http://ssi.zhijiandao.cn

[Q35] 内连接
来源：http://ist.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rfc.fktsv.cn


<!-- 参考信息 -->