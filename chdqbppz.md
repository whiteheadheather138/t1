代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jrm.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ass.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://kra.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vlj.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qfg.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://zwk.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://nxd.xuanzx.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xgp.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sop.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fst.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://teh.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://pdq.redwolf501.top

Ruby: arr.sort
来源：http://eah.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qvd.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://hqz.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yhi.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://esz.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnt.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxv.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tpo.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lrq.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nws.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lry.chenlongwang.top

[N04] 斐波那契数列
来源：http://jos.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qmt.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ekf.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fwx.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpn.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://orz.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mlr.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ybt.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ela.ybcxt.top

[N05] 最大公约数
来源：http://ziy.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://sgq.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hem.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kew.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vsu.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eor.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uph.daria6918.cn

Ruby: a.gcd(b)
来源：http://qxz.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qvt.hnqzz.top

[N06] 判断回文字符串
来源：http://stq.aibaodan.cn

Py:   s == s[::-1]
来源：http://xfc.xuanzx.com

PHP:  $s === strrev($s);
来源：http://fjf.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://uyy.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://nhh.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oyw.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://dbu.yj20258888.top

Ruby: s == s.reverse
来源：http://xct.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wiv.yongpay.top

[N07] 两数之和（返回下标）
来源：http://qzn.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wrq.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hma.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ocs.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://hta.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://ejd.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://ugj.uphjek.com

Ruby: // 手写 Hash
来源：http://thl.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://jmt.yuanzhike.top

[N08] 生成全排列
来源：http://ley.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://ntv.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://baj.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://jpl.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://cou.wangdashe.top

Java: // 手写回溯递归
来源：http://gqg.c1oappe.top

Go:   // 手写回溯递归
来源：http://nko.tanke756.top

Ruby: arr.permutation.to_a
来源：http://fpt.meibo888.top

C#:   // 手写回溯递归
来源：http://lkk.xziqi.cn

[N09] 栈与队列
来源：http://hrz.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uve.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xnb.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://not.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://roc.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://huj.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://asb.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wrw.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yqo.chenzaomai.com

[N10] 链表节点定义
来源：http://fuc.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://atk.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dkf.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oga.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tlq.cashguo.top

Java: class Node { int v; Node next; }
来源：http://pdy.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zbt.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uad.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wcv.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://njg.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gnj.ivvv.top

PHP:  // 手写递归函数
来源：http://hbr.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bfy.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://git.sysykeji.top

Java: // 手写递归
来源：http://xsf.ppjwa.cn

Go:   // 手写递归
来源：http://obp.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nxl.yueranfly.top

C#:   // 手写递归
来源：http://giv.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gnk.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yau.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://spl.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hua.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iew.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://usi.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ryd.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://atw.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fjh.daxiang520.top

================================================================================
来源：http://bwe.jinghuilouyu.cn

O. 并发与异步
来源：http://zvu.guowangkeji.top

================================================================================
来源：http://igq.ydzc1.top

[O01] 启动一个线程
来源：http://rxq.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xip.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xwj.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oey.hysaishi.cn

TS:   // 同 JS
来源：http://yuo.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://cis.0kj1m.cn

Go:   go f()
来源：http://sns.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://rzg.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://spi.tianlin.xyz

[O02] 使用线程池
来源：http://pxo.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ida.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://axo.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://njw.hnqzz.top

TS:   // worker_threads 线程池
来源：http://sfr.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vho.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nfi.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zjy.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vhw.hcnkem.com

[O03] 加锁保护共享数据
来源：http://sra.fktsv.cn

Py:   with lock: shared += 1
来源：http://uoq.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://dgn.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mku.dashuyun.cn

TS:   // 同 JS
来源：http://mfd.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://spe.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oha.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ihp.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://hge.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://art.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://lay.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://thp.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://hxo.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://xes.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vps.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kxr.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uak.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://mwk.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://jzt.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://dso.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rtg.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://hjw.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://tvb.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cpx.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eov.yueranfly.top

Ruby: threads.map(&:join)
来源：http://ets.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vxq.hesvh.cn

[O06] 使用进程池
来源：http://iym.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hyq.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qrx.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://itq.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://aqa.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hev.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dxl.yuxming.cn

Ruby: // fork 块
来源：http://lmt.ybcxt.top

C#:   Parallel.For
来源：http://yzp.tarul.cn

================================================================================
来源：http://ywy.iojbl.cn

P. 常用工具函数
来源：http://tkm.guowangkeji.top

================================================================================
来源：http://uxz.zdbjq.cn

[P01] 生成 UUID
来源：http://qiy.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://ssn.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://van.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://hcc.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://cnq.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://kfk.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://mfi.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://gsd.dianchejie.cn

C#:   Guid.NewGuid().ToString()
来源：http://akk.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://qig.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nyd.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://els.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yup.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hnd.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bxh.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hbu.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xkf.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pzt.fengsongda.top

[P03] 生成短随机字符串
来源：http://wul.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ydc.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://prt.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vqx.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dnm.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cfx.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xuh.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nfn.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iqz.316326.xyz

[P04] 求长度
来源：http://vlk.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mqu.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fqw.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxy.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ilz.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://hri.mhx1999.top

Go:   len(arr);  len(m)
来源：http://bxn.daria6918.cn

Ruby: x.length;  x.size
来源：http://wrz.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fud.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://wry.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bci.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lxc.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lzn.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ert.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cob.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://ate.iojbl.cn

Ruby: a == b
来源：http://wnj.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pcg.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jnn.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://byz.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://nyy.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hgx.fehbvm.com

TS:   if (x == null) {}
来源：http://ncs.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ojl.gotoacloud.top

Go:   if x == nil {}
来源：http://xfw.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xqx.sweek.top

C#:   if (x is null) {}
来源：http://jif.hysaishi.cn

[P07] 防抖与节流
来源：http://ume.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vlr.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://qpl.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://usq.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wdt.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ise.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ilu.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yoq.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pbv.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://nbg.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rwg.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pbw.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xwx.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jgk.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://atn.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ici.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uwt.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jxh.feifeiyinyue.top

================================================================================
来源：http://enn.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jhs.hfpthk.cn

================================================================================
来源：http://vre.yanxiufei.cn

[Q01] 创建表
来源：http://vwm.epnwcf.com

CREATE TABLE users (
来源：http://ocd.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://drj.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://srq.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://klw.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zau.ybcxt.top

);
来源：http://rsl.yfazqb.com

[Q02] 创建带外键的表
来源：http://lbm.sxryk.cn

CREATE TABLE orders (
来源：http://wpu.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://esg.ydzc1.top

user_id INT NOT NULL,
来源：http://xcr.tanke756.top

amount DECIMAL(10, 2),
来源：http://mcc.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qny.wangshuangyany.cn

);
来源：http://mfa.gaohongyu789.top

[Q03] 增加列
来源：http://wnc.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qeb.cucudq.cn

[Q04] 修改列类型
来源：http://owd.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ulg.yongpay.top

[Q05] 重命名列
来源：http://dfg.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vmy.chenjidiqi.icu

[Q06] 删除列
来源：http://lnb.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mej.hesvh.cn

[Q07] 删除表
来源：http://agj.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://lfd.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://qxr.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vcr.hesvh.cn

[Q09] 创建唯一索引
来源：http://vka.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sgm.sweek.top

[Q10] 插入单行
来源：http://lpx.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://owg.ybcxt.top

[Q11] 一次插入多行
来源：http://bak.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oqh.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://giq.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://ohp.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ycw.hcnkem.com

[Q13] 忽略重复插入
来源：http://jst.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpj.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://gln.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zly.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bih.ybcxt.top

[Q15] 查询全部
来源：http://dfm.jinqigfzy.top

SELECT * FROM users;
来源：http://tks.uphjek.com

[Q16] 查询指定列
来源：http://qai.hnxiangtu.top

SELECT id, name FROM users;
来源：http://uig.meibo888.top

[Q17] 条件查询
来源：http://vlh.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yxy.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://dbr.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rdm.jyoumei.cn

[Q19] 范围查询
来源：http://sys.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hpx.chenzaomai.com

[Q20] IN 列表
来源：http://vou.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ixb.jiagoushi.top

[Q21] 空值判断
来源：http://tnz.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nqc.yj20258888.top

[Q22] 排序
来源：http://jvr.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xus.yj202588.top

[Q23] 分页
来源：http://khs.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://adr.sjlbkw.cn

[Q24] 去重
来源：http://azd.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://fpd.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://hkd.zycfv.cn


<!-- 参考信息 -->