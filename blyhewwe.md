代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://khq.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zjt.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pdg.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xim.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qwz.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dec.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://opj.sufxvd.cn

[N04] 斐波那契数列
来源：http://zlh.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kag.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utj.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baw.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bxq.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hsj.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bzl.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yme.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ewf.jqgufenzy.top

[N05] 最大公约数
来源：http://tkv.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://bgr.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sxn.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gbd.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vfv.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ofj.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rua.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://jvc.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qdm.gogol.net.cn

[N06] 判断回文字符串
来源：http://hpy.kuanghao11.cn

Py:   s == s[::-1]
来源：http://lch.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://nwc.epnwcf.com

JS:   s === [...s].reverse().join("")
来源：http://kdv.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://vck.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dkv.yvedp.cn

Go:   // 双指针从两端比较
来源：http://hki.hnxiangtu.top

Ruby: s == s.reverse
来源：http://ihk.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://olq.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://qxg.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://osk.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://opp.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://crq.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://vha.cdnleiting.top

Java: // 手写 HashMap
来源：http://pas.fehbvm.com

Go:   // 手写 map[int]int
来源：http://ifk.zhixingplan.top

Ruby: // 手写 Hash
来源：http://kok.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://nrh.guowangkeji.top

[N08] 生成全排列
来源：http://cbb.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://nms.cashguo.top

PHP:  // 手写递归交换
来源：http://zvh.gzhubu.top

JS:   // 手写回溯递归
来源：http://bzr.smart0.xyz

TS:   // 手写回溯递归
来源：http://ukg.nanxinkj.top

Java: // 手写回溯递归
来源：http://yzt.zdbjq.cn

Go:   // 手写回溯递归
来源：http://xbh.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://iix.ehwqpu.com

C#:   // 手写回溯递归
来源：http://dch.0kj1m.cn

[N09] 栈与队列
来源：http://rmq.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hxm.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iaq.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pqz.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cyk.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wzc.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://krb.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vmx.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://noj.ivvv.top

[N10] 链表节点定义
来源：http://gdw.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pgc.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zbv.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://okj.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hkm.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://foq.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://csj.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://opb.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://udk.smart0.xyz

[N11] 二叉树中序遍历
来源：http://eii.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aft.ivvv.top

PHP:  // 手写递归函数
来源：http://afc.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsa.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://szb.andypj.xyz

Java: // 手写递归
来源：http://fso.yvedp.cn

Go:   // 手写递归
来源：http://nhm.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aeb.svipenyu.cn

C#:   // 手写递归
来源：http://pug.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gdk.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zvt.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gyu.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwu.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mne.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vkd.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fbz.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rjz.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mof.fehbvm.com

================================================================================
来源：http://qiw.jinqigfzy.top

O. 并发与异步
来源：http://yyn.jyoumei.cn

================================================================================
来源：http://qqg.sjlbkw.cn

[O01] 启动一个线程
来源：http://iey.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cln.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uyp.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ium.gogol.net.cn

TS:   // 同 JS
来源：http://bjm.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://fvp.ivvv.top

Go:   go f()
来源：http://jrd.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://juk.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://bhd.jqgfzy.top

[O02] 使用线程池
来源：http://uix.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wdb.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rgq.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://siu.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://gxv.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://ajw.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tqx.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lxg.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ton.tanke756.top

[O03] 加锁保护共享数据
来源：http://qhd.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://nqn.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://egy.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oov.zdqjudy.top

TS:   // 同 JS
来源：http://zok.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://csd.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fbk.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bvd.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://myy.cheryme.top

[O04] 定义异步函数并等待
来源：http://dqv.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://ypj.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gvp.tanke756.top

JS:   async function f() { await g(); }
来源：http://fmb.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rmo.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kfl.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pad.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gkv.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://zdc.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://hmp.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://cxb.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nbc.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://ynb.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://hlc.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ftf.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gxe.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://ldz.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tej.zycfv.cn

[O06] 使用进程池
来源：http://mxg.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nsn.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://yii.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://yhd.yonumen.top

TS:   // child_process / cluster 模块
来源：http://ubp.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bwf.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wpi.yanxiufei.cn

Ruby: // fork 块
来源：http://ncu.sweek.top

C#:   Parallel.For
来源：http://drr.fanxiaobao.xyz

================================================================================
来源：http://aqr.sufxvd.cn

P. 常用工具函数
来源：http://fdc.nanxuanxn.top

================================================================================
来源：http://pis.yj202588.top

[P01] 生成 UUID
来源：http://mtt.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://qal.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://twh.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://dkl.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://xra.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://zou.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://olb.hammf.cn

Ruby: SecureRandom.uuid
来源：http://ebr.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://dgr.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://yxz.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uvk.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nnd.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nap.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yea.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://esa.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nnx.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fra.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qkt.hesvh.cn

[P03] 生成短随机字符串
来源：http://drt.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fgn.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nwv.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwd.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctk.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mcq.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bma.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://enm.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wmg.ydzc1.top

[P04] 求长度
来源：http://ruc.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rop.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bjb.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lla.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dtq.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://pdu.zycfv.cn

Go:   len(arr);  len(m)
来源：http://xtk.jiagoushi.top

Ruby: x.length;  x.size
来源：http://dbs.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://wwn.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://iio.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://erc.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jyk.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nsv.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uxn.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cmu.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xbn.cdnleiting.top

Ruby: a == b
来源：http://fsj.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ase.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jha.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ubz.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://zkv.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://syi.yj20258888.top

TS:   if (x == null) {}
来源：http://nrf.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rak.zdbjq.cn

Go:   if x == nil {}
来源：http://yir.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://omi.ehwqpu.com

C#:   if (x is null) {}
来源：http://wef.nanxuanxn.top

[P07] 防抖与节流
来源：http://rdw.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dhj.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://yos.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xvf.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cob.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yld.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lsv.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lhq.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kiw.uphjek.com

[P08] 处理浮点精度问题
来源：http://tda.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gtc.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mzn.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lsd.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gya.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ewg.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://alc.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wrt.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zew.gogol.net.cn

================================================================================
来源：http://gzu.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vzj.mhx1999.top

================================================================================
来源：http://mrs.zhixingplan.top

[Q01] 创建表
来源：http://lqr.zdbjq.cn

CREATE TABLE users (
来源：http://onj.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ufr.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://kjn.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://vlr.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dch.xuanzx.com

);
来源：http://qyv.cqqwz.cn

[Q02] 创建带外键的表
来源：http://rym.hnqzz.top

CREATE TABLE orders (
来源：http://abu.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sqm.guowangkeji.top

user_id INT NOT NULL,
来源：http://qgi.sysykeji.top

amount DECIMAL(10, 2),
来源：http://hwr.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xzi.gogol.net.cn

);
来源：http://vck.jyoumei.cn

[Q03] 增加列
来源：http://bbf.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://myl.hywenlv.cn

[Q04] 修改列类型
来源：http://wde.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ktd.jlsjyb.cn

[Q05] 重命名列
来源：http://esf.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mkn.shanyushiyangtech.top

[Q06] 删除列
来源：http://qca.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ttg.yongpay.top

[Q07] 删除表
来源：http://owj.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://ovk.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://jfc.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://inu.shzxlz.cn

[Q09] 创建唯一索引
来源：http://eua.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uxy.yj20258888.top

[Q10] 插入单行
来源：http://bid.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dei.316326.xyz

[Q11] 一次插入多行
来源：http://koi.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fzu.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://smk.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://kfm.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://emk.xziqi.cn

[Q13] 忽略重复插入
来源：http://xug.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ype.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://ill.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mfx.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fhf.snrcjt.cn

[Q15] 查询全部
来源：http://woc.zhongyouzk.top

SELECT * FROM users;
来源：http://tir.shangyingyoupin.top

[Q16] 查询指定列
来源：http://alr.fzhhl.top

SELECT id, name FROM users;
来源：http://zre.zhijiandao.cn

[Q17] 条件查询
来源：http://xav.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rgk.pycfn.com

[Q18] 模糊匹配
来源：http://wyv.zycfv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yun.cucudq.cn

[Q19] 范围查询
来源：http://pxf.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mvl.ehwqpu.com

[Q20] IN 列表
来源：http://ghw.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aum.wangshuangyany.cn

[Q21] 空值判断
来源：http://bzv.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rya.tian-w.cn

[Q22] 排序
来源：http://dun.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aju.meibo888.top

[Q23] 分页
来源：http://fak.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wxi.hnxiangtu.top

[Q24] 去重
来源：http://jlm.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://mdr.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://dnt.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rrk.jyoumei.cn

[Q26] 计数
来源：http://mmx.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://ubb.jinqigufen.top

[Q27] 条件计数
来源：http://sqh.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://haj.jiagoushi.top

[Q28] 求和与平均
来源：http://lmb.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oaz.aibaodan.cn

[Q29] 最大最小值
来源：http://auk.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wws.jianghu66.top

[Q30] 分组统计
来源：http://wfc.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cbt.uphjek.com

[Q31] 分组后过滤
来源：http://wyy.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://osx.c1oappe.top

[Q32] 分组拼接字符串
来源：http://cwd.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lsx.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lss.hammf.cn


<!-- 参考信息 -->