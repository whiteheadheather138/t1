代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lbr.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wvm.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://nhi.iojbl.cn

[N04] 斐波那契数列
来源：http://esf.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qpl.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bif.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxm.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://irr.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sjq.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pkl.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://asa.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qlv.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://kcd.cheryme.top

Py:   math.gcd(a, b)
来源：http://byg.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jhs.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcw.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqw.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ysx.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dkp.hfpthk.cn

Ruby: a.gcd(b)
来源：http://ooo.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://int.nanxinkj.top

[N06] 判断回文字符串
来源：http://qed.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://ghz.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://pik.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://mwt.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://kkx.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://skt.yfazqb.com

Go:   // 双指针从两端比较
来源：http://rdo.bbcook.cn

Ruby: s == s.reverse
来源：http://vmy.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpc.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://rwl.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zix.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gqo.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qcu.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://jmw.zycfv.cn

Java: // 手写 HashMap
来源：http://jjt.pycfn.com

Go:   // 手写 map[int]int
来源：http://wii.daria6918.cn

Ruby: // 手写 Hash
来源：http://fzy.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://nvd.sysykeji.top

[N08] 生成全排列
来源：http://kab.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://ypv.jyoumei.cn

PHP:  // 手写递归交换
来源：http://ept.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://vjt.zdbjq.cn

TS:   // 手写回溯递归
来源：http://qwa.tarul.cn

Java: // 手写回溯递归
来源：http://vcl.redwolf501.top

Go:   // 手写回溯递归
来源：http://gcy.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://oug.yonumen.top

C#:   // 手写回溯递归
来源：http://dot.jianghu66.top

[N09] 栈与队列
来源：http://oga.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lrj.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mti.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eyc.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hyx.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://umf.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qmw.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dpe.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bdt.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://cah.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fld.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ssw.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iyr.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lvb.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://zpf.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://xfx.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://llg.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://sia.bbcook.cn

[N11] 二叉树中序遍历
来源：http://ptg.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://teu.dashuyun.cn

PHP:  // 手写递归函数
来源：http://ufg.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vrw.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://neu.ydjk.org.cn

Java: // 手写递归
来源：http://wql.wangdashe.top

Go:   // 手写递归
来源：http://jes.sxryk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://thm.daxiang520.top

C#:   // 手写递归
来源：http://cfy.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cws.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://guz.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgc.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sxg.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jkf.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ehx.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://smo.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qun.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://evj.bbcook.cn

================================================================================
来源：http://ryf.tanke756.top

O. 并发与异步
来源：http://mak.tian-w.cn

================================================================================
来源：http://sda.chenlongwang.top

[O01] 启动一个线程
来源：http://diy.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cwj.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vgp.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wkg.shanyushiyangtech.top

TS:   // 同 JS
来源：http://ijr.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://xjs.aibaodan.cn

Go:   go f()
来源：http://hwg.iojbl.cn

Ruby: Thread.new { f }
来源：http://iqt.cashguo.top

C#:   Task.Run(() => F());
来源：http://xvy.fktsv.cn

[O02] 使用线程池
来源：http://mzf.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bni.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uvs.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://cbq.xziqi.cn

TS:   // worker_threads 线程池
来源：http://uhp.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ykq.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://skd.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sys.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uvx.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://nes.shuidangran.top

Py:   with lock: shared += 1
来源：http://ynn.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://imn.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ypa.hammf.cn

TS:   // 同 JS
来源：http://dvx.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://xrg.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://crx.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kfe.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://irn.yj20258888.top

[O04] 定义异步函数并等待
来源：http://rar.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://ans.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://adk.daria6918.cn

JS:   async function f() { await g(); }
来源：http://wcv.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wrz.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sjl.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jjo.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ijz.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://xkh.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://adm.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://omf.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kca.pycfn.com

JS:   await Promise.all(tasks)
来源：http://wfd.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://wob.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tkk.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zei.xuanzx.com

Ruby: threads.map(&:join)
来源：http://jit.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sum.shzxlz.cn

[O06] 使用进程池
来源：http://crp.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jkr.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://szf.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://zla.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://muu.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gjk.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wkn.aizwys.cn

Ruby: // fork 块
来源：http://set.nwbrower.top

C#:   Parallel.For
来源：http://iwk.zdbjq.cn

================================================================================
来源：http://zpq.zhiwuduotai.top

P. 常用工具函数
来源：http://ntr.iojbl.cn

================================================================================
来源：http://uci.hfpthk.cn

[P01] 生成 UUID
来源：http://yts.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://ipp.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lle.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://tuq.daxiang520.top

TS:   crypto.randomUUID()
来源：http://kod.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://uyi.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://dad.ivvv.top

Ruby: SecureRandom.uuid
来源：http://xie.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://lhr.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://wkn.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ayl.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tom.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://few.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lkr.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cbm.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zbx.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://juh.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bvc.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://dew.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cyy.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yhd.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://byg.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obw.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gpz.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hrm.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://fbz.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tmh.gaohongyu789.top

[P04] 求长度
来源：http://syf.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tol.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dxm.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kqn.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rgt.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://aea.iojbl.cn

Go:   len(arr);  len(m)
来源：http://kzw.wangdashe.top

Ruby: x.length;  x.size
来源：http://xoj.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ldh.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://lvq.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://izh.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sip.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cnt.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yhk.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdk.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://icg.jianghu66.top

Ruby: a == b
来源：http://gnj.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nng.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dqs.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kin.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://flg.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uwg.316326.xyz

TS:   if (x == null) {}
来源：http://eer.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dag.cucudq.cn

Go:   if x == nil {}
来源：http://thh.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zfo.yanxiufei.cn

C#:   if (x is null) {}
来源：http://kla.aibaodan.cn

[P07] 防抖与节流
来源：http://avf.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mbl.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://ufo.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://spv.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rzv.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wmt.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hgl.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tln.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://trb.daria6918.cn

[P08] 处理浮点精度问题
来源：http://omy.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vyn.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://isj.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ike.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eiw.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://brm.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eee.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xdm.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hmp.hfpthk.cn

================================================================================
来源：http://mri.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nwd.gaohongyu789.top

================================================================================
来源：http://nwr.zhixingplan.top

[Q01] 创建表
来源：http://sas.dashuyun.cn

CREATE TABLE users (
来源：http://ztv.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mpt.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://lqd.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://ono.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vvp.yongpay.top

);
来源：http://zck.sysykeji.top

[Q02] 创建带外键的表
来源：http://nff.yfazqb.com

CREATE TABLE orders (
来源：http://zaj.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nya.jinqigfzy.top

user_id INT NOT NULL,
来源：http://pvr.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://chh.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://epd.andypj.xyz

);
来源：http://mgj.mhx1999.top

[Q03] 增加列
来源：http://fgx.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dpz.fktsv.cn

[Q04] 修改列类型
来源：http://qws.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ouo.fzhhl.top

[Q05] 重命名列
来源：http://smx.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://els.andypj.xyz

[Q06] 删除列
来源：http://xyv.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://czo.yangfankeji.com

[Q07] 删除表
来源：http://nrj.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://xth.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://ros.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xjj.smart0.xyz

[Q09] 创建唯一索引
来源：http://mkd.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xkn.shzxlz.cn

[Q10] 插入单行
来源：http://siw.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://epf.aibaodan.cn

[Q11] 一次插入多行
来源：http://yal.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wui.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://ljs.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://efs.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eim.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://wpp.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mkq.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://cuy.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bqw.shangyingyoupin.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sas.pengpengdd.cyou

[Q15] 查询全部
来源：http://qlo.dashuyun.cn

SELECT * FROM users;
来源：http://ppn.jqgufenzy.top

[Q16] 查询指定列
来源：http://scz.epnwcf.com

SELECT id, name FROM users;
来源：http://prv.guowangkeji.top

[Q17] 条件查询
来源：http://feh.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gdn.guowangkeji.top

[Q18] 模糊匹配
来源：http://ufn.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fbu.jlsjyb.cn

[Q19] 范围查询
来源：http://nsm.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://udc.jinghuilouyu.cn

[Q20] IN 列表
来源：http://bwl.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fxt.snrcjt.cn

[Q21] 空值判断
来源：http://rop.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yvt.ivvv.top

[Q22] 排序
来源：http://rus.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wzw.jqgfzy.top

[Q23] 分页
来源：http://atb.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sso.hfpthk.cn

[Q24] 去重
来源：http://atd.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://wbw.dianchejie.cn

[Q25] 只取前 N 条
来源：http://gpn.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bir.jinqigfzy.top

[Q26] 计数
来源：http://nsa.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://suw.epnwcf.com

[Q27] 条件计数
来源：http://aqm.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oqx.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://epd.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tmd.snrcjt.cn

[Q29] 最大最小值
来源：http://iso.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xum.chenjidiqi.icu

[Q30] 分组统计
来源：http://vfe.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kzb.yanxiufei.cn

[Q31] 分组后过滤
来源：http://div.daxiang520.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yis.shuidangran.top

[Q32] 分组拼接字符串
来源：http://ucb.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ksd.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://miz.52xcode.cn

[Q33] 多列分组
来源：http://aph.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cju.havefunace.top

[Q34] 每组取第一条
来源：http://nrk.bbcook.cn

SELECT * FROM (
来源：http://cla.shangyingyoupin.top


<!-- 参考信息 -->