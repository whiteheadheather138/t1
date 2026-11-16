代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eew.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ttr.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://zuk.quarkkingdee.top

[N04] 斐波那契数列
来源：http://cny.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tgn.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rjk.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tgr.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnl.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pwe.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qoa.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xcm.hammf.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vrn.cdnleiting.top

[N05] 最大公约数
来源：http://upy.daria6918.cn

Py:   math.gcd(a, b)
来源：http://ejr.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vkx.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jcn.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yql.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hgf.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dcd.ctjpmb.com

Ruby: a.gcd(b)
来源：http://pvr.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iio.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://zac.hammf.cn

Py:   s == s[::-1]
来源：http://jyb.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://gry.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://hzq.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://drb.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vcu.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://yap.yangfankeji.com

Ruby: s == s.reverse
来源：http://teb.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://med.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://nyi.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hqb.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ggk.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://psn.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://wlj.yanxiufei.cn

Java: // 手写 HashMap
来源：http://kbf.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://fzc.yuanzhike.top

Ruby: // 手写 Hash
来源：http://fzn.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zib.zhengqikj.top

[N08] 生成全排列
来源：http://svp.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://wok.bjfxy.top

PHP:  // 手写递归交换
来源：http://dkk.aizwys.cn

JS:   // 手写回溯递归
来源：http://kco.daxiang520.top

TS:   // 手写回溯递归
来源：http://yqh.wangdashe.top

Java: // 手写回溯递归
来源：http://yju.ehwqpu.com

Go:   // 手写回溯递归
来源：http://imh.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://oqp.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://vxf.gaohongyu789.top

[N09] 栈与队列
来源：http://lnb.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ruv.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eau.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lqb.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vxf.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mlw.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gua.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bcy.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cao.0kj1m.cn

[N10] 链表节点定义
来源：http://pbd.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpd.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mzi.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://itr.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qnm.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://kbq.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pjj.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xtp.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bmp.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://tha.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ayo.tanke756.top

PHP:  // 手写递归函数
来源：http://agm.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ozu.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwg.hfpthk.cn

Java: // 手写递归
来源：http://fia.aibaodan.cn

Go:   // 手写递归
来源：http://heu.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://drc.hnxiangtu.top

C#:   // 手写递归
来源：http://dly.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ebs.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pdc.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lrx.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qem.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbb.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mox.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nbv.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://laf.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mrz.xziqi.cn

================================================================================
来源：http://sqy.aibaodan.cn

O. 并发与异步
来源：http://nic.dianchejie.cn

================================================================================
来源：http://zhv.zhoulong.xyz

[O01] 启动一个线程
来源：http://vhp.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ylj.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xah.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wgd.daria6918.cn

TS:   // 同 JS
来源：http://yif.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://swy.bbcook.cn

Go:   go f()
来源：http://vti.uphjek.com

Ruby: Thread.new { f }
来源：http://dlf.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://yuw.zhiwuduotai.top

[O02] 使用线程池
来源：http://plo.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ksc.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qdn.hnqzz.top

JS:   // worker_threads 线程池
来源：http://ucj.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://xlu.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://psa.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ecw.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zwa.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uni.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://pgy.snrcjt.cn

Py:   with lock: shared += 1
来源：http://dqr.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://sxf.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wec.svipenyu.cn

TS:   // 同 JS
来源：http://mjg.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://kiu.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wcb.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bbh.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://lag.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://uzg.pycfn.com

Py:   async def f():⏎    await g()
来源：http://yxp.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zgo.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://xvw.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sow.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wzx.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xwq.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ybt.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://kvn.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://hry.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://fww.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://shp.yj20258.top

JS:   await Promise.all(tasks)
来源：http://rsm.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://ker.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lqj.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eqz.sysykeji.top

Ruby: threads.map(&:join)
来源：http://ecb.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://saf.yongpay.top

[O06] 使用进程池
来源：http://jme.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qar.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gou.316326.xyz

JS:   // child_process / cluster 模块
来源：http://ogf.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://doa.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lht.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ken.hammf.cn

Ruby: // fork 块
来源：http://yaj.yongpay.top

C#:   Parallel.For
来源：http://tcu.zdqjudy.top

================================================================================
来源：http://erp.hongshengwenyu.top

P. 常用工具函数
来源：http://phz.iojbl.cn

================================================================================
来源：http://qbn.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://fsw.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://jcr.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fsi.316326.xyz

JS:   crypto.randomUUID()
来源：http://lbd.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://ola.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://deu.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://ucy.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://ege.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://mer.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://imh.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://byi.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mqf.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dlg.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kuk.uphjek.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zbj.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aep.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ccx.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tnt.hcnkem.com

[P03] 生成短随机字符串
来源：http://fji.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bvh.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vrr.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwn.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bio.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gli.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zgc.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ceh.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jvs.shzxlz.cn

[P04] 求长度
来源：http://yfe.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://chy.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://spy.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pre.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jaa.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://oob.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://bib.yfazqb.com

Ruby: x.length;  x.size
来源：http://oil.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oqm.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://nbq.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://kup.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gco.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://udt.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://glc.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aos.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wtg.mhx1999.top

Ruby: a == b
来源：http://zwp.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mdr.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ilq.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mjw.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://ikk.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iup.vehdjk.com

TS:   if (x == null) {}
来源：http://lbn.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://saj.daxiang520.top

Go:   if x == nil {}
来源：http://sht.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://urx.yangfankeji.com

C#:   if (x is null) {}
来源：http://olw.iojbl.cn

[P07] 防抖与节流
来源：http://twd.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dmd.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://ezc.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://poc.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyz.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://smd.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://huw.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://clh.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hjk.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://ape.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yyu.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gba.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gug.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xxr.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rdk.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwc.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yen.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xdo.9152youxi.cn

================================================================================
来源：http://dfq.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zvw.zhixingplan.top

================================================================================
来源：http://kjk.jyoumei.cn

[Q01] 创建表
来源：http://jdf.ppjwa.cn

CREATE TABLE users (
来源：http://bkx.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvn.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://koy.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://wkp.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ylx.sufxvd.cn

);
来源：http://dxj.fehbvm.com

[Q02] 创建带外键的表
来源：http://iep.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://dqq.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://veb.haohaochexian.top

user_id INT NOT NULL,
来源：http://hwc.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://pys.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bud.mhx1999.top

);
来源：http://tdf.cashguo.top

[Q03] 增加列
来源：http://bkn.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zwh.cqqwz.cn

[Q04] 修改列类型
来源：http://neq.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wcf.smart0.xyz

[Q05] 重命名列
来源：http://azd.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qqi.svipenyu.cn

[Q06] 删除列
来源：http://qlm.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://rsq.aibaodan.cn

[Q07] 删除表
来源：http://bic.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://fcn.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://nxy.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://vmy.tarul.cn

[Q09] 创建唯一索引
来源：http://bqf.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sfl.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://ihh.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hij.tian-w.cn

[Q11] 一次插入多行
来源：http://dpo.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vao.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://mlf.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://tgl.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqm.vehdjk.com

[Q13] 忽略重复插入
来源：http://dvy.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xwv.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://jzw.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nkf.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jsm.yj202588.top

[Q15] 查询全部
来源：http://cgo.yueranfly.top

SELECT * FROM users;
来源：http://nee.dashuyun.cn

[Q16] 查询指定列
来源：http://utq.gotoacloud.top

SELECT id, name FROM users;
来源：http://ged.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://mwb.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xfz.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://dkd.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sfn.fehbvm.com

[Q19] 范围查询
来源：http://jjw.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ibz.yuanzhike.top

[Q20] IN 列表
来源：http://bax.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tzc.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://qtx.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rns.ywan-chungtsiang.top

[Q22] 排序
来源：http://xum.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xed.birdmap.top

[Q23] 分页
来源：http://rgs.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://svl.dianchejie.cn

[Q24] 去重
来源：http://shb.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://nbv.316326.xyz

[Q25] 只取前 N 条
来源：http://dli.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yyb.zdbjq.cn

[Q26] 计数
来源：http://yle.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://cjj.zhixingplan.top

[Q27] 条件计数
来源：http://oat.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bdg.ybcxt.top

[Q28] 求和与平均
来源：http://zyq.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fgh.hywenlv.cn

[Q29] 最大最小值
来源：http://kgb.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ctn.chenzaomai.com

[Q30] 分组统计
来源：http://apa.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ibm.havefunace.top

[Q31] 分组后过滤
来源：http://rqt.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lwb.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://qzw.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sty.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ezv.dashuyun.cn

[Q33] 多列分组
来源：http://luw.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pzq.yuxming.cn

[Q34] 每组取第一条
来源：http://jyz.yuanzhike.top

SELECT * FROM (
来源：http://qfv.hcnkem.com


<!-- 参考信息 -->