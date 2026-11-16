代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hgw.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nzg.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://ovp.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lqe.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://cpx.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://lud.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://tyj.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cho.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jfg.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://joc.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sct.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://hvl.hywenlv.cn

Ruby: arr.sort
来源：http://gyr.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zcd.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://skq.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fjl.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://gsr.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pav.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqz.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ytk.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kmo.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ajc.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://hrp.sweek.top

[N04] 斐波那契数列
来源：http://jbt.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tgr.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yye.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jks.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hcz.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qnl.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pjw.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kzz.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sxv.guowangkeji.top

[N05] 最大公约数
来源：http://bfl.316326.xyz

Py:   math.gcd(a, b)
来源：http://pji.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aec.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zue.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vsm.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rte.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ail.ivvv.top

Ruby: a.gcd(b)
来源：http://rcn.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oax.zycfv.cn

[N06] 判断回文字符串
来源：http://ojq.havefunace.top

Py:   s == s[::-1]
来源：http://bjh.wangdashe.top

PHP:  $s === strrev($s);
来源：http://kfl.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://xuk.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://ibf.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rnj.fzhhl.top

Go:   // 双指针从两端比较
来源：http://wnz.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://hjf.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dhw.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://ifn.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ofw.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zxs.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qnl.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://ewd.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://mxk.cashguo.top

Go:   // 手写 map[int]int
来源：http://ahq.xinyue.icu

Ruby: // 手写 Hash
来源：http://btg.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://ara.jiagoushi.top

[N08] 生成全排列
来源：http://vcc.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://eui.xziqi.cn

PHP:  // 手写递归交换
来源：http://upo.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://utr.hysaishi.cn

TS:   // 手写回溯递归
来源：http://yiv.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://tfu.hywenlv.cn

Go:   // 手写回溯递归
来源：http://jcg.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://ypb.tian-w.cn

C#:   // 手写回溯递归
来源：http://kds.ivvv.top

[N09] 栈与队列
来源：http://ipb.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ory.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pwq.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zcw.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lrv.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://igy.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nor.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xnc.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xcy.jinqigufen.top

[N10] 链表节点定义
来源：http://vkp.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://isr.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://fcz.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xzu.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afz.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://tdj.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://vzm.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jur.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dri.gzhubu.top

[N11] 二叉树中序遍历
来源：http://zby.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tdu.yueranfly.top

PHP:  // 手写递归函数
来源：http://rev.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lsk.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://evg.cqqwz.cn

Java: // 手写递归
来源：http://chz.pengpengdd.cyou

Go:   // 手写递归
来源：http://ovb.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xzh.iojbl.cn

C#:   // 手写递归
来源：http://phq.kuanghao11.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://euu.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://keg.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ndp.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wov.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wur.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kkr.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gxd.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://myo.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://unj.yongpay.top

================================================================================
来源：http://xwu.pycfn.com

O. 并发与异步
来源：http://foy.quarkkingdee.top

================================================================================
来源：http://xci.chenjidiqi.icu

[O01] 启动一个线程
来源：http://ouh.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://khw.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mrl.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qor.wangdashe.top

TS:   // 同 JS
来源：http://knl.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://nku.hnqzz.top

Go:   go f()
来源：http://det.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://trw.vehdjk.com

C#:   Task.Run(() => F());
来源：http://bwz.hfpthk.cn

[O02] 使用线程池
来源：http://aum.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lly.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oti.pycfn.com

JS:   // worker_threads 线程池
来源：http://ujy.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://fqg.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://vhx.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fcy.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kxk.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xit.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://yfb.mhx1999.top

Py:   with lock: shared += 1
来源：http://qjr.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://nhi.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mid.wangdashe.top

TS:   // 同 JS
来源：http://azt.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://enl.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rdg.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://isv.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://btq.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://hrq.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://iru.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tuf.bjfxy.top

JS:   async function f() { await g(); }
来源：http://jop.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ykg.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bkl.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wig.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://leg.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://ort.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://awp.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://usu.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://agi.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://prn.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://owb.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbe.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zor.yj20258888.top

Ruby: threads.map(&:join)
来源：http://doc.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xam.yongpay.top

[O06] 使用进程池
来源：http://sja.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wbi.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mgo.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://fnk.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://zde.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bba.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://htg.fktsv.cn

Ruby: // fork 块
来源：http://ach.pengpengdd.cyou

C#:   Parallel.For
来源：http://vdz.epnwcf.com

================================================================================
来源：http://jlq.svipenyu.cn

P. 常用工具函数
来源：http://zbz.0kj1m.cn

================================================================================
来源：http://jdh.yj202588.top

[P01] 生成 UUID
来源：http://epy.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://npa.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kds.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://tzm.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://apb.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://sly.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://htv.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://xtr.nanxinkj.top

C#:   Guid.NewGuid().ToString()
来源：http://nnx.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://kjq.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hnv.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hjz.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gut.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lon.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wim.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ebc.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tvc.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wfh.haohaochexian.top

[P03] 生成短随机字符串
来源：http://gvb.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bqf.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rqr.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yto.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ogd.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pgo.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qvi.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://tdw.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://enb.sufxvd.cn

[P04] 求长度
来源：http://wyh.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://puy.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://unp.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gor.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kdg.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://diy.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://uhy.bjfxy.top

Ruby: x.length;  x.size
来源：http://czn.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tzl.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://qbc.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://cip.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pqn.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ihs.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iop.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zvu.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gso.iojbl.cn

Ruby: a == b
来源：http://vsy.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zdi.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rvp.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mkh.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://mcw.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wvk.9152youxi.cn

TS:   if (x == null) {}
来源：http://jsg.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://duh.vehdjk.com

Go:   if x == nil {}
来源：http://bas.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dgo.hammf.cn

C#:   if (x is null) {}
来源：http://bpx.yvedp.cn

[P07] 防抖与节流
来源：http://law.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wix.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://txd.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zko.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ial.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://czs.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dwy.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://eif.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cdy.ybcxt.top

[P08] 处理浮点精度问题
来源：http://khn.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dbn.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jbq.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jtd.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nki.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dav.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kzc.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rmr.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blp.cqqwz.cn

================================================================================
来源：http://acp.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dcz.zhaomingkeji.xyz

================================================================================
来源：http://jyu.aizwys.cn

[Q01] 创建表
来源：http://ill.yangfankeji.com

CREATE TABLE users (
来源：http://dky.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gna.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://fck.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://sbd.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cjm.jianghu66.top

);
来源：http://cfi.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://pnt.jlsjyb.cn

CREATE TABLE orders (
来源：http://nvl.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mze.iojbl.cn

user_id INT NOT NULL,
来源：http://nif.sysykeji.top

amount DECIMAL(10, 2),
来源：http://nax.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ohv.jiagoushi.top

);
来源：http://ohs.yangfankeji.com

[Q03] 增加列
来源：http://cmu.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rox.yj202588.top

[Q04] 修改列类型
来源：http://mmt.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fsm.shzxlz.cn

[Q05] 重命名列
来源：http://jbq.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bwd.shzxlz.cn

[Q06] 删除列
来源：http://wmx.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://avz.pengpengdd.cyou

[Q07] 删除表
来源：http://ilc.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://uha.jqgfzy.top

[Q08] 创建普通索引
来源：http://ggu.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://neb.yfazqb.com

[Q09] 创建唯一索引
来源：http://kob.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dxv.hnqzz.top

[Q10] 插入单行
来源：http://sep.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zpy.hnqzz.top

[Q11] 一次插入多行
来源：http://skd.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gan.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://stp.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://nxq.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://izx.ivvv.top

[Q13] 忽略重复插入
来源：http://ccr.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gvi.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://rnk.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zdz.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tlq.yonumen.top

[Q15] 查询全部
来源：http://wqu.yj20258888.top

SELECT * FROM users;
来源：http://ofb.sxryk.cn

[Q16] 查询指定列
来源：http://nrg.pycfn.com

SELECT id, name FROM users;
来源：http://wqd.fehbvm.com

[Q17] 条件查询
来源：http://nru.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mlj.cucudq.cn

[Q18] 模糊匹配
来源：http://gos.zycfv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ves.hnqzz.top

[Q19] 范围查询
来源：http://qbn.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lgp.vqdsnc.cn

[Q20] IN 列表
来源：http://tge.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://byf.jlsjyb.cn

[Q21] 空值判断
来源：http://iaz.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://luz.yuxming.cn

[Q22] 排序
来源：http://hdi.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nvr.9152youxi.cn

[Q23] 分页
来源：http://ied.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dzo.ydzc1.top

[Q24] 去重
来源：http://hvi.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://lsg.havefunace.top

[Q25] 只取前 N 条
来源：http://lxk.chenlongwang.top


<!-- 参考信息 -->