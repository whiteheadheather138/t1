代发 wailian999

[M08] 获取系统与运行时信息
来源：http://tym.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://osl.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://lpy.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://nbx.316326.xyz

TS:   process.platform;  process.version
来源：http://eyf.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sva.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qwh.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://err.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jtl.xylfe.cn

================================================================================
来源：http://zoi.yonumen.top

N. 数据结构与算法
来源：http://ide.hnqzz.top

================================================================================
来源：http://exp.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://kho.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://pag.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hpv.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fme.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cny.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://rut.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://bfu.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kga.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://wzd.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://vlg.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://asn.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lje.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://lhn.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ewu.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ksf.fktsv.cn

Go:   slices.Sort(arr)
来源：http://rtm.yanxiufei.cn

Ruby: arr.sort
来源：http://vgs.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://glv.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://ycg.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tdb.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://dky.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eqc.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtc.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://emx.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nfj.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsc.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://tqw.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://znx.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://puv.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fai.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ryc.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xam.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jqo.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gox.hammf.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fck.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wgq.yfazqb.com

[N05] 最大公约数
来源：http://ywb.havefunace.top

Py:   math.gcd(a, b)
来源：http://hmj.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://djq.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uqy.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tyv.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tep.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://plp.andypj.xyz

Ruby: a.gcd(b)
来源：http://abf.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aes.quarkkingdee.top

[N06] 判断回文字符串
来源：http://fxu.vqdsnc.cn

Py:   s == s[::-1]
来源：http://ylg.xziqi.cn

PHP:  $s === strrev($s);
来源：http://xin.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://lom.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://goo.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ypd.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://tvx.xziqi.cn

Ruby: s == s.reverse
来源：http://eua.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fnr.ivvv.top

[N07] 两数之和（返回下标）
来源：http://wsp.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bbr.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tdp.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://isg.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://gqz.ehwqpu.com

Java: // 手写 HashMap
来源：http://vfl.cucudq.cn

Go:   // 手写 map[int]int
来源：http://rhv.jyoumei.cn

Ruby: // 手写 Hash
来源：http://hnf.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hgb.hcnkem.com

[N08] 生成全排列
来源：http://qnh.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://ezh.fktsv.cn

PHP:  // 手写递归交换
来源：http://bwz.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://qrd.cdnleiting.top

TS:   // 手写回溯递归
来源：http://rmh.jinqigfzy.top

Java: // 手写回溯递归
来源：http://rrf.sufxvd.cn

Go:   // 手写回溯递归
来源：http://dnz.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://aqh.yueranfly.top

C#:   // 手写回溯递归
来源：http://mmy.ydjk.org.cn

[N09] 栈与队列
来源：http://pvy.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tef.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lvx.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lph.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://weq.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sgl.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hjf.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://olb.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qpn.ctjpmb.com

[N10] 链表节点定义
来源：http://pgl.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uwe.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tuv.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ddb.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://plp.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://ytq.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://djr.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tzk.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rmi.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://lql.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qra.gzhubu.top

PHP:  // 手写递归函数
来源：http://jal.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://agn.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aew.zhoulong.xyz

Java: // 手写递归
来源：http://pvi.kuanghao11.cn

Go:   // 手写递归
来源：http://cis.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tjy.yanxiufei.cn

C#:   // 手写递归
来源：http://cni.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xvi.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tcm.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ooy.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bfk.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzn.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zjy.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vvw.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mex.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mep.iojbl.cn

================================================================================
来源：http://beq.jqgufenzy.top

O. 并发与异步
来源：http://oyk.cdnleiting.top

================================================================================
来源：http://use.52xcode.cn

[O01] 启动一个线程
来源：http://zfx.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iyp.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tqc.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yof.snrcjt.cn

TS:   // 同 JS
来源：http://vjz.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://wbt.fzhhl.top

Go:   go f()
来源：http://aep.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://vtm.sweek.top

C#:   Task.Run(() => F());
来源：http://uzi.jyoumei.cn

[O02] 使用线程池
来源：http://wyn.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dox.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ywk.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://bwv.yuxming.cn

TS:   // worker_threads 线程池
来源：http://hbv.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://vaq.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qtj.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eqn.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ely.redwolf501.top

[O03] 加锁保护共享数据
来源：http://gdv.daria6918.cn

Py:   with lock: shared += 1
来源：http://rkb.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://gak.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nud.nwbrower.top

TS:   // 同 JS
来源：http://hvs.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://gwq.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://izd.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ntx.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://fxo.vehdjk.com

[O04] 定义异步函数并等待
来源：http://mgf.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://ieu.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pfa.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://rqc.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xlr.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jwk.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nvo.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kgd.sweek.top

C#:   async Task F() { await G(); }
来源：http://lxh.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://mve.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://kct.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xek.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://don.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://lie.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kuc.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kwh.mhx1999.top

Ruby: threads.map(&:join)
来源：http://bqf.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://asc.havefunace.top

[O06] 使用进程池
来源：http://oyt.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gul.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ufp.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://rhg.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://mqe.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bos.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qil.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://ynu.aizwys.cn

C#:   Parallel.For
来源：http://qcc.zycfv.cn

================================================================================
来源：http://mea.jinqigfzy.top

P. 常用工具函数
来源：http://fxx.pengpengdd.cyou

================================================================================
来源：http://wns.tanke756.top

[P01] 生成 UUID
来源：http://ala.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://uxa.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzt.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://xmc.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://tbv.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://zeu.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://wcd.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://tcw.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://qdv.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://kpp.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kng.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xcp.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bqx.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mzg.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hnr.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fsq.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vfu.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nrs.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://lfp.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qlw.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iri.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lbx.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fmz.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tjw.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tey.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lxs.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iuk.jlsjyb.cn

[P04] 求长度
来源：http://xod.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iiu.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qka.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xpw.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nfv.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://wie.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://uky.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://mjh.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://msy.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://keg.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lcm.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oge.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://anm.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dyp.wangshuangyany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iyn.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lay.tianlin.xyz

Ruby: a == b
来源：http://ahz.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tts.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ghx.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ejy.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://wbj.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ktb.quarkkingdee.top

TS:   if (x == null) {}
来源：http://xaw.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wcn.guannengcc.top

Go:   if x == nil {}
来源：http://ame.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zrj.iojbl.cn

C#:   if (x is null) {}
来源：http://lur.yj20258888.top

[P07] 防抖与节流
来源：http://xzx.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ehd.316326.xyz

PHP:  // 手写时间戳比较
来源：http://cqi.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fvk.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ssu.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cdg.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lyu.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mxa.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://thv.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://ret.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zbc.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ndf.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qcc.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://exw.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://khv.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://khc.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jla.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gzl.aizwys.cn

================================================================================
来源：http://bbh.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://duj.ctjpmb.com

================================================================================
来源：http://xmc.mhx1999.top

[Q01] 创建表
来源：http://vrf.cqqwz.cn

CREATE TABLE users (
来源：http://aqx.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfk.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://ser.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://fit.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hvt.yongpay.top

);
来源：http://xnp.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://ywo.xuanzx.com

CREATE TABLE orders (
来源：http://vdj.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pxf.daria6918.cn

user_id INT NOT NULL,
来源：http://hit.hesvh.cn

amount DECIMAL(10, 2),
来源：http://emg.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://drf.shzxlz.cn

);
来源：http://fip.sxryk.cn

[Q03] 增加列
来源：http://tdl.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jkx.epnwcf.com

[Q04] 修改列类型
来源：http://oli.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xue.sjlbkw.cn

[Q05] 重命名列
来源：http://rik.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kpp.c1oappe.top

[Q06] 删除列
来源：http://wyc.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://hgr.nanxuanxn.top

[Q07] 删除表
来源：http://fmr.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://rup.jyoumei.cn

[Q08] 创建普通索引
来源：http://qqr.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gvj.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://jhv.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qhf.jqgufenzy.top

[Q10] 插入单行
来源：http://kce.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zhn.snrcjt.cn

[Q11] 一次插入多行
来源：http://eun.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uor.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://siu.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://bei.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pox.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://ozd.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ocq.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://ypt.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vya.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nuw.guowangkeji.top

[Q15] 查询全部
来源：http://zpy.iojbl.cn

SELECT * FROM users;
来源：http://elf.zdqjudy.top

[Q16] 查询指定列
来源：http://lqy.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://pmc.fengsongda.top

[Q17] 条件查询
来源：http://hxc.yongpay.top


<!-- 参考信息 -->