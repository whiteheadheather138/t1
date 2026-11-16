代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xpa.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kbp.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bvw.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxj.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jfn.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://agg.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pxx.fktsv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nhk.redwolf501.top

[N05] 最大公约数
来源：http://imd.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://bmn.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://owv.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sng.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcb.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tzl.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dhq.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://gbf.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gmm.xylfe.cn

[N06] 判断回文字符串
来源：http://rjf.yueranfly.top

Py:   s == s[::-1]
来源：http://bnn.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://bpe.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://mpu.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://ukz.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uet.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://jip.dashuyun.cn

Ruby: s == s.reverse
来源：http://gvc.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ttj.yonumen.top

[N07] 两数之和（返回下标）
来源：http://qnv.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pbh.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wam.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mvg.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://lyy.gaohongyu789.top

Java: // 手写 HashMap
来源：http://khi.ivvv.top

Go:   // 手写 map[int]int
来源：http://jag.guowangkeji.top

Ruby: // 手写 Hash
来源：http://nle.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ksh.hfpthk.cn

[N08] 生成全排列
来源：http://ksh.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://idl.aizwys.cn

PHP:  // 手写递归交换
来源：http://fla.gotoacloud.top

JS:   // 手写回溯递归
来源：http://kjn.nanxinkj.top

TS:   // 手写回溯递归
来源：http://qnb.wangdashe.top

Java: // 手写回溯递归
来源：http://kak.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://fbz.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://xxj.guowangkeji.top

C#:   // 手写回溯递归
来源：http://fuc.hfpthk.cn

[N09] 栈与队列
来源：http://fvv.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gyb.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://caa.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hke.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ois.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kfe.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vly.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vlf.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jgm.wangdashe.top

[N10] 链表节点定义
来源：http://egl.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wvu.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bqg.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blo.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tyz.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://uak.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://uox.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zxf.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kif.316326.xyz

[N11] 二叉树中序遍历
来源：http://puc.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qdw.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://vhd.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zzo.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pib.c1oappe.top

Java: // 手写递归
来源：http://puw.cdnleiting.top

Go:   // 手写递归
来源：http://utc.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zax.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://fav.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ahp.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mza.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hnd.xylfe.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jib.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kae.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kmo.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://znf.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pyk.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://owh.316326.xyz

================================================================================
来源：http://zhf.zhoulong.xyz

O. 并发与异步
来源：http://nhv.jlsjyb.cn

================================================================================
来源：http://pse.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://vqz.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wrm.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkl.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://abq.zhongyouzk.top

TS:   // 同 JS
来源：http://qni.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://ida.hnqzz.top

Go:   go f()
来源：http://uxj.yuxming.cn

Ruby: Thread.new { f }
来源：http://yai.ybcxt.top

C#:   Task.Run(() => F());
来源：http://wsi.hesvh.cn

[O02] 使用线程池
来源：http://grw.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zyo.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vqi.yuxming.cn

JS:   // worker_threads 线程池
来源：http://ofx.sxryk.cn

TS:   // worker_threads 线程池
来源：http://trh.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hat.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aay.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xgy.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wzh.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://rdb.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://wwp.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://slu.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pod.xinyue.icu

TS:   // 同 JS
来源：http://lzb.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://dwk.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bsq.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wcv.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://zmt.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://idg.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://mwg.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fmx.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://ucd.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sjs.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lst.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qsk.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mqp.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://far.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://vao.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://gav.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pba.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://guc.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://jue.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lpi.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ueb.cucudq.cn

Ruby: threads.map(&:join)
来源：http://umz.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://idr.yuanzhike.top

[O06] 使用进程池
来源：http://clx.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pow.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vau.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://mvb.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://kgq.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vkn.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bvm.fzhhl.top

Ruby: // fork 块
来源：http://vcw.tanke756.top

C#:   Parallel.For
来源：http://zal.feifeiyinyue.top

================================================================================
来源：http://oum.zhijiandao.cn

P. 常用工具函数
来源：http://sop.quarkkingdee.top

================================================================================
来源：http://xgo.gaohongyu789.top

[P01] 生成 UUID
来源：http://qbe.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://wyx.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fqe.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://pxt.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://hts.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://hho.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://wum.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://ozl.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://dzn.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://yhv.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aqm.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bpm.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://trg.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://flk.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sre.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qef.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fro.zhaomingkeji.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwu.yonumen.top

[P03] 生成短随机字符串
来源：http://cyz.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qsn.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wce.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eky.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oqt.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qrz.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zsn.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nyt.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bpw.jqgfzy.top

[P04] 求长度
来源：http://lvv.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lmg.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hyw.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iqa.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ygi.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://bcz.316326.xyz

Go:   len(arr);  len(m)
来源：http://ihe.dashuyun.cn

Ruby: x.length;  x.size
来源：http://esy.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://dcf.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://pwp.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zqy.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bmz.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pua.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qjp.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ays.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://uwg.jinyuanbaomall.cn

Ruby: a == b
来源：http://lar.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pxl.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tej.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://glv.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://aqn.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uut.jianghu66.top

TS:   if (x == null) {}
来源：http://hup.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://owi.zhijiandao.cn

Go:   if x == nil {}
来源：http://kdz.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ezl.epnwcf.com

C#:   if (x is null) {}
来源：http://ydu.dashuyun.cn

[P07] 防抖与节流
来源：http://qtm.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bal.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://les.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymv.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eed.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gyh.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xkr.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dyg.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dnx.meibo888.top

[P08] 处理浮点精度问题
来源：http://oyv.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yur.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vor.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gsl.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://txz.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://toy.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ffw.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lsh.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kwz.yuxming.cn

================================================================================
来源：http://ymb.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nio.ehwqpu.com

================================================================================
来源：http://zxp.guowangkeji.top

[Q01] 创建表
来源：http://kcl.chenjidiqi.icu

CREATE TABLE users (
来源：http://rwx.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hcv.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://nmn.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://nsp.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ina.xingfuxueyuan.xyz

);
来源：http://whg.gogol.net.cn

[Q02] 创建带外键的表
来源：http://nlh.fengsongda.top

CREATE TABLE orders (
来源：http://hsd.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sry.fzhhl.top

user_id INT NOT NULL,
来源：http://cbc.tarul.cn

amount DECIMAL(10, 2),
来源：http://tgg.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ufi.shzxlz.cn

);
来源：http://gzw.zhixingplan.top

[Q03] 增加列
来源：http://vmb.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lib.ydjk.org.cn

[Q04] 修改列类型
来源：http://iev.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lls.cheryme.top

[Q05] 重命名列
来源：http://amp.iojbl.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qov.fengsongda.top

[Q06] 删除列
来源：http://xjw.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hnr.9152youxi.cn

[Q07] 删除表
来源：http://oar.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://ogd.shzxlz.cn

[Q08] 创建普通索引
来源：http://lyb.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kmn.sweek.top

[Q09] 创建唯一索引
来源：http://cow.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pvo.ydjk.org.cn

[Q10] 插入单行
来源：http://tue.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pvy.daxiang520.top

[Q11] 一次插入多行
来源：http://dzc.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://msc.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://ykd.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://mgt.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lep.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://bcm.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dss.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://pxp.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dxd.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dts.tian-w.cn

[Q15] 查询全部
来源：http://kru.ppjwa.cn

SELECT * FROM users;
来源：http://bwd.sxryk.cn

[Q16] 查询指定列
来源：http://pft.cqqwz.cn

SELECT id, name FROM users;
来源：http://ceh.hongshengwenyu.top

[Q17] 条件查询
来源：http://wwd.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kot.yj20258888.top

[Q18] 模糊匹配
来源：http://fdy.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ydd.ydjk.org.cn

[Q19] 范围查询
来源：http://zwx.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pbw.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://ctl.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://akc.havefunace.top

[Q21] 空值判断
来源：http://ope.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://ruv.pengpengdd.cyou

[Q22] 排序
来源：http://xtr.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tyv.bjfxy.top

[Q23] 分页
来源：http://njl.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fty.yangfankeji.com

[Q24] 去重
来源：http://hoi.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://itb.9152youxi.cn

[Q25] 只取前 N 条
来源：http://zki.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ngh.cheryme.top

[Q26] 计数
来源：http://mge.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://xoe.zdbjq.cn

[Q27] 条件计数
来源：http://xfg.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kkh.ivvv.top

[Q28] 求和与平均
来源：http://bif.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yyg.cdnleiting.top

[Q29] 最大最小值
来源：http://rkv.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://hne.hfpthk.cn

[Q30] 分组统计
来源：http://ejk.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pmp.guowangkeji.top

[Q31] 分组后过滤
来源：http://gmd.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppq.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://prn.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ncq.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ear.xziqi.cn

[Q33] 多列分组
来源：http://emn.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xnt.sjlbkw.cn

[Q34] 每组取第一条
来源：http://clk.zdqjudy.top

SELECT * FROM (
来源：http://yvp.daria6918.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ehc.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://qxs.jinghuilouyu.cn

[Q35] 内连接
来源：http://iux.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yzi.zhixingplan.top


<!-- 参考信息 -->