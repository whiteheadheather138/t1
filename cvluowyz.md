代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://txf.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mnp.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ibt.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kes.jinghuilouyu.cn

[N05] 最大公约数
来源：http://zbe.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://ucx.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gkv.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvf.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qwl.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fqv.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xfx.hnqzz.top

Ruby: a.gcd(b)
来源：http://pgb.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hnj.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://lnn.yj202588.top

Py:   s == s[::-1]
来源：http://xou.hcnkem.com

PHP:  $s === strrev($s);
来源：http://vkx.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://lbl.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://hfs.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pyw.fengsongda.top

Go:   // 双指针从两端比较
来源：http://fuw.haohaochexian.top

Ruby: s == s.reverse
来源：http://itt.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zoa.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://qwd.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://exu.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iqc.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://mpe.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://byz.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://dpc.xylfe.cn

Go:   // 手写 map[int]int
来源：http://odz.yueranfly.top

Ruby: // 手写 Hash
来源：http://adc.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://nry.epnwcf.com

[N08] 生成全排列
来源：http://jfz.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://xua.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://rto.nwbrower.top

JS:   // 手写回溯递归
来源：http://qpn.fzhhl.top

TS:   // 手写回溯递归
来源：http://udr.yuanzhike.top

Java: // 手写回溯递归
来源：http://hbp.mhx1999.top

Go:   // 手写回溯递归
来源：http://ody.havefunace.top

Ruby: arr.permutation.to_a
来源：http://utl.fehbvm.com

C#:   // 手写回溯递归
来源：http://mvl.jqgfzy.top

[N09] 栈与队列
来源：http://rxe.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fvr.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xgd.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jvh.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pjl.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://scf.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bmq.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dqw.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://efx.gogol.net.cn

[N10] 链表节点定义
来源：http://ndp.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zwr.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yxt.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lui.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ooe.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://nsy.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dmd.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xst.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://oxx.pycfn.com

[N11] 二叉树中序遍历
来源：http://zdj.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xek.aibaodan.cn

PHP:  // 手写递归函数
来源：http://dhk.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nmu.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kif.yonumen.top

Java: // 手写递归
来源：http://wmm.uphjek.com

Go:   // 手写递归
来源：http://yvk.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yak.52xcode.cn

C#:   // 手写递归
来源：http://cns.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jrt.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vkr.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lci.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dds.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ygk.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ati.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pum.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dsh.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cmw.ivvv.top

================================================================================
来源：http://ujt.feifeiyinyue.top

O. 并发与异步
来源：http://kgg.uphjek.com

================================================================================
来源：http://lvk.pengpengdd.cyou

[O01] 启动一个线程
来源：http://bel.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://apo.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jlu.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tug.yj202588.top

TS:   // 同 JS
来源：http://fvf.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://cyx.tanke756.top

Go:   go f()
来源：http://pzf.hesvh.cn

Ruby: Thread.new { f }
来源：http://ckw.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://kfh.zhoulong.xyz

[O02] 使用线程池
来源：http://hpy.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lij.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uqd.zycfv.cn

JS:   // worker_threads 线程池
来源：http://osk.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://hnp.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eiq.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vgv.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://awe.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tyq.bbcook.cn

[O03] 加锁保护共享数据
来源：http://zfd.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://fvt.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://svn.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iwh.zdbjq.cn

TS:   // 同 JS
来源：http://dui.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://wkx.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zrk.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sal.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://pfq.yj20258.top

[O04] 定义异步函数并等待
来源：http://uqr.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://ceh.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vhs.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://tna.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qji.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyn.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qho.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ifz.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://wct.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://frz.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://zyl.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://okx.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://bbi.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://gpq.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://scc.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ngf.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://neh.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://fbi.ybcxt.top

[O06] 使用进程池
来源：http://bdv.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lbl.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eam.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://dmd.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://hfr.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://feb.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uxb.wangdashe.top

Ruby: // fork 块
来源：http://efm.gogol.net.cn

C#:   Parallel.For
来源：http://rxh.cheryme.top

================================================================================
来源：http://oif.vehdjk.com

P. 常用工具函数
来源：http://gqb.xylfe.cn

================================================================================
来源：http://tvb.meibo888.top

[P01] 生成 UUID
来源：http://wpi.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://wun.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yes.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://pmq.ybcxt.top

TS:   crypto.randomUUID()
来源：http://hev.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://wcb.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://fbc.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://tdu.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://vsp.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://eht.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sih.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://mhl.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rcd.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rcr.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hmb.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://drh.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xkd.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://att.uphjek.com

[P03] 生成短随机字符串
来源：http://llr.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vcb.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xwt.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yuh.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://soy.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zlm.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wfw.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nyu.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xmh.zhiwuduotai.top

[P04] 求长度
来源：http://xzo.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iwf.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sfk.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jrw.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://okq.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://mqq.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://kyh.zhixingplan.top

Ruby: x.length;  x.size
来源：http://wne.yangfankeji.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mlz.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://tfr.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sir.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rms.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yao.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://soe.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gxu.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://vbw.fzhhl.top

Ruby: a == b
来源：http://gyt.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://stt.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iit.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zgf.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://otf.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rfn.chenlongwang.top

TS:   if (x == null) {}
来源：http://huq.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://osr.9152youxi.cn

Go:   if x == nil {}
来源：http://beu.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jow.smart0.xyz

C#:   if (x is null) {}
来源：http://vll.gotoacloud.top

[P07] 防抖与节流
来源：http://ysv.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lsd.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://evx.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ban.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msq.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dkx.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qjy.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rqr.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kdu.iojbl.cn

[P08] 处理浮点精度问题
来源：http://rko.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jrh.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qqh.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hoq.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hqs.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vtw.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tle.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ccl.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vur.hnxiangtu.top

================================================================================
来源：http://hwp.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hin.nanxuanxn.top

================================================================================
来源：http://kkl.fengsongda.top

[Q01] 创建表
来源：http://lms.zhongyouzk.top

CREATE TABLE users (
来源：http://lyn.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dta.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://pxq.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://mjm.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eci.yongpay.top

);
来源：http://smq.ehwqpu.com

[Q02] 创建带外键的表
来源：http://gwd.cashguo.top

CREATE TABLE orders (
来源：http://azg.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wto.cashguo.top

user_id INT NOT NULL,
来源：http://wfh.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://cbk.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qry.hcnkem.com

);
来源：http://qsp.daria6918.cn

[Q03] 增加列
来源：http://kzj.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zco.nanxuanxn.top

[Q04] 修改列类型
来源：http://zxk.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eyz.dashuyun.cn

[Q05] 重命名列
来源：http://zqe.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mhr.yj20258.top

[Q06] 删除列
来源：http://vyv.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zvq.zycfv.cn

[Q07] 删除表
来源：http://llr.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://rfz.jiagoushi.top

[Q08] 创建普通索引
来源：http://gwq.wangshuangyany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fku.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://kwv.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sdh.daria6918.cn

[Q10] 插入单行
来源：http://hli.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fhb.vehdjk.com

[Q11] 一次插入多行
来源：http://ddn.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://flu.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://gvs.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fgi.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://srv.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://tlk.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zix.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://jwe.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uug.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yvk.jqgfzy.top

[Q15] 查询全部
来源：http://rqc.zhixingplan.top

SELECT * FROM users;
来源：http://mjg.birdmap.top

[Q16] 查询指定列
来源：http://tlv.zhixingplan.top

SELECT id, name FROM users;
来源：http://qfr.yj202588.top

[Q17] 条件查询
来源：http://ido.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qob.9152youxi.cn

[Q18] 模糊匹配
来源：http://cdx.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bhh.hnxiangtu.top

[Q19] 范围查询
来源：http://egb.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tem.jlsjyb.cn

[Q20] IN 列表
来源：http://rnk.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://koy.quarkkingdee.top

[Q21] 空值判断
来源：http://ruu.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iuv.c1oappe.top

[Q22] 排序
来源：http://ecs.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vzk.fzhhl.top

[Q23] 分页
来源：http://jhc.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://moe.xziqi.cn

[Q24] 去重
来源：http://ydz.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://wmx.hysaishi.cn

[Q25] 只取前 N 条
来源：http://rpw.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tcp.chenzaomai.com

[Q26] 计数
来源：http://xil.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://kdh.0kj1m.cn

[Q27] 条件计数
来源：http://qne.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hxe.svipenyu.cn

[Q28] 求和与平均
来源：http://vrj.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jqc.hesvh.cn

[Q29] 最大最小值
来源：http://yyr.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://pny.daria6918.cn

[Q30] 分组统计
来源：http://hke.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://drf.c1oappe.top

[Q31] 分组后过滤
来源：http://djy.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vjl.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://hvy.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oxb.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mnz.cqqwz.cn

[Q33] 多列分组
来源：http://xbc.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kyd.c1oappe.top

[Q34] 每组取第一条
来源：http://klg.bbcook.cn

SELECT * FROM (
来源：http://bij.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sqe.daxiang520.top

) t WHERE rn = 1;
来源：http://job.bjfxy.top

[Q35] 内连接
来源：http://tgi.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://huu.shuidangran.top

[Q36] 左连接
来源：http://rsm.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fpx.tianlin.xyz

[Q37] 右连接
来源：http://lsv.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ryr.birdmap.top


<!-- 参考信息 -->