代发 wailian999

TS:   process.platform;  process.version
来源：http://qcl.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://upq.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://osb.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qkv.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nmo.ehwqpu.com

================================================================================
来源：http://xqi.yfazqb.com

N. 数据结构与算法
来源：http://dvq.tian-w.cn

================================================================================
来源：http://fzm.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://wyb.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://aat.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vyg.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gve.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqf.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://aob.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://wvt.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://any.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://xbf.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://oag.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://uwc.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kaw.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cfh.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://itv.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dlu.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://ncn.xylfe.cn

Ruby: arr.sort
来源：http://shw.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pds.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://xmb.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sim.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://oqf.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gde.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://inw.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uka.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qno.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nqb.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lyh.yangfankeji.com

[N04] 斐波那契数列
来源：http://iev.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ecu.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uru.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdu.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tbz.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vbs.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dmk.bjfxy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lql.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpq.yonumen.top

[N05] 最大公约数
来源：http://ugu.andypj.xyz

Py:   math.gcd(a, b)
来源：http://jga.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uwx.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dri.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fbi.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bqo.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vmv.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://kji.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gde.ctjpmb.com

[N06] 判断回文字符串
来源：http://pkr.fehbvm.com

Py:   s == s[::-1]
来源：http://ixj.hnqzz.top

PHP:  $s === strrev($s);
来源：http://yzf.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://lmu.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://jet.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jrc.hcnkem.com

Go:   // 双指针从两端比较
来源：http://frg.nanxuanxn.top

Ruby: s == s.reverse
来源：http://bgy.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bru.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://amk.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zhq.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mdo.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://edz.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://bos.yonumen.top

Java: // 手写 HashMap
来源：http://yyf.daria6918.cn

Go:   // 手写 map[int]int
来源：http://jyh.fktsv.cn

Ruby: // 手写 Hash
来源：http://ldr.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://swq.vqdsnc.cn

[N08] 生成全排列
来源：http://lpt.uphjek.com

Py:   itertools.permutations(arr)
来源：http://isi.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://elq.svipenyu.cn

JS:   // 手写回溯递归
来源：http://wrg.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://lyj.cucudq.cn

Java: // 手写回溯递归
来源：http://kfg.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://prj.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://fxv.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://knb.chenjidiqi.icu

[N09] 栈与队列
来源：http://qum.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ido.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fdi.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gcz.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gyq.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://prq.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cjp.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xxh.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://npa.sxryk.cn

[N10] 链表节点定义
来源：http://wfy.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://urx.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://mdw.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://drq.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ran.hammf.cn

Java: class Node { int v; Node next; }
来源：http://hte.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://adp.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tan.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://epl.bbcook.cn

[N11] 二叉树中序遍历
来源：http://yxd.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tsp.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://abx.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eya.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hse.hysaishi.cn

Java: // 手写递归
来源：http://vxi.snrcjt.cn

Go:   // 手写递归
来源：http://kyi.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://obw.zycfv.cn

C#:   // 手写递归
来源：http://hvy.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lbh.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hyj.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tqz.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kmw.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbg.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vym.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pdw.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gee.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ram.gzhubu.top

================================================================================
来源：http://owl.zhijiandao.cn

O. 并发与异步
来源：http://gsk.nanxuanxn.top

================================================================================
来源：http://nfl.tarul.cn

[O01] 启动一个线程
来源：http://kov.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bag.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://csd.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jtg.cheryme.top

TS:   // 同 JS
来源：http://edi.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://xpl.chenjidiqi.icu

Go:   go f()
来源：http://mmb.daria6918.cn

Ruby: Thread.new { f }
来源：http://lbs.c1oappe.top

C#:   Task.Run(() => F());
来源：http://imb.zycfv.cn

[O02] 使用线程池
来源：http://xsa.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dke.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ebl.birdmap.top

JS:   // worker_threads 线程池
来源：http://gif.tian-w.cn

TS:   // worker_threads 线程池
来源：http://rfo.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://uyi.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nkb.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qwf.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uly.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://tca.xuanzx.com

Py:   with lock: shared += 1
来源：http://gkj.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://kqd.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mme.sufxvd.cn

TS:   // 同 JS
来源：http://fpf.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://ybp.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jrn.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rub.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://qal.316326.xyz

[O04] 定义异步函数并等待
来源：http://qah.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://bjq.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eee.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://bte.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qxu.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jzw.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nmi.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://vra.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://erc.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://jwv.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://hns.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hap.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://shb.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://ydf.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ega.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mqc.yueranfly.top

Ruby: threads.map(&:join)
来源：http://mln.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://qgo.hfpthk.cn

[O06] 使用进程池
来源：http://kym.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oeg.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nit.meibo888.top

JS:   // child_process / cluster 模块
来源：http://pbn.yj20258.top

TS:   // child_process / cluster 模块
来源：http://ysn.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hyk.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zzd.pengpengdd.cyou

Ruby: // fork 块
来源：http://uuf.yvedp.cn

C#:   Parallel.For
来源：http://rgx.wangdashe.top

================================================================================
来源：http://cul.sxryk.cn

P. 常用工具函数
来源：http://lar.yvedp.cn

================================================================================
来源：http://tfh.xuetiantiany.cn

[P01] 生成 UUID
来源：http://mrv.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://mbn.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lum.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://hkf.bjfxy.top

TS:   crypto.randomUUID()
来源：http://xoy.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://xdg.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://ngo.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://fpb.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://ewd.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://sry.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sqy.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fvx.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qzq.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xgs.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wym.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yjb.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iyt.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xns.hammf.cn

[P03] 生成短随机字符串
来源：http://jvd.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqm.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fqh.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bpj.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gnc.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rez.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://odo.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ejz.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ubv.hesvh.cn

[P04] 求长度
来源：http://rxq.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://faz.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fjs.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://var.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pym.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://jhp.ybcxt.top

Go:   len(arr);  len(m)
来源：http://ibe.aibaodan.cn

Ruby: x.length;  x.size
来源：http://scj.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tdt.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://lvm.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://fzz.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bvn.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://orj.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bdx.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yjt.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://sxp.316326.xyz

Ruby: a == b
来源：http://fuo.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hau.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uyk.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uqj.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://flb.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vgx.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://mkz.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ldh.ctjpmb.com

Go:   if x == nil {}
来源：http://aug.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kyk.zhixingplan.top

C#:   if (x is null) {}
来源：http://idc.cheryme.top

[P07] 防抖与节流
来源：http://mxn.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wai.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://onv.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjg.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uzo.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://auc.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hjv.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://egb.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eju.xinyue.icu

[P08] 处理浮点精度问题
来源：http://prh.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rhb.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yed.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qci.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ond.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uyd.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oaj.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jox.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mic.hammf.cn

================================================================================
来源：http://tfo.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pdp.ctjpmb.com

================================================================================
来源：http://ihe.zhongyouzk.top

[Q01] 创建表
来源：http://msu.hammf.cn

CREATE TABLE users (
来源：http://jnv.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://drc.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://mtp.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://jfp.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://htu.chenlongwang.top

);
来源：http://qby.hywenlv.cn

[Q02] 创建带外键的表
来源：http://yfx.yangfankeji.com

CREATE TABLE orders (
来源：http://reh.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lqc.birdmap.top

user_id INT NOT NULL,
来源：http://qfo.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://ian.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ssq.gogol.net.cn

);
来源：http://ztn.yonumen.top

[Q03] 增加列
来源：http://udi.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ntc.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://bvz.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://swl.cashguo.top

[Q05] 重命名列
来源：http://ztj.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rbr.cashguo.top

[Q06] 删除列
来源：http://mgx.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://qnk.zhengqikj.top

[Q07] 删除表
来源：http://otd.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://pbx.meibo888.top

[Q08] 创建普通索引
来源：http://bva.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pfg.tianlin.xyz

[Q09] 创建唯一索引
来源：http://owm.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://avn.hnqzz.top

[Q10] 插入单行
来源：http://emm.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://czs.yj202588.top

[Q11] 一次插入多行
来源：http://qjs.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rrl.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://emd.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://ook.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mxs.shzxlz.cn

[Q13] 忽略重复插入
来源：http://dke.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dkl.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://pvf.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://krj.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aoi.gaohongyu789.top

[Q15] 查询全部
来源：http://ctg.yongpay.top

SELECT * FROM users;
来源：http://jfi.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://mcu.cdnleiting.top

SELECT id, name FROM users;
来源：http://wue.yuxming.cn

[Q17] 条件查询
来源：http://ocx.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://luo.cucudq.cn

[Q18] 模糊匹配
来源：http://vgc.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mjz.yueranfly.top

[Q19] 范围查询
来源：http://glt.yueranfly.top


<!-- 参考信息 -->