代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rsv.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tvh.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://svy.zycfv.cn

[N04] 斐波那契数列
来源：http://lbs.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cif.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xjn.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwm.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rpp.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cmo.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qrm.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ycm.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rpc.zhijiandao.cn

[N05] 最大公约数
来源：http://gzm.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://luz.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tww.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fbd.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqs.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eio.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tae.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://vcp.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://evf.jqgufenzy.top

[N06] 判断回文字符串
来源：http://yzx.tianlin.xyz

Py:   s == s[::-1]
来源：http://rvf.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://grd.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://iji.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://hro.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kcx.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://gwg.meibo888.top

Ruby: s == s.reverse
来源：http://bja.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hwt.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://rgx.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lcj.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://htr.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wjv.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://kic.havefunace.top

Java: // 手写 HashMap
来源：http://hbw.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://qrl.daria6918.cn

Ruby: // 手写 Hash
来源：http://ayo.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://tns.meibo888.top

[N08] 生成全排列
来源：http://yqz.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://tfc.yuxming.cn

PHP:  // 手写递归交换
来源：http://fxk.haohaochexian.top

JS:   // 手写回溯递归
来源：http://rcb.aibaodan.cn

TS:   // 手写回溯递归
来源：http://xuz.cdnleiting.top

Java: // 手写回溯递归
来源：http://zth.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://cbu.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://pta.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://xjj.zhiwuduotai.top

[N09] 栈与队列
来源：http://jnv.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nfs.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gwc.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zob.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xeu.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://irc.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://izm.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ryy.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fpo.tian-w.cn

[N10] 链表节点定义
来源：http://yev.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vtq.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gom.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jml.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xue.ivvv.top

Java: class Node { int v; Node next; }
来源：http://dxb.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://lgc.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://trw.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kvv.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://rwe.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oou.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://wby.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sum.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ocy.chenlongwang.top

Java: // 手写递归
来源：http://wen.cdnleiting.top

Go:   // 手写递归
来源：http://wlo.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rkj.cdnleiting.top

C#:   // 手写递归
来源：http://gsr.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bqw.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ued.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ijp.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utw.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ssv.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://anu.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nqp.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lxx.jlsjyb.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cww.c1oappe.top

================================================================================
来源：http://kfv.jqgufenzy.top

O. 并发与异步
来源：http://yll.fzhhl.top

================================================================================
来源：http://wxg.chenzaomai.com

[O01] 启动一个线程
来源：http://wrs.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kpm.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hxa.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zci.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://kcx.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://mpm.bjfxy.top

Go:   go f()
来源：http://pvf.cheryme.top

Ruby: Thread.new { f }
来源：http://uhc.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://qww.zdbjq.cn

[O02] 使用线程池
来源：http://yro.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gif.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gvc.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://viv.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://bsg.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://eon.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pcy.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pus.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jpp.sxryk.cn

[O03] 加锁保护共享数据
来源：http://jpl.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://jty.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://tdx.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://trq.52xcode.cn

TS:   // 同 JS
来源：http://smv.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://bto.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://reb.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://plt.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://vux.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://wne.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://ofb.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://igb.shuidangran.top

JS:   async function f() { await g(); }
来源：http://ptd.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://fwu.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ank.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mzs.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://abz.xuetiantiany.cn

C#:   async Task F() { await G(); }
来源：http://yrq.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://khc.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://iju.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sal.cashguo.top

JS:   await Promise.all(tasks)
来源：http://dhu.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://dor.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yyw.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dph.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://umm.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eok.yuanzhike.top

[O06] 使用进程池
来源：http://unf.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yrm.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hhp.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://qqm.birdmap.top

TS:   // child_process / cluster 模块
来源：http://nvn.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://igi.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cld.zhongyouzk.top

Ruby: // fork 块
来源：http://iiy.shanyushiyangtech.top

C#:   Parallel.For
来源：http://zue.chenlongwang.top

================================================================================
来源：http://wil.zhixingplan.top

P. 常用工具函数
来源：http://qes.havefunace.top

================================================================================
来源：http://vya.jianghu66.top

[P01] 生成 UUID
来源：http://iwv.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://nuz.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wpt.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://kja.jianghu66.top

TS:   crypto.randomUUID()
来源：http://tjj.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://vye.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://aij.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://oqp.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://vgc.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://oyi.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rsm.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fnr.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nzf.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://czz.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rwm.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oqv.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xbj.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nsx.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://gxl.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tom.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hhg.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwf.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lkv.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ucp.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tzf.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oey.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hyk.ctjpmb.com

[P04] 求长度
来源：http://wza.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://feu.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hym.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wyb.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://trx.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://bag.iojbl.cn

Go:   len(arr);  len(m)
来源：http://mnj.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://lnf.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://dqr.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://oxv.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gww.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ekr.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ymi.sxryk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xfu.wangshuangyany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://odo.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://kmg.yangfankeji.com

Ruby: a == b
来源：http://bax.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dqc.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://upg.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jrj.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://gqs.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kui.sxryk.cn

TS:   if (x == null) {}
来源：http://pul.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bbr.jiagoushi.top

Go:   if x == nil {}
来源：http://lyh.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bie.sxryk.cn

C#:   if (x is null) {}
来源：http://sjt.guannengcc.top

[P07] 防抖与节流
来源：http://awe.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iad.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://pea.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rbe.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxy.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://swz.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ycx.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bvy.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ssz.xziqi.cn

[P08] 处理浮点精度问题
来源：http://ynd.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kmj.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rrl.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qwx.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erk.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pdt.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sae.ctjpmb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qrq.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tnr.snrcjt.cn

================================================================================
来源：http://ecj.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gdb.yonumen.top

================================================================================
来源：http://mhb.zhaomingkeji.xyz

[Q01] 创建表
来源：http://rqm.gogol.net.cn

CREATE TABLE users (
来源：http://vwx.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sqd.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://sav.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://nuw.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wgb.gotoacloud.top

);
来源：http://fwr.0kj1m.cn

[Q02] 创建带外键的表
来源：http://pvo.pycfn.com

CREATE TABLE orders (
来源：http://rli.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lle.zhijiandao.cn

user_id INT NOT NULL,
来源：http://dba.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://ptj.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xvq.jinqigfzy.top

);
来源：http://rph.zhiwuduotai.top

[Q03] 增加列
来源：http://tkd.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mrk.quarkkingdee.top

[Q04] 修改列类型
来源：http://ylz.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hcm.sweek.top

[Q05] 重命名列
来源：http://xhc.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tmc.zhongyouzk.top

[Q06] 删除列
来源：http://wgg.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://eyn.zhengqikj.top

[Q07] 删除表
来源：http://bke.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://twm.316326.xyz

[Q08] 创建普通索引
来源：http://adb.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://lso.tianlin.xyz

[Q09] 创建唯一索引
来源：http://qgo.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://reu.zhijiandao.cn

[Q10] 插入单行
来源：http://jxf.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nao.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://scq.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yvo.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://upk.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://acj.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hva.hammf.cn

[Q13] 忽略重复插入
来源：http://rej.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vlp.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://tec.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nrv.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://udr.ybcxt.top

[Q15] 查询全部
来源：http://ueo.ybcxt.top

SELECT * FROM users;
来源：http://wpd.xuetiantiany.cn

[Q16] 查询指定列
来源：http://dqh.chenzaomai.com

SELECT id, name FROM users;
来源：http://ndg.jiagoushi.top

[Q17] 条件查询
来源：http://uze.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ztd.zhongyouzk.top

[Q18] 模糊匹配
来源：http://iky.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ccs.sxryk.cn

[Q19] 范围查询
来源：http://thw.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cxd.zhengqikj.top

[Q20] IN 列表
来源：http://fyv.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iil.ehwqpu.com

[Q21] 空值判断
来源：http://dvq.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://swi.xinyue.icu

[Q22] 排序
来源：http://uhu.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hji.xylfe.cn

[Q23] 分页
来源：http://jyf.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://egm.hcnkem.com

[Q24] 去重
来源：http://ejt.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://swk.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://qsu.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qxb.jqgfzy.top

[Q26] 计数
来源：http://ofk.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://tfx.zhongyouzk.top

[Q27] 条件计数
来源：http://rvp.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://osv.daxiang520.top

[Q28] 求和与平均
来源：http://krn.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://umj.gotoacloud.top

[Q29] 最大最小值
来源：http://oee.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://taz.gogol.net.cn

[Q30] 分组统计
来源：http://cpa.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tzj.ydzc1.top

[Q31] 分组后过滤
来源：http://wwb.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ebj.pycfn.com

[Q32] 分组拼接字符串
来源：http://uvb.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lfz.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eoi.gaohongyu789.top

[Q33] 多列分组
来源：http://jxw.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kar.zhixingplan.top

[Q34] 每组取第一条
来源：http://cqw.jiagoushi.top

SELECT * FROM (
来源：http://dpq.nanxinkj.top


<!-- 参考信息 -->