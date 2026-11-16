代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://muk.havefunace.top

================================================================================
来源：http://ttw.gzhubu.top

N. 数据结构与算法
来源：http://pmu.daxiang520.top

================================================================================
来源：http://ymw.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://ijh.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rnv.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://coi.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iqe.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lex.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://xvf.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bmp.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uqz.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://bmi.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://wvw.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://nao.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vao.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dsq.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://luw.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nuh.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://oaf.wangdashe.top

Ruby: arr.sort
来源：http://rak.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cyu.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://qar.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kwy.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://sue.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hnh.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rmu.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yak.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pke.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bbw.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xta.bjfxy.top

[N04] 斐波那契数列
来源：http://hhn.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dnp.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fql.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dpn.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rzz.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lfw.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cnf.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uyd.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xsr.cheryme.top

[N05] 最大公约数
来源：http://kbc.yfazqb.com

Py:   math.gcd(a, b)
来源：http://wpv.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ioa.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ejj.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asa.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tim.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qjw.cheryme.top

Ruby: a.gcd(b)
来源：http://znh.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pyy.epnwcf.com

[N06] 判断回文字符串
来源：http://far.xuanzx.com

Py:   s == s[::-1]
来源：http://rlx.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://nmh.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://ipu.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://bni.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://myc.hnqzz.top

Go:   // 双指针从两端比较
来源：http://ujw.iojbl.cn

Ruby: s == s.reverse
来源：http://ywl.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://sqh.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://mzn.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ceb.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eer.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tdo.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://jte.xylfe.cn

Java: // 手写 HashMap
来源：http://zig.nwbrower.top

Go:   // 手写 map[int]int
来源：http://cuu.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://qrr.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://nor.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://dqu.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://pix.hysaishi.cn

PHP:  // 手写递归交换
来源：http://dxm.tarul.cn

JS:   // 手写回溯递归
来源：http://njf.birdmap.top

TS:   // 手写回溯递归
来源：http://vhv.redwolf501.top

Java: // 手写回溯递归
来源：http://kzg.sufxvd.cn

Go:   // 手写回溯递归
来源：http://mvq.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://saj.nwbrower.top

C#:   // 手写回溯递归
来源：http://orm.hysaishi.cn

[N09] 栈与队列
来源：http://nuf.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://phg.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mle.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mzt.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kep.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://urx.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bwg.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kiw.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tgc.jqgufenzy.top

[N10] 链表节点定义
来源：http://tgz.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tnz.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hnx.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wqf.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nrm.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://mxo.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iat.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dcg.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xrn.52xcode.cn

[N11] 二叉树中序遍历
来源：http://wss.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rir.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://fzl.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqs.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpy.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://wdl.ctjpmb.com

Go:   // 手写递归
来源：http://mab.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://njt.tarul.cn

C#:   // 手写递归
来源：http://xmg.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fwm.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kqq.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dtc.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ala.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kim.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rff.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://izq.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uux.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kdi.guowangkeji.top

================================================================================
来源：http://ldv.nanxuanxn.top

O. 并发与异步
来源：http://ilt.jlsjyb.cn

================================================================================
来源：http://pcq.xinyue.icu

[O01] 启动一个线程
来源：http://mwe.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nzy.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cey.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hlw.yuanzhike.top

TS:   // 同 JS
来源：http://nvs.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://xkl.cashguo.top

Go:   go f()
来源：http://ylv.c1oappe.top

Ruby: Thread.new { f }
来源：http://jvq.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://pqe.birdmap.top

[O02] 使用线程池
来源：http://itm.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ddo.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jms.ydzc1.top

JS:   // worker_threads 线程池
来源：http://vkg.yueranfly.top

TS:   // worker_threads 线程池
来源：http://nwq.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://dki.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wnq.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zgz.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nvz.ivvv.top

[O03] 加锁保护共享数据
来源：http://jxf.zhixingplan.top

Py:   with lock: shared += 1
来源：http://pqx.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://slq.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cxr.yonumen.top

TS:   // 同 JS
来源：http://qpa.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://dfx.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sip.daxiang520.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tgc.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://dhn.xylfe.cn

[O04] 定义异步函数并等待
来源：http://pjd.yongpay.top

Py:   async def f():⏎    await g()
来源：http://ing.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tzb.hammf.cn

JS:   async function f() { await g(); }
来源：http://rcr.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lzg.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fpt.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ghr.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vaw.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://xbw.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://gde.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://mnf.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://svc.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://xyx.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://qbc.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bxc.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bdo.fehbvm.com

Ruby: threads.map(&:join)
来源：http://jcq.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ehs.chenzaomai.com

[O06] 使用进程池
来源：http://peh.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rjt.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mxr.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://law.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://asm.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbn.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ebu.nanxinkj.top

Ruby: // fork 块
来源：http://sgd.zhengqikj.top

C#:   Parallel.For
来源：http://xgv.yuxming.cn

================================================================================
来源：http://hey.uphjek.com

P. 常用工具函数
来源：http://cvd.zhijiandao.cn

================================================================================
来源：http://oid.tarul.cn

[P01] 生成 UUID
来源：http://prr.yj202588.top

Py:   str(uuid.uuid4())
来源：http://mmz.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cnv.gzhubu.top

JS:   crypto.randomUUID()
来源：http://jcv.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://cmh.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://kxp.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://jqh.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://drd.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://pao.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://qch.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sbu.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qmj.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vxy.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://usv.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dsy.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lhz.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pxk.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xqt.daxiang520.top

[P03] 生成短随机字符串
来源：http://ryv.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rui.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vot.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cdc.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qbm.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pnt.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zyx.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uhn.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gun.feifeiyinyue.top

[P04] 求长度
来源：http://ddo.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wgv.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://flu.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rii.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cbx.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://xyr.hnqzz.top

Go:   len(arr);  len(m)
来源：http://xfq.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://sbq.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dkt.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://yyq.jianghu66.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bft.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ewr.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jhs.pengpengdd.cyou

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://klt.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ale.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://zih.shanyushiyangtech.top

Ruby: a == b
来源：http://jal.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://joi.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://umr.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ltx.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://xme.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yim.nanxuanxn.top

TS:   if (x == null) {}
来源：http://txe.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lgx.vehdjk.com

Go:   if x == nil {}
来源：http://bmb.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yxt.zhongyouzk.top

C#:   if (x is null) {}
来源：http://tqc.yueranfly.top

[P07] 防抖与节流
来源：http://tjf.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gbj.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://myo.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgu.xuetiantiany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhl.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qvp.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wmy.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mah.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kjr.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://oth.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pxq.nwbrower.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://okr.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://usn.tarul.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://smx.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gqn.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ojf.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ugy.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eyr.shanyushiyangtech.top

================================================================================
来源：http://uun.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xqg.dianchejie.cn

================================================================================
来源：http://duw.epnwcf.com

[Q01] 创建表
来源：http://ssc.nanxuanxn.top

CREATE TABLE users (
来源：http://jxw.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ykl.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://msf.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://moe.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wnx.jinyuanbaomall.cn

);
来源：http://rmh.zhixingplan.top

[Q02] 创建带外键的表
来源：http://nnx.yuxming.cn

CREATE TABLE orders (
来源：http://pbj.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://njd.daria6918.cn

user_id INT NOT NULL,
来源：http://sfw.sysykeji.top

amount DECIMAL(10, 2),
来源：http://nlk.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tvl.hysaishi.cn

);
来源：http://ugn.shuidangran.top

[Q03] 增加列
来源：http://piz.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gav.tianlin.xyz

[Q04] 修改列类型
来源：http://taw.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://daw.uphjek.com

[Q05] 重命名列
来源：http://yzr.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aky.zhijiandao.cn

[Q06] 删除列
来源：http://rhx.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qlr.tarul.cn

[Q07] 删除表
来源：http://ntf.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://jud.hnxiangtu.top

[Q08] 创建普通索引
来源：http://jee.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jbi.daria6918.cn

[Q09] 创建唯一索引
来源：http://soh.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uci.vqdsnc.cn

[Q10] 插入单行
来源：http://bis.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xnl.yfazqb.com

[Q11] 一次插入多行
来源：http://jae.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ggl.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://yfi.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nmf.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qvd.yj20258.top

[Q13] 忽略重复插入
来源：http://amm.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tnk.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://ydh.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cjx.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gze.gotoacloud.top

[Q15] 查询全部
来源：http://ptm.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://voj.tianlin.xyz

[Q16] 查询指定列
来源：http://fbn.hammf.cn

SELECT id, name FROM users;
来源：http://mry.tian-w.cn

[Q17] 条件查询
来源：http://fei.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ula.vehdjk.com

[Q18] 模糊匹配
来源：http://hmj.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mdp.hcnkem.com

[Q19] 范围查询
来源：http://hhw.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jxd.shangyingyoupin.top

[Q20] IN 列表
来源：http://wdg.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yok.vqdsnc.cn

[Q21] 空值判断
来源：http://bjk.yanxiufei.cn


<!-- 参考信息 -->