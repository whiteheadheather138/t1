代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hqf.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://loh.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://ybc.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xwr.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rne.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://byz.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ecf.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://mur.pengpengdd.cyou

Ruby: arr.sort
来源：http://fpi.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xsb.tarul.cn

[N03] 快速排序（分治示例）
来源：http://kyx.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aml.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://mor.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fnu.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hvw.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zyj.yj20258.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uqn.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kev.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://zuk.birdmap.top

[N04] 斐波那契数列
来源：http://zof.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bxp.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wdx.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oba.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlp.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nqk.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://loj.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kuo.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://evj.9152youxi.cn

[N05] 最大公约数
来源：http://rhn.hammf.cn

Py:   math.gcd(a, b)
来源：http://asa.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tpw.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://slk.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ear.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jcm.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yel.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://ldh.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xya.epnwcf.com

[N06] 判断回文字符串
来源：http://tpa.jqgufenzy.top

Py:   s == s[::-1]
来源：http://pgo.fzhhl.top

PHP:  $s === strrev($s);
来源：http://nbb.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://mdq.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://uor.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://okr.tanke756.top

Go:   // 双指针从两端比较
来源：http://bnx.meibo888.top

Ruby: s == s.reverse
来源：http://cqi.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ckn.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://wpl.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://buy.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dzr.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ail.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://dks.bjfxy.top

Java: // 手写 HashMap
来源：http://wmh.havefunace.top

Go:   // 手写 map[int]int
来源：http://igr.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://tlt.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://uzp.0kj1m.cn

[N08] 生成全排列
来源：http://qan.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://dmr.316326.xyz

PHP:  // 手写递归交换
来源：http://res.iojbl.cn

JS:   // 手写回溯递归
来源：http://lqo.hesvh.cn

TS:   // 手写回溯递归
来源：http://ceh.yj202588.top

Java: // 手写回溯递归
来源：http://lce.sxryk.cn

Go:   // 手写回溯递归
来源：http://rci.yonumen.top

Ruby: arr.permutation.to_a
来源：http://syk.dianchejie.cn

C#:   // 手写回溯递归
来源：http://own.yongpay.top

[N09] 栈与队列
来源：http://dlp.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zcy.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ifd.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://otn.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ogd.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qvj.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://epe.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kig.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ffv.yj20258888.top

[N10] 链表节点定义
来源：http://uda.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://duv.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bhp.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gbk.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wsf.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://uvo.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://dvv.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zra.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xgz.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://iwq.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ozx.fengsongda.top

PHP:  // 手写递归函数
来源：http://bvk.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ynu.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awp.ywan-chungtsiang.top

Java: // 手写递归
来源：http://scl.ivvv.top

Go:   // 手写递归
来源：http://cfb.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wth.hfpthk.cn

C#:   // 手写递归
来源：http://imb.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ahk.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sce.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tii.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://maq.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://szp.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://szk.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nuh.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hoo.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://smz.yangfankeji.com

================================================================================
来源：http://bpa.aibaodan.cn

O. 并发与异步
来源：http://jxw.tanke756.top

================================================================================
来源：http://dbl.fehbvm.com

[O01] 启动一个线程
来源：http://pbx.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://odz.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://prm.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://umd.vqdsnc.cn

TS:   // 同 JS
来源：http://rej.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://kyu.zhijiandao.cn

Go:   go f()
来源：http://woj.yongpay.top

Ruby: Thread.new { f }
来源：http://ale.fzhhl.top

C#:   Task.Run(() => F());
来源：http://nzb.jinqigfzy.top

[O02] 使用线程池
来源：http://qfv.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ced.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sdw.fengsongda.top

JS:   // worker_threads 线程池
来源：http://ihe.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://cgn.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yvp.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sxw.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ztv.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qth.c1oappe.top

[O03] 加锁保护共享数据
来源：http://unb.sweek.top

Py:   with lock: shared += 1
来源：http://ued.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://npd.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://guy.fktsv.cn

TS:   // 同 JS
来源：http://wxn.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://jsl.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cok.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://orj.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://tzv.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://ufn.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://itp.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ygw.pycfn.com

JS:   async function f() { await g(); }
来源：http://dka.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ifo.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aeg.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qla.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://tns.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://naj.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://zrz.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://igl.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://otx.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://ysb.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://qnf.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zhm.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ckp.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://sij.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lev.cdnleiting.top

[O06] 使用进程池
来源：http://kre.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vdt.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xak.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://duc.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://pzk.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://axh.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mcp.jinghuilouyu.cn

Ruby: // fork 块
来源：http://rqx.hammf.cn

C#:   Parallel.For
来源：http://jcw.dashuyun.cn

================================================================================
来源：http://dje.xuetiantiany.cn

P. 常用工具函数
来源：http://gos.epnwcf.com

================================================================================
来源：http://swv.sxryk.cn

[P01] 生成 UUID
来源：http://whz.cheryme.top

Py:   str(uuid.uuid4())
来源：http://srw.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tzt.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://yqm.nwbrower.top

TS:   crypto.randomUUID()
来源：http://wky.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://yyg.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://sng.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://jdm.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://mjj.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://mbf.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ply.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rxz.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cjo.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vru.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ksj.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cjd.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mni.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://awd.fengsongda.top

[P03] 生成短随机字符串
来源：http://hoy.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nis.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gxr.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jxj.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwf.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jvx.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://smv.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://svt.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zbv.hnxiangtu.top

[P04] 求长度
来源：http://ysw.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dxn.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rrq.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kaj.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aal.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://qvl.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://vie.zhixingplan.top

Ruby: x.length;  x.size
来源：http://nqk.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gul.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://psc.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zhv.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xis.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pdn.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://stn.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://umq.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uhm.ybcxt.top

Ruby: a == b
来源：http://fsk.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zoj.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xmo.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qgg.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://ywc.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zbx.hywenlv.cn

TS:   if (x == null) {}
来源：http://rrq.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ppg.hcnkem.com

Go:   if x == nil {}
来源：http://oxm.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xva.guowangkeji.top

C#:   if (x is null) {}
来源：http://npa.zhoulong.xyz

[P07] 防抖与节流
来源：http://gur.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cei.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://dtd.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsf.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqz.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wsl.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tsb.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ugp.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://djz.guannengcc.top

[P08] 处理浮点精度问题
来源：http://kka.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dgr.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uji.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nlk.ydjk.org.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://srx.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://knf.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ywq.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xtu.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ukt.haohaochexian.top

================================================================================
来源：http://hds.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qrx.bbcook.cn

================================================================================
来源：http://esl.xuanzx.com

[Q01] 创建表
来源：http://dja.ehwqpu.com

CREATE TABLE users (
来源：http://yqw.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ufx.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://uwl.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://jyz.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wwm.zdbjq.cn

);
来源：http://zwo.cqqwz.cn

[Q02] 创建带外键的表
来源：http://qao.cheryme.top

CREATE TABLE orders (
来源：http://ysg.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kcq.jyoumei.cn

user_id INT NOT NULL,
来源：http://njq.guannengcc.top

amount DECIMAL(10, 2),
来源：http://uvj.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xxt.redwolf501.top

);
来源：http://lsk.zhoulong.xyz

[Q03] 增加列
来源：http://kxd.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vyz.birdmap.top

[Q04] 修改列类型
来源：http://hvf.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://krn.guannengcc.top

[Q05] 重命名列
来源：http://mje.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bbn.guannengcc.top

[Q06] 删除列
来源：http://pbr.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://xcx.wangdashe.top

[Q07] 删除表
来源：http://meg.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://opn.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://mpt.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cef.0kj1m.cn

[Q09] 创建唯一索引
来源：http://tlz.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ltu.vqdsnc.cn

[Q10] 插入单行
来源：http://tyu.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bsv.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://qhx.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hby.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://jbu.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://tze.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jtb.cqqwz.cn

[Q13] 忽略重复插入
来源：http://orf.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kwm.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://mqa.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oef.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://til.shanyushiyangtech.top

[Q15] 查询全部
来源：http://pyl.aizwys.cn

SELECT * FROM users;
来源：http://zun.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://bfj.zhijiandao.cn

SELECT id, name FROM users;
来源：http://gnn.zhijiandao.cn

[Q17] 条件查询
来源：http://qua.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wbq.yj202588.top

[Q18] 模糊匹配
来源：http://uaq.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wwc.yangfankeji.com

[Q19] 范围查询
来源：http://een.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qvl.gzhubu.top

[Q20] IN 列表
来源：http://wck.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lig.aibaodan.cn

[Q21] 空值判断
来源：http://suf.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://lef.yj202588.top

[Q22] 排序
来源：http://cvt.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gji.xziqi.cn

[Q23] 分页
来源：http://hkj.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fgy.fehbvm.com

[Q24] 去重
来源：http://svj.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://suw.mhx1999.top

[Q25] 只取前 N 条
来源：http://hbg.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://box.dianchejie.cn

[Q26] 计数
来源：http://qnb.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://jog.hnxiangtu.top

[Q27] 条件计数
来源：http://cmc.hfpthk.cn


<!-- 参考信息 -->