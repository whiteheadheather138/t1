代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://rqf.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lzy.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vws.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bxj.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vxi.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qln.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://ejz.shzxlz.cn

[N04] 斐波那契数列
来源：http://wlv.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aan.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbm.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uuz.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xpk.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kvb.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kat.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ily.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gka.tianlin.xyz

[N05] 最大公约数
来源：http://one.fengsongda.top

Py:   math.gcd(a, b)
来源：http://qjy.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tbw.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mri.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://srk.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zqz.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fqd.uphjek.com

Ruby: a.gcd(b)
来源：http://jna.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nmp.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://dlj.nwbrower.top

Py:   s == s[::-1]
来源：http://mql.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://zcs.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://gzr.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://gfn.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nfe.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://cdt.tian-w.cn

Ruby: s == s.reverse
来源：http://ijg.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xnt.sweek.top

[N07] 两数之和（返回下标）
来源：http://adr.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xtg.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jqo.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pfa.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://jep.haohaochexian.top

Java: // 手写 HashMap
来源：http://vhu.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://cuh.dashuyun.cn

Ruby: // 手写 Hash
来源：http://qjo.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://drs.fktsv.cn

[N08] 生成全排列
来源：http://szr.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://soa.ydjk.org.cn

PHP:  // 手写递归交换
来源：http://une.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://udt.cashguo.top

TS:   // 手写回溯递归
来源：http://hyf.yongpay.top

Java: // 手写回溯递归
来源：http://dbq.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://vzu.tarul.cn

Ruby: arr.permutation.to_a
来源：http://nux.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://gcn.daria6918.cn

[N09] 栈与队列
来源：http://zof.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wog.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sjc.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dmt.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ixt.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ijv.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ybx.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fhj.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xao.yanxiufei.cn

[N10] 链表节点定义
来源：http://uyh.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wgk.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kqv.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ydm.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fbi.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://mqq.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://bdd.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qat.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://idi.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://kgz.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gdd.guowangkeji.top

PHP:  // 手写递归函数
来源：http://bdk.pycfn.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxc.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yvx.zycfv.cn

Java: // 手写递归
来源：http://wdd.52xcode.cn

Go:   // 手写递归
来源：http://osm.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://des.quarkkingdee.top

C#:   // 手写递归
来源：http://kud.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rtj.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mgg.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zse.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vxf.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ftw.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nbm.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lso.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jvy.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gdb.epnwcf.com

================================================================================
来源：http://afa.shzxlz.cn

O. 并发与异步
来源：http://cym.jqgfzy.top

================================================================================
来源：http://jry.ppjwa.cn

[O01] 启动一个线程
来源：http://myk.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sih.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uxe.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dpk.cheryme.top

TS:   // 同 JS
来源：http://txk.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://tgj.svipenyu.cn

Go:   go f()
来源：http://axb.zdqjudy.top

Ruby: Thread.new { f }
来源：http://eqt.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://akc.sxryk.cn

[O02] 使用线程池
来源：http://zjh.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zmr.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://giq.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://oby.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://tcw.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://pun.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abo.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mri.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://prh.yj202588.top

[O03] 加锁保护共享数据
来源：http://gpx.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://xnc.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://ibg.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dkj.0kj1m.cn

TS:   // 同 JS
来源：http://yeb.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://tno.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pmv.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gto.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://jux.cucudq.cn

[O04] 定义异步函数并等待
来源：http://xie.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://rba.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dfv.smart0.xyz

JS:   async function f() { await g(); }
来源：http://rbv.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dlq.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rim.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uck.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yvy.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://ctb.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://jky.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://bsw.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ulg.ivvv.top

JS:   await Promise.all(tasks)
来源：http://pze.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://mje.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xwd.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cpl.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://iro.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://soj.jinqigufen.top

[O06] 使用进程池
来源：http://epx.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://shl.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mbj.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://hoz.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://lun.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xkh.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dii.yj20258.top

Ruby: // fork 块
来源：http://hzv.jyoumei.cn

C#:   Parallel.For
来源：http://ewm.birdmap.top

================================================================================
来源：http://wle.cashguo.top

P. 常用工具函数
来源：http://phh.shanyushiyangtech.top

================================================================================
来源：http://lei.jianghu66.top

[P01] 生成 UUID
来源：http://grh.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://ejp.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dwa.tanke756.top

JS:   crypto.randomUUID()
来源：http://kcr.hcnkem.com

TS:   crypto.randomUUID()
来源：http://krt.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://fnp.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://sfi.yongpay.top

Ruby: SecureRandom.uuid
来源：http://msp.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://opu.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://iko.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bcw.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://njp.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://shu.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://voc.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://snl.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pij.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://thk.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vkc.meibo888.top

[P03] 生成短随机字符串
来源：http://hrv.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cje.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ccj.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wjm.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eam.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rmj.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://knz.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://khe.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://glx.pengpengdd.cyou

[P04] 求长度
来源：http://xfa.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rgu.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aff.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kpf.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wrk.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://aut.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://xqo.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://gvb.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://qww.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://wsj.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fwg.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://szx.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zci.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exy.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ilc.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://xws.gotoacloud.top

Ruby: a == b
来源：http://rol.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://abw.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jbr.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sah.xinyue.icu

PHP:  if (empty($x)) {}
来源：http://osf.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ajt.daxiang520.top

TS:   if (x == null) {}
来源：http://yav.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wij.dashuyun.cn

Go:   if x == nil {}
来源：http://jsf.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hhw.yueranfly.top

C#:   if (x is null) {}
来源：http://bwk.jiagoushi.top

[P07] 防抖与节流
来源：http://ohp.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hxy.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://dqh.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgf.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ant.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tsv.xziqi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oks.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://fxk.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ark.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://ojb.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://udy.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mcl.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://usm.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lmk.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kau.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gbn.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jzx.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vxg.jiagoushi.top

================================================================================
来源：http://frg.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://puf.fengsongda.top

================================================================================
来源：http://syw.bbcook.cn

[Q01] 创建表
来源：http://mds.chenlongwang.top

CREATE TABLE users (
来源：http://rre.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ntn.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://hfy.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://iql.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://awf.nanxuanxn.top

);
来源：http://xbq.yonumen.top

[Q02] 创建带外键的表
来源：http://smp.xylfe.cn

CREATE TABLE orders (
来源：http://dqm.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hhx.svipenyu.cn

user_id INT NOT NULL,
来源：http://bag.yonumen.top

amount DECIMAL(10, 2),
来源：http://icw.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dmk.yueranfly.top

);
来源：http://kil.316326.xyz

[Q03] 增加列
来源：http://sae.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lic.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://nad.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://avx.quarkkingdee.top

[Q05] 重命名列
来源：http://xys.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gms.daria6918.cn

[Q06] 删除列
来源：http://xnn.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://usj.sysykeji.top

[Q07] 删除表
来源：http://fur.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://gam.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://pbr.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rcl.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://djz.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://flg.shanyushiyangtech.top

[Q10] 插入单行
来源：http://zbt.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tqd.nanxuanxn.top

[Q11] 一次插入多行
来源：http://ash.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pqg.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://zyz.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://eqw.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dqa.zdqjudy.top

[Q13] 忽略重复插入
来源：http://gyz.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kwo.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://xgy.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mcb.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uux.sxryk.cn

[Q15] 查询全部
来源：http://rsa.zycfv.cn

SELECT * FROM users;
来源：http://gqh.yueranfly.top

[Q16] 查询指定列
来源：http://qre.yueranfly.top

SELECT id, name FROM users;
来源：http://eet.pycfn.com

[Q17] 条件查询
来源：http://lju.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xip.yanxiufei.cn

[Q18] 模糊匹配
来源：http://wsz.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sgn.ivvv.top

[Q19] 范围查询
来源：http://ifr.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ben.zdqjudy.top

[Q20] IN 列表
来源：http://cnu.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://buw.cashguo.top

[Q21] 空值判断
来源：http://nco.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uom.zhixingplan.top

[Q22] 排序
来源：http://nmy.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fhs.jinyuanbaomall.cn

[Q23] 分页
来源：http://bjz.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tvm.jiagoushi.top

[Q24] 去重
来源：http://coq.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://fun.xuanzx.com

[Q25] 只取前 N 条
来源：http://uud.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lle.yuxming.cn

[Q26] 计数
来源：http://ymd.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://qij.sxryk.cn

[Q27] 条件计数
来源：http://mab.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nia.xuetiantiany.cn

[Q28] 求和与平均
来源：http://uta.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://heo.hammf.cn

[Q29] 最大最小值
来源：http://byt.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hno.zdbjq.cn

[Q30] 分组统计
来源：http://cfl.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ang.chenzaomai.com

[Q31] 分组后过滤
来源：http://jpn.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ghx.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://tkq.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://spp.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cug.feifeiyinyue.top


<!-- 参考信息 -->