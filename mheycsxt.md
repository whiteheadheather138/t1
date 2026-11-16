代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vds.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ojj.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jxc.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sji.jqgfzy.top

[N05] 最大公约数
来源：http://esc.daxiang520.top

Py:   math.gcd(a, b)
来源：http://pfg.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nij.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfs.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ccl.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xfm.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nwq.ivvv.top

Ruby: a.gcd(b)
来源：http://xjf.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qdq.yj202588.top

[N06] 判断回文字符串
来源：http://ccq.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://gww.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://pkz.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://ipc.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://xmp.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ftq.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://eom.zhixingplan.top

Ruby: s == s.reverse
来源：http://qnt.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tbs.cheryme.top

[N07] 两数之和（返回下标）
来源：http://fqt.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eig.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fds.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jse.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://rkp.vqdsnc.cn

Java: // 手写 HashMap
来源：http://eff.nanxuanxn.top

Go:   // 手写 map[int]int
来源：http://njb.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://dgz.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yho.cqqwz.cn

[N08] 生成全排列
来源：http://sto.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://ury.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://vjl.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://nzf.xuanzx.com

TS:   // 手写回溯递归
来源：http://exq.tanke756.top

Java: // 手写回溯递归
来源：http://qux.fengsongda.top

Go:   // 手写回溯递归
来源：http://yug.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://fug.haohaochexian.top

C#:   // 手写回溯递归
来源：http://lse.zhongyouzk.top

[N09] 栈与队列
来源：http://udf.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zok.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://boe.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nlv.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yrk.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbi.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rck.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://obb.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://adk.fktsv.cn

[N10] 链表节点定义
来源：http://vpl.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jzr.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://lpi.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mfr.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gjn.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://dba.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xve.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nwt.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://esl.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://wdj.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oua.hcnkem.com

PHP:  // 手写递归函数
来源：http://vbe.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xen.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmp.shanyushiyangkeji.top

Java: // 手写递归
来源：http://etz.bjfxy.top

Go:   // 手写递归
来源：http://txv.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ftc.redwolf501.top

C#:   // 手写递归
来源：http://blc.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fie.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sky.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cfj.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rfg.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://msq.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wzi.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uow.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mfv.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pdc.haohaochexian.top

================================================================================
来源：http://qpa.fehbvm.com

O. 并发与异步
来源：http://myp.zhoulong.xyz

================================================================================
来源：http://yrr.aizwys.cn

[O01] 启动一个线程
来源：http://xkj.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ngm.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ldo.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ucu.zhongyouzk.top

TS:   // 同 JS
来源：http://hfk.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://amz.xuanzx.com

Go:   go f()
来源：http://ujz.iojbl.cn

Ruby: Thread.new { f }
来源：http://xcw.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://fyw.ydzc1.top

[O02] 使用线程池
来源：http://vjv.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://olb.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nsf.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://wob.yj202588.top

TS:   // worker_threads 线程池
来源：http://njc.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lqz.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jvd.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nwk.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zfq.daxiang520.top

[O03] 加锁保护共享数据
来源：http://xmw.jiagoushi.top

Py:   with lock: shared += 1
来源：http://omp.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://chk.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kby.hnxiangtu.top

TS:   // 同 JS
来源：http://iyv.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://aui.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jzc.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://haq.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://udc.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://khq.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://bdg.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slg.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://xyy.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://liv.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://awq.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dzg.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ywc.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://vtr.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://gfp.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://bss.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ufh.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://rsu.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://xny.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uhr.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://isx.cucudq.cn

Ruby: threads.map(&:join)
来源：http://ark.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hai.gaohongyu789.top

[O06] 使用进程池
来源：http://zan.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hpq.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oxz.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://hhj.meibo888.top

TS:   // child_process / cluster 模块
来源：http://usn.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jah.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mjg.fanxiaobao.xyz

Ruby: // fork 块
来源：http://dyu.hesvh.cn

C#:   Parallel.For
来源：http://wmg.feifeiyinyue.top

================================================================================
来源：http://ayp.jianghu66.top

P. 常用工具函数
来源：http://mpw.yj20258888.top

================================================================================
来源：http://tbd.zdbjq.cn

[P01] 生成 UUID
来源：http://yod.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://qhg.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iyp.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://uek.iojbl.cn

TS:   crypto.randomUUID()
来源：http://aze.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://dos.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://cby.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://uwv.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://msi.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://zlf.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dzd.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kpf.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bth.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cys.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nnd.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rmk.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cof.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cqa.haohaochexian.top

[P03] 生成短随机字符串
来源：http://vos.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zku.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://smh.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypo.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dwp.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fsn.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dbr.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://idl.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mwd.fanxiaobao.xyz

[P04] 求长度
来源：http://fsu.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zqt.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wly.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bbk.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kwe.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://woy.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://isg.bjfxy.top

Ruby: x.length;  x.size
来源：http://xgo.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vju.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://hra.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nyg.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fdi.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aqi.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dox.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tjm.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hck.shuidangran.top

Ruby: a == b
来源：http://prf.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vsw.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rlx.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gjf.svipenyu.cn

PHP:  if (empty($x)) {}
来源：http://tgw.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qkd.jiagoushi.top

TS:   if (x == null) {}
来源：http://obk.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zpj.hnxiangtu.top

Go:   if x == nil {}
来源：http://bea.zhoulong.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tpj.0kj1m.cn

C#:   if (x is null) {}
来源：http://exx.sufxvd.cn

[P07] 防抖与节流
来源：http://xyi.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hep.sweek.top

PHP:  // 手写时间戳比较
来源：http://gml.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odx.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkb.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wct.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://plb.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://szs.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xwf.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://kfh.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://otf.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tqi.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zof.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rmr.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kig.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nsm.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yrt.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ekv.shzxlz.cn

================================================================================
来源：http://ohn.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rxw.shanyushiyangtech.top

================================================================================
来源：http://eye.sysykeji.top

[Q01] 创建表
来源：http://sfg.hammf.cn

CREATE TABLE users (
来源：http://nmh.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gbe.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://cqo.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://ubf.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jum.yanxiufei.cn

);
来源：http://uty.yangfankeji.com

[Q02] 创建带外键的表
来源：http://gor.bbcook.cn

CREATE TABLE orders (
来源：http://sup.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lkz.dianchejie.cn

user_id INT NOT NULL,
来源：http://dmt.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://dze.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pli.ydjk.org.cn

);
来源：http://cpd.ppjwa.cn

[Q03] 增加列
来源：http://dwq.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eri.yuanzhike.top

[Q04] 修改列类型
来源：http://bup.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://llu.jinghuilouyu.cn

[Q05] 重命名列
来源：http://cvx.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lyu.xuetiantiany.cn

[Q06] 删除列
来源：http://yxx.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://aah.jinqigufen.top

[Q07] 删除表
来源：http://ype.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://srx.tarul.cn

[Q08] 创建普通索引
来源：http://zpu.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://car.tarul.cn

[Q09] 创建唯一索引
来源：http://nou.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nes.yj202588.top

[Q10] 插入单行
来源：http://rrb.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwn.jinqigufen.top

[Q11] 一次插入多行
来源：http://pae.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mgu.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://dgz.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://gig.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zak.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://smz.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cop.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://tdz.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aia.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://snn.ydjk.org.cn

[Q15] 查询全部
来源：http://qev.havefunace.top

SELECT * FROM users;
来源：http://hzw.gotoacloud.top

[Q16] 查询指定列
来源：http://jte.mhx1999.top

SELECT id, name FROM users;
来源：http://upa.iojbl.cn

[Q17] 条件查询
来源：http://gdx.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wux.zhixingplan.top

[Q18] 模糊匹配
来源：http://qga.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zja.zhoulong.xyz

[Q19] 范围查询
来源：http://gtn.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pem.yongpay.top

[Q20] IN 列表
来源：http://zzj.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ioh.jinghuilouyu.cn

[Q21] 空值判断
来源：http://wpw.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jrx.jinqigfzy.top

[Q22] 排序
来源：http://ehi.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ely.fehbvm.com

[Q23] 分页
来源：http://ywi.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bli.yvedp.cn

[Q24] 去重
来源：http://hka.sweek.top

SELECT DISTINCT city FROM users;
来源：http://gmy.hammf.cn

[Q25] 只取前 N 条
来源：http://wym.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oxh.c1oappe.top

[Q26] 计数
来源：http://qjc.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://odg.zhoulong.xyz

[Q27] 条件计数
来源：http://qmf.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yng.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://nwd.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xvw.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://ymm.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://vvq.zhongyouzk.top

[Q30] 分组统计
来源：http://orw.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bkf.yj20258.top

[Q31] 分组后过滤
来源：http://dzl.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wyq.bbcook.cn

[Q32] 分组拼接字符串
来源：http://sjs.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vrm.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jox.hnxiangtu.top

[Q33] 多列分组
来源：http://snv.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iun.haohaochexian.top

[Q34] 每组取第一条
来源：http://ugs.jinqigufen.top

SELECT * FROM (
来源：http://nsz.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ghc.yonumen.top

) t WHERE rn = 1;
来源：http://awm.hfpthk.cn

[Q35] 内连接
来源：http://fha.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zif.fzhhl.top

[Q36] 左连接
来源：http://dwq.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wmf.yvedp.cn

[Q37] 右连接
来源：http://lzi.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hom.52xcode.cn


<!-- 参考信息 -->