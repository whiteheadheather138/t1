代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xbz.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://szj.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://wja.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://aco.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rma.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uhe.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vac.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vzu.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ehw.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pej.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bma.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mym.svipenyu.cn

[N05] 最大公约数
来源：http://zpc.tian-w.cn

Py:   math.gcd(a, b)
来源：http://sib.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://igq.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pfg.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pps.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://grk.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fmw.aibaodan.cn

Ruby: a.gcd(b)
来源：http://cfi.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zxj.zhijiandao.cn

[N06] 判断回文字符串
来源：http://fgr.hesvh.cn

Py:   s == s[::-1]
来源：http://hvx.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://scd.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://yau.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://zyz.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ihu.pycfn.com

Go:   // 双指针从两端比较
来源：http://baf.yj202588.top

Ruby: s == s.reverse
来源：http://ffc.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://cnp.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://ita.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gma.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yqc.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cqd.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://lqp.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://wxn.meibo888.top

Go:   // 手写 map[int]int
来源：http://bry.zdqjudy.top

Ruby: // 手写 Hash
来源：http://rws.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://dcm.zhoulong.xyz

[N08] 生成全排列
来源：http://hsv.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://vef.bbcook.cn

PHP:  // 手写递归交换
来源：http://iml.fzhhl.top

JS:   // 手写回溯递归
来源：http://uyf.yj20258888.top

TS:   // 手写回溯递归
来源：http://tll.cqqwz.cn

Java: // 手写回溯递归
来源：http://nfu.tian-w.cn

Go:   // 手写回溯递归
来源：http://ijd.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://kbx.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://czv.xinyue.icu

[N09] 栈与队列
来源：http://dzf.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://shp.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://afp.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uqk.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://inm.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ysp.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://izi.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lnk.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tle.c1oappe.top

[N10] 链表节点定义
来源：http://iwz.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://frs.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kzr.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blf.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ufb.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://wue.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tez.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gyr.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uxl.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://zbl.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mgf.gzhubu.top

PHP:  // 手写递归函数
来源：http://dbg.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oyf.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://egs.hammf.cn

Java: // 手写递归
来源：http://ggf.hywenlv.cn

Go:   // 手写递归
来源：http://vno.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oon.yuanzhike.top

C#:   // 手写递归
来源：http://vfy.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dzf.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rzf.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://duj.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmz.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjr.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ytk.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fpx.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://laz.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://spj.wangshuangyany.cn

================================================================================
来源：http://vwu.jianghu66.top

O. 并发与异步
来源：http://krz.iojbl.cn

================================================================================
来源：http://ozj.gzhubu.top

[O01] 启动一个线程
来源：http://uke.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://azh.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mqv.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tot.zhixingplan.top

TS:   // 同 JS
来源：http://kdv.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://cwd.dianchejie.cn

Go:   go f()
来源：http://ful.ydzc1.top

Ruby: Thread.new { f }
来源：http://iwg.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://tnh.daxiang520.top

[O02] 使用线程池
来源：http://jim.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vph.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bqf.zycfv.cn

JS:   // worker_threads 线程池
来源：http://ccd.yongpay.top

TS:   // worker_threads 线程池
来源：http://zgu.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://axm.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sfy.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lue.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zgu.andypj.xyz

[O03] 加锁保护共享数据
来源：http://umw.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://hsu.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://kxz.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdq.bjfxy.top

TS:   // 同 JS
来源：http://rwr.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://fsa.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ihc.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ffk.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://uhs.zhengqikj.top

[O04] 定义异步函数并等待
来源：http://uof.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://ksq.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vkn.hcnkem.com

JS:   async function f() { await g(); }
来源：http://ppj.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://nbd.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cbg.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lbr.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://fst.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://srm.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://kmq.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://kal.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iyn.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://nqv.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://gfl.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wos.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ypu.xinyue.icu

Ruby: threads.map(&:join)
来源：http://izn.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qjp.yj20258888.top

[O06] 使用进程池
来源：http://bnj.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cnu.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://wez.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://dyh.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://vax.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yqn.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kyc.smart0.xyz

Ruby: // fork 块
来源：http://nxc.mhx1999.top

C#:   Parallel.For
来源：http://pno.fktsv.cn

================================================================================
来源：http://iex.epnwcf.com

P. 常用工具函数
来源：http://pnq.yanxiufei.cn

================================================================================
来源：http://hyv.xuanzx.com

[P01] 生成 UUID
来源：http://svl.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://ctm.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hnr.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://dmk.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://skt.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://rib.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://tfu.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://hpk.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://lrj.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://rmo.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bwn.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmb.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uvn.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yxm.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iqy.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jps.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jkd.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hps.hfpthk.cn

[P03] 生成短随机字符串
来源：http://ekp.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cjt.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mwd.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hoy.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xss.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mhy.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xow.jqgfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qet.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qzm.ywan-chungtsiang.top

[P04] 求长度
来源：http://zmw.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uas.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://enb.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hba.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vup.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://ztk.cashguo.top

Go:   len(arr);  len(m)
来源：http://xbw.aibaodan.cn

Ruby: x.length;  x.size
来源：http://hkm.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cld.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://prf.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dpr.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://evm.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://svu.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xdk.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lzm.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jmx.hywenlv.cn

Ruby: a == b
来源：http://ljb.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rbr.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jqj.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qin.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://boy.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bnb.guowangkeji.top

TS:   if (x == null) {}
来源：http://fgd.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bgm.zhixingplan.top

Go:   if x == nil {}
来源：http://kyn.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ymw.havefunace.top

C#:   if (x is null) {}
来源：http://gbx.svipenyu.cn

[P07] 防抖与节流
来源：http://ytn.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dbz.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://nuo.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://igj.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsp.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://akz.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zau.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://uyu.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fbw.smart0.xyz

[P08] 处理浮点精度问题
来源：http://hhs.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://waq.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rtl.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://anm.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pba.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oeg.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iry.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kuc.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://soz.dashuyun.cn

================================================================================
来源：http://urb.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xeb.fanxiaobao.xyz

================================================================================
来源：http://wnl.jinyuanbaomall.cn

[Q01] 创建表
来源：http://mip.pycfn.com

CREATE TABLE users (
来源：http://iph.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iei.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://cbn.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://oxr.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gus.fengsongda.top

);
来源：http://gah.svipenyu.cn

[Q02] 创建带外键的表
来源：http://ruc.pengpengdd.cyou

CREATE TABLE orders (
来源：http://jgy.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qqe.jyoumei.cn

user_id INT NOT NULL,
来源：http://lfk.daria6918.cn

amount DECIMAL(10, 2),
来源：http://lrr.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://teh.dashuyun.cn

);
来源：http://htx.jianghu66.top

[Q03] 增加列
来源：http://muv.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ctg.zdqjudy.top

[Q04] 修改列类型
来源：http://qhe.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ugi.jyoumei.cn

[Q05] 重命名列
来源：http://wfz.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gux.aizwys.cn

[Q06] 删除列
来源：http://jug.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://tdo.hesvh.cn

[Q07] 删除表
来源：http://vlj.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://loa.cashguo.top

[Q08] 创建普通索引
来源：http://ooe.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qrz.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://vhd.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fzm.chenlongwang.top

[Q10] 插入单行
来源：http://tlc.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xas.ivvv.top

[Q11] 一次插入多行
来源：http://fea.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pog.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://hbj.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://tju.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vxr.316326.xyz

[Q13] 忽略重复插入
来源：http://dxu.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nfl.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://fov.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fmr.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yus.hongshengwenyu.top

[Q15] 查询全部
来源：http://oco.yuxming.cn

SELECT * FROM users;
来源：http://uxl.xuanzx.com

[Q16] 查询指定列
来源：http://alz.zhongyouzk.top

SELECT id, name FROM users;
来源：http://qha.wangshuangyany.cn

[Q17] 条件查询
来源：http://lep.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://izf.yongpay.top

[Q18] 模糊匹配
来源：http://shz.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qik.zhengqikj.top

[Q19] 范围查询
来源：http://noe.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xqe.uphjek.com

[Q20] IN 列表
来源：http://vlf.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xal.cheryme.top

[Q21] 空值判断
来源：http://smu.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://usf.0kj1m.cn

[Q22] 排序
来源：http://rpr.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://brb.ybcxt.top

[Q23] 分页
来源：http://syp.hywenlv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jmt.fktsv.cn

[Q24] 去重
来源：http://fpu.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://szt.bbcook.cn

[Q25] 只取前 N 条
来源：http://mmx.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdy.haohaochexian.top

[Q26] 计数
来源：http://cll.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://wkk.fanxiaobao.xyz

[Q27] 条件计数
来源：http://had.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://glm.9152youxi.cn

[Q28] 求和与平均
来源：http://rio.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jgt.yuxming.cn

[Q29] 最大最小值
来源：http://dzu.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dou.yangfankeji.com

[Q30] 分组统计
来源：http://hjp.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dtv.yangfankeji.com

[Q31] 分组后过滤
来源：http://ubq.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pev.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://phf.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pgn.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vga.hysaishi.cn

[Q33] 多列分组
来源：http://ubt.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spw.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://umg.tanke756.top

SELECT * FROM (
来源：http://fdh.zhiwuduotai.top


<!-- 参考信息 -->