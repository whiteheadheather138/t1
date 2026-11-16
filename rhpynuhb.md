代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jkx.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jua.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://clf.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gzl.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://llv.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hey.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vuv.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dws.cdnleiting.top

[N05] 最大公约数
来源：http://ohh.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://vkh.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ttj.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qil.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tuj.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ylv.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eco.cqqwz.cn

Ruby: a.gcd(b)
来源：http://vyq.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxv.sjlbkw.cn

[N06] 判断回文字符串
来源：http://ucw.xinyue.icu

Py:   s == s[::-1]
来源：http://uvs.cucudq.cn

PHP:  $s === strrev($s);
来源：http://klz.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://vrl.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://xal.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zax.ydzc1.top

Go:   // 双指针从两端比较
来源：http://umw.meibo888.top

Ruby: s == s.reverse
来源：http://edm.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mdu.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://pme.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kna.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wdv.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ytl.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://xem.sjlbkw.cn

Java: // 手写 HashMap
来源：http://bdg.daxiang520.top

Go:   // 手写 map[int]int
来源：http://rlz.daxiang520.top

Ruby: // 手写 Hash
来源：http://ebm.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://skp.cheryme.top

[N08] 生成全排列
来源：http://byk.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://ndp.nanxinkj.top

PHP:  // 手写递归交换
来源：http://mpu.guannengcc.top

JS:   // 手写回溯递归
来源：http://zfb.hysaishi.cn

TS:   // 手写回溯递归
来源：http://gsc.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://zaz.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://edl.yonumen.top

Ruby: arr.permutation.to_a
来源：http://fay.tanke756.top

C#:   // 手写回溯递归
来源：http://czo.svipenyu.cn

[N09] 栈与队列
来源：http://lru.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://amk.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wcc.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qdi.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kve.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jig.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zxc.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mzg.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lcc.yvedp.cn

[N10] 链表节点定义
来源：http://pvv.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xuo.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cwf.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hhw.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aad.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://ppt.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oux.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ktd.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tbd.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://mlf.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ekp.snrcjt.cn

PHP:  // 手写递归函数
来源：http://hvx.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ran.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tnn.mhx1999.top

Java: // 手写递归
来源：http://hch.gogol.net.cn

Go:   // 手写递归
来源：http://wrx.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://riz.zhongyouzk.top

C#:   // 手写递归
来源：http://grm.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jki.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://klw.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xxk.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nza.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uei.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jzg.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://all.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rbe.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fob.cqqwz.cn

================================================================================
来源：http://wrs.yvedp.cn

O. 并发与异步
来源：http://cqk.epnwcf.com

================================================================================
来源：http://wxl.guowangkeji.top

[O01] 启动一个线程
来源：http://hsi.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xdb.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fze.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fcm.gotoacloud.top

TS:   // 同 JS
来源：http://sos.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://ili.xziqi.cn

Go:   go f()
来源：http://ffa.guowangkeji.top

Ruby: Thread.new { f }
来源：http://feq.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://zrk.tanke756.top

[O02] 使用线程池
来源：http://uqo.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mpc.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pex.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://ewb.bbcook.cn

TS:   // worker_threads 线程池
来源：http://lix.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://jnb.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ply.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ufm.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ofh.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://aej.316326.xyz

Py:   with lock: shared += 1
来源：http://mya.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://bkx.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vyi.bbcook.cn

TS:   // 同 JS
来源：http://udu.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://vuv.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cdi.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nud.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://usd.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://riu.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://rya.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ndu.yuxming.cn

JS:   async function f() { await g(); }
来源：http://oms.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://lgh.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://inc.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tuz.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://fzl.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://xkt.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://gir.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://mqk.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jqc.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://ogj.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://nar.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gox.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pdf.epnwcf.com

Ruby: threads.map(&:join)
来源：http://eod.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://puo.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://kvn.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ibr.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wnr.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://ure.yj20258.top

TS:   // child_process / cluster 模块
来源：http://oig.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cnp.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nlh.zhongyouzk.top

Ruby: // fork 块
来源：http://vzd.epnwcf.com

C#:   Parallel.For
来源：http://lnj.vehdjk.com

================================================================================
来源：http://zuv.shuidangran.top

P. 常用工具函数
来源：http://jmu.chenzaomai.com

================================================================================
来源：http://xec.zhiwuduotai.top

[P01] 生成 UUID
来源：http://bgf.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://mzt.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nsm.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://ejw.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://are.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://vvd.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://aaj.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://etu.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://iyd.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://lpu.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jcg.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vav.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wgw.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xue.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ckb.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lwc.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zjg.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mal.birdmap.top

[P03] 生成短随机字符串
来源：http://yuu.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hmf.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iwq.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqy.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mnu.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://udc.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zam.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lkt.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xye.ivvv.top

[P04] 求长度
来源：http://hpu.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aay.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oty.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rmd.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hdi.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://esv.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://env.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://qvc.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vei.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://ofd.jinqigfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eoq.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ghl.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gic.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nxr.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ypg.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://tgs.snrcjt.cn

Ruby: a == b
来源：http://zim.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://phi.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://duu.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bka.meibo888.top

PHP:  if (empty($x)) {}
来源：http://jux.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tue.tarul.cn

TS:   if (x == null) {}
来源：http://cvz.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bma.xziqi.cn

Go:   if x == nil {}
来源：http://unn.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ayj.shzxlz.cn

C#:   if (x is null) {}
来源：http://mxq.sysykeji.top

[P07] 防抖与节流
来源：http://tpr.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hsd.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://enf.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kub.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbk.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://koo.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ntv.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://yuy.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zwt.fengsongda.top

[P08] 处理浮点精度问题
来源：http://hvu.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zzs.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ytb.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nji.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rwa.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rgs.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mya.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hti.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sit.hywenlv.cn

================================================================================
来源：http://iqx.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ovf.cdnleiting.top

================================================================================
来源：http://hqr.pycfn.com

[Q01] 创建表
来源：http://axz.sufxvd.cn

CREATE TABLE users (
来源：http://jeh.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sou.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://jlh.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://rks.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nez.fengsongda.top

);
来源：http://kfv.jinqigufen.top

[Q02] 创建带外键的表
来源：http://sll.ivvv.top

CREATE TABLE orders (
来源：http://adb.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xdf.ybcxt.top

user_id INT NOT NULL,
来源：http://wuz.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://sui.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gbf.hysaishi.cn

);
来源：http://pnu.dashuyun.cn

[Q03] 增加列
来源：http://mnj.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gfz.guannengcc.top

[Q04] 修改列类型
来源：http://brz.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ejp.guannengcc.top

[Q05] 重命名列
来源：http://khl.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sev.shanyushiyangtech.top

[Q06] 删除列
来源：http://gth.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://sss.vehdjk.com

[Q07] 删除表
来源：http://pnk.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://dzf.316326.xyz

[Q08] 创建普通索引
来源：http://qgk.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://pif.hnqzz.top

[Q09] 创建唯一索引
来源：http://zft.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rep.tianlin.xyz

[Q10] 插入单行
来源：http://xqw.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fiy.wangdashe.top

[Q11] 一次插入多行
来源：http://ess.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://syg.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://yyh.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://wsn.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ngm.zhixingplan.top

[Q13] 忽略重复插入
来源：http://noh.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rnt.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://itg.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fld.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dum.ydjk.org.cn

[Q15] 查询全部
来源：http://mqr.quarkkingdee.top

SELECT * FROM users;
来源：http://hks.cucudq.cn

[Q16] 查询指定列
来源：http://bwq.ydjk.org.cn

SELECT id, name FROM users;
来源：http://zux.yfazqb.com

[Q17] 条件查询
来源：http://jyl.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://drd.tarul.cn

[Q18] 模糊匹配
来源：http://atr.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tyr.shzxlz.cn

[Q19] 范围查询
来源：http://lwt.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yyb.hcnkem.com

[Q20] IN 列表
来源：http://pca.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bqx.chenlongwang.top

[Q21] 空值判断
来源：http://agl.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://rio.xinyue.icu

[Q22] 排序
来源：http://hlm.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fis.hammf.cn

[Q23] 分页
来源：http://bny.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pgi.wangdashe.top

[Q24] 去重
来源：http://buk.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://nno.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://djd.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ufr.tanke756.top

[Q26] 计数
来源：http://uqn.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://shn.wangdashe.top

[Q27] 条件计数
来源：http://wko.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://orc.nanxinkj.top

[Q28] 求和与平均
来源：http://ixv.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aor.ppjwa.cn

[Q29] 最大最小值
来源：http://ims.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pft.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://xga.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dpv.yanxiufei.cn

[Q31] 分组后过滤
来源：http://bri.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mda.iojbl.cn

[Q32] 分组拼接字符串
来源：http://pox.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kqj.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://puy.zdqjudy.top

[Q33] 多列分组
来源：http://bzo.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uff.shuidangran.top

[Q34] 每组取第一条
来源：http://qgh.yj20258.top

SELECT * FROM (
来源：http://cta.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dpq.aizwys.cn

) t WHERE rn = 1;
来源：http://grh.hysaishi.cn

[Q35] 内连接
来源：http://wkm.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cxa.tarul.cn


<!-- 参考信息 -->