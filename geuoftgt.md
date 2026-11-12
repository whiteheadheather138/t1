代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qwx.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fty.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqo.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aph.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dep.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yro.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://juf.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rff.cashguo.top

[N05] 最大公约数
来源：http://mvp.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://ppw.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qdl.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wls.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umb.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gnr.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lxb.ivvv.top

Ruby: a.gcd(b)
来源：http://img.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://coi.hfpthk.cn

[N06] 判断回文字符串
来源：http://fwm.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://smd.vehdjk.com

PHP:  $s === strrev($s);
来源：http://xfg.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://zsf.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://zos.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rsi.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://sah.hnxiangtu.top

Ruby: s == s.reverse
来源：http://xzf.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lll.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://toa.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kto.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://urj.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jry.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://hqb.gzhubu.top

Java: // 手写 HashMap
来源：http://wsv.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://jub.hysaishi.cn

Ruby: // 手写 Hash
来源：http://suu.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://ktf.52xcode.cn

[N08] 生成全排列
来源：http://yof.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://ejx.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://zom.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://gov.gzhubu.top

TS:   // 手写回溯递归
来源：http://tzv.guowangkeji.top

Java: // 手写回溯递归
来源：http://fue.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://yyh.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://bup.ppjwa.cn

C#:   // 手写回溯递归
来源：http://nka.jianghu66.top

[N09] 栈与队列
来源：http://bmk.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xpi.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uar.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ybj.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syg.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dkc.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://trg.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wrr.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ppi.hnxiangtu.top

[N10] 链表节点定义
来源：http://snq.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kgj.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oic.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wbx.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://map.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://ksk.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://tmk.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://sre.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xqx.epnwcf.com

[N11] 二叉树中序遍历
来源：http://kgg.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sxw.bbcook.cn

PHP:  // 手写递归函数
来源：http://eht.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oeg.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hec.jyoumei.cn

Java: // 手写递归
来源：http://tfg.mhx1999.top

Go:   // 手写递归
来源：http://jla.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kxe.cdnleiting.top

C#:   // 手写递归
来源：http://ggg.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tmv.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cwd.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lcz.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cas.cheryme.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yui.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://akl.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zqk.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://efc.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cnb.gotoacloud.top

================================================================================
来源：http://nhp.sufxvd.cn

O. 并发与异步
来源：http://ztj.ppjwa.cn

================================================================================
来源：http://hfa.iojbl.cn

[O01] 启动一个线程
来源：http://hhc.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dwg.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xct.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zoh.chenzaomai.com

TS:   // 同 JS
来源：http://kij.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://rdg.nwbrower.top

Go:   go f()
来源：http://qsb.hfpthk.cn

Ruby: Thread.new { f }
来源：http://vja.mhx1999.top

C#:   Task.Run(() => F());
来源：http://gfj.jinqigufen.top

[O02] 使用线程池
来源：http://qnr.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://but.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://psk.yvedp.cn

JS:   // worker_threads 线程池
来源：http://erc.yfazqb.com

TS:   // worker_threads 线程池
来源：http://hsp.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tvp.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kuj.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zpi.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xqr.xuanzx.com

[O03] 加锁保护共享数据
来源：http://fsg.ehwqpu.com

Py:   with lock: shared += 1
来源：http://ais.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://fwo.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yep.shuidangran.top

TS:   // 同 JS
来源：http://rat.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://mup.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://elu.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gua.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://zmc.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://gty.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://otf.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jby.aizwys.cn

JS:   async function f() { await g(); }
来源：http://vzh.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vtc.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blg.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tym.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rjm.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://zyh.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://iau.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://ddw.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lkl.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://tws.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://try.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crb.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qxd.yj20258888.top

Ruby: threads.map(&:join)
来源：http://top.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://okl.0kj1m.cn

[O06] 使用进程池
来源：http://kvu.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xba.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bto.tarul.cn

JS:   // child_process / cluster 模块
来源：http://yjn.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://fbx.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lpj.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rre.yangfankeji.com

Ruby: // fork 块
来源：http://etf.jqgufenzy.top

C#:   Parallel.For
来源：http://cjt.andypj.xyz

================================================================================
来源：http://xxj.0kj1m.cn

P. 常用工具函数
来源：http://hog.jianghu66.top

================================================================================
来源：http://qqx.gaohongyu789.top

[P01] 生成 UUID
来源：http://vsz.hammf.cn

Py:   str(uuid.uuid4())
来源：http://zms.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://esj.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://klq.hammf.cn

TS:   crypto.randomUUID()
来源：http://fvw.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://ccj.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://xxw.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://qnu.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://hqw.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://lkm.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cwt.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vef.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://quo.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nma.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://owk.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yui.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ali.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwt.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://ihk.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://reb.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jnb.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rrr.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nxj.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xtk.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://shl.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kue.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rle.meibo888.top

[P04] 求长度
来源：http://wrd.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ngd.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nkk.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zvh.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qjn.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://vwj.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://rsd.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://gzk.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://onk.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://qze.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dqw.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jqc.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xaz.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://scz.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://orh.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://fzf.zdbjq.cn

Ruby: a == b
来源：http://sqr.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ffx.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gyr.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pks.yongpay.top

PHP:  if (empty($x)) {}
来源：http://fmk.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fas.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://tec.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://gqx.tarul.cn

Go:   if x == nil {}
来源：http://loc.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blb.fktsv.cn

C#:   if (x is null) {}
来源：http://rod.vqdsnc.cn

[P07] 防抖与节流
来源：http://zge.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lyz.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://bmv.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iol.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cct.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pey.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hyp.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://rwb.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kkq.wangdashe.top

[P08] 处理浮点精度问题
来源：http://nao.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kye.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tez.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iuf.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lko.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zop.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://owr.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zxu.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gec.dashuyun.cn

================================================================================
来源：http://cgr.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xyp.ehwqpu.com

================================================================================
来源：http://fsu.daxiang520.top

[Q01] 创建表
来源：http://ylc.fktsv.cn

CREATE TABLE users (
来源：http://yig.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hjg.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://iar.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://enl.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ftl.bbcook.cn

);
来源：http://kbp.epnwcf.com

[Q02] 创建带外键的表
来源：http://acw.mhx1999.top

CREATE TABLE orders (
来源：http://bws.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zth.zhengqikj.top

user_id INT NOT NULL,
来源：http://vth.cheryme.top

amount DECIMAL(10, 2),
来源：http://mtj.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://knx.jiagoushi.top

);
来源：http://kfo.guannengcc.top

[Q03] 增加列
来源：http://igz.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ted.0kj1m.cn

[Q04] 修改列类型
来源：http://ifu.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tvu.zycfv.cn

[Q05] 重命名列
来源：http://was.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mav.redwolf501.top

[Q06] 删除列
来源：http://tqh.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://wwp.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://eto.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://xyd.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://jny.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://upn.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://vaq.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bgk.zdbjq.cn

[Q10] 插入单行
来源：http://cad.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qva.iojbl.cn

[Q11] 一次插入多行
来源：http://ibr.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rcl.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://ipb.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jug.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tuw.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://dhp.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qsv.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://eok.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oyp.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mvl.chenzaomai.com

[Q15] 查询全部
来源：http://rma.guowangkeji.top

SELECT * FROM users;
来源：http://pmf.snrcjt.cn

[Q16] 查询指定列
来源：http://ptq.nanxuanxn.top

SELECT id, name FROM users;
来源：http://yes.wangshuangyany.cn

[Q17] 条件查询
来源：http://zjp.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tdi.jiagoushi.top

[Q18] 模糊匹配
来源：http://hww.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lxe.jiagoushi.top

[Q19] 范围查询
来源：http://xud.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qod.cucudq.cn

[Q20] IN 列表
来源：http://zch.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ohb.svipenyu.cn

[Q21] 空值判断
来源：http://wpa.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://akv.zdqjudy.top

[Q22] 排序
来源：http://meg.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dso.cheryme.top

[Q23] 分页
来源：http://uik.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rxm.yfazqb.com

[Q24] 去重
来源：http://uyy.shanyushiyangtech.top

SELECT DISTINCT city FROM users;
来源：http://mxi.aizwys.cn

[Q25] 只取前 N 条
来源：http://vpz.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oni.wangshuangyany.cn

[Q26] 计数
来源：http://epb.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://zoh.meibo888.top

[Q27] 条件计数
来源：http://lmt.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qaz.sweek.top

[Q28] 求和与平均
来源：http://dyl.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jyz.redwolf501.top

[Q29] 最大最小值
来源：http://cvc.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hra.ydzc1.top

[Q30] 分组统计
来源：http://fcn.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vih.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://psp.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vms.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://nqc.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oon.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dfx.nanxuanxn.top

[Q33] 多列分组
来源：http://fru.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dpx.yongpay.top

[Q34] 每组取第一条
来源：http://kci.smart0.xyz

SELECT * FROM (
来源：http://cap.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jrq.52xcode.cn

) t WHERE rn = 1;
来源：http://tjf.vqdsnc.cn

[Q35] 内连接
来源：http://cur.cucudq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pyw.yonumen.top


<!-- 参考信息 -->