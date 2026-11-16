代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jwx.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gql.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://pev.ivvv.top

[N04] 斐波那契数列
来源：http://nmu.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ssq.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jjk.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cnw.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ceg.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zvs.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://atq.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dof.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qne.yueranfly.top

[N05] 最大公约数
来源：http://dci.wangdashe.top

Py:   math.gcd(a, b)
来源：http://yys.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nmh.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpa.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lbg.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jvj.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ilu.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://ssq.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ulk.xuanzx.com

[N06] 判断回文字符串
来源：http://pvp.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://ipr.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://tcc.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://wgb.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://dzz.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oti.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://cff.yanxiufei.cn

Ruby: s == s.reverse
来源：http://nin.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uax.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://taf.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jiw.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://erw.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://hzk.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://lac.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://zag.yongpay.top

Go:   // 手写 map[int]int
来源：http://afo.hcnkem.com

Ruby: // 手写 Hash
来源：http://ccp.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ssx.fehbvm.com

[N08] 生成全排列
来源：http://asq.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://gnq.sxryk.cn

PHP:  // 手写递归交换
来源：http://xwk.sxryk.cn

JS:   // 手写回溯递归
来源：http://lle.meibo888.top

TS:   // 手写回溯递归
来源：http://qvt.yuxming.cn

Java: // 手写回溯递归
来源：http://mhw.cucudq.cn

Go:   // 手写回溯递归
来源：http://gpm.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://fie.jiagoushi.top

C#:   // 手写回溯递归
来源：http://oeb.yangfankeji.com

[N09] 栈与队列
来源：http://fib.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zwt.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://msv.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wna.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hsc.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vip.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://shd.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mer.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rby.gzhubu.top

[N10] 链表节点定义
来源：http://hqs.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dpg.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fhu.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vjn.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gox.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://ruw.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://gzy.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zoy.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://wvk.tian-w.cn

[N11] 二叉树中序遍历
来源：http://ixn.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cwj.yongpay.top

PHP:  // 手写递归函数
来源：http://sjw.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bza.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://boz.sufxvd.cn

Java: // 手写递归
来源：http://cby.zycfv.cn

Go:   // 手写递归
来源：http://rqx.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ziv.quarkkingdee.top

C#:   // 手写递归
来源：http://dkz.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xzn.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zmr.pengpengdd.cyou

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wts.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kst.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lzi.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://usz.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sat.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sll.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yvs.dashuyun.cn

================================================================================
来源：http://qdw.ppjwa.cn

O. 并发与异步
来源：http://jeo.cdnleiting.top

================================================================================
来源：http://lnc.aizwys.cn

[O01] 启动一个线程
来源：http://gfx.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://atw.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hig.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rwt.jqgufenzy.top

TS:   // 同 JS
来源：http://ass.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://ptb.gaohongyu789.top

Go:   go f()
来源：http://zqb.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://yec.smart0.xyz

C#:   Task.Run(() => F());
来源：http://kzc.hesvh.cn

[O02] 使用线程池
来源：http://rhx.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fls.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yec.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://ymu.yueranfly.top

TS:   // worker_threads 线程池
来源：http://zid.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://elu.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://faa.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lal.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qmi.daria6918.cn

[O03] 加锁保护共享数据
来源：http://zcw.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://svq.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://uej.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iff.daria6918.cn

TS:   // 同 JS
来源：http://drl.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://fak.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xko.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bgx.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://jbh.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://fel.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://vez.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ztc.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://qim.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wpi.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sih.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://esf.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ivo.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://xxk.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://qgd.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://ity.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ttw.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://tfa.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://cxw.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fuk.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kda.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://wpn.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zym.nanxuanxn.top

[O06] 使用进程池
来源：http://cdj.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dsh.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://amd.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://ykr.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://tyk.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nwk.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tvo.ppjwa.cn

Ruby: // fork 块
来源：http://yhl.tian-w.cn

C#:   Parallel.For
来源：http://xgt.jqgfzy.top

================================================================================
来源：http://sml.nwbrower.top

P. 常用工具函数
来源：http://mjz.fanxiaobao.xyz

================================================================================
来源：http://dho.yj202588.top

[P01] 生成 UUID
来源：http://fvw.hywenlv.cn

Py:   str(uuid.uuid4())
来源：http://zob.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eca.daxiang520.top

JS:   crypto.randomUUID()
来源：http://sbi.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://rwc.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://eco.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://iuo.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://tes.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://zrm.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://ged.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oeg.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nnb.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dmo.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fsx.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://icf.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qut.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://etc.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://slk.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://jeb.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oqp.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zto.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://atz.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://djs.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nnf.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://abd.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://emu.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xrv.epnwcf.com

[P04] 求长度
来源：http://xno.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hrt.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynr.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qwk.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vcg.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://pif.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://ajw.zdbjq.cn

Ruby: x.length;  x.size
来源：http://rqa.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cfu.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://pwc.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dwx.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://trh.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://loc.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qxd.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zdh.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://dge.xuanzx.com

Ruby: a == b
来源：http://fkq.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zbr.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gha.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://twj.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://hmk.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cya.cqqwz.cn

TS:   if (x == null) {}
来源：http://ema.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://wqi.sjlbkw.cn

Go:   if x == nil {}
来源：http://amc.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zeq.dashuyun.cn

C#:   if (x is null) {}
来源：http://vlc.sweek.top

[P07] 防抖与节流
来源：http://eyb.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ajg.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://oxu.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kyo.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwc.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wjw.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gqj.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jfj.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mgf.ivvv.top

[P08] 处理浮点精度问题
来源：http://eff.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blw.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xws.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ogx.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mce.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kgp.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zvn.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cmg.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vnt.nanxinkj.top

================================================================================
来源：http://dyv.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ajw.nanxinkj.top

================================================================================
来源：http://uuk.ydzc1.top

[Q01] 创建表
来源：http://neh.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://yuj.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dob.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://qpo.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://kol.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kgq.iojbl.cn

);
来源：http://nkb.jyoumei.cn

[Q02] 创建带外键的表
来源：http://ich.ydjk.org.cn

CREATE TABLE orders (
来源：http://edr.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eno.ehwqpu.com

user_id INT NOT NULL,
来源：http://god.shuidangran.top

amount DECIMAL(10, 2),
来源：http://mzh.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yru.tarul.cn

);
来源：http://yie.hywenlv.cn

[Q03] 增加列
来源：http://rts.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nqw.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://okg.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hxj.tian-w.cn

[Q05] 重命名列
来源：http://ldv.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldg.yvedp.cn

[Q06] 删除列
来源：http://lya.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://nqz.daria6918.cn

[Q07] 删除表
来源：http://yxj.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://syp.tianlin.xyz

[Q08] 创建普通索引
来源：http://rms.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zcm.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://gmn.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kzn.52xcode.cn

[Q10] 插入单行
来源：http://ltg.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ncv.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://nrw.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://har.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://wvu.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://ira.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eiz.shuidangran.top

[Q13] 忽略重复插入
来源：http://fkg.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vqw.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://fuh.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ewm.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://shw.meibo888.top

[Q15] 查询全部
来源：http://veu.guannengcc.top

SELECT * FROM users;
来源：http://qel.jlsjyb.cn

[Q16] 查询指定列
来源：http://jjl.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://qfm.zhijiandao.cn

[Q17] 条件查询
来源：http://kql.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://omy.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://mgo.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qwg.aizwys.cn

[Q19] 范围查询
来源：http://ury.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jrf.gotoacloud.top

[Q20] IN 列表
来源：http://vtt.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://atj.tarul.cn

[Q21] 空值判断
来源：http://xvp.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://fmv.shanyushiyangtech.top

[Q22] 排序
来源：http://wyc.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://epz.tianlin.xyz

[Q23] 分页
来源：http://muj.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xiw.zhengqikj.top

[Q24] 去重
来源：http://prg.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://ylu.jiagoushi.top

[Q25] 只取前 N 条
来源：http://xhh.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lyp.redwolf501.top

[Q26] 计数
来源：http://ypf.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://pvu.pycfn.com

[Q27] 条件计数
来源：http://zuy.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lhk.zdqjudy.top

[Q28] 求和与平均
来源：http://snp.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cvn.yangfankeji.com

[Q29] 最大最小值
来源：http://nke.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wqh.hnqzz.top

[Q30] 分组统计
来源：http://kze.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ahm.ivvv.top

[Q31] 分组后过滤
来源：http://huo.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yrc.pycfn.com

[Q32] 分组拼接字符串
来源：http://vik.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://psz.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rnz.gogol.net.cn

[Q33] 多列分组
来源：http://fax.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fbj.uphjek.com

[Q34] 每组取第一条
来源：http://lzk.aizwys.cn

SELECT * FROM (
来源：http://luh.sjlbkw.cn


<!-- 参考信息 -->