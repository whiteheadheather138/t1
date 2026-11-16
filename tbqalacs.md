代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://uwf.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wkk.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pot.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qwd.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pyx.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rit.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://rrp.hcnkem.com

[N04] 斐波那契数列
来源：http://uvt.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ojs.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dlh.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vnh.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jul.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tfd.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dux.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://goo.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gkg.shanyushiyangtech.top

[N05] 最大公约数
来源：http://qfy.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://cjg.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ygv.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://icp.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dzd.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aaw.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lcg.ehwqpu.com

Ruby: a.gcd(b)
来源：http://dwx.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://igl.cashguo.top

[N06] 判断回文字符串
来源：http://lkh.bjfxy.top

Py:   s == s[::-1]
来源：http://hpz.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://ilw.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://klm.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://hge.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wfv.fktsv.cn

Go:   // 双指针从两端比较
来源：http://zzf.sysykeji.top

Ruby: s == s.reverse
来源：http://zqf.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yrj.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://sli.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rne.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vrw.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://quy.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://fyl.haohaochexian.top

Java: // 手写 HashMap
来源：http://hvu.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://vof.52xcode.cn

Ruby: // 手写 Hash
来源：http://ybp.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fdm.jinqigfzy.top

[N08] 生成全排列
来源：http://qra.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://brb.cdnleiting.top

PHP:  // 手写递归交换
来源：http://ywn.aibaodan.cn

JS:   // 手写回溯递归
来源：http://wuw.sweek.top

TS:   // 手写回溯递归
来源：http://ewk.yvedp.cn

Java: // 手写回溯递归
来源：http://npp.pycfn.com

Go:   // 手写回溯递归
来源：http://vqn.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://mdj.smart0.xyz

C#:   // 手写回溯递归
来源：http://ktn.0kj1m.cn

[N09] 栈与队列
来源：http://iuy.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yvz.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ogk.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bzv.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bra.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xjw.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rgm.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jkj.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://etg.bjfxy.top

[N10] 链表节点定义
来源：http://yvw.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gdl.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cng.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://acv.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mbd.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://jfc.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://rjb.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ltc.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jnq.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://pjb.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gul.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://uwa.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cdn.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yqp.zhengqikj.top

Java: // 手写递归
来源：http://fiq.birdmap.top

Go:   // 手写递归
来源：http://ejb.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fpx.sxryk.cn

C#:   // 手写递归
来源：http://ose.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pho.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kpx.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bcn.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tog.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gfc.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qqh.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sbz.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://usi.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ztb.fengsongda.top

================================================================================
来源：http://pya.zdbjq.cn

O. 并发与异步
来源：http://myu.fktsv.cn

================================================================================
来源：http://prr.iojbl.cn

[O01] 启动一个线程
来源：http://uxa.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iat.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bdm.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://paz.gaohongyu789.top

TS:   // 同 JS
来源：http://ljd.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://ecr.sxryk.cn

Go:   go f()
来源：http://rwc.xziqi.cn

Ruby: Thread.new { f }
来源：http://fcw.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://ytc.hammf.cn

[O02] 使用线程池
来源：http://kjy.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vbg.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jom.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://qfi.nwbrower.top

TS:   // worker_threads 线程池
来源：http://yjq.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bid.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fzw.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://obb.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mhe.gzhubu.top

[O03] 加锁保护共享数据
来源：http://psh.sufxvd.cn

Py:   with lock: shared += 1
来源：http://kkw.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://rrx.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yvu.cucudq.cn

TS:   // 同 JS
来源：http://hiw.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://swb.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fin.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cbs.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://rdr.daxiang520.top

[O04] 定义异步函数并等待
来源：http://jmf.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://tie.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yea.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://hsd.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hrw.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://amz.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qqm.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://jrb.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://ztm.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://snw.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://djb.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jiw.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://bpq.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://hrn.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lpf.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://txt.fzhhl.top

Ruby: threads.map(&:join)
来源：http://shj.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ghn.0kj1m.cn

[O06] 使用进程池
来源：http://qla.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://txu.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kpf.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://fcq.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://cve.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://duk.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iwj.vqdsnc.cn

Ruby: // fork 块
来源：http://jsi.epnwcf.com

C#:   Parallel.For
来源：http://oqf.quarkkingdee.top

================================================================================
来源：http://ftz.yueranfly.top

P. 常用工具函数
来源：http://xty.jiagoushi.top

================================================================================
来源：http://jdx.tian-w.cn

[P01] 生成 UUID
来源：http://ycw.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://eab.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xdv.hammf.cn

JS:   crypto.randomUUID()
来源：http://eyr.shuidangran.top

TS:   crypto.randomUUID()
来源：http://zfm.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://krv.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://fbm.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://kil.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://xqa.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://jew.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wwl.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kuy.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mhk.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mfg.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lli.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dtq.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cil.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sjk.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://zqh.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://edz.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tna.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wxq.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://igs.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wzk.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tyu.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://per.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jqv.gzhubu.top

[P04] 求长度
来源：http://hhi.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xhu.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ice.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jia.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://npl.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://qdg.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://qva.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://oih.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wla.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://ojh.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://klz.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qyp.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ttr.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rfc.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qtx.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nme.hfpthk.cn

Ruby: a == b
来源：http://pfu.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uzl.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tbg.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxj.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://vzs.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fzj.tianlin.xyz

TS:   if (x == null) {}
来源：http://ffb.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://eyn.pycfn.com

Go:   if x == nil {}
来源：http://zqw.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kmy.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://gqc.jlsjyb.cn

[P07] 防抖与节流
来源：http://cgn.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jxu.yj20258.top

PHP:  // 手写时间戳比较
来源：http://enw.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmx.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhd.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gvw.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zba.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oia.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jnh.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://hju.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iqz.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://muk.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fwd.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://apf.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vre.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bwx.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ngz.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lin.yvedp.cn

================================================================================
来源：http://hkx.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gqk.shanyushiyangtech.top

================================================================================
来源：http://qgn.zdbjq.cn

[Q01] 创建表
来源：http://ufw.nanxuanxn.top

CREATE TABLE users (
来源：http://lmz.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dmd.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://mju.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://amu.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://trl.fengsongda.top

);
来源：http://agu.tanke756.top

[Q02] 创建带外键的表
来源：http://flv.52xcode.cn

CREATE TABLE orders (
来源：http://wsy.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jnf.sxryk.cn

user_id INT NOT NULL,
来源：http://swv.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://kya.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nbk.feifeiyinyue.top

);
来源：http://jfq.bjfxy.top

[Q03] 增加列
来源：http://jah.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iiy.jianghu66.top

[Q04] 修改列类型
来源：http://cck.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bcd.ctjpmb.com

[Q05] 重命名列
来源：http://edn.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zhz.yfazqb.com

[Q06] 删除列
来源：http://fhj.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://gac.hnqzz.top

[Q07] 删除表
来源：http://xxr.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://hbs.ehwqpu.com

[Q08] 创建普通索引
来源：http://jil.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://haa.redwolf501.top

[Q09] 创建唯一索引
来源：http://axe.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://obn.xinyue.icu

[Q10] 插入单行
来源：http://eob.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cfj.aibaodan.cn

[Q11] 一次插入多行
来源：http://gzw.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xev.ivvv.top

[Q12] 插入后取自增 ID
来源：http://xjn.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://oqz.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://evz.yuxming.cn

[Q13] 忽略重复插入
来源：http://jbz.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xeb.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://ori.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://edh.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jaf.ybcxt.top

[Q15] 查询全部
来源：http://jib.yj20258888.top

SELECT * FROM users;
来源：http://trc.zhengqikj.top

[Q16] 查询指定列
来源：http://zpy.chenzaomai.com

SELECT id, name FROM users;
来源：http://mfy.ybcxt.top

[Q17] 条件查询
来源：http://xbj.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://myn.ivvv.top

[Q18] 模糊匹配
来源：http://wpx.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzi.sufxvd.cn

[Q19] 范围查询
来源：http://wsj.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ytn.yj20258.top

[Q20] IN 列表
来源：http://mvx.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dtv.daria6918.cn

[Q21] 空值判断
来源：http://zeb.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yxo.aizwys.cn

[Q22] 排序
来源：http://ocm.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xij.svipenyu.cn

[Q23] 分页
来源：http://xbg.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hbb.yanxiufei.cn

[Q24] 去重
来源：http://kcq.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://zdo.shzxlz.cn

[Q25] 只取前 N 条
来源：http://hic.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdk.cucudq.cn

[Q26] 计数
来源：http://pxk.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://hsk.tarul.cn

[Q27] 条件计数
来源：http://isq.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://orj.cucudq.cn

[Q28] 求和与平均
来源：http://gae.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jno.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://eps.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wjy.yongpay.top

[Q30] 分组统计
来源：http://unl.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yxa.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://eok.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jck.fehbvm.com

[Q32] 分组拼接字符串
来源：http://qtl.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bkm.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lcu.uphjek.com


<!-- 参考信息 -->