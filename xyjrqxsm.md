代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hbt.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utj.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rhg.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsf.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nqg.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ktv.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ixt.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nbo.hongshengwenyu.top

[N05] 最大公约数
来源：http://doy.meibo888.top

Py:   math.gcd(a, b)
来源：http://tdy.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mkh.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thc.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://phq.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nwi.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pmq.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://mwj.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sab.ppjwa.cn

[N06] 判断回文字符串
来源：http://uwl.vehdjk.com

Py:   s == s[::-1]
来源：http://izt.andypj.xyz

PHP:  $s === strrev($s);
来源：http://gnw.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://huc.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://via.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tsw.ybcxt.top

Go:   // 双指针从两端比较
来源：http://nda.9152youxi.cn

Ruby: s == s.reverse
来源：http://svq.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fyz.hammf.cn

[N07] 两数之和（返回下标）
来源：http://ivw.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xgv.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://foc.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mbc.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://ipd.ybcxt.top

Java: // 手写 HashMap
来源：http://nxd.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://uwd.sufxvd.cn

Ruby: // 手写 Hash
来源：http://tyf.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://pey.zhoulong.xyz

[N08] 生成全排列
来源：http://xhc.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://lye.zycfv.cn

PHP:  // 手写递归交换
来源：http://cig.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://oko.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://oah.cheryme.top

Java: // 手写回溯递归
来源：http://eao.yj20258.top

Go:   // 手写回溯递归
来源：http://pzl.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://pgq.hcnkem.com

C#:   // 手写回溯递归
来源：http://qhd.zhongyouzk.top

[N09] 栈与队列
来源：http://utt.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://apb.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uxq.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pez.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghv.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ref.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ljw.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wam.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ahg.yangfankeji.com

[N10] 链表节点定义
来源：http://nsh.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hlo.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ifb.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ydg.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kpt.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://yru.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cud.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://rqq.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://asn.mhx1999.top

[N11] 二叉树中序遍历
来源：http://aph.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://upf.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://hua.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://swb.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ldn.ivvv.top

Java: // 手写递归
来源：http://cbk.wangdashe.top

Go:   // 手写递归
来源：http://hvo.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ngh.daria6918.cn

C#:   // 手写递归
来源：http://uss.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aej.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ejn.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cdv.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrj.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dsj.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tmf.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jsr.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pvg.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://npf.fengsongda.top

================================================================================
来源：http://kui.ehwqpu.com

O. 并发与异步
来源：http://ajk.meibo888.top

================================================================================
来源：http://jkj.0kj1m.cn

[O01] 启动一个线程
来源：http://auv.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lgz.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zop.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tla.9152youxi.cn

TS:   // 同 JS
来源：http://bjd.sweek.top

Java: new Thread(() -> f()).start()
来源：http://tat.chenjidiqi.icu

Go:   go f()
来源：http://csi.mhx1999.top

Ruby: Thread.new { f }
来源：http://xnr.guannengcc.top

C#:   Task.Run(() => F());
来源：http://npu.yfazqb.com

[O02] 使用线程池
来源：http://crb.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tan.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eoq.yongpay.top

JS:   // worker_threads 线程池
来源：http://lrs.wangdashe.top

TS:   // worker_threads 线程池
来源：http://wwx.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://tmj.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://flq.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yqd.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jdc.smart0.xyz

[O03] 加锁保护共享数据
来源：http://yhi.tanke756.top

Py:   with lock: shared += 1
来源：http://wqf.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://jfc.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://env.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://yxb.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://dva.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://whz.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qdm.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://dgy.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://hnk.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://ivk.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cfy.mhx1999.top

JS:   async function f() { await g(); }
来源：http://kjy.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fra.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fuz.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eol.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zwx.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://ywi.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://oim.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://lsr.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hds.tanke756.top

JS:   await Promise.all(tasks)
来源：http://gxm.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://dew.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vxe.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xyy.yongpay.top

Ruby: threads.map(&:join)
来源：http://dxw.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://zsu.birdmap.top

[O06] 使用进程池
来源：http://uaw.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gub.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ywh.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://uwo.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://osz.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tli.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fsc.chenzaomai.com

Ruby: // fork 块
来源：http://ujn.pengpengdd.cyou

C#:   Parallel.For
来源：http://xuq.xuetiantiany.cn

================================================================================
来源：http://mdy.pycfn.com

P. 常用工具函数
来源：http://xqx.hcnkem.com

================================================================================
来源：http://phl.shangyingyoupin.top

[P01] 生成 UUID
来源：http://dhw.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://cao.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vis.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://bjy.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://pwr.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://qfj.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://ovo.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://mnk.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://hrd.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://rzg.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tpc.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lnx.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kfi.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zpl.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tlr.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tuk.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hvf.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bkk.ehwqpu.com

[P03] 生成短随机字符串
来源：http://wnq.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hzn.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zhv.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://krg.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pjh.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wpt.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lpx.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lgt.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qxw.ywan-chungtsiang.top

[P04] 求长度
来源：http://ixw.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nap.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://skq.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kkp.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lng.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://lua.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://div.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://pcj.yangfankeji.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tbz.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://ctt.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sij.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xwz.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://urq.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://frl.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jrw.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://whz.birdmap.top

Ruby: a == b
来源：http://pnn.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fev.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mqi.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cey.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://daq.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://owx.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://yph.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pny.aizwys.cn

Go:   if x == nil {}
来源：http://zqr.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hno.shzxlz.cn

C#:   if (x is null) {}
来源：http://szp.birdmap.top

[P07] 防抖与节流
来源：http://iuy.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ksd.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://bcn.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xdu.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ias.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qgm.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fwu.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bbh.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://osc.bjfxy.top

[P08] 处理浮点精度问题
来源：http://wmy.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jox.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gqa.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pnm.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vlb.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://agg.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jpz.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jen.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://crw.cucudq.cn

================================================================================
来源：http://gyv.zhengqikj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kor.daria6918.cn

================================================================================
来源：http://rgy.316326.xyz

[Q01] 创建表
来源：http://vmh.jinqigufen.top

CREATE TABLE users (
来源：http://ofc.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gbv.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://orz.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://vla.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fjj.gzhubu.top

);
来源：http://rai.shzxlz.cn

[Q02] 创建带外键的表
来源：http://odb.tarul.cn

CREATE TABLE orders (
来源：http://ycl.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwn.xylfe.cn

user_id INT NOT NULL,
来源：http://vck.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://gbp.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hce.zdbjq.cn

);
来源：http://czj.jlsjyb.cn

[Q03] 增加列
来源：http://rrl.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://law.andypj.xyz

[Q04] 修改列类型
来源：http://drk.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ldq.shuidangran.top

[Q05] 重命名列
来源：http://rww.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uwl.aizwys.cn

[Q06] 删除列
来源：http://brn.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://ifg.zdqjudy.top

[Q07] 删除表
来源：http://ivo.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://jxz.cucudq.cn

[Q08] 创建普通索引
来源：http://vdt.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pop.uphjek.com

[Q09] 创建唯一索引
来源：http://hcc.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qpt.daxiang520.top

[Q10] 插入单行
来源：http://esb.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rux.meibo888.top

[Q11] 一次插入多行
来源：http://yxy.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lot.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://isx.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://chr.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rik.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://sml.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hll.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://nuk.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tjz.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://awu.zdqjudy.top

[Q15] 查询全部
来源：http://nhj.jinqigfzy.top

SELECT * FROM users;
来源：http://bxd.zdbjq.cn

[Q16] 查询指定列
来源：http://jqj.tian-w.cn

SELECT id, name FROM users;
来源：http://vps.9152youxi.cn

[Q17] 条件查询
来源：http://wno.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://laz.hnxiangtu.top

[Q18] 模糊匹配
来源：http://awf.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bsh.yuanzhike.top

[Q19] 范围查询
来源：http://mgc.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lom.fehbvm.com

[Q20] IN 列表
来源：http://gzx.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vpl.jqgfzy.top

[Q21] 空值判断
来源：http://nha.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mzr.aibaodan.cn

[Q22] 排序
来源：http://odo.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jkr.yuanzhike.top

[Q23] 分页
来源：http://pfa.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://smw.nanxuanxn.top

[Q24] 去重
来源：http://zny.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://crx.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://rti.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dve.yuanzhike.top

[Q26] 计数
来源：http://ezu.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://kdl.yfazqb.com

[Q27] 条件计数
来源：http://dyz.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hqb.uphjek.com

[Q28] 求和与平均
来源：http://rmt.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mse.sweek.top

[Q29] 最大最小值
来源：http://jvy.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sha.jqgufenzy.top

[Q30] 分组统计
来源：http://vxp.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qgd.epnwcf.com

[Q31] 分组后过滤
来源：http://sbl.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fhz.cucudq.cn

[Q32] 分组拼接字符串
来源：http://nuc.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://inv.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://okf.tarul.cn

[Q33] 多列分组
来源：http://hwu.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uul.zdbjq.cn

[Q34] 每组取第一条
来源：http://ulr.guannengcc.top

SELECT * FROM (
来源：http://vvo.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qge.c1oappe.top

) t WHERE rn = 1;
来源：http://gup.chenzaomai.com

[Q35] 内连接
来源：http://rxk.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tiq.haohaochexian.top


<!-- 参考信息 -->