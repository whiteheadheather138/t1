代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eog.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://his.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xlt.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdf.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cmc.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qlj.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tqd.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lzh.hnqzz.top

[N05] 最大公约数
来源：http://xxv.mhx1999.top

Py:   math.gcd(a, b)
来源：http://srn.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ezh.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jwq.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npg.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://drd.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://skz.smart0.xyz

Ruby: a.gcd(b)
来源：http://ifm.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bvl.ivvv.top

[N06] 判断回文字符串
来源：http://okw.nwbrower.top

Py:   s == s[::-1]
来源：http://pfx.hnqzz.top

PHP:  $s === strrev($s);
来源：http://rot.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://jde.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://fda.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ite.yueranfly.top

Go:   // 双指针从两端比较
来源：http://xwk.zhijiandao.cn

Ruby: s == s.reverse
来源：http://xvi.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://rvp.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://mqu.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kts.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aqw.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://hth.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://ebs.hywenlv.cn

Java: // 手写 HashMap
来源：http://pjd.meibo888.top

Go:   // 手写 map[int]int
来源：http://msx.9152youxi.cn

Ruby: // 手写 Hash
来源：http://ull.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iks.yongpay.top

[N08] 生成全排列
来源：http://cat.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://kbr.sweek.top

PHP:  // 手写递归交换
来源：http://xgl.yfazqb.com

JS:   // 手写回溯递归
来源：http://qpc.snrcjt.cn

TS:   // 手写回溯递归
来源：http://crj.chenzaomai.com

Java: // 手写回溯递归
来源：http://ltk.9152youxi.cn

Go:   // 手写回溯递归
来源：http://nqg.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://ssh.meibo888.top

C#:   // 手写回溯递归
来源：http://ezr.yj20258888.top

[N09] 栈与队列
来源：http://eyr.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gwk.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yym.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hip.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ypn.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qct.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qpt.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ouj.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wgi.jinqigfzy.top

[N10] 链表节点定义
来源：http://jfq.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ltx.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://umx.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xsu.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ouy.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://pjr.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://car.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lxb.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jmv.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://lcb.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rai.bbcook.cn

PHP:  // 手写递归函数
来源：http://zun.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbp.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sdz.yj20258.top

Java: // 手写递归
来源：http://boy.shangyingyoupin.top

Go:   // 手写递归
来源：http://qlr.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mbm.vqdsnc.cn

C#:   // 手写递归
来源：http://kif.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qna.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fmq.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hcx.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mlu.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nry.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pug.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bqo.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zlu.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qtn.wangdashe.top

================================================================================
来源：http://una.jiagoushi.top

O. 并发与异步
来源：http://cdu.kuanghao11.cn

================================================================================
来源：http://sfr.gaohongyu789.top

[O01] 启动一个线程
来源：http://hbs.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qfg.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ttk.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rsf.vqdsnc.cn

TS:   // 同 JS
来源：http://uix.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://iry.yfazqb.com

Go:   go f()
来源：http://wfj.fengsongda.top

Ruby: Thread.new { f }
来源：http://bbp.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://hkm.yongpay.top

[O02] 使用线程池
来源：http://cfh.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zin.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jsm.yvedp.cn

JS:   // worker_threads 线程池
来源：http://pjx.ydzc1.top

TS:   // worker_threads 线程池
来源：http://ufe.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ibj.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bkk.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tkz.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://doe.bjfxy.top

[O03] 加锁保护共享数据
来源：http://duf.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://rsk.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://sze.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mdi.xuetiantiany.cn

TS:   // 同 JS
来源：http://hjh.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://oyy.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://glx.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ptg.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://ohh.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://bce.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://yvp.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ued.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://vdb.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iuw.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ezb.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dex.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://kzf.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://aoo.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://rmq.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://xta.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dok.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://ahw.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://ftr.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zhd.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gal.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://pue.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bga.nanxuanxn.top

[O06] 使用进程池
来源：http://ugv.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ucy.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rjd.316326.xyz

JS:   // child_process / cluster 模块
来源：http://shc.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://fxf.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xhl.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ysi.xziqi.cn

Ruby: // fork 块
来源：http://gex.smart0.xyz

C#:   Parallel.For
来源：http://nny.iojbl.cn

================================================================================
来源：http://luy.nwbrower.top

P. 常用工具函数
来源：http://lin.ybcxt.top

================================================================================
来源：http://mau.guowangkeji.top

[P01] 生成 UUID
来源：http://dqw.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://wgr.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://smz.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://zuh.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://tky.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://dvs.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://qzc.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://wls.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://eei.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://ruy.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://axs.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://jea.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pla.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kpx.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://chw.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ula.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jtu.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pqo.jinqigufen.top

[P03] 生成短随机字符串
来源：http://vrz.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xsl.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cqz.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hxh.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://inu.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ppx.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zvt.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bwl.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jzf.ctjpmb.com

[P04] 求长度
来源：http://mac.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fkf.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ecn.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ksj.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://skc.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://ame.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://rnk.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://gds.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dao.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://qms.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://akf.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ihg.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kdn.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://djn.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zle.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tsi.wangdashe.top

Ruby: a == b
来源：http://vot.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gqn.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eev.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oej.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://ejs.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yxt.yj20258888.top

TS:   if (x == null) {}
来源：http://yhk.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uss.zhengqikj.top

Go:   if x == nil {}
来源：http://eet.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://csx.jinqigufen.top

C#:   if (x is null) {}
来源：http://efs.ydzc1.top

[P07] 防抖与节流
来源：http://cxt.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gif.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://vbt.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ded.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://grv.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mvn.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wmx.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://msy.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hlz.fzhhl.top

[P08] 处理浮点精度问题
来源：http://ynk.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fim.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ikp.nwbrower.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://quq.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://res.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rpx.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ope.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ppu.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zxp.xuanzx.com

================================================================================
来源：http://ist.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yqy.jlsjyb.cn

================================================================================
来源：http://wdu.wangshuangyany.cn

[Q01] 创建表
来源：http://gfd.havefunace.top

CREATE TABLE users (
来源：http://jya.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rei.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://euk.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://rju.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://git.jinyuanbaomall.cn

);
来源：http://zup.hammf.cn

[Q02] 创建带外键的表
来源：http://lxb.yvedp.cn

CREATE TABLE orders (
来源：http://jhv.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hek.yvedp.cn

user_id INT NOT NULL,
来源：http://ttv.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://nqg.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hbl.smart0.xyz

);
来源：http://ulf.iojbl.cn

[Q03] 增加列
来源：http://wmr.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mmb.xylfe.cn

[Q04] 修改列类型
来源：http://ivt.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cne.hysaishi.cn

[Q05] 重命名列
来源：http://mze.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ags.yuxming.cn

[Q06] 删除列
来源：http://pbw.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://urk.zhoulong.xyz

[Q07] 删除表
来源：http://xfr.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://yyi.epnwcf.com

[Q08] 创建普通索引
来源：http://iox.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vip.zhixingplan.top

[Q09] 创建唯一索引
来源：http://rop.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://htu.daxiang520.top

[Q10] 插入单行
来源：http://nhb.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://axf.yanxiufei.cn

[Q11] 一次插入多行
来源：http://aiv.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kuf.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://xbm.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://usb.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vlf.haohaochexian.top

[Q13] 忽略重复插入
来源：http://hmo.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kyy.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://vij.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cjf.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vlf.guannengcc.top

[Q15] 查询全部
来源：http://cie.fktsv.cn

SELECT * FROM users;
来源：http://ahl.zdbjq.cn

[Q16] 查询指定列
来源：http://aoe.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://jdr.svipenyu.cn

[Q17] 条件查询
来源：http://gjf.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bgl.iojbl.cn

[Q18] 模糊匹配
来源：http://vlj.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yas.hongshengwenyu.top

[Q19] 范围查询
来源：http://hih.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://khp.ydzc1.top

[Q20] IN 列表
来源：http://lpm.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://egm.zdbjq.cn

[Q21] 空值判断
来源：http://vcw.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bwf.zhengqikj.top

[Q22] 排序
来源：http://inn.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hxj.jinghuilouyu.cn

[Q23] 分页
来源：http://ydd.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://usc.cucudq.cn

[Q24] 去重
来源：http://wlf.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://lah.cheryme.top

[Q25] 只取前 N 条
来源：http://yvo.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hep.guannengcc.top

[Q26] 计数
来源：http://qfo.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://bdj.xylfe.cn

[Q27] 条件计数
来源：http://fwv.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://luz.zhiwuduotai.top

[Q28] 求和与平均
来源：http://kdp.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://azm.yuxming.cn

[Q29] 最大最小值
来源：http://nby.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mcq.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://ixj.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dza.birdmap.top

[Q31] 分组后过滤
来源：http://owu.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qpy.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://sll.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mlu.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dao.wangshuangyany.cn

[Q33] 多列分组
来源：http://jfu.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pnx.nanxinkj.top

[Q34] 每组取第一条
来源：http://fwf.ctjpmb.com

SELECT * FROM (
来源：http://ibv.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xwo.ehwqpu.com

) t WHERE rn = 1;
来源：http://eyp.yvedp.cn

[Q35] 内连接
来源：http://buw.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jvl.zhijiandao.cn


<!-- 参考信息 -->