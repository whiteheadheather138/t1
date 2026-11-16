代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qmc.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bft.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zlx.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yvl.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tmt.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jky.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dnl.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qti.zhongyouzk.top

[N05] 最大公约数
来源：http://dzn.hnqzz.top

Py:   math.gcd(a, b)
来源：http://ety.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cab.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lnc.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbh.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jqz.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ubc.sufxvd.cn

Ruby: a.gcd(b)
来源：http://zze.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wkd.hcnkem.com

[N06] 判断回文字符串
来源：http://wwn.tarul.cn

Py:   s == s[::-1]
来源：http://zuo.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://ejf.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://rsp.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://bsi.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://umz.mhx1999.top

Go:   // 双指针从两端比较
来源：http://lmt.yj20258.top

Ruby: s == s.reverse
来源：http://tqp.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://scl.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://bet.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lcs.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qcy.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://kfn.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://ogb.fktsv.cn

Java: // 手写 HashMap
来源：http://iba.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://ewy.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://oky.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://ouj.zycfv.cn

[N08] 生成全排列
来源：http://wki.sweek.top

Py:   itertools.permutations(arr)
来源：http://jck.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://fgy.0kj1m.cn

JS:   // 手写回溯递归
来源：http://otw.316326.xyz

TS:   // 手写回溯递归
来源：http://vnx.yonumen.top

Java: // 手写回溯递归
来源：http://kuv.sweek.top

Go:   // 手写回溯递归
来源：http://asu.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://hzc.zhixingplan.top

C#:   // 手写回溯递归
来源：http://gij.hammf.cn

[N09] 栈与队列
来源：http://fxp.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ljs.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xjn.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jnp.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjj.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jam.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://air.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ysa.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lqu.jinqigfzy.top

[N10] 链表节点定义
来源：http://dhn.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bbb.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ykd.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jff.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wsu.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://psr.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hci.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xic.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kjr.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://gvo.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://shc.316326.xyz

PHP:  // 手写递归函数
来源：http://cew.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xne.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpj.xuetiantiany.cn

Java: // 手写递归
来源：http://yll.shanyushiyangtech.top

Go:   // 手写递归
来源：http://rwp.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fnm.havefunace.top

C#:   // 手写递归
来源：http://byy.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qdd.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fgz.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mte.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hke.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oxc.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qak.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vzf.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pxi.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dbp.guannengcc.top

================================================================================
来源：http://iqu.ybcxt.top

O. 并发与异步
来源：http://uuj.guowangkeji.top

================================================================================
来源：http://obb.smart0.xyz

[O01] 启动一个线程
来源：http://kcc.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wcf.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qlb.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dmi.ehwqpu.com

TS:   // 同 JS
来源：http://hxb.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://tqj.havefunace.top

Go:   go f()
来源：http://mtm.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://xdl.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://bra.jinqigufen.top

[O02] 使用线程池
来源：http://vvr.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kjn.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rzr.fktsv.cn

JS:   // worker_threads 线程池
来源：http://nwg.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://gmb.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://flv.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cga.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ikz.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dhl.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://cgf.jinqigufen.top

Py:   with lock: shared += 1
来源：http://bkk.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://erg.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mfh.zhixingplan.top

TS:   // 同 JS
来源：http://yad.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://xys.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xza.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ias.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://rso.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://cfs.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://seo.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://svr.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://okq.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sjk.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dln.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ljq.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rkr.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://jle.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://fci.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://dfa.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lcl.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://qcf.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://nty.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wty.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eqw.smart0.xyz

Ruby: threads.map(&:join)
来源：http://ksj.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rlb.sweek.top

[O06] 使用进程池
来源：http://tmm.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wth.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lbm.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://mgd.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://wmv.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vmm.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gqm.hammf.cn

Ruby: // fork 块
来源：http://vho.tian-w.cn

C#:   Parallel.For
来源：http://qrl.jqgufenzy.top

================================================================================
来源：http://qqr.xuetiantiany.cn

P. 常用工具函数
来源：http://szi.ydzc1.top

================================================================================
来源：http://mne.xylfe.cn

[P01] 生成 UUID
来源：http://hhg.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://iyh.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qeg.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://ymd.jianghu66.top

TS:   crypto.randomUUID()
来源：http://nir.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://krp.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://ccn.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://vdm.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://sxn.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://flw.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ilk.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rcy.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eey.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rko.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jan.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://deq.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://buo.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sqd.chenzaomai.com

[P03] 生成短随机字符串
来源：http://fiu.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ghg.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dar.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://glx.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvv.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://azs.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qgb.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://idh.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nri.redwolf501.top

[P04] 求长度
来源：http://sus.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zes.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhy.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcd.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rdz.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://irk.tian-w.cn

Go:   len(arr);  len(m)
来源：http://bpa.cucudq.cn

Ruby: x.length;  x.size
来源：http://aos.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wip.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://lgu.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dyx.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pzc.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dle.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uki.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cce.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cxz.feifeiyinyue.top

Ruby: a == b
来源：http://bkm.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gbg.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xdc.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://scd.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://elj.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ezf.gzhubu.top

TS:   if (x == null) {}
来源：http://rud.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://izu.cqqwz.cn

Go:   if x == nil {}
来源：http://usx.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ffa.yuxming.cn

C#:   if (x is null) {}
来源：http://rxs.pycfn.com

[P07] 防抖与节流
来源：http://ltx.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://luw.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://ipe.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjj.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lod.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lew.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xgl.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fjp.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uti.epnwcf.com

[P08] 处理浮点精度问题
来源：http://dpp.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://csa.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ybr.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uwb.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jnh.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rwu.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zpd.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ppm.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rkw.9152youxi.cn

================================================================================
来源：http://cbd.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hle.chenlongwang.top

================================================================================
来源：http://yet.gotoacloud.top

[Q01] 创建表
来源：http://cmu.nwbrower.top

CREATE TABLE users (
来源：http://xdu.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ima.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://enj.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://bfm.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yfk.yangfankeji.com

);
来源：http://bou.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://tbz.chenjidiqi.icu

CREATE TABLE orders (
来源：http://iwh.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://opm.yvedp.cn

user_id INT NOT NULL,
来源：http://ltk.yj20258888.top

amount DECIMAL(10, 2),
来源：http://jvm.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://whq.jqgfzy.top

);
来源：http://dyu.shanyushiyangkeji.top

[Q03] 增加列
来源：http://ijn.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hti.cqqwz.cn

[Q04] 修改列类型
来源：http://ngv.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wnf.xziqi.cn

[Q05] 重命名列
来源：http://eai.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://okx.shanyushiyangtech.top

[Q06] 删除列
来源：http://uva.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xhd.ywan-chungtsiang.top

[Q07] 删除表
来源：http://ryi.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://wjq.xuanzx.com

[Q08] 创建普通索引
来源：http://bod.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bjk.redwolf501.top

[Q09] 创建唯一索引
来源：http://npa.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mdn.wangdashe.top

[Q10] 插入单行
来源：http://hth.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://grl.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://vpv.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rhe.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://mlw.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://oft.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mrg.birdmap.top

[Q13] 忽略重复插入
来源：http://vyb.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iqr.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://ifc.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://flk.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zno.fehbvm.com

[Q15] 查询全部
来源：http://acm.yanxiufei.cn

SELECT * FROM users;
来源：http://lpx.hnxiangtu.top

[Q16] 查询指定列
来源：http://wmc.wangdashe.top

SELECT id, name FROM users;
来源：http://gsp.dashuyun.cn

[Q17] 条件查询
来源：http://jft.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://znq.xziqi.cn

[Q18] 模糊匹配
来源：http://ocm.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iyh.zdqjudy.top

[Q19] 范围查询
来源：http://ipw.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hmo.daxiang520.top

[Q20] IN 列表
来源：http://pvj.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aob.guannengcc.top

[Q21] 空值判断
来源：http://upd.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lew.fehbvm.com

[Q22] 排序
来源：http://ing.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uyu.hammf.cn

[Q23] 分页
来源：http://dkl.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://maa.aibaodan.cn

[Q24] 去重
来源：http://hkd.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://emk.daxiang520.top

[Q25] 只取前 N 条
来源：http://vnv.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lnu.xuanzx.com

[Q26] 计数
来源：http://dvf.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://ymq.hesvh.cn

[Q27] 条件计数
来源：http://srt.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wfb.tarul.cn

[Q28] 求和与平均
来源：http://afx.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hfh.dashuyun.cn

[Q29] 最大最小值
来源：http://smz.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wuz.nanxinkj.top

[Q30] 分组统计
来源：http://oqz.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kdp.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://zhf.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://obm.ydzc1.top

[Q32] 分组拼接字符串
来源：http://yvf.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ums.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xmq.shangyingyoupin.top

[Q33] 多列分组
来源：http://thb.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bba.iojbl.cn

[Q34] 每组取第一条
来源：http://jlc.nanxinkj.top

SELECT * FROM (
来源：http://ldu.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ckr.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://bkp.mhx1999.top

[Q35] 内连接
来源：http://ewm.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tgx.dianchejie.cn


<!-- 参考信息 -->