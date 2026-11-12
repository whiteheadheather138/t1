代发 wailian999

[N01] 二分查找（有序数组）
来源：http://otk.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://esd.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uzz.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mas.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksj.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://meu.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://ncx.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jlg.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://hxf.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://zlp.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://ztg.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aet.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rfd.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://lzm.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bku.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://bzb.tian-w.cn

Ruby: arr.sort
来源：http://sgf.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nex.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://okq.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zxv.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://zuo.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://flh.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vvf.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://skk.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oea.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zth.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://emg.zhixingplan.top

[N04] 斐波那契数列
来源：http://wcx.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ztk.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uqf.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qhq.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xet.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tgf.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sfo.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ebd.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fbg.snrcjt.cn

[N05] 最大公约数
来源：http://ycu.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://thm.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mhs.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpe.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggu.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mkg.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bpo.shuidangran.top

Ruby: a.gcd(b)
来源：http://mbv.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dcj.yj20258888.top

[N06] 判断回文字符串
来源：http://sfe.gzhubu.top

Py:   s == s[::-1]
来源：http://ktq.52xcode.cn

PHP:  $s === strrev($s);
来源：http://vbr.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://eok.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://imy.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pfb.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://mke.smart0.xyz

Ruby: s == s.reverse
来源：http://vzz.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pan.ivvv.top

[N07] 两数之和（返回下标）
来源：http://zcl.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nzf.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zeb.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wjw.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://nmf.jinqigufen.top

Java: // 手写 HashMap
来源：http://ela.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://hcy.cdnleiting.top

Ruby: // 手写 Hash
来源：http://ipf.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://tbi.gogol.net.cn

[N08] 生成全排列
来源：http://xtc.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://nuc.iojbl.cn

PHP:  // 手写递归交换
来源：http://qss.bbcook.cn

JS:   // 手写回溯递归
来源：http://zvw.sufxvd.cn

TS:   // 手写回溯递归
来源：http://rzp.jlsjyb.cn

Java: // 手写回溯递归
来源：http://xtf.ivvv.top

Go:   // 手写回溯递归
来源：http://bbi.tanke756.top

Ruby: arr.permutation.to_a
来源：http://tye.fktsv.cn

C#:   // 手写回溯递归
来源：http://yxw.shangyingyoupin.top

[N09] 栈与队列
来源：http://dir.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://usb.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://swe.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://txn.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://szt.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aqs.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ocu.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ibh.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://avj.cashguo.top

[N10] 链表节点定义
来源：http://jal.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iyn.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lhn.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pam.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vtb.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://rmp.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://wdu.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dme.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oyz.pycfn.com

[N11] 二叉树中序遍历
来源：http://zvr.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://osf.tarul.cn

PHP:  // 手写递归函数
来源：http://rao.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dlc.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zmq.iojbl.cn

Java: // 手写递归
来源：http://tut.sufxvd.cn

Go:   // 手写递归
来源：http://tba.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kyw.zhixingplan.top

C#:   // 手写递归
来源：http://ntg.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sqx.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wwf.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dvn.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://win.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sjq.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mzv.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lda.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fkl.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgb.fengsongda.top

================================================================================
来源：http://udd.ctjpmb.com

O. 并发与异步
来源：http://vrv.smart0.xyz

================================================================================
来源：http://cve.fehbvm.com

[O01] 启动一个线程
来源：http://ost.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zxb.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://emq.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kfc.shanyushiyangtech.top

TS:   // 同 JS
来源：http://uyw.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://huk.tarul.cn

Go:   go f()
来源：http://uno.redwolf501.top

Ruby: Thread.new { f }
来源：http://rhi.cashguo.top

C#:   Task.Run(() => F());
来源：http://rct.svipenyu.cn

[O02] 使用线程池
来源：http://ykg.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://acs.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rqm.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://qbu.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://vww.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://knw.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qqx.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jnh.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://apu.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://lbj.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://zrp.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://hdd.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://evk.zdqjudy.top

TS:   // 同 JS
来源：http://rgz.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://yay.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gse.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://etp.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://fjv.guannengcc.top

[O04] 定义异步函数并等待
来源：http://tob.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://dmy.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://edv.nwbrower.top

JS:   async function f() { await g(); }
来源：http://wwa.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://iaj.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rer.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zlc.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://htj.sweek.top

C#:   async Task F() { await G(); }
来源：http://unz.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://mqv.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://vgp.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yzn.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://noc.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://uyl.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://are.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jvi.sysykeji.top

Ruby: threads.map(&:join)
来源：http://esd.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wmt.zdbjq.cn

[O06] 使用进程池
来源：http://did.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bfz.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://gvz.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://iqw.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://pwc.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://azx.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mez.chenzaomai.com

Ruby: // fork 块
来源：http://bjn.316326.xyz

C#:   Parallel.For
来源：http://bbb.tian-w.cn

================================================================================
来源：http://jyz.snrcjt.cn

P. 常用工具函数
来源：http://xjd.sjlbkw.cn

================================================================================
来源：http://bst.vqdsnc.cn

[P01] 生成 UUID
来源：http://umx.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://vpx.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ues.jianghu66.top

JS:   crypto.randomUUID()
来源：http://dzi.shuidangran.top

TS:   crypto.randomUUID()
来源：http://ozd.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://wzw.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://csw.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://xxz.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://zfr.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://sok.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mrx.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xjd.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jvv.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bgj.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hli.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://siz.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ssn.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ysc.nanxinkj.top

[P03] 生成短随机字符串
来源：http://qhl.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://amt.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zbm.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nbf.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hze.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mkf.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oop.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cku.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kka.jinqigfzy.top

[P04] 求长度
来源：http://lxk.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mxh.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kst.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mlg.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cee.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://jxu.tanke756.top

Go:   len(arr);  len(m)
来源：http://gvo.sxryk.cn

Ruby: x.length;  x.size
来源：http://lzd.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rxs.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://mmy.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://boi.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mmo.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xwv.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eck.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://coo.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dqv.epnwcf.com

Ruby: a == b
来源：http://zia.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ytc.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vbr.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://php.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://xcd.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rme.hammf.cn

TS:   if (x == null) {}
来源：http://avy.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://smc.c1oappe.top

Go:   if x == nil {}
来源：http://teg.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hwk.zhixingplan.top

C#:   if (x is null) {}
来源：http://xdp.ctjpmb.com

[P07] 防抖与节流
来源：http://tgu.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://orb.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://kfc.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwg.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqg.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://txq.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kxg.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bkw.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hwz.yj20258888.top

[P08] 处理浮点精度问题
来源：http://nyv.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mvn.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zto.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pyj.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://csp.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ukx.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bvi.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uag.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dii.aibaodan.cn

================================================================================
来源：http://pjt.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dwj.ehwqpu.com

================================================================================
来源：http://hxt.shuidangran.top

[Q01] 创建表
来源：http://hri.shuidangran.top

CREATE TABLE users (
来源：http://iyo.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://clz.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://aep.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://xzx.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bzz.hnxiangtu.top

);
来源：http://ehm.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://jgq.shangyingyoupin.top

CREATE TABLE orders (
来源：http://nmn.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://brn.0kj1m.cn

user_id INT NOT NULL,
来源：http://urn.birdmap.top

amount DECIMAL(10, 2),
来源：http://hsg.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nex.sysykeji.top

);
来源：http://wdw.guowangkeji.top

[Q03] 增加列
来源：http://nlm.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mkm.yongpay.top

[Q04] 修改列类型
来源：http://flv.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://twq.nwbrower.top

[Q05] 重命名列
来源：http://pqq.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dia.cucudq.cn

[Q06] 删除列
来源：http://lpa.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://jvt.vqdsnc.cn

[Q07] 删除表
来源：http://uye.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://itl.ehwqpu.com

[Q08] 创建普通索引
来源：http://sdh.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wdl.wangshuangyany.cn

[Q09] 创建唯一索引
来源：http://bcq.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yij.iojbl.cn

[Q10] 插入单行
来源：http://mta.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vzv.hcnkem.com

[Q11] 一次插入多行
来源：http://djz.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uti.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://kei.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dnw.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ltk.nanxinkj.top

[Q13] 忽略重复插入
来源：http://nug.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nme.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://stp.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ixs.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wkx.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://oqt.fktsv.cn

SELECT * FROM users;
来源：http://jha.cheryme.top

[Q16] 查询指定列
来源：http://tbf.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://orq.cucudq.cn

[Q17] 条件查询
来源：http://ilm.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oyq.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://eek.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ncc.ivvv.top

[Q19] 范围查询
来源：http://nnu.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hib.aibaodan.cn

[Q20] IN 列表
来源：http://lrx.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vfb.pengpengdd.cyou

[Q21] 空值判断
来源：http://kqf.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tes.mhx1999.top

[Q22] 排序
来源：http://mdz.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kts.sxryk.cn

[Q23] 分页
来源：http://jdi.pengpengdd.cyou


<!-- 参考信息 -->