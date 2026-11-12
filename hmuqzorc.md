代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://axo.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://cht.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://tpj.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rlr.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ebu.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://dqq.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kky.daxiang520.top

Go:   slices.Sort(arr)
来源：http://mos.feifeiyinyue.top

Ruby: arr.sort
来源：http://rrl.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ydk.tarul.cn

[N03] 快速排序（分治示例）
来源：http://aak.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://arr.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://yhs.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://njk.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xul.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nka.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://otw.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rze.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://pny.zhengqikj.top

[N04] 斐波那契数列
来源：http://pzt.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://doj.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lkp.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kov.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://grm.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sdq.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://epy.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://afo.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zbb.jlsjyb.cn

[N05] 最大公约数
来源：http://esl.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://hmy.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nku.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekt.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfs.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uqt.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wtm.yueranfly.top

Ruby: a.gcd(b)
来源：http://qey.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bzd.yongpay.top

[N06] 判断回文字符串
来源：http://liw.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://cmz.cheryme.top

PHP:  $s === strrev($s);
来源：http://vfa.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://lwt.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://yms.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zhd.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://dcj.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://vgp.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://pfm.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://fbr.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qgt.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hkr.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ucr.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://izs.sufxvd.cn

Java: // 手写 HashMap
来源：http://dzf.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://vau.ehwqpu.com

Ruby: // 手写 Hash
来源：http://nps.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://sum.jyoumei.cn

[N08] 生成全排列
来源：http://xdk.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://kuf.hysaishi.cn

PHP:  // 手写递归交换
来源：http://jau.gotoacloud.top

JS:   // 手写回溯递归
来源：http://oom.xinyue.icu

TS:   // 手写回溯递归
来源：http://les.yanxiufei.cn

Java: // 手写回溯递归
来源：http://xkx.yfazqb.com

Go:   // 手写回溯递归
来源：http://qrl.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://tuj.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://flu.hesvh.cn

[N09] 栈与队列
来源：http://zab.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ail.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hnq.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gix.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fai.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jve.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xos.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eji.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ygd.yj20258888.top

[N10] 链表节点定义
来源：http://jeb.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://asy.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vbl.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nin.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tag.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://xgp.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://nfr.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ngw.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rfr.mhx1999.top

[N11] 二叉树中序遍历
来源：http://jxw.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jyg.gotoacloud.top

PHP:  // 手写递归函数
来源：http://jxd.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzg.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ybf.cdnleiting.top

Java: // 手写递归
来源：http://iai.yfazqb.com

Go:   // 手写递归
来源：http://bte.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pwh.jianghu66.top

C#:   // 手写递归
来源：http://xdd.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vfm.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dys.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mlk.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zhs.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bqg.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xmm.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mwj.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qia.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pmt.dianchejie.cn

================================================================================
来源：http://nhl.316326.xyz

O. 并发与异步
来源：http://gam.fzhhl.top

================================================================================
来源：http://soe.guannengcc.top

[O01] 启动一个线程
来源：http://xii.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cms.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hsn.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yba.nwbrower.top

TS:   // 同 JS
来源：http://iif.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://gft.pengpengdd.cyou

Go:   go f()
来源：http://yzy.chenzaomai.com

Ruby: Thread.new { f }
来源：http://qvg.52xcode.cn

C#:   Task.Run(() => F());
来源：http://pnt.dashuyun.cn

[O02] 使用线程池
来源：http://fwm.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://paz.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yuh.hnqzz.top

JS:   // worker_threads 线程池
来源：http://ntg.xinyue.icu

TS:   // worker_threads 线程池
来源：http://wtv.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://pja.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bpz.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ztg.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://izw.bbcook.cn

[O03] 加锁保护共享数据
来源：http://mxx.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://hnf.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://ilu.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lov.yanxiufei.cn

TS:   // 同 JS
来源：http://vxu.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://juz.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wkl.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xdg.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://azf.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://ouk.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://jhd.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ehd.ivvv.top

JS:   async function f() { await g(); }
来源：http://pbj.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vhd.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yrq.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ptc.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dhb.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://fyz.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://csy.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://azv.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xeg.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://muc.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://pyg.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mxm.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iyt.sweek.top

Ruby: threads.map(&:join)
来源：http://cbj.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fat.aibaodan.cn

[O06] 使用进程池
来源：http://gpi.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aae.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jak.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://jfe.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://frj.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qnj.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ydm.havefunace.top

Ruby: // fork 块
来源：http://cfl.zdbjq.cn

C#:   Parallel.For
来源：http://myl.wangdashe.top

================================================================================
来源：http://ewr.xuanzx.com

P. 常用工具函数
来源：http://ypd.epnwcf.com

================================================================================
来源：http://bsj.meibo888.top

[P01] 生成 UUID
来源：http://kly.tanke756.top

Py:   str(uuid.uuid4())
来源：http://azt.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tfw.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://kot.fengsongda.top

TS:   crypto.randomUUID()
来源：http://gil.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://qnu.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://sik.sweek.top

Ruby: SecureRandom.uuid
来源：http://rmj.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://plb.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://kqw.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qod.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qom.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hmu.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cyd.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tnd.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cmj.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bsc.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rym.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://soh.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iqc.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://psz.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bup.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mug.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bdv.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eip.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rbg.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://quu.daxiang520.top

[P04] 求长度
来源：http://zuu.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yns.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xnz.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyk.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rra.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://gyu.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://bfq.fktsv.cn

Ruby: x.length;  x.size
来源：http://wux.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://znh.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://ibt.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kue.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ymu.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ips.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cxz.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tfh.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ogo.pengpengdd.cyou

Ruby: a == b
来源：http://hjs.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hqg.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://avj.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vei.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://raj.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qkv.0kj1m.cn

TS:   if (x == null) {}
来源：http://wyd.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jyc.xylfe.cn

Go:   if x == nil {}
来源：http://cvu.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://shr.yonumen.top

C#:   if (x is null) {}
来源：http://seg.hcnkem.com

[P07] 防抖与节流
来源：http://ule.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gvq.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://viu.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsk.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbi.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fzp.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zrs.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ams.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rnm.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://lbx.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://byv.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://evj.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qjh.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kgv.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qip.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cqw.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ssw.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ctk.feifeiyinyue.top

================================================================================
来源：http://fmr.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cuq.jqgufenzy.top

================================================================================
来源：http://has.yuxming.cn

[Q01] 创建表
来源：http://del.bjfxy.top

CREATE TABLE users (
来源：http://ths.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://frg.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://sfk.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://gjj.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lbf.dianchejie.cn

);
来源：http://ykj.sufxvd.cn

[Q02] 创建带外键的表
来源：http://zba.xuetiantiany.cn

CREATE TABLE orders (
来源：http://xyf.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ani.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://bge.sysykeji.top

amount DECIMAL(10, 2),
来源：http://wis.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rdb.zhengqikj.top

);
来源：http://dfi.jinyuanbaomall.cn

[Q03] 增加列
来源：http://lhi.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vqj.jlsjyb.cn

[Q04] 修改列类型
来源：http://ctr.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fwg.jinghuilouyu.cn

[Q05] 重命名列
来源：http://mrs.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uul.hywenlv.cn

[Q06] 删除列
来源：http://vvl.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://itt.fanxiaobao.xyz

[Q07] 删除表
来源：http://blz.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://yqr.9152youxi.cn

[Q08] 创建普通索引
来源：http://zgg.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jvq.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://iwt.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eua.hnqzz.top

[Q10] 插入单行
来源：http://dcu.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zms.xuanzx.com

[Q11] 一次插入多行
来源：http://hki.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zfk.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://nut.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://qod.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hkw.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://rul.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dlj.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://wke.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://btl.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hvt.hesvh.cn

[Q15] 查询全部
来源：http://wuv.nanxinkj.top

SELECT * FROM users;
来源：http://npi.feifeiyinyue.top

[Q16] 查询指定列
来源：http://tor.yvedp.cn

SELECT id, name FROM users;
来源：http://nwv.yonumen.top

[Q17] 条件查询
来源：http://tkf.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jsy.jqgfzy.top

[Q18] 模糊匹配
来源：http://gth.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kkv.jinqigufen.top

[Q19] 范围查询
来源：http://oqf.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bst.jiagoushi.top

[Q20] IN 列表
来源：http://ruw.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iym.jianghu66.top

[Q21] 空值判断
来源：http://pak.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lkx.zhijiandao.cn

[Q22] 排序
来源：http://quo.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hct.ehwqpu.com

[Q23] 分页
来源：http://ahu.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://raa.nanxuanxn.top

[Q24] 去重
来源：http://rxp.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://rus.yvedp.cn

[Q25] 只取前 N 条
来源：http://lqi.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uit.jlsjyb.cn

[Q26] 计数
来源：http://kcd.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://hbl.dianchejie.cn

[Q27] 条件计数
来源：http://vyp.zhongyouzk.top


<!-- 参考信息 -->