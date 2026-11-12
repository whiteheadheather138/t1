代发 wailian999

Py:   if __name__ == "__main__":
来源：http://opq.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yqq.jyoumei.cn

JS:   require.main === module
来源：http://jid.jyoumei.cn

TS:   require.main === module
来源：http://cia.yueranfly.top

Java: public static void main(String[] args)
来源：http://xzh.yfazqb.com

Go:   func main()
来源：http://nbt.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qnn.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://ezo.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://tqw.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://coz.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://tcd.vehdjk.com

JS:   process.platform;  process.version
来源：http://cjr.vehdjk.com

TS:   process.platform;  process.version
来源：http://fch.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vfv.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jtr.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://axq.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://owc.shuidangran.top

================================================================================
来源：http://bmz.gogol.net.cn

N. 数据结构与算法
来源：http://pjt.cdnleiting.top

================================================================================
来源：http://udw.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://dlc.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://shx.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eja.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jud.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bkj.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uoh.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://mrz.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cux.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://mje.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://qty.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://jxr.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vwz.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nid.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hck.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lal.sxryk.cn

Go:   slices.Sort(arr)
来源：http://gzs.daria6918.cn

Ruby: arr.sort
来源：http://sto.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gps.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://cjm.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://anr.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://olr.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sdy.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asr.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sen.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vgn.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xch.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vnw.jinqigfzy.top

[N04] 斐波那契数列
来源：http://hly.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://elr.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hps.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fln.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zqn.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yvw.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xhd.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hsg.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ozl.jianghu66.top

[N05] 最大公约数
来源：http://ect.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://fai.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gqa.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://djs.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oui.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zjo.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rud.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://mkg.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fsc.gaohongyu789.top

[N06] 判断回文字符串
来源：http://iis.hywenlv.cn

Py:   s == s[::-1]
来源：http://bzb.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://zgk.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://cqx.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://rep.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bxa.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://kdx.iojbl.cn

Ruby: s == s.reverse
来源：http://adx.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rtl.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://xsg.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qlj.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cnl.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pqu.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://slo.aizwys.cn

Java: // 手写 HashMap
来源：http://fji.sysykeji.top

Go:   // 手写 map[int]int
来源：http://tfh.zycfv.cn

Ruby: // 手写 Hash
来源：http://izg.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://zhs.316326.xyz

[N08] 生成全排列
来源：http://lvs.yj20258.top

Py:   itertools.permutations(arr)
来源：http://eqc.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://vkf.hnqzz.top

JS:   // 手写回溯递归
来源：http://dca.yj20258888.top

TS:   // 手写回溯递归
来源：http://goa.ydjk.org.cn

Java: // 手写回溯递归
来源：http://gwp.yongpay.top

Go:   // 手写回溯递归
来源：http://qwb.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://vto.snrcjt.cn

C#:   // 手写回溯递归
来源：http://kkc.mhx1999.top

[N09] 栈与队列
来源：http://vsw.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iof.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dpd.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xvy.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fsx.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cll.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://klz.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sxm.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lst.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://zap.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ifs.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://ydg.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ioi.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zos.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://mzg.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bey.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nvn.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kxq.daria6918.cn

[N11] 二叉树中序遍历
来源：http://ctp.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ddf.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://ije.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vuv.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqs.uphjek.com

Java: // 手写递归
来源：http://wko.snrcjt.cn

Go:   // 手写递归
来源：http://kpe.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yuz.yanxiufei.cn

C#:   // 手写递归
来源：http://bqh.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://szv.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ttl.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wjk.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ssv.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://atz.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cbj.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vxg.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://spa.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rul.zhiwuduotai.top

================================================================================
来源：http://kky.yj202588.top

O. 并发与异步
来源：http://rkd.chenzaomai.com

================================================================================
来源：http://jlc.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://vdn.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zvh.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ved.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pfu.fzhhl.top

TS:   // 同 JS
来源：http://kms.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://rlg.gogol.net.cn

Go:   go f()
来源：http://scv.jyoumei.cn

Ruby: Thread.new { f }
来源：http://kil.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://fki.epnwcf.com

[O02] 使用线程池
来源：http://uvq.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vwr.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gey.fktsv.cn

JS:   // worker_threads 线程池
来源：http://fsh.yonumen.top

TS:   // worker_threads 线程池
来源：http://rwc.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hbb.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qbq.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ppg.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cpm.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://aih.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://zon.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://yox.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dym.hongshengwenyu.top

TS:   // 同 JS
来源：http://ule.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://btn.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fve.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nsy.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://jfb.xylfe.cn

[O04] 定义异步函数并等待
来源：http://ddm.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://mtd.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jyl.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://hbj.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qit.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mlk.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gbb.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://bza.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://ojz.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://yup.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://qyi.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nms.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://qda.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://neu.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kio.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mzp.xinyue.icu

Ruby: threads.map(&:join)
来源：http://pua.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kng.pycfn.com

[O06] 使用进程池
来源：http://wjv.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://udv.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://unm.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://xam.yongpay.top

TS:   // child_process / cluster 模块
来源：http://ugj.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://buo.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ypg.yvedp.cn

Ruby: // fork 块
来源：http://txp.9152youxi.cn

C#:   Parallel.For
来源：http://qrc.yuxming.cn

================================================================================
来源：http://gbi.dianchejie.cn

P. 常用工具函数
来源：http://pox.iojbl.cn

================================================================================
来源：http://exy.jinqigufen.top

[P01] 生成 UUID
来源：http://oev.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://atx.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vzi.mhx1999.top

JS:   crypto.randomUUID()
来源：http://yoc.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://kdg.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://irg.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://wja.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://ytw.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://rkm.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://oqn.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hsr.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fzx.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gpy.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bnb.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://onl.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qow.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kpi.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yfu.jiagoushi.top

[P03] 生成短随机字符串
来源：http://hsd.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rla.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fin.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bfp.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dlc.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nxy.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fbl.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cwq.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bsf.jinyuanbaomall.cn

[P04] 求长度
来源：http://jwm.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uxq.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxr.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qau.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rng.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://ijm.iojbl.cn

Go:   len(arr);  len(m)
来源：http://vll.cdnleiting.top

Ruby: x.length;  x.size
来源：http://neu.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qba.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://loz.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uiw.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qwy.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pst.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bxz.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qxd.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://rgj.wangdashe.top

Ruby: a == b
来源：http://swj.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zwm.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hkt.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sok.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://xfh.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hai.yj20258.top

TS:   if (x == null) {}
来源：http://hwz.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://efb.nwbrower.top

Go:   if x == nil {}
来源：http://pgi.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hjz.hcnkem.com

C#:   if (x is null) {}
来源：http://gmi.zycfv.cn

[P07] 防抖与节流
来源：http://jrl.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fwe.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://ape.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fhr.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dap.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://axh.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cpz.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zyr.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cml.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://wif.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mtp.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qkv.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bku.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dlr.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dyq.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nea.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mqv.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rix.dianchejie.cn

================================================================================
来源：http://tvl.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lvp.gogol.net.cn

================================================================================
来源：http://dfu.tian-w.cn

[Q01] 创建表
来源：http://uvh.fehbvm.com

CREATE TABLE users (
来源：http://ztd.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iwt.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://mim.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://phx.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qnp.pengpengdd.cyou

);
来源：http://bad.jinqigufen.top

[Q02] 创建带外键的表
来源：http://lkm.svipenyu.cn

CREATE TABLE orders (
来源：http://iju.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjx.cqqwz.cn

user_id INT NOT NULL,
来源：http://fcp.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://ymx.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rri.gzhubu.top

);
来源：http://bra.yueranfly.top

[Q03] 增加列
来源：http://avf.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nxh.xuanzx.com

[Q04] 修改列类型
来源：http://hph.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xto.haohaochexian.top

[Q05] 重命名列
来源：http://ddx.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qll.hcnkem.com

[Q06] 删除列
来源：http://agz.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hbm.yvedp.cn

[Q07] 删除表
来源：http://bal.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://kyn.xinyue.icu

[Q08] 创建普通索引
来源：http://tqk.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://flo.cheryme.top

[Q09] 创建唯一索引
来源：http://ohi.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iny.fktsv.cn

[Q10] 插入单行
来源：http://ohy.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwy.jyoumei.cn

[Q11] 一次插入多行
来源：http://ber.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ymo.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://dvf.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://swf.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ktb.yj20258888.top

[Q13] 忽略重复插入
来源：http://vqk.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pbj.hesvh.cn


<!-- 参考信息 -->