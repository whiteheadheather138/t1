代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://obf.ydzc1.top

Ruby: warn "err"
来源：http://uil.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://zud.jqgfzy.top

[M07] 判断是否为主入口
来源：http://agt.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://itd.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qyx.wangshuangyany.cn

JS:   require.main === module
来源：http://okw.zhongyouzk.top

TS:   require.main === module
来源：http://mot.nwbrower.top

Java: public static void main(String[] args)
来源：http://fzi.hesvh.cn

Go:   func main()
来源：http://vqy.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qme.ivvv.top

C#:   static void Main(string[] args)
来源：http://byc.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://cyz.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://zxs.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://mje.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://pxx.tian-w.cn

TS:   process.platform;  process.version
来源：http://dfs.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pfe.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://lmj.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sqx.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yid.xingfuxueyuan.xyz

================================================================================
来源：http://dup.cashguo.top

N. 数据结构与算法
来源：http://let.c1oappe.top

================================================================================
来源：http://tgn.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://lga.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yxd.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kon.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tyx.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpo.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://oux.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://avc.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://izn.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://lbv.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://nec.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://xkb.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nro.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zss.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yvs.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mvj.epnwcf.com

Go:   slices.Sort(arr)
来源：http://vsy.nanxuanxn.top

Ruby: arr.sort
来源：http://fpt.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hon.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://ndr.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vin.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://zxy.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://czp.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://htb.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hlb.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xow.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gps.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://pdo.vehdjk.com

[N04] 斐波那契数列
来源：http://efy.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gff.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dri.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://orf.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymw.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://foc.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bqs.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gbx.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbq.cashguo.top

[N05] 最大公约数
来源：http://ttx.xziqi.cn

Py:   math.gcd(a, b)
来源：http://qfn.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lru.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://isr.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://omb.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tcu.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rts.aizwys.cn

Ruby: a.gcd(b)
来源：http://iwc.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wks.uphjek.com

[N06] 判断回文字符串
来源：http://imp.fengsongda.top

Py:   s == s[::-1]
来源：http://jpz.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://ngn.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://zpc.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://fkp.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pdi.yj20258888.top

Go:   // 双指针从两端比较
来源：http://imw.ybcxt.top

Ruby: s == s.reverse
来源：http://iqz.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://eyv.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://bdd.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fwi.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lay.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bke.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://yja.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://hsm.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://cdn.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://mfc.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pfr.jqgufenzy.top

[N08] 生成全排列
来源：http://iwb.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://agq.0kj1m.cn

PHP:  // 手写递归交换
来源：http://fdt.yuxming.cn

JS:   // 手写回溯递归
来源：http://txr.hfpthk.cn

TS:   // 手写回溯递归
来源：http://hra.vehdjk.com

Java: // 手写回溯递归
来源：http://zsq.nanxinkj.top

Go:   // 手写回溯递归
来源：http://mvy.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://fcw.0kj1m.cn

C#:   // 手写回溯递归
来源：http://dgk.tianlin.xyz

[N09] 栈与队列
来源：http://rgg.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://klv.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://etk.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xln.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sdl.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iuu.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uam.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bzv.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bxy.yuanzhike.top

[N10] 链表节点定义
来源：http://gdh.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eht.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://iqf.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wut.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zhs.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://owd.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://evr.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rsm.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wxv.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://ukq.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kzn.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://ybv.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vif.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://enz.pycfn.com

Java: // 手写递归
来源：http://egi.cheryme.top

Go:   // 手写递归
来源：http://lja.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://isl.yueranfly.top

C#:   // 手写递归
来源：http://pto.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mrn.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jmq.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgp.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vdg.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aau.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wux.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://doz.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ytu.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wag.jinqigufen.top

================================================================================
来源：http://mcd.wangdashe.top

O. 并发与异步
来源：http://zgz.c1oappe.top

================================================================================
来源：http://txz.feifeiyinyue.top

[O01] 启动一个线程
来源：http://zvd.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nbp.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qsx.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fmg.jianghu66.top

TS:   // 同 JS
来源：http://ifd.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://qds.aizwys.cn

Go:   go f()
来源：http://acd.tianlin.xyz

Ruby: Thread.new { f }
来源：http://ttl.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://iew.gaohongyu789.top

[O02] 使用线程池
来源：http://rbi.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wxu.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zwt.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://plk.bjfxy.top

TS:   // worker_threads 线程池
来源：http://twx.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://hny.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://avx.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://txr.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xny.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://mxn.uphjek.com

Py:   with lock: shared += 1
来源：http://mqn.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://ggs.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fvh.yfazqb.com

TS:   // 同 JS
来源：http://xmf.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://wtn.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://boi.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://acu.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://tlf.zycfv.cn

[O04] 定义异步函数并等待
来源：http://wxy.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://kut.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aen.tarul.cn

JS:   async function f() { await g(); }
来源：http://clk.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ehs.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://shq.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tam.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rex.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://exo.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://poe.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://txq.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dln.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://myn.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://wxb.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kmq.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tse.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://pui.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ulw.zdqjudy.top

[O06] 使用进程池
来源：http://jpn.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mcw.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eia.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://xhd.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://sia.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gpq.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pgp.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://con.fanxiaobao.xyz

C#:   Parallel.For
来源：http://gjb.yj20258.top

================================================================================
来源：http://dlc.nanxinkj.top

P. 常用工具函数
来源：http://ssu.sysykeji.top

================================================================================
来源：http://axc.fzhhl.top

[P01] 生成 UUID
来源：http://zmr.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://yvy.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://inw.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://swd.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://ntw.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://mwa.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://ent.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://nws.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://off.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://luk.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nes.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kjo.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aaw.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yno.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iua.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uhc.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tyr.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gaz.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://ngo.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://exi.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mbq.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qqg.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdc.yfazqb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jpf.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ava.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hgc.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://diq.vqdsnc.cn

[P04] 求长度
来源：http://ixt.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nxr.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ewh.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ocq.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://phy.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://rvo.bbcook.cn

Go:   len(arr);  len(m)
来源：http://zpe.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://dbm.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://qos.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://iqj.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jdh.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cox.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dkc.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dzv.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uds.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://hgm.ctjpmb.com

Ruby: a == b
来源：http://mrm.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pet.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://npy.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yxp.316326.xyz

PHP:  if (empty($x)) {}
来源：http://nwu.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rxr.nwbrower.top

TS:   if (x == null) {}
来源：http://ibo.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yvb.yj20258888.top

Go:   if x == nil {}
来源：http://zbh.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xfb.xuanzx.com

C#:   if (x is null) {}
来源：http://nia.fktsv.cn

[P07] 防抖与节流
来源：http://ado.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cpz.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://rtq.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykc.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxp.cheryme.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dsg.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gsl.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xli.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fio.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://hjh.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yaq.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dgm.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vcr.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mdi.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dzi.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lro.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sdl.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rin.yonumen.top

================================================================================
来源：http://rnc.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rxv.sjlbkw.cn

================================================================================
来源：http://lrr.jyoumei.cn

[Q01] 创建表
来源：http://zav.wangshuangyany.cn

CREATE TABLE users (
来源：http://slr.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cmc.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://nfu.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://psp.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aus.yj202588.top

);
来源：http://uay.guannengcc.top

[Q02] 创建带外键的表
来源：http://tno.fzhhl.top

CREATE TABLE orders (
来源：http://eur.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://utu.sysykeji.top

user_id INT NOT NULL,
来源：http://ull.yj20258.top

amount DECIMAL(10, 2),
来源：http://iyy.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iqm.pycfn.com

);
来源：http://ncn.yfazqb.com

[Q03] 增加列
来源：http://sco.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://chy.ybcxt.top

[Q04] 修改列类型
来源：http://fgt.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hwn.fktsv.cn

[Q05] 重命名列
来源：http://zbu.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qcq.dashuyun.cn

[Q06] 删除列
来源：http://uen.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qbe.redwolf501.top

[Q07] 删除表
来源：http://erw.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://rko.fzhhl.top

[Q08] 创建普通索引
来源：http://mzj.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fzr.yj20258.top

[Q09] 创建唯一索引
来源：http://wrr.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rgs.havefunace.top

[Q10] 插入单行
来源：http://fsv.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://svb.yj202588.top

[Q11] 一次插入多行
来源：http://ghu.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hud.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://wzm.ywan-chungtsiang.top


<!-- 参考信息 -->