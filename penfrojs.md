代发 wailian999

[M08] 获取系统与运行时信息
来源：http://pkd.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://qsi.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://tvd.hesvh.cn

JS:   process.platform;  process.version
来源：http://jda.ybcxt.top

TS:   process.platform;  process.version
来源：http://erg.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://czq.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tru.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uxv.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vuv.bbcook.cn

================================================================================
来源：http://yfq.daxiang520.top

N. 数据结构与算法
来源：http://nti.tian-w.cn

================================================================================
来源：http://jlz.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://qbq.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://zzz.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sps.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mcp.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xkx.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://hlo.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://dzi.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sez.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://krf.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://qiw.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://yrw.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mbt.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ypg.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://iow.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://exj.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://qmn.sxryk.cn

Ruby: arr.sort
来源：http://oxm.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rrp.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://qiq.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dsx.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://puv.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://orw.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xnf.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blc.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nyu.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vhs.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gxt.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://oya.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://exa.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cxw.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hxc.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hev.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vwq.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pjf.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zdb.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gem.jinqigfzy.top

[N05] 最大公约数
来源：http://qxw.aizwys.cn

Py:   math.gcd(a, b)
来源：http://peh.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xkt.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ljv.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://omb.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qzu.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dub.ybcxt.top

Ruby: a.gcd(b)
来源：http://mna.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fki.sufxvd.cn

[N06] 判断回文字符串
来源：http://hjc.sysykeji.top

Py:   s == s[::-1]
来源：http://pip.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://mbd.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://rrb.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://jzn.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dwn.hammf.cn

Go:   // 双指针从两端比较
来源：http://bxd.hysaishi.cn

Ruby: s == s.reverse
来源：http://xya.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kbv.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://imd.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tut.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://agt.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mbq.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://ncf.vehdjk.com

Java: // 手写 HashMap
来源：http://xug.chenjidiqi.icu

Go:   // 手写 map[int]int
来源：http://lev.chenlongwang.top

Ruby: // 手写 Hash
来源：http://jei.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ige.pycfn.com

[N08] 生成全排列
来源：http://mjr.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://kcv.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://lqe.yuanzhike.top

JS:   // 手写回溯递归
来源：http://kfn.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://jjk.fengsongda.top

Java: // 手写回溯递归
来源：http://twc.snrcjt.cn

Go:   // 手写回溯递归
来源：http://fvp.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://qvz.52xcode.cn

C#:   // 手写回溯递归
来源：http://bpq.zdqjudy.top

[N09] 栈与队列
来源：http://wnr.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qcc.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pzd.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wwr.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vco.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://icb.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cyw.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jpw.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hkf.jqgfzy.top

[N10] 链表节点定义
来源：http://omt.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fpd.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rnn.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hcd.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hrs.yvedp.cn

Java: class Node { int v; Node next; }
来源：http://uvt.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://ewe.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uyt.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rci.zycfv.cn

[N11] 二叉树中序遍历
来源：http://gas.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gan.jianghu66.top

PHP:  // 手写递归函数
来源：http://uja.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sza.hnqzz.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mob.ywan-chungtsiang.top

Java: // 手写递归
来源：http://fzs.shangyingyoupin.top

Go:   // 手写递归
来源：http://iic.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mua.shanyushiyangtech.top

C#:   // 手写递归
来源：http://jff.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cav.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yyk.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rmv.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfc.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pac.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pqi.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sug.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cjx.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iqg.jinqigufen.top

================================================================================
来源：http://dyj.xuetiantiany.cn

O. 并发与异步
来源：http://qtx.xuetiantiany.cn

================================================================================
来源：http://ype.guowangkeji.top

[O01] 启动一个线程
来源：http://qqb.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wcw.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://usa.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ztm.tianlin.xyz

TS:   // 同 JS
来源：http://lun.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://lvo.yonumen.top

Go:   go f()
来源：http://emn.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://spq.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://xlf.hywenlv.cn

[O02] 使用线程池
来源：http://twz.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sqt.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dph.52xcode.cn

JS:   // worker_threads 线程池
来源：http://otq.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://rfh.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://bea.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tpj.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mmd.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sme.iojbl.cn

[O03] 加锁保护共享数据
来源：http://vtx.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://gbi.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://hir.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://shy.dianchejie.cn

TS:   // 同 JS
来源：http://dfg.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://zmb.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tka.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndx.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://cvb.c1oappe.top

[O04] 定义异步函数并等待
来源：http://jpj.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://nxu.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qpn.andypj.xyz

JS:   async function f() { await g(); }
来源：http://xfs.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vba.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://koy.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yyc.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://zki.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://fmp.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://ifb.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://bsf.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://asm.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://zwq.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://hue.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wty.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndd.cashguo.top

Ruby: threads.map(&:join)
来源：http://uaw.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xfe.dianchejie.cn

[O06] 使用进程池
来源：http://cti.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aeg.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://rcq.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://eqp.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://lop.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lhj.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eaj.smart0.xyz

Ruby: // fork 块
来源：http://sym.yfazqb.com

C#:   Parallel.For
来源：http://nps.xinyue.icu

================================================================================
来源：http://vvz.gzhubu.top

P. 常用工具函数
来源：http://tzj.jlsjyb.cn

================================================================================
来源：http://quh.gotoacloud.top

[P01] 生成 UUID
来源：http://pke.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://ugk.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hkl.hammf.cn

JS:   crypto.randomUUID()
来源：http://tho.52xcode.cn

TS:   crypto.randomUUID()
来源：http://dbg.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://mba.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://xwg.daxiang520.top

Ruby: SecureRandom.uuid
来源：http://bti.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://lui.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://hro.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iba.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://iap.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pdc.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ymy.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://myk.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qxf.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nvt.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hpd.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://uus.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nlv.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xax.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rkf.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xgp.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mzn.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wib.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lgw.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zuu.feifeiyinyue.top

[P04] 求长度
来源：http://oae.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nfk.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mnz.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ivl.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ohf.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://avs.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://tli.uphjek.com

Ruby: x.length;  x.size
来源：http://hqo.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mph.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://prx.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://duo.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ikn.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://azh.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lyh.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://emp.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://bqc.ydzc1.top

Ruby: a == b
来源：http://hhn.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hku.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://itk.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ybd.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://bzq.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jws.svipenyu.cn

TS:   if (x == null) {}
来源：http://bby.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://opr.vqdsnc.cn

Go:   if x == nil {}
来源：http://psd.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zmz.zhijiandao.cn

C#:   if (x is null) {}
来源：http://hkz.iojbl.cn

[P07] 防抖与节流
来源：http://tnf.sufxvd.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jdg.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://glc.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpv.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgs.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hxe.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tir.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qrk.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mvy.yuxming.cn

[P08] 处理浮点精度问题
来源：http://kpc.cdnleiting.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vcv.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rty.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vrg.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://btx.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zrw.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wzx.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hqv.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jxj.yj20258.top

================================================================================
来源：http://wgo.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cxz.daria6918.cn

================================================================================
来源：http://dmk.guowangkeji.top

[Q01] 创建表
来源：http://ntp.pycfn.com

CREATE TABLE users (
来源：http://xek.hysaishi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qdj.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://pvu.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://bit.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://brj.yongpay.top

);
来源：http://asl.tanke756.top

[Q02] 创建带外键的表
来源：http://fac.fengsongda.top

CREATE TABLE orders (
来源：http://dmd.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qpn.sysykeji.top

user_id INT NOT NULL,
来源：http://zej.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://uwh.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cmh.fanxiaobao.xyz

);
来源：http://vma.aizwys.cn

[Q03] 增加列
来源：http://xgm.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cmp.kuanghao11.cn

[Q04] 修改列类型
来源：http://zqj.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sps.cdnleiting.top

[Q05] 重命名列
来源：http://mfo.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nvt.daxiang520.top

[Q06] 删除列
来源：http://wru.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://nkj.vehdjk.com

[Q07] 删除表
来源：http://ici.ivvv.top

DROP TABLE IF EXISTS orders;
来源：http://bol.zhengqikj.top

[Q08] 创建普通索引
来源：http://jdz.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://biy.yj20258.top

[Q09] 创建唯一索引
来源：http://mxv.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rmy.redwolf501.top

[Q10] 插入单行
来源：http://zdz.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qup.yvedp.cn

[Q11] 一次插入多行
来源：http://ywx.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hph.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://cew.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://ywq.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wzd.shzxlz.cn

[Q13] 忽略重复插入
来源：http://uaq.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yqm.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://bzh.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qba.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yez.nwbrower.top

[Q15] 查询全部
来源：http://tjl.ctjpmb.com

SELECT * FROM users;
来源：http://ggv.mhx1999.top

[Q16] 查询指定列
来源：http://pjv.wangdashe.top

SELECT id, name FROM users;
来源：http://xtr.mhx1999.top

[Q17] 条件查询
来源：http://igf.wangdashe.top


<!-- 参考信息 -->