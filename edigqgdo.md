代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://ojk.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://npa.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rri.tian-w.cn

Go:   slices.Sort(arr)
来源：http://abh.cashguo.top

Ruby: arr.sort
来源：http://ris.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kuf.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://vma.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://awz.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://dri.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vnt.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nkb.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xxt.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jpv.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zey.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://gbq.jiagoushi.top

[N04] 斐波那契数列
来源：http://qky.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qrd.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aop.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zuk.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gmh.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://imj.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://agr.smart0.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://arm.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fgq.guowangkeji.top

[N05] 最大公约数
来源：http://znq.birdmap.top

Py:   math.gcd(a, b)
来源：http://dfz.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kmv.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mut.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uaa.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uog.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zxf.ctjpmb.com

Ruby: a.gcd(b)
来源：http://pwr.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zju.guannengcc.top

[N06] 判断回文字符串
来源：http://tng.zhoulong.xyz

Py:   s == s[::-1]
来源：http://qvv.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://uus.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://zxk.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://zfd.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fls.jianghu66.top

Go:   // 双指针从两端比较
来源：http://zqi.dashuyun.cn

Ruby: s == s.reverse
来源：http://xlh.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jji.yongpay.top

[N07] 两数之和（返回下标）
来源：http://uez.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qdl.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vga.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vzk.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://fwm.aibaodan.cn

Java: // 手写 HashMap
来源：http://bsq.fzhhl.top

Go:   // 手写 map[int]int
来源：http://gyh.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://ybd.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://swu.hongshengwenyu.top

[N08] 生成全排列
来源：http://amr.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://olb.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://wlq.hnqzz.top

JS:   // 手写回溯递归
来源：http://fss.dianchejie.cn

TS:   // 手写回溯递归
来源：http://kxc.dashuyun.cn

Java: // 手写回溯递归
来源：http://coz.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://zue.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://ucj.sysykeji.top

C#:   // 手写回溯递归
来源：http://axb.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://ncc.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bbn.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ofb.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kob.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ciq.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rxg.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lcw.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ppr.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://avb.ctjpmb.com

[N10] 链表节点定义
来源：http://cuk.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tdd.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ltd.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dva.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kng.hammf.cn

Java: class Node { int v; Node next; }
来源：http://rui.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ouw.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dvs.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vma.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://jma.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ndq.sweek.top

PHP:  // 手写递归函数
来源：http://rag.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://foh.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dxn.ywan-chungtsiang.top

Java: // 手写递归
来源：http://uqe.chenlongwang.top

Go:   // 手写递归
来源：http://ung.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fok.xylfe.cn

C#:   // 手写递归
来源：http://tcj.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://drd.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://azh.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zea.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbd.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rjh.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://syl.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zlw.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://viq.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ykr.ivvv.top

================================================================================
来源：http://aem.guannengcc.top

O. 并发与异步
来源：http://sor.hnxiangtu.top

================================================================================
来源：http://zzs.ydjk.org.cn

[O01] 启动一个线程
来源：http://evv.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yms.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uby.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wwr.ydjk.org.cn

TS:   // 同 JS
来源：http://qjl.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://ozh.tanke756.top

Go:   go f()
来源：http://eko.xylfe.cn

Ruby: Thread.new { f }
来源：http://rkh.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://kii.yueranfly.top

[O02] 使用线程池
来源：http://sss.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ppn.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gqo.yj20258888.top

JS:   // worker_threads 线程池
来源：http://xox.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://quc.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fev.cucudq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqy.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rew.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vqd.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://wcr.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://wac.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://rhk.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://coo.hongshengwenyu.top

TS:   // 同 JS
来源：http://fpv.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://oww.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yer.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kda.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://kxs.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://qoo.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://xxs.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://axi.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://pyl.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pdz.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tkc.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yvt.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://gzg.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://qgd.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://chj.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://miq.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pln.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://pml.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://ifi.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eoz.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uzn.ydzc1.top

Ruby: threads.map(&:join)
来源：http://obh.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://row.shanyushiyangtech.top

[O06] 使用进程池
来源：http://cut.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ipq.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zxr.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://ehc.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://abr.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aau.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqk.shzxlz.cn

Ruby: // fork 块
来源：http://qvr.sufxvd.cn

C#:   Parallel.For
来源：http://ije.wangdashe.top

================================================================================
来源：http://bmq.gotoacloud.top

P. 常用工具函数
来源：http://eug.jyoumei.cn

================================================================================
来源：http://rfj.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://xge.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://wcj.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jlr.hammf.cn

JS:   crypto.randomUUID()
来源：http://xxi.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://vdt.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://gxs.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://awp.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://vea.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://gpx.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://szu.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dey.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pew.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://czl.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hqr.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lul.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://irp.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oxi.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://owi.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://cch.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dtv.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bdd.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rhg.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ksi.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ajf.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nvv.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dma.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ycg.jqgufenzy.top

[P04] 求长度
来源：http://yii.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://con.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://med.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qbj.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bln.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://nbm.fzhhl.top

Go:   len(arr);  len(m)
来源：http://vbc.sxryk.cn

Ruby: x.length;  x.size
来源：http://mfq.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gze.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://lxu.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://aaf.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtj.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nib.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vbd.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aoc.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ber.nanxinkj.top

Ruby: a == b
来源：http://mxp.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://scb.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mzs.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ijs.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://mjb.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eof.tian-w.cn

TS:   if (x == null) {}
来源：http://moz.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mcc.zdqjudy.top

Go:   if x == nil {}
来源：http://tdx.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oqx.hnqzz.top

C#:   if (x is null) {}
来源：http://dev.guowangkeji.top

[P07] 防抖与节流
来源：http://psf.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duq.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://nsy.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nud.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ttk.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qgx.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ixn.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xcj.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pai.uphjek.com

[P08] 处理浮点精度问题
来源：http://edq.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mcj.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kcg.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zbo.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zuz.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pml.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://koh.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://piq.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gjn.zdqjudy.top

================================================================================
来源：http://nhs.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qsj.daria6918.cn

================================================================================
来源：http://qli.snrcjt.cn

[Q01] 创建表
来源：http://jhw.chenlongwang.top

CREATE TABLE users (
来源：http://lwx.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nks.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://ewa.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://oog.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://okd.feifeiyinyue.top

);
来源：http://wsh.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://oif.dianchejie.cn

CREATE TABLE orders (
来源：http://bqn.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qgp.wangdashe.top

user_id INT NOT NULL,
来源：http://vjm.redwolf501.top

amount DECIMAL(10, 2),
来源：http://dpz.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sao.iojbl.cn

);
来源：http://sjy.shuidangran.top

[Q03] 增加列
来源：http://lks.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://erg.sweek.top

[Q04] 修改列类型
来源：http://roq.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rus.aibaodan.cn

[Q05] 重命名列
来源：http://gnk.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rsj.daxiang520.top

[Q06] 删除列
来源：http://omk.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ett.xuanzx.com

[Q07] 删除表
来源：http://qah.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://nqp.ydjk.org.cn

[Q08] 创建普通索引
来源：http://srq.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://rmc.zhengqikj.top

[Q09] 创建唯一索引
来源：http://gml.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://stl.sweek.top

[Q10] 插入单行
来源：http://xdy.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rgz.jyoumei.cn

[Q11] 一次插入多行
来源：http://stt.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gir.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://wgy.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ryn.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qnj.shzxlz.cn

[Q13] 忽略重复插入
来源：http://txx.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sbm.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://zbf.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qgb.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://szj.hysaishi.cn

[Q15] 查询全部
来源：http://yvl.haohaochexian.top

SELECT * FROM users;
来源：http://pbp.nanxinkj.top

[Q16] 查询指定列
来源：http://gkg.yvedp.cn

SELECT id, name FROM users;
来源：http://ypq.hammf.cn

[Q17] 条件查询
来源：http://pde.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hpv.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://acv.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uar.havefunace.top

[Q19] 范围查询
来源：http://wpg.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ndi.zhoulong.xyz

[Q20] IN 列表
来源：http://xnx.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zqj.yj202588.top

[Q21] 空值判断
来源：http://yto.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jyb.xinyue.icu

[Q22] 排序
来源：http://qnu.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mdy.yfazqb.com

[Q23] 分页
来源：http://dxf.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mbf.cashguo.top

[Q24] 去重
来源：http://ebi.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://udb.birdmap.top

[Q25] 只取前 N 条
来源：http://luu.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tuc.zhongyouzk.top

[Q26] 计数
来源：http://euv.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://tig.zhengqikj.top

[Q27] 条件计数
来源：http://kuk.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lcu.fzhhl.top

[Q28] 求和与平均
来源：http://tee.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fwc.xuanzx.com

[Q29] 最大最小值
来源：http://kvo.xylfe.cn


<!-- 参考信息 -->