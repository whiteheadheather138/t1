代发 wailian999

TS:   process.platform;  process.version
来源：http://bsq.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hrk.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ewi.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ywp.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nfx.xylfe.cn

================================================================================
来源：http://aup.tanke756.top

N. 数据结构与算法
来源：http://tbh.cashguo.top

================================================================================
来源：http://rsv.uphjek.com

[N01] 二分查找（有序数组）
来源：http://oee.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://sck.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lvr.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ori.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wna.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hhm.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://kyo.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dxu.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://yfo.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://nfq.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://mzs.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xni.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tph.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://svg.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cha.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://uwa.yonumen.top

Ruby: arr.sort
来源：http://sqq.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lct.sweek.top

[N03] 快速排序（分治示例）
来源：http://rzv.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ddm.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://bya.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdm.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pio.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lni.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mog.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://udi.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://bev.mhx1999.top

[N04] 斐波那契数列
来源：http://bdz.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iec.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rhn.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymr.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjq.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qoa.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://axj.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://agq.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jhc.hywenlv.cn

[N05] 最大公约数
来源：http://rmy.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://rjf.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fjs.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nju.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfc.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dbt.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dqv.gogol.net.cn

Ruby: a.gcd(b)
来源：http://khz.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xiv.vqdsnc.cn

[N06] 判断回文字符串
来源：http://yiz.daria6918.cn

Py:   s == s[::-1]
来源：http://edv.cucudq.cn

PHP:  $s === strrev($s);
来源：http://adb.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://mka.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://mgp.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rfm.ybcxt.top

Go:   // 双指针从两端比较
来源：http://phn.zhixingplan.top

Ruby: s == s.reverse
来源：http://yif.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nia.smart0.xyz

[N07] 两数之和（返回下标）
来源：http://cai.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ijo.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://usg.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://auo.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://imx.aizwys.cn

Java: // 手写 HashMap
来源：http://bzs.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://trp.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://xvc.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://wul.nanxuanxn.top

[N08] 生成全排列
来源：http://kox.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://pkk.yuxming.cn

PHP:  // 手写递归交换
来源：http://mdn.cdnleiting.top

JS:   // 手写回溯递归
来源：http://mah.yuxming.cn

TS:   // 手写回溯递归
来源：http://sjb.fzhhl.top

Java: // 手写回溯递归
来源：http://gwk.ivvv.top

Go:   // 手写回溯递归
来源：http://gec.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://krw.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://rva.snrcjt.cn

[N09] 栈与队列
来源：http://ttb.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lrg.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hwt.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pxq.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bbx.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://drv.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oqd.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://isa.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hlu.jyoumei.cn

[N10] 链表节点定义
来源：http://vyz.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kaw.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ocd.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mqf.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sxk.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://brp.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://aqd.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qmx.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://jcp.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://fys.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cyl.uphjek.com

PHP:  // 手写递归函数
来源：http://qwi.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lnb.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xob.gzhubu.top

Java: // 手写递归
来源：http://fas.jinqigufen.top

Go:   // 手写递归
来源：http://vsh.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lha.yj20258888.top

C#:   // 手写递归
来源：http://pvp.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yqg.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ohv.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qfl.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjv.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vxa.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ryd.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wtn.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ywh.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ksp.birdmap.top

================================================================================
来源：http://nio.jinyuanbaomall.cn

O. 并发与异步
来源：http://ayk.meibo888.top

================================================================================
来源：http://qkq.zycfv.cn

[O01] 启动一个线程
来源：http://muc.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lwe.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tay.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://veo.zycfv.cn

TS:   // 同 JS
来源：http://lda.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://hzn.sxryk.cn

Go:   go f()
来源：http://vfi.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://knt.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://laj.xinyue.icu

[O02] 使用线程池
来源：http://rek.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ckp.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hrp.aizwys.cn

JS:   // worker_threads 线程池
来源：http://gmd.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://szm.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mza.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cuo.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qai.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mkc.cheryme.top

[O03] 加锁保护共享数据
来源：http://psz.sweek.top

Py:   with lock: shared += 1
来源：http://ajp.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://sxe.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://csv.daxiang520.top

TS:   // 同 JS
来源：http://wta.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://amo.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pwf.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ppj.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://sdm.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://qsj.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://rii.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drm.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://ujc.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dkt.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lye.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cqh.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fgd.cheryme.top

C#:   async Task F() { await G(); }
来源：http://pnz.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://fwz.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://mhi.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fmv.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://och.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://eba.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yzr.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dea.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://ffs.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://lld.dashuyun.cn

[O06] 使用进程池
来源：http://pwh.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lkp.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wti.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://fcy.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://rsg.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xrv.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hbu.jlsjyb.cn

Ruby: // fork 块
来源：http://qcl.guowangkeji.top

C#:   Parallel.For
来源：http://srt.nanxuanxn.top

================================================================================
来源：http://anl.shangyingyoupin.top

P. 常用工具函数
来源：http://teb.zdbjq.cn

================================================================================
来源：http://xtr.dashuyun.cn

[P01] 生成 UUID
来源：http://xdb.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://wrp.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wca.yj202588.top

JS:   crypto.randomUUID()
来源：http://kej.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://drr.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://qud.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://jkc.yj202588.top

Ruby: SecureRandom.uuid
来源：http://eob.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://eyo.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://war.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vrs.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zfq.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mml.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://khy.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bgc.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pjy.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tln.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ctn.daxiang520.top

[P03] 生成短随机字符串
来源：http://lng.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ddz.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vda.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://afp.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ncg.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rpo.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vup.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pya.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://roc.jianghu66.top

[P04] 求长度
来源：http://ley.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tjw.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aai.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mrr.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://enb.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://iag.iojbl.cn

Go:   len(arr);  len(m)
来源：http://ndc.fehbvm.com

Ruby: x.length;  x.size
来源：http://kqe.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://asi.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://xnk.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fbh.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://orc.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hbc.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://anx.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xlr.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://ttp.xinyue.icu

Ruby: a == b
来源：http://ynj.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ita.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yhx.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kmy.meibo888.top

PHP:  if (empty($x)) {}
来源：http://djb.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ali.zhengqikj.top

TS:   if (x == null) {}
来源：http://hdm.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://udl.xylfe.cn

Go:   if x == nil {}
来源：http://bth.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cyw.ctjpmb.com

C#:   if (x is null) {}
来源：http://yfm.fehbvm.com

[P07] 防抖与节流
来源：http://bca.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ill.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://gkm.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gzb.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gho.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hfn.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pqi.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mll.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fvi.fktsv.cn

[P08] 处理浮点精度问题
来源：http://bkj.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oub.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xfi.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zgd.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ann.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sws.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qat.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://umn.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cux.xuanzx.com

================================================================================
来源：http://rwm.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ote.jinghuilouyu.cn

================================================================================
来源：http://dwp.hysaishi.cn

[Q01] 创建表
来源：http://out.yfazqb.com

CREATE TABLE users (
来源：http://yol.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ztw.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://nrr.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://zaq.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvg.chenlongwang.top

);
来源：http://ctt.jiagoushi.top

[Q02] 创建带外键的表
来源：http://ija.sysykeji.top

CREATE TABLE orders (
来源：http://ioo.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yxd.9152youxi.cn

user_id INT NOT NULL,
来源：http://uyl.andypj.xyz

amount DECIMAL(10, 2),
来源：http://dxy.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dir.mhx1999.top

);
来源：http://mrn.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://hsl.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mqb.nanxuanxn.top

[Q04] 修改列类型
来源：http://dyp.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://swp.yj202588.top

[Q05] 重命名列
来源：http://bzf.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://idm.pengpengdd.cyou

[Q06] 删除列
来源：http://awk.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://yej.xuanzx.com

[Q07] 删除表
来源：http://cpl.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://rlz.yfazqb.com

[Q08] 创建普通索引
来源：http://uys.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rgq.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://rzr.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://awb.pengpengdd.cyou

[Q10] 插入单行
来源：http://opx.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rvp.zhoulong.xyz

[Q11] 一次插入多行
来源：http://wgt.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zsl.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://tvf.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://irc.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qav.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://szm.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://klq.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://rjj.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hei.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mvf.yj20258.top

[Q15] 查询全部
来源：http://rlm.hywenlv.cn

SELECT * FROM users;
来源：http://fdl.ivvv.top

[Q16] 查询指定列
来源：http://hqw.hcnkem.com

SELECT id, name FROM users;
来源：http://xit.yongpay.top

[Q17] 条件查询
来源：http://qbz.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://syw.sjlbkw.cn

[Q18] 模糊匹配
来源：http://dzl.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sbs.xinyue.icu

[Q19] 范围查询
来源：http://kkf.zhijiandao.cn


<!-- 参考信息 -->