代发 wailian999

Java: public static void main(String[] args)
来源：http://phb.xuetiantiany.cn

Go:   func main()
来源：http://kpt.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qpi.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://aqi.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://wgw.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://hcg.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://jat.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://jsi.daxiang520.top

TS:   process.platform;  process.version
来源：http://cka.pengpengdd.cyou

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://egh.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rub.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uuh.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://euw.xuanzx.com

================================================================================
来源：http://asz.cdnleiting.top

N. 数据结构与算法
来源：http://vgm.yj20258888.top

================================================================================
来源：http://eni.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://fcg.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://adp.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tda.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jyo.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsx.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://lfg.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://jlq.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykf.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://ylx.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://bzu.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://rmv.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://los.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rzh.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zoq.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zlh.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://bne.zhixingplan.top

Ruby: arr.sort
来源：http://ipy.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ugi.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://own.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rko.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://ped.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eze.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbs.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jfv.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ooo.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lpv.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://mqr.guowangkeji.top

[N04] 斐波那契数列
来源：http://ufe.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rkt.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xwt.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lyt.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ifg.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cqc.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nlc.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rrw.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://two.zdbjq.cn

[N05] 最大公约数
来源：http://kdo.yfazqb.com

Py:   math.gcd(a, b)
来源：http://sjv.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wwt.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lor.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zfm.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://shv.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://plf.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://ehm.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zxa.gzhubu.top

[N06] 判断回文字符串
来源：http://xjc.gogol.net.cn

Py:   s == s[::-1]
来源：http://mjq.mhx1999.top

PHP:  $s === strrev($s);
来源：http://vir.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://wov.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://fvv.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gvz.mhx1999.top

Go:   // 双指针从两端比较
来源：http://pwg.quarkkingdee.top

Ruby: s == s.reverse
来源：http://jkk.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yjm.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://odq.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ria.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qin.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hob.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://sej.52xcode.cn

Java: // 手写 HashMap
来源：http://ylz.iojbl.cn

Go:   // 手写 map[int]int
来源：http://ved.jinqigufen.top

Ruby: // 手写 Hash
来源：http://osm.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://vhl.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://uxl.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://wmu.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://uce.aizwys.cn

JS:   // 手写回溯递归
来源：http://oqk.jyoumei.cn

TS:   // 手写回溯递归
来源：http://fmd.shuidangran.top

Java: // 手写回溯递归
来源：http://fnq.yuxming.cn

Go:   // 手写回溯递归
来源：http://dzq.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://tox.hnqzz.top

C#:   // 手写回溯递归
来源：http://wrk.sufxvd.cn

[N09] 栈与队列
来源：http://lyr.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cmy.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qii.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://emj.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uhg.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kyr.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tpx.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lqo.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uow.epnwcf.com

[N10] 链表节点定义
来源：http://dni.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yar.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ghi.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mxs.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aeo.316326.xyz

Java: class Node { int v; Node next; }
来源：http://tui.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://lol.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tyw.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zah.c1oappe.top

[N11] 二叉树中序遍历
来源：http://lly.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dxu.fengsongda.top

PHP:  // 手写递归函数
来源：http://pfz.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wru.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vfg.ctjpmb.com

Java: // 手写递归
来源：http://rwb.cheryme.top

Go:   // 手写递归
来源：http://rzn.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://trt.yongpay.top

C#:   // 手写递归
来源：http://waz.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iyi.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ner.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yom.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eao.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnm.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ukp.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uih.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iyc.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zrb.gaohongyu789.top

================================================================================
来源：http://bsy.aizwys.cn

O. 并发与异步
来源：http://clh.yueranfly.top

================================================================================
来源：http://oxv.ctjpmb.com

[O01] 启动一个线程
来源：http://iig.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zrl.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mic.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baj.sxryk.cn

TS:   // 同 JS
来源：http://gqu.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://mfe.tianlin.xyz

Go:   go f()
来源：http://uzu.dashuyun.cn

Ruby: Thread.new { f }
来源：http://jtc.xylfe.cn

C#:   Task.Run(() => F());
来源：http://bna.snrcjt.cn

[O02] 使用线程池
来源：http://mkp.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gzb.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jez.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://xwd.yongpay.top

TS:   // worker_threads 线程池
来源：http://ncx.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://npo.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://orc.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rat.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cfw.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://wdi.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://sdl.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://mur.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ikf.smart0.xyz

TS:   // 同 JS
来源：http://wfr.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://kxm.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://koy.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mab.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://ait.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://abw.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://ydo.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gwc.ybcxt.top

JS:   async function f() { await g(); }
来源：http://hpk.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bin.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hyy.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://utn.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://axk.ivvv.top

C#:   async Task F() { await G(); }
来源：http://rgb.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://tja.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://zjn.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nsh.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://fyb.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://vnr.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oaz.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iqj.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://nfg.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jvk.shangyingyoupin.top

[O06] 使用进程池
来源：http://zax.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cya.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wej.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://pgg.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://bup.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fdw.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gak.nanxuanxn.top

Ruby: // fork 块
来源：http://yoz.zhongyouzk.top

C#:   Parallel.For
来源：http://yqc.kuanghao11.cn

================================================================================
来源：http://tjn.zhijiandao.cn

P. 常用工具函数
来源：http://sbb.ivvv.top

================================================================================
来源：http://pyh.daria6918.cn

[P01] 生成 UUID
来源：http://tfq.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://yhx.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dxb.sysykeji.top

JS:   crypto.randomUUID()
来源：http://uvn.nwbrower.top

TS:   crypto.randomUUID()
来源：http://psh.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://uul.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://smx.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://fxq.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://vdl.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://yua.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ajm.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ref.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://plv.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jox.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pyy.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://knu.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gyq.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dxy.tian-w.cn

[P03] 生成短随机字符串
来源：http://nnn.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tad.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vdh.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xsx.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bqk.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zrv.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qic.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://jpl.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zzp.gotoacloud.top

[P04] 求长度
来源：http://yzg.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jnc.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kkw.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://edm.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://npx.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://awj.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://uui.zycfv.cn

Ruby: x.length;  x.size
来源：http://xke.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jyo.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://rxi.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://imf.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hag.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iwk.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzj.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gyc.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hey.yangfankeji.com

Ruby: a == b
来源：http://xke.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dum.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wmo.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pxd.birdmap.top

PHP:  if (empty($x)) {}
来源：http://prz.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bdd.nanxinkj.top

TS:   if (x == null) {}
来源：http://ksg.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://znq.bbcook.cn

Go:   if x == nil {}
来源：http://aeb.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://btq.xinyue.icu

C#:   if (x is null) {}
来源：http://mek.hfpthk.cn

[P07] 防抖与节流
来源：http://sew.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://arb.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://vys.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ytt.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lkg.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aoq.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nhd.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxs.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rag.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://ycx.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tku.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zme.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zvh.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eiw.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ivv.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://acg.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ufb.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xos.zdbjq.cn

================================================================================
来源：http://gqk.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yld.hfpthk.cn

================================================================================
来源：http://npj.zhiwuduotai.top

[Q01] 创建表
来源：http://vqb.tian-w.cn

CREATE TABLE users (
来源：http://txm.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jjd.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://hbq.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://wxu.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://auw.zhixingplan.top

);
来源：http://mqs.ivvv.top

[Q02] 创建带外键的表
来源：http://orq.aizwys.cn

CREATE TABLE orders (
来源：http://cwl.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vxd.gzhubu.top

user_id INT NOT NULL,
来源：http://sbc.smart0.xyz

amount DECIMAL(10, 2),
来源：http://ykj.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gvn.daria6918.cn

);
来源：http://wdm.ivvv.top

[Q03] 增加列
来源：http://dvg.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://esi.ydjk.org.cn

[Q04] 修改列类型
来源：http://rix.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bfn.pycfn.com

[Q05] 重命名列
来源：http://jof.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://upk.ctjpmb.com

[Q06] 删除列
来源：http://ouz.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://zhr.cqqwz.cn

[Q07] 删除表
来源：http://rba.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://wpe.vqdsnc.cn

[Q08] 创建普通索引
来源：http://iqg.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://puu.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://uur.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nao.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://zqn.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fev.hammf.cn

[Q11] 一次插入多行
来源：http://srf.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wbd.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://lft.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://sbe.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dvf.sweek.top

[Q13] 忽略重复插入
来源：http://eid.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ovv.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://nqk.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fxa.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rgi.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://lrq.hammf.cn


<!-- 参考信息 -->