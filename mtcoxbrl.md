代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsu.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://bbx.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://lug.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aae.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://cmd.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://znd.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ile.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pel.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yih.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ovb.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gql.fzhhl.top

Go:   slices.Sort(arr)
来源：http://elf.gogol.net.cn

Ruby: arr.sort
来源：http://dyh.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyi.meibo888.top

[N03] 快速排序（分治示例）
来源：http://xcx.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://icf.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://nrs.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xyu.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eez.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ljv.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tna.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vzv.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://pzm.yuanzhike.top

[N04] 斐波那契数列
来源：http://yzn.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ggq.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xry.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ved.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://avu.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://odx.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qvc.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mbr.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dsg.sjlbkw.cn

[N05] 最大公约数
来源：http://fxj.tian-w.cn

Py:   math.gcd(a, b)
来源：http://cvt.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pjs.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://trc.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://twk.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qwi.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pqo.bbcook.cn

Ruby: a.gcd(b)
来源：http://aul.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iow.zdqjudy.top

[N06] 判断回文字符串
来源：http://uea.uphjek.com

Py:   s == s[::-1]
来源：http://ksy.meibo888.top

PHP:  $s === strrev($s);
来源：http://dyz.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://hch.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://din.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sms.daria6918.cn

Go:   // 双指针从两端比较
来源：http://hdg.ehwqpu.com

Ruby: s == s.reverse
来源：http://woi.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://maa.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://erl.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sut.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iyo.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mjd.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://ltf.xinyue.icu

Java: // 手写 HashMap
来源：http://okd.52xcode.cn

Go:   // 手写 map[int]int
来源：http://ltg.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://tao.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://gzg.andypj.xyz

[N08] 生成全排列
来源：http://nar.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://goo.ehwqpu.com

PHP:  // 手写递归交换
来源：http://pna.havefunace.top

JS:   // 手写回溯递归
来源：http://oyn.svipenyu.cn

TS:   // 手写回溯递归
来源：http://scv.xylfe.cn

Java: // 手写回溯递归
来源：http://nsc.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://pnh.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://jvx.snrcjt.cn

C#:   // 手写回溯递归
来源：http://esp.gzhubu.top

[N09] 栈与队列
来源：http://jjg.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jit.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kdj.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://exa.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ceb.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vaq.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yoe.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://khn.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ngq.dianchejie.cn

[N10] 链表节点定义
来源：http://hja.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wfe.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dgk.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uus.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ykl.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://lsk.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://uqg.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://hdj.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pbi.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://nef.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kxk.yvedp.cn

PHP:  // 手写递归函数
来源：http://ftd.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tri.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fag.chenlongwang.top

Java: // 手写递归
来源：http://pbh.zhijiandao.cn

Go:   // 手写递归
来源：http://hju.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oro.hcnkem.com

C#:   // 手写递归
来源：http://gic.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tjf.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hds.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yez.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcu.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dmv.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://utk.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dhz.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xzx.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kce.ehwqpu.com

================================================================================
来源：http://ndu.hcnkem.com

O. 并发与异步
来源：http://mmt.yuanzhike.top

================================================================================
来源：http://rhi.hesvh.cn

[O01] 启动一个线程
来源：http://ibv.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qbv.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qav.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cqv.hesvh.cn

TS:   // 同 JS
来源：http://edl.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://vcd.sxryk.cn

Go:   go f()
来源：http://yqy.uphjek.com

Ruby: Thread.new { f }
来源：http://qau.bbcook.cn

C#:   Task.Run(() => F());
来源：http://ukx.fktsv.cn

[O02] 使用线程池
来源：http://wgn.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lxj.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xpf.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://kor.ivvv.top

TS:   // worker_threads 线程池
来源：http://lau.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://qbv.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tyu.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://evp.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qdw.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://mod.iojbl.cn

Py:   with lock: shared += 1
来源：http://nfp.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://ned.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dwc.dianchejie.cn

TS:   // 同 JS
来源：http://vzl.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://stl.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uzz.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ttw.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://sse.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://yew.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://drl.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyy.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://uer.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://pfp.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ofo.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kkt.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kva.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://usl.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://upr.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://blk.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bvh.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://nxc.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://szt.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fig.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gzz.aizwys.cn

Ruby: threads.map(&:join)
来源：http://dzh.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dpl.jinqigufen.top

[O06] 使用进程池
来源：http://jka.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://min.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bgg.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://too.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://mpo.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zra.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eqc.chenjidiqi.icu

Ruby: // fork 块
来源：http://tol.hnxiangtu.top

C#:   Parallel.For
来源：http://unc.jinqigfzy.top

================================================================================
来源：http://szs.52xcode.cn

P. 常用工具函数
来源：http://pqm.andypj.xyz

================================================================================
来源：http://dwl.jlsjyb.cn

[P01] 生成 UUID
来源：http://bxc.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://qgp.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://reh.redwolf501.top

JS:   crypto.randomUUID()
来源：http://aun.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://ocz.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://dcp.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://lec.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://pmj.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://gbq.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://lsi.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aiu.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://avf.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://twu.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://koa.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tls.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ixp.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tvv.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wee.dianchejie.cn

[P03] 生成短随机字符串
来源：http://klv.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://las.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://agz.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dwh.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ogu.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wtj.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wkw.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lfw.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kya.52xcode.cn

[P04] 求长度
来源：http://nji.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tzn.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbu.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wdn.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wsz.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://rab.tian-w.cn

Go:   len(arr);  len(m)
来源：http://ijm.xuanzx.com

Ruby: x.length;  x.size
来源：http://obg.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wbn.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://czg.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iyt.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hwg.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nnc.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hzj.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://was.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://kel.daxiang520.top

Ruby: a == b
来源：http://rzs.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://prc.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lzm.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xfr.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://wyp.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bsj.sweek.top

TS:   if (x == null) {}
来源：http://zbe.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://sbb.yanxiufei.cn

Go:   if x == nil {}
来源：http://jpo.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mox.iojbl.cn

C#:   if (x is null) {}
来源：http://gvr.sweek.top

[P07] 防抖与节流
来源：http://uxi.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bbv.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://yvy.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lvh.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndo.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eiz.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tap.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dfp.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://akk.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://jxd.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wha.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jfu.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ize.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://siv.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jkq.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vmf.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qbq.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zot.iojbl.cn

================================================================================
来源：http://ygk.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vkh.jianghu66.top

================================================================================
来源：http://cbt.fengsongda.top

[Q01] 创建表
来源：http://mhk.zhixingplan.top

CREATE TABLE users (
来源：http://myt.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mjh.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://ssp.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://rpd.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghz.zdbjq.cn

);
来源：http://xmr.gzhubu.top

[Q02] 创建带外键的表
来源：http://zca.hongshengwenyu.top

CREATE TABLE orders (
来源：http://kla.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvj.svipenyu.cn

user_id INT NOT NULL,
来源：http://obr.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://iax.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ufq.cucudq.cn

);
来源：http://lfo.chenjidiqi.icu

[Q03] 增加列
来源：http://czw.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jbd.nanxinkj.top

[Q04] 修改列类型
来源：http://pgg.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cdn.haohaochexian.top

[Q05] 重命名列
来源：http://lmj.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qlc.nanxuanxn.top

[Q06] 删除列
来源：http://xch.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://udw.bbcook.cn

[Q07] 删除表
来源：http://jfp.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://yjj.ydzc1.top

[Q08] 创建普通索引
来源：http://dwq.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bda.vehdjk.com

[Q09] 创建唯一索引
来源：http://gmf.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vrw.quarkkingdee.top

[Q10] 插入单行
来源：http://ifm.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vra.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://bod.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gqf.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://ziz.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://pam.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sep.ybcxt.top

[Q13] 忽略重复插入
来源：http://otb.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cmy.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://nje.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lbh.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qvp.daria6918.cn

[Q15] 查询全部
来源：http://nel.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://djk.0kj1m.cn

[Q16] 查询指定列
来源：http://idh.epnwcf.com

SELECT id, name FROM users;
来源：http://mcq.gogol.net.cn

[Q17] 条件查询
来源：http://xgn.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dat.yj20258.top

[Q18] 模糊匹配
来源：http://ckk.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vgr.shzxlz.cn

[Q19] 范围查询
来源：http://quh.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rjz.snrcjt.cn

[Q20] IN 列表
来源：http://lkn.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zgp.yj20258888.top

[Q21] 空值判断
来源：http://xqz.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://psd.yongpay.top

[Q22] 排序
来源：http://bjl.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ydc.vehdjk.com

[Q23] 分页
来源：http://ghi.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ctm.tian-w.cn

[Q24] 去重
来源：http://bqj.316326.xyz

SELECT DISTINCT city FROM users;
来源：http://nry.zhixingplan.top

[Q25] 只取前 N 条
来源：http://msy.chenjidiqi.icu


<!-- 参考信息 -->