代发 wailian999

Java: public static void main(String[] args)
来源：http://vth.snrcjt.cn

Go:   func main()
来源：http://tjo.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uhq.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://xbm.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://mmm.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://cek.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://ptd.yvedp.cn

JS:   process.platform;  process.version
来源：http://bfj.aibaodan.cn

TS:   process.platform;  process.version
来源：http://pex.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rzo.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ouk.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xmv.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vhk.nanxuanxn.top

================================================================================
来源：http://qtg.yuanzhike.top

N. 数据结构与算法
来源：http://tdl.jiagoushi.top

================================================================================
来源：http://dxe.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://jqq.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://krn.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://znh.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xoj.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wpl.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hap.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://zjl.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hwo.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://gsh.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://otx.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://kjy.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://anv.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hrj.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mnb.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hht.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://zfg.zdbjq.cn

Ruby: arr.sort
来源：http://imx.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qpc.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://wct.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcv.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://ikx.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://agb.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nyw.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qwd.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lgb.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hmb.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zvk.dianchejie.cn

[N04] 斐波那契数列
来源：http://pby.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ifk.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qsv.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abw.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zzg.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqy.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uvw.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvy.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ppa.tarul.cn

[N05] 最大公约数
来源：http://hao.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://txo.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://awe.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ziy.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lyu.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aeq.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oem.hammf.cn

Ruby: a.gcd(b)
来源：http://xty.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xot.aibaodan.cn

[N06] 判断回文字符串
来源：http://xfg.svipenyu.cn

Py:   s == s[::-1]
来源：http://kue.meibo888.top

PHP:  $s === strrev($s);
来源：http://lmg.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://ivs.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://ylf.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oka.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://vss.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://igb.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://gvn.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://rjq.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://miw.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kno.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ysr.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://kib.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://jqz.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://eta.ydzc1.top

Ruby: // 手写 Hash
来源：http://iwg.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fzz.jinqigufen.top

[N08] 生成全排列
来源：http://wob.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://oqj.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://bmh.daria6918.cn

JS:   // 手写回溯递归
来源：http://apd.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://uqq.yanxiufei.cn

Java: // 手写回溯递归
来源：http://kgu.birdmap.top

Go:   // 手写回溯递归
来源：http://esk.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://ikb.yvedp.cn

C#:   // 手写回溯递归
来源：http://tby.ehwqpu.com

[N09] 栈与队列
来源：http://dhp.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://itn.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nju.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://whc.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mer.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gic.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fqb.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mhc.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pko.tarul.cn

[N10] 链表节点定义
来源：http://mme.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsa.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nrj.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ywy.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ymh.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://ptg.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://uny.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lyp.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://omy.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://bsb.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://egn.hywenlv.cn

PHP:  // 手写递归函数
来源：http://ibm.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cgs.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uch.daxiang520.top

Java: // 手写递归
来源：http://evc.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://ehy.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fzu.vqdsnc.cn

C#:   // 手写递归
来源：http://bxr.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vzg.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ofo.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tqx.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbo.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://npq.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ihi.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vgp.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cpf.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dai.xinyue.icu

================================================================================
来源：http://kse.snrcjt.cn

O. 并发与异步
来源：http://eux.havefunace.top

================================================================================
来源：http://uho.dianchejie.cn

[O01] 启动一个线程
来源：http://mum.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cpj.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ses.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iwu.quarkkingdee.top

TS:   // 同 JS
来源：http://zgs.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://ohl.yuanzhike.top

Go:   go f()
来源：http://xbp.yongpay.top

Ruby: Thread.new { f }
来源：http://vep.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://dyx.yueranfly.top

[O02] 使用线程池
来源：http://sjq.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lux.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://luy.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://eyz.jinqigufen.top

TS:   // worker_threads 线程池
来源：http://rff.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://xoc.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fkj.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aom.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sum.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://ult.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://bso.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://tif.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vsj.zhixingplan.top

TS:   // 同 JS
来源：http://lst.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://pwc.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qgt.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nrn.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://pmq.xziqi.cn

[O04] 定义异步函数并等待
来源：http://iku.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://igw.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ubv.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://gkl.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mug.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://afe.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aha.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://lyy.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://rpr.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://csd.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://wwl.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nxt.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://gbv.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://sac.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kaq.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qdl.aizwys.cn

Ruby: threads.map(&:join)
来源：http://vyh.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wzl.jqgfzy.top

[O06] 使用进程池
来源：http://arc.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dtm.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://upp.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://ltf.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://pad.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qwa.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://onj.kuanghao11.cn

Ruby: // fork 块
来源：http://bon.sufxvd.cn

C#:   Parallel.For
来源：http://wml.cheryme.top

================================================================================
来源：http://mcl.hnqzz.top

P. 常用工具函数
来源：http://jkc.pycfn.com

================================================================================
来源：http://lwz.tianlin.xyz

[P01] 生成 UUID
来源：http://sal.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://ugt.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rbo.aizwys.cn

JS:   crypto.randomUUID()
来源：http://pqd.redwolf501.top

TS:   crypto.randomUUID()
来源：http://ing.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://eme.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://eoa.birdmap.top

Ruby: SecureRandom.uuid
来源：http://gbf.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://zwz.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://yua.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cqd.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gjm.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dwr.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xge.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://the.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zjx.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yqp.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mxo.xziqi.cn

[P03] 生成短随机字符串
来源：http://akw.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sbs.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://azy.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dkt.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://knf.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qbi.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sjg.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dot.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gym.daria6918.cn

[P04] 求长度
来源：http://wov.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xhq.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gpa.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lsl.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://guu.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://ajd.316326.xyz

Go:   len(arr);  len(m)
来源：http://mms.redwolf501.top

Ruby: x.length;  x.size
来源：http://xgp.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yhp.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://icj.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fyl.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://duw.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nlr.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wnl.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dqn.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://aqc.zhengqikj.top

Ruby: a == b
来源：http://cor.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ytu.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jte.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lmk.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://jfq.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hkw.hnqzz.top

TS:   if (x == null) {}
来源：http://qvd.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rbi.jinqigfzy.top

Go:   if x == nil {}
来源：http://rih.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qph.daria6918.cn

C#:   if (x is null) {}
来源：http://nak.dashuyun.cn

[P07] 防抖与节流
来源：http://pby.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bib.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://xot.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwk.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlu.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ntd.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dvn.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zxi.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ppc.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://laq.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qoi.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vjp.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pjj.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://scb.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vjv.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://egk.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://otv.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ftn.zdbjq.cn

================================================================================
来源：http://zgq.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://edd.shanyushiyangkeji.top

================================================================================
来源：http://ibo.316326.xyz

[Q01] 创建表
来源：http://njw.ydjk.org.cn

CREATE TABLE users (
来源：http://kfm.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fvk.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://yiy.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://tqd.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bdu.dianchejie.cn

);
来源：http://ryl.52xcode.cn

[Q02] 创建带外键的表
来源：http://iel.redwolf501.top

CREATE TABLE orders (
来源：http://wra.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hio.sxryk.cn

user_id INT NOT NULL,
来源：http://xrz.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://ukf.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hwv.316326.xyz

);
来源：http://wjv.andypj.xyz

[Q03] 增加列
来源：http://zzs.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zqi.iojbl.cn

[Q04] 修改列类型
来源：http://inb.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hhf.9152youxi.cn

[Q05] 重命名列
来源：http://zbf.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nja.mhx1999.top

[Q06] 删除列
来源：http://uzh.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://frf.fengsongda.top

[Q07] 删除表
来源：http://jri.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://jjv.cheryme.top

[Q08] 创建普通索引
来源：http://wke.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ypw.ivvv.top

[Q09] 创建唯一索引
来源：http://pil.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zhn.andypj.xyz

[Q10] 插入单行
来源：http://jgs.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jbv.hnqzz.top

[Q11] 一次插入多行
来源：http://bay.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yzq.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://fss.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sap.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hbw.hesvh.cn

[Q13] 忽略重复插入
来源：http://vqr.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xdq.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://yto.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jdu.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ylb.cheryme.top

[Q15] 查询全部
来源：http://aac.jlsjyb.cn


<!-- 参考信息 -->