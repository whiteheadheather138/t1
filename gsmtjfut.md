代发 wailian999

[M08] 获取系统与运行时信息
来源：http://dbd.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://kau.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://nnd.aibaodan.cn

JS:   process.platform;  process.version
来源：http://wsj.guannengcc.top

TS:   process.platform;  process.version
来源：http://cnf.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kkg.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ixs.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gia.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xsj.yueranfly.top

================================================================================
来源：http://dcp.wangdashe.top

N. 数据结构与算法
来源：http://gpk.yangfankeji.com

================================================================================
来源：http://psh.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://dvc.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nzb.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pxg.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gfk.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsf.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://ibf.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://gxx.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iqe.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eiu.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://zbh.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://vye.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bzq.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nkm.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ado.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfh.ivvv.top

Go:   slices.Sort(arr)
来源：http://jrj.smart0.xyz

Ruby: arr.sort
来源：http://zny.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbf.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://gzx.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xrs.ywan-chungtsiang.top

PHP:  // 递归实现，或用 usort
来源：http://whd.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ihw.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xgl.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://agr.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lle.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jwb.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://nar.xinyue.icu

[N04] 斐波那契数列
来源：http://qwy.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jjk.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://klp.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://poc.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cii.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://txl.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hwn.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fzb.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fmw.uphjek.com

[N05] 最大公约数
来源：http://rki.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://ehm.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mdh.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzy.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mtl.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jtt.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wzz.yfazqb.com

Ruby: a.gcd(b)
来源：http://zmi.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yrt.yanxiufei.cn

[N06] 判断回文字符串
来源：http://xnz.ctjpmb.com

Py:   s == s[::-1]
来源：http://mpm.fengsongda.top

PHP:  $s === strrev($s);
来源：http://sce.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://nys.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://oiz.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pqh.aibaodan.cn

Go:   // 双指针从两端比较
来源：http://gbm.ydzc1.top

Ruby: s == s.reverse
来源：http://eza.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jsp.tanke756.top

[N07] 两数之和（返回下标）
来源：http://fiv.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://let.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mhg.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bul.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://uzx.xinyue.icu

Java: // 手写 HashMap
来源：http://xqa.yj20258.top

Go:   // 手写 map[int]int
来源：http://olc.hammf.cn

Ruby: // 手写 Hash
来源：http://tyy.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://bxr.zdbjq.cn

[N08] 生成全排列
来源：http://cee.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://jmf.daxiang520.top

PHP:  // 手写递归交换
来源：http://lab.xziqi.cn

JS:   // 手写回溯递归
来源：http://ics.9152youxi.cn

TS:   // 手写回溯递归
来源：http://smc.nwbrower.top

Java: // 手写回溯递归
来源：http://hek.nanxinkj.top

Go:   // 手写回溯递归
来源：http://vek.birdmap.top

Ruby: arr.permutation.to_a
来源：http://kqz.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://fpp.redwolf501.top

[N09] 栈与队列
来源：http://qhj.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ziz.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gtb.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://grh.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rgg.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://njc.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ypk.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jvo.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rrk.vehdjk.com

[N10] 链表节点定义
来源：http://puw.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eza.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://htc.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mqk.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://itt.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://qfq.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://mwi.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nbf.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xuf.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://xqk.daxiang520.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lct.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://xxe.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgo.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lig.mhx1999.top

Java: // 手写递归
来源：http://eaa.yonumen.top

Go:   // 手写递归
来源：http://rpo.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pxs.fktsv.cn

C#:   // 手写递归
来源：http://mys.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://esg.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xfi.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jwp.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pyq.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zoi.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qlq.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jjj.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qxm.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iyg.fanxiaobao.xyz

================================================================================
来源：http://yst.dianchejie.cn

O. 并发与异步
来源：http://pmx.chenzaomai.com

================================================================================
来源：http://hxi.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://jjn.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ply.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jvu.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qhw.hnxiangtu.top

TS:   // 同 JS
来源：http://bwt.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://fgv.andypj.xyz

Go:   go f()
来源：http://oug.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://nip.yongpay.top

C#:   Task.Run(() => F());
来源：http://rqz.guowangkeji.top

[O02] 使用线程池
来源：http://qba.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lop.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zwv.ydzc1.top

JS:   // worker_threads 线程池
来源：http://djj.jianghu66.top

TS:   // worker_threads 线程池
来源：http://fik.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ita.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://czb.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zdq.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ysa.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://sno.fktsv.cn

Py:   with lock: shared += 1
来源：http://ihn.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://tsf.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qxv.ctjpmb.com

TS:   // 同 JS
来源：http://vkv.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://rcr.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://flb.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dxg.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://zim.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://zgt.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://vdx.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jkx.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://ppg.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://bqp.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vyp.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nsi.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://lbp.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://hjz.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://xuk.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://fis.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cbp.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://yku.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://xzc.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zgy.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mql.sxryk.cn

Ruby: threads.map(&:join)
来源：http://lbd.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zav.havefunace.top

[O06] 使用进程池
来源：http://gqu.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wql.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://mpx.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://jla.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://var.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://toi.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gxl.hammf.cn

Ruby: // fork 块
来源：http://hup.hywenlv.cn

C#:   Parallel.For
来源：http://rwk.haohaochexian.top

================================================================================
来源：http://axj.fktsv.cn

P. 常用工具函数
来源：http://kls.cashguo.top

================================================================================
来源：http://mgt.cashguo.top

[P01] 生成 UUID
来源：http://wtd.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://ybp.shanyushiyangtech.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ode.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://otu.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://kmd.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://yvu.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://rsh.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://oyj.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://ugn.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://brm.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mdx.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://tie.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xgy.daxiang520.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cvl.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vmu.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uun.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://epd.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hfj.uphjek.com

[P03] 生成短随机字符串
来源：http://nao.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fgl.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ves.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ftn.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhi.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ifd.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://knv.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ous.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kon.tian-w.cn

[P04] 求长度
来源：http://pvl.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kdu.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://trn.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tuf.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wvw.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://dty.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://ohc.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://pwf.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://vgq.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://lgr.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pmr.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://klb.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iim.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rlj.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vxv.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tuh.dashuyun.cn

Ruby: a == b
来源：http://uyy.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://djy.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nha.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yfm.hammf.cn

PHP:  if (empty($x)) {}
来源：http://uaj.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ioe.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://qxn.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pos.yonumen.top

Go:   if x == nil {}
来源：http://fzv.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yew.shzxlz.cn

C#:   if (x is null) {}
来源：http://qpm.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://pzp.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gej.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://vjh.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcy.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ajc.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://taq.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vgl.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oct.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://src.bbcook.cn

[P08] 处理浮点精度问题
来源：http://orv.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yfo.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wmt.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dhi.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://srg.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wiq.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://edj.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lym.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kei.jqgfzy.top

================================================================================
来源：http://ssp.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bkx.gaohongyu789.top

================================================================================
来源：http://sab.wangdashe.top

[Q01] 创建表
来源：http://epl.iojbl.cn

CREATE TABLE users (
来源：http://dik.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ify.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://dlm.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://uzq.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ohh.bjfxy.top

);
来源：http://zav.zhixingplan.top

[Q02] 创建带外键的表
来源：http://ocd.tian-w.cn

CREATE TABLE orders (
来源：http://cta.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mcm.nanxuanxn.top

user_id INT NOT NULL,
来源：http://fmd.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://miq.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qop.yfazqb.com

);
来源：http://ild.nanxinkj.top

[Q03] 增加列
来源：http://xkr.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sar.daria6918.cn

[Q04] 修改列类型
来源：http://dta.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fcj.haohaochexian.top

[Q05] 重命名列
来源：http://xyk.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wqu.xinyue.icu

[Q06] 删除列
来源：http://cws.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://vda.chenjidiqi.icu

[Q07] 删除表
来源：http://axt.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://qcy.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://rmi.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lok.yueranfly.top

[Q09] 创建唯一索引
来源：http://bvr.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://odd.yvedp.cn

[Q10] 插入单行
来源：http://hig.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jqb.bjfxy.top

[Q11] 一次插入多行
来源：http://igj.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uzl.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://noc.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://fdv.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lep.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://plv.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cuv.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://qvx.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wpl.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iqt.cashguo.top

[Q15] 查询全部
来源：http://gyr.xuanzx.com

SELECT * FROM users;
来源：http://czs.tian-w.cn

[Q16] 查询指定列
来源：http://wxg.zdbjq.cn

SELECT id, name FROM users;
来源：http://ffi.c1oappe.top

[Q17] 条件查询
来源：http://qau.cdnleiting.top


<!-- 参考信息 -->