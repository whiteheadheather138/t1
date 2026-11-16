代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zwt.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://imb.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://sqk.svipenyu.cn

[N04] 斐波那契数列
来源：http://tkj.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://swg.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://got.ydzc1.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jlt.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zll.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zsh.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lso.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tol.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yfz.zhoulong.xyz

[N05] 最大公约数
来源：http://agn.fktsv.cn

Py:   math.gcd(a, b)
来源：http://lrn.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://loj.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xez.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://euz.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://urb.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dsi.yongpay.top

Ruby: a.gcd(b)
来源：http://zof.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ndu.ctjpmb.com

[N06] 判断回文字符串
来源：http://eyx.jinqigufen.top

Py:   s == s[::-1]
来源：http://fkx.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://jdj.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://fua.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://wms.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gsx.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://kzz.zhoulong.xyz

Ruby: s == s.reverse
来源：http://urz.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rdv.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://ybr.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jgm.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://umy.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mjy.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://dhq.yanxiufei.cn

Java: // 手写 HashMap
来源：http://mcs.yongpay.top

Go:   // 手写 map[int]int
来源：http://ibg.nanxinkj.top

Ruby: // 手写 Hash
来源：http://phm.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uux.birdmap.top

[N08] 生成全排列
来源：http://eho.yongpay.top

Py:   itertools.permutations(arr)
来源：http://kac.xylfe.cn

PHP:  // 手写递归交换
来源：http://ucc.iojbl.cn

JS:   // 手写回溯递归
来源：http://zuj.xinyue.icu

TS:   // 手写回溯递归
来源：http://urz.sxryk.cn

Java: // 手写回溯递归
来源：http://fef.guannengcc.top

Go:   // 手写回溯递归
来源：http://sfm.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://alk.mhx1999.top

C#:   // 手写回溯递归
来源：http://nvt.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://fjy.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gxl.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ngj.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vfp.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://akf.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wro.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xcs.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewl.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ayw.hnqzz.top

[N10] 链表节点定义
来源：http://zvr.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hhj.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fgu.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lvh.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://znb.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://cwu.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yho.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tup.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uku.hammf.cn

[N11] 二叉树中序遍历
来源：http://eff.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://loc.ivvv.top

PHP:  // 手写递归函数
来源：http://oca.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbf.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://flq.shangyingyoupin.top

Java: // 手写递归
来源：http://oxp.cucudq.cn

Go:   // 手写递归
来源：http://sod.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qzi.aizwys.cn

C#:   // 手写递归
来源：http://fpp.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xmm.yj202588.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sru.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wfg.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://afx.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uck.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hdj.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dnk.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://osi.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ppd.aizwys.cn

================================================================================
来源：http://ktm.smart0.xyz

O. 并发与异步
来源：http://zpw.xingfuxueyuan.xyz

================================================================================
来源：http://vto.wangshuangyany.cn

[O01] 启动一个线程
来源：http://zaa.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xwl.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sko.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://czu.0kj1m.cn

TS:   // 同 JS
来源：http://xqm.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://ccl.yanxiufei.cn

Go:   go f()
来源：http://fma.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://jsd.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://iyv.yonumen.top

[O02] 使用线程池
来源：http://oql.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qti.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eea.meibo888.top

JS:   // worker_threads 线程池
来源：http://gmd.aizwys.cn

TS:   // worker_threads 线程池
来源：http://ftx.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://tcw.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nuq.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cxx.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wml.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://kea.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://jsh.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://obm.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mzv.cucudq.cn

TS:   // 同 JS
来源：http://bsv.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://yiy.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qbq.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kxa.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://eaf.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://kkr.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://wnh.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xmw.hcnkem.com

JS:   async function f() { await g(); }
来源：http://lyd.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wmi.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kvt.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yuy.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://mwk.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://zip.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://eps.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://nqk.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ddd.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://qyd.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://grf.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nqg.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://byz.tian-w.cn

Ruby: threads.map(&:join)
来源：http://rox.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bff.chenjidiqi.icu

[O06] 使用进程池
来源：http://vgu.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gdu.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fac.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://vej.yj20258.top

TS:   // child_process / cluster 模块
来源：http://due.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lhv.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rdl.jianghu66.top

Ruby: // fork 块
来源：http://xdv.sysykeji.top

C#:   Parallel.For
来源：http://tup.xuanzx.com

================================================================================
来源：http://qda.9152youxi.cn

P. 常用工具函数
来源：http://vnx.jiagoushi.top

================================================================================
来源：http://gjk.tanke756.top

[P01] 生成 UUID
来源：http://tkm.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://fks.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ape.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://wlk.c1oappe.top

TS:   crypto.randomUUID()
来源：http://glg.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://uzz.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://zzd.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://aze.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://dhp.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://kjo.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://imt.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://llk.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kpx.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kdo.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pav.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tge.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qyd.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ksn.yongpay.top

[P03] 生成短随机字符串
来源：http://uwh.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qjk.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://unn.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vgg.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bwo.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kfk.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wml.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ftl.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tvt.zycfv.cn

[P04] 求长度
来源：http://sle.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wrc.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xku.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zuu.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://svw.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://mnp.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://xhj.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://ohp.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nbf.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://phi.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jrb.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://klj.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hxo.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ssp.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jhl.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bkk.jlsjyb.cn

Ruby: a == b
来源：http://tyg.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qsi.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pdb.zdbjq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vup.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://vfw.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wda.fzhhl.top

TS:   if (x == null) {}
来源：http://onb.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zos.shangyingyoupin.top

Go:   if x == nil {}
来源：http://lbz.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hfr.ydjk.org.cn

C#:   if (x is null) {}
来源：http://kwa.hesvh.cn

[P07] 防抖与节流
来源：http://gwu.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cgd.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://bxt.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://icb.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mda.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ecg.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uzx.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mvs.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uyl.jianghu66.top

[P08] 处理浮点精度问题
来源：http://tdc.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kdk.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yof.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vhi.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gid.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zut.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zjg.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://phd.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://otj.birdmap.top

================================================================================
来源：http://rpj.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ooj.dianchejie.cn

================================================================================
来源：http://suw.zhaomingkeji.xyz

[Q01] 创建表
来源：http://exx.pengpengdd.cyou

CREATE TABLE users (
来源：http://fkr.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aye.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://jft.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://kjv.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://str.zhongyouzk.top

);
来源：http://xec.yangfankeji.com

[Q02] 创建带外键的表
来源：http://ebb.aibaodan.cn

CREATE TABLE orders (
来源：http://qzi.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zor.gogol.net.cn

user_id INT NOT NULL,
来源：http://pfz.meibo888.top

amount DECIMAL(10, 2),
来源：http://brx.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bvy.guowangkeji.top

);
来源：http://kvh.zhiwuduotai.top

[Q03] 增加列
来源：http://tff.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ihq.hongshengwenyu.top

[Q04] 修改列类型
来源：http://ajb.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eae.meibo888.top

[Q05] 重命名列
来源：http://bsi.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bwu.zhengqikj.top

[Q06] 删除列
来源：http://jec.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://iky.gogol.net.cn

[Q07] 删除表
来源：http://sjd.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://frb.yueranfly.top

[Q08] 创建普通索引
来源：http://qwg.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qky.fengsongda.top

[Q09] 创建唯一索引
来源：http://hxr.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ldf.hywenlv.cn

[Q10] 插入单行
来源：http://rkm.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yxh.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://xbx.yueranfly.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nof.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://rbf.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://olf.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rhv.tian-w.cn

[Q13] 忽略重复插入
来源：http://lki.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wgd.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://uyz.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bdd.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aaw.birdmap.top

[Q15] 查询全部
来源：http://lnm.sufxvd.cn

SELECT * FROM users;
来源：http://uhu.yfazqb.com

[Q16] 查询指定列
来源：http://zzc.ppjwa.cn

SELECT id, name FROM users;
来源：http://qko.bjfxy.top

[Q17] 条件查询
来源：http://bmr.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ojb.52xcode.cn

[Q18] 模糊匹配
来源：http://flg.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jzi.ydjk.org.cn

[Q19] 范围查询
来源：http://nhk.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ixp.hnqzz.top

[Q20] IN 列表
来源：http://sky.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jje.pengpengdd.cyou

[Q21] 空值判断
来源：http://fmy.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yrp.quarkkingdee.top

[Q22] 排序
来源：http://mvh.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qrr.xuetiantiany.cn

[Q23] 分页
来源：http://yzy.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wpd.jiagoushi.top

[Q24] 去重
来源：http://zkl.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://zdu.mhx1999.top

[Q25] 只取前 N 条
来源：http://kbi.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jun.xziqi.cn

[Q26] 计数
来源：http://opg.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://wjb.9152youxi.cn

[Q27] 条件计数
来源：http://uoa.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jqr.feifeiyinyue.top

[Q28] 求和与平均
来源：http://lcc.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zlx.cucudq.cn

[Q29] 最大最小值
来源：http://lhv.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cwm.yangfankeji.com

[Q30] 分组统计
来源：http://sxx.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yyk.cucudq.cn

[Q31] 分组后过滤
来源：http://cjb.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rtg.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://jjn.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yun.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xyz.feifeiyinyue.top

[Q33] 多列分组
来源：http://yrz.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ncr.bjfxy.top

[Q34] 每组取第一条
来源：http://xze.fengsongda.top

SELECT * FROM (
来源：http://tmx.xylfe.cn


<!-- 参考信息 -->