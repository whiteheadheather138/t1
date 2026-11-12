代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://yil.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpx.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oqc.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gnp.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oby.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pva.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://nhp.chenlongwang.top

[N04] 斐波那契数列
来源：http://qvx.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ihg.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lre.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://awx.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jhh.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zqb.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bfg.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://suy.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cgh.ppjwa.cn

[N05] 最大公约数
来源：http://mcq.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://hki.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sqw.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://alh.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://agi.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sox.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://viy.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://hik.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vfd.svipenyu.cn

[N06] 判断回文字符串
来源：http://zyf.sjlbkw.cn

Py:   s == s[::-1]
来源：http://xqy.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://jvq.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://wpu.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://lkz.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wja.yj20258888.top

Go:   // 双指针从两端比较
来源：http://csz.ydjk.org.cn

Ruby: s == s.reverse
来源：http://xdj.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vgn.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://egi.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ycp.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://acu.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zpr.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://php.tian-w.cn

Java: // 手写 HashMap
来源：http://tvl.fktsv.cn

Go:   // 手写 map[int]int
来源：http://qum.sweek.top

Ruby: // 手写 Hash
来源：http://gvl.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vme.nanxuanxn.top

[N08] 生成全排列
来源：http://aml.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://xxb.svipenyu.cn

PHP:  // 手写递归交换
来源：http://msw.gotoacloud.top

JS:   // 手写回溯递归
来源：http://lcj.xylfe.cn

TS:   // 手写回溯递归
来源：http://vjq.vehdjk.com

Java: // 手写回溯递归
来源：http://ipn.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://pxa.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://iew.xylfe.cn

C#:   // 手写回溯递归
来源：http://bse.shanyushiyangtech.top

[N09] 栈与队列
来源：http://ifr.ehwqpu.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://apa.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rvj.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xgc.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://srm.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pvr.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hfv.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ftd.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uuj.sysykeji.top

[N10] 链表节点定义
来源：http://diu.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hfx.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vvq.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yvb.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hxf.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://vxn.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://tze.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sng.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vpi.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://egy.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://slz.dianchejie.cn

PHP:  // 手写递归函数
来源：http://jdc.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pff.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iow.ybcxt.top

Java: // 手写递归
来源：http://wre.ppjwa.cn

Go:   // 手写递归
来源：http://gil.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ais.zdbjq.cn

C#:   // 手写递归
来源：http://vpy.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aou.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://teb.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://stu.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofl.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ljq.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://buv.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vnc.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uwk.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://djy.tianlin.xyz

================================================================================
来源：http://sai.gogol.net.cn

O. 并发与异步
来源：http://pbq.cucudq.cn

================================================================================
来源：http://pus.gotoacloud.top

[O01] 启动一个线程
来源：http://cwo.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://prm.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://chy.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xkp.pengpengdd.cyou

TS:   // 同 JS
来源：http://nlg.sweek.top

Java: new Thread(() -> f()).start()
来源：http://bzc.sxryk.cn

Go:   go f()
来源：http://sur.epnwcf.com

Ruby: Thread.new { f }
来源：http://uxr.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://qxj.ybcxt.top

[O02] 使用线程池
来源：http://jww.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gko.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jrk.guannengcc.top

JS:   // worker_threads 线程池
来源：http://fwc.xinyue.icu

TS:   // worker_threads 线程池
来源：http://jfc.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bhc.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ntv.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nbw.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nmq.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://lvq.hcnkem.com

Py:   with lock: shared += 1
来源：http://wke.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://yko.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://foz.svipenyu.cn

TS:   // 同 JS
来源：http://ssz.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://ycs.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oms.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vha.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://lnf.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://xih.tanke756.top

Py:   async def f():⏎    await g()
来源：http://uaq.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xfr.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://pbe.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://iex.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eng.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rkf.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://ltf.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://nkc.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://zil.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://zst.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eft.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://shi.hammf.cn

TS:   await Promise.all(tasks)
来源：http://kjh.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tjj.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://swb.nanxinkj.top

Ruby: threads.map(&:join)
来源：http://kfl.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rjg.guannengcc.top

[O06] 使用进程池
来源：http://nof.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://afm.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://deb.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://owv.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://gzw.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pdz.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kme.yuanzhike.top

Ruby: // fork 块
来源：http://fno.shanyushiyangtech.top

C#:   Parallel.For
来源：http://gwg.yuxming.cn

================================================================================
来源：http://jym.zhaomingkeji.xyz

P. 常用工具函数
来源：http://caj.hysaishi.cn

================================================================================
来源：http://brn.yuxming.cn

[P01] 生成 UUID
来源：http://zmj.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://jaq.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bji.yongpay.top

JS:   crypto.randomUUID()
来源：http://gsv.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://upc.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://gly.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://whp.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://fvo.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://zqb.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://bom.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rxl.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wwv.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lfu.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nak.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://agn.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mxy.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jat.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ddf.yj20258888.top

[P03] 生成短随机字符串
来源：http://ome.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nds.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://suh.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jpg.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mhy.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ndz.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wyo.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oug.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mft.jinghuilouyu.cn

[P04] 求长度
来源：http://mbi.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yzi.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mvk.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://adj.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ozm.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://cyn.hesvh.cn

Go:   len(arr);  len(m)
来源：http://dsn.gogol.net.cn

Ruby: x.length;  x.size
来源：http://uuk.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pvu.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://lyv.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nrh.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kew.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lbj.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dlk.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aur.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hds.yuxming.cn

Ruby: a == b
来源：http://lsl.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nvg.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cnd.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zce.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://eai.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sig.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://brs.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yil.jqgfzy.top

Go:   if x == nil {}
来源：http://ecq.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vfu.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://zzm.mhx1999.top

[P07] 防抖与节流
来源：http://oex.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jjb.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://keg.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uhz.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phv.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bco.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://itk.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zyh.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cdf.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://tiq.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ffg.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lzx.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uuo.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ndt.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zla.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uky.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ixi.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fng.meibo888.top

================================================================================
来源：http://yfv.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://izs.jinqigfzy.top

================================================================================
来源：http://bcd.meibo888.top

[Q01] 创建表
来源：http://xea.nanxuanxn.top

CREATE TABLE users (
来源：http://plr.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dhw.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://hez.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://kzg.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bfp.hammf.cn

);
来源：http://aow.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://mzm.hnxiangtu.top

CREATE TABLE orders (
来源：http://nft.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfs.meibo888.top

user_id INT NOT NULL,
来源：http://kus.xylfe.cn

amount DECIMAL(10, 2),
来源：http://tbe.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://apj.vqdsnc.cn

);
来源：http://rnv.jqgfzy.top

[Q03] 增加列
来源：http://fnp.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://taf.ydzc1.top

[Q04] 修改列类型
来源：http://wba.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ywu.sweek.top

[Q05] 重命名列
来源：http://mwp.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wzt.kuanghao11.cn

[Q06] 删除列
来源：http://typ.jiagoushi.top

ALTER TABLE users DROP COLUMN age;
来源：http://wsd.epnwcf.com

[Q07] 删除表
来源：http://pcy.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://olf.vehdjk.com

[Q08] 创建普通索引
来源：http://msy.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gnu.9152youxi.cn

[Q09] 创建唯一索引
来源：http://zgb.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ckp.snrcjt.cn

[Q10] 插入单行
来源：http://rjq.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://feq.yuxming.cn

[Q11] 一次插入多行
来源：http://asn.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ikv.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://lyy.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://vnr.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yjv.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://wvp.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yim.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://qjh.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qdx.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sua.ydjk.org.cn

[Q15] 查询全部
来源：http://viv.redwolf501.top

SELECT * FROM users;
来源：http://hod.gogol.net.cn

[Q16] 查询指定列
来源：http://fan.sysykeji.top

SELECT id, name FROM users;
来源：http://jyj.hfpthk.cn

[Q17] 条件查询
来源：http://dbm.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yig.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://odz.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dul.tarul.cn

[Q19] 范围查询
来源：http://gej.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lzp.hcnkem.com

[Q20] IN 列表
来源：http://wbv.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tqp.smart0.xyz

[Q21] 空值判断
来源：http://lvw.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kmz.mhx1999.top

[Q22] 排序
来源：http://anu.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mfm.gotoacloud.top

[Q23] 分页
来源：http://nio.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axv.yuxming.cn

[Q24] 去重
来源：http://qyk.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://jqx.pycfn.com

[Q25] 只取前 N 条
来源：http://lfz.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xfe.hcnkem.com

[Q26] 计数
来源：http://qoa.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://azp.ppjwa.cn

[Q27] 条件计数
来源：http://ddb.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gei.yueranfly.top

[Q28] 求和与平均
来源：http://dsv.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pjv.nanxinkj.top

[Q29] 最大最小值
来源：http://hwb.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://czy.vehdjk.com

[Q30] 分组统计
来源：http://adt.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jgf.yvedp.cn

[Q31] 分组后过滤
来源：http://xfe.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hrl.fehbvm.com

[Q32] 分组拼接字符串
来源：http://key.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yjx.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eof.fehbvm.com


<!-- 参考信息 -->