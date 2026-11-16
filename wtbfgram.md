代发 wailian999

[N01] 二分查找（有序数组）
来源：http://vwt.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://voi.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aop.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tcg.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksb.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://zkk.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://wuc.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fpf.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://bjt.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://jsy.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pzk.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ecd.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://qmi.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tum.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://atk.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://amx.ydjk.org.cn

Ruby: arr.sort
来源：http://taj.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aac.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://zac.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ebb.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://jub.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ajd.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbf.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xgn.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gtx.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ccs.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cxz.nanxinkj.top

[N04] 斐波那契数列
来源：http://met.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qyi.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vgm.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wmv.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wav.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fsa.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bom.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zxt.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gav.gaohongyu789.top

[N05] 最大公约数
来源：http://hms.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://yuo.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ezn.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bib.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yzh.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xsc.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lpb.uphjek.com

Ruby: a.gcd(b)
来源：http://ydy.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ept.hcnkem.com

[N06] 判断回文字符串
来源：http://xpi.hywenlv.cn

Py:   s == s[::-1]
来源：http://mrw.xinyue.icu

PHP:  $s === strrev($s);
来源：http://ycr.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://col.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://gaq.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hpu.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://sxr.quarkkingdee.top

Ruby: s == s.reverse
来源：http://rhv.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yzd.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://tdm.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cqv.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cna.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://znl.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://epx.chenzaomai.com

Java: // 手写 HashMap
来源：http://wcx.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://lzi.wangdashe.top

Ruby: // 手写 Hash
来源：http://enw.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://aia.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://lka.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://abz.haohaochexian.top

PHP:  // 手写递归交换
来源：http://nom.xinyue.icu

JS:   // 手写回溯递归
来源：http://zos.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://owy.svipenyu.cn

Java: // 手写回溯递归
来源：http://hxy.cheryme.top

Go:   // 手写回溯递归
来源：http://iiu.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://akx.snrcjt.cn

C#:   // 手写回溯递归
来源：http://rcw.hywenlv.cn

[N09] 栈与队列
来源：http://sqo.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ojs.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dab.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cvr.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iyq.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iqo.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ckn.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uji.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kxf.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://wjr.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nfr.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://oks.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://utb.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vpb.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://yjj.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wsw.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gwn.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ikg.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://slq.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wnk.tian-w.cn

PHP:  // 手写递归函数
来源：http://pix.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xto.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://abp.nanxuanxn.top

Java: // 手写递归
来源：http://ekj.zdqjudy.top

Go:   // 手写递归
来源：http://tks.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ahx.zhixingplan.top

C#:   // 手写递归
来源：http://kqh.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rfz.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wzr.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fxt.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://erh.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cse.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fso.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://shf.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jsv.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://abb.316326.xyz

================================================================================
来源：http://yvm.hammf.cn

O. 并发与异步
来源：http://ixf.andypj.xyz

================================================================================
来源：http://xij.jinqigfzy.top

[O01] 启动一个线程
来源：http://dee.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://khu.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aqq.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pwy.jlsjyb.cn

TS:   // 同 JS
来源：http://ofz.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://uuj.pycfn.com

Go:   go f()
来源：http://xkm.0kj1m.cn

Ruby: Thread.new { f }
来源：http://bmx.epnwcf.com

C#:   Task.Run(() => F());
来源：http://vdr.cqqwz.cn

[O02] 使用线程池
来源：http://wgb.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rha.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vcm.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://xfy.ybcxt.top

TS:   // worker_threads 线程池
来源：http://ukb.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://xju.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nql.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jmr.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xeq.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://qeb.nwbrower.top

Py:   with lock: shared += 1
来源：http://ctx.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://pio.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pza.vqdsnc.cn

TS:   // 同 JS
来源：http://tam.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://pnz.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://smi.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jmi.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://euh.yonumen.top

[O04] 定义异步函数并等待
来源：http://nod.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://twz.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wzb.yonumen.top

JS:   async function f() { await g(); }
来源：http://esb.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zne.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bpq.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jbn.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://jvp.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://vyh.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://zqc.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://yci.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ckr.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://qce.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://hxj.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ttw.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mai.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://yqd.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hxk.fehbvm.com

[O06] 使用进程池
来源：http://evs.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qxd.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tcu.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://boa.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://gvf.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tyw.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://obj.gzhubu.top

Ruby: // fork 块
来源：http://lmv.shzxlz.cn

C#:   Parallel.For
来源：http://mzn.316326.xyz

================================================================================
来源：http://but.hesvh.cn

P. 常用工具函数
来源：http://upx.guannengcc.top

================================================================================
来源：http://rea.jyoumei.cn

[P01] 生成 UUID
来源：http://ivp.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://egu.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tyk.fengsongda.top

JS:   crypto.randomUUID()
来源：http://npq.jianghu66.top

TS:   crypto.randomUUID()
来源：http://qdp.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://lpq.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://mws.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://zyb.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://zab.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://khp.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lin.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gsj.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rdw.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tjr.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kcr.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nfg.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gke.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eyj.smart0.xyz

[P03] 生成短随机字符串
来源：http://uds.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kgm.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baf.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dsc.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://apv.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xcn.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gzh.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pzk.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kmh.jinqigufen.top

[P04] 求长度
来源：http://hrw.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://khv.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bqs.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhl.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://syn.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://lze.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://ggv.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://iqr.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zhy.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://tvl.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nik.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kzz.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pze.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://men.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cpj.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://vdz.zhongyouzk.top

Ruby: a == b
来源：http://hvs.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ebt.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ljk.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xvv.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://dfs.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dsf.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://onk.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cpm.chenjidiqi.icu

Go:   if x == nil {}
来源：http://lko.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cwn.nanxuanxn.top

C#:   if (x is null) {}
来源：http://wuj.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://zud.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hfa.meibo888.top

PHP:  // 手写时间戳比较
来源：http://rvs.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxh.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hnm.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kyb.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://olh.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zto.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://otd.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://oea.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://crt.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zid.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://avp.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zkh.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tvh.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wpu.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fmw.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pco.cashguo.top

================================================================================
来源：http://yay.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wvq.jinyuanbaomall.cn

================================================================================
来源：http://vsp.zhixingplan.top

[Q01] 创建表
来源：http://amq.quarkkingdee.top

CREATE TABLE users (
来源：http://dzj.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqf.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://box.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://err.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jrx.havefunace.top

);
来源：http://szf.xziqi.cn

[Q02] 创建带外键的表
来源：http://lot.wangshuangyany.cn

CREATE TABLE orders (
来源：http://hky.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xsj.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://ljz.ybcxt.top

amount DECIMAL(10, 2),
来源：http://doq.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lev.zhongyouzk.top

);
来源：http://bvq.haohaochexian.top

[Q03] 增加列
来源：http://pbz.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://haq.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://hzr.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://brc.jianghu66.top

[Q05] 重命名列
来源：http://ynt.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wef.chenzaomai.com

[Q06] 删除列
来源：http://tzi.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://txb.meibo888.top

[Q07] 删除表
来源：http://ujp.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://qsm.nanxinkj.top

[Q08] 创建普通索引
来源：http://pga.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kyq.xziqi.cn

[Q09] 创建唯一索引
来源：http://yez.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://klo.jlsjyb.cn

[Q10] 插入单行
来源：http://jul.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xck.gzhubu.top

[Q11] 一次插入多行
来源：http://lqk.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pbm.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://xhx.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://zel.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tvf.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://vsm.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qvw.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://bsi.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://smp.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hei.zhixingplan.top

[Q15] 查询全部
来源：http://lhs.kuanghao11.cn

SELECT * FROM users;
来源：http://hdj.cqqwz.cn

[Q16] 查询指定列
来源：http://ytv.zhoulong.xyz

SELECT id, name FROM users;
来源：http://evg.52xcode.cn

[Q17] 条件查询
来源：http://wnb.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xmc.xuetiantiany.cn

[Q18] 模糊匹配
来源：http://kji.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vtp.ehwqpu.com

[Q19] 范围查询
来源：http://noz.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lgm.sjlbkw.cn

[Q20] IN 列表
来源：http://nca.hnqzz.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xdf.fengsongda.top

[Q21] 空值判断
来源：http://iul.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://grc.daxiang520.top

[Q22] 排序
来源：http://env.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://thd.zhaomingkeji.xyz

[Q23] 分页
来源：http://scp.quarkkingdee.top


<!-- 参考信息 -->