代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://qqt.zhongyouzk.top

JS:   console.error("err")
来源：http://jcv.daria6918.cn

TS:   console.error("err")
来源：http://bdc.shzxlz.cn

Java: System.err.println("err")
来源：http://bly.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xxs.yonumen.top

Ruby: warn "err"
来源：http://pes.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://fqc.cucudq.cn

[M07] 判断是否为主入口
来源：http://oot.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://kqa.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vmg.guowangkeji.top

JS:   require.main === module
来源：http://kdd.hfpthk.cn

TS:   require.main === module
来源：http://wqn.sxryk.cn

Java: public static void main(String[] args)
来源：http://ulx.tanke756.top

Go:   func main()
来源：http://gjy.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://soy.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://rir.316326.xyz

[M08] 获取系统与运行时信息
来源：http://mal.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://fbm.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://ycm.haohaochexian.top

JS:   process.platform;  process.version
来源：http://das.tian-w.cn

TS:   process.platform;  process.version
来源：http://pnz.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rbx.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://whm.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bmy.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fqt.fanxiaobao.xyz

================================================================================
来源：http://efm.fanxiaobao.xyz

N. 数据结构与算法
来源：http://bme.ehwqpu.com

================================================================================
来源：http://pxu.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://ucz.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://yzj.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tmu.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dbx.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmz.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://nux.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xta.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sid.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vdn.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://max.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://wbo.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ohx.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jug.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://een.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://phc.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://smh.meibo888.top

Ruby: arr.sort
来源：http://uxv.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pai.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://izw.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nrk.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://ijn.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdb.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkt.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hlz.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gyl.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rgk.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dao.0kj1m.cn

[N04] 斐波那契数列
来源：http://vbf.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fzg.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uxu.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmj.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkj.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mvn.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://njq.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xhj.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vqc.jianghu66.top

[N05] 最大公约数
来源：http://cnw.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://xpi.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://adw.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wra.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://srl.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ubc.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ybo.shuidangran.top

Ruby: a.gcd(b)
来源：http://vre.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://crp.guannengcc.top

[N06] 判断回文字符串
来源：http://eto.aizwys.cn

Py:   s == s[::-1]
来源：http://zme.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://bmu.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://skw.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://gzp.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iav.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://sni.sysykeji.top

Ruby: s == s.reverse
来源：http://rto.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jei.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://mkm.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://toa.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ava.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://smr.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://gbj.quarkkingdee.top

Java: // 手写 HashMap
来源：http://eep.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://nuw.yuxming.cn

Ruby: // 手写 Hash
来源：http://pxx.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jvw.xylfe.cn

[N08] 生成全排列
来源：http://pgr.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://tng.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://pzy.aizwys.cn

JS:   // 手写回溯递归
来源：http://vld.epnwcf.com

TS:   // 手写回溯递归
来源：http://mjl.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://bpf.yuanzhike.top

Go:   // 手写回溯递归
来源：http://zpt.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://vvu.xziqi.cn

C#:   // 手写回溯递归
来源：http://qmc.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://bwk.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ltw.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zri.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ygx.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://shw.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qss.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://twn.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kzf.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://olb.0kj1m.cn

[N10] 链表节点定义
来源：http://uos.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lru.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ykx.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ydz.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://exg.birdmap.top

Java: class Node { int v; Node next; }
来源：http://rue.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://xii.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vkn.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hbn.shuidangran.top

[N11] 二叉树中序遍历
来源：http://zrz.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ase.xuanzx.com

PHP:  // 手写递归函数
来源：http://nmi.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://woh.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mdd.mhx1999.top

Java: // 手写递归
来源：http://xyv.yfazqb.com

Go:   // 手写递归
来源：http://mpq.sxryk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lwc.hesvh.cn

C#:   // 手写递归
来源：http://fff.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xph.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rcb.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fvo.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sxb.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iyt.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ffg.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zhc.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uxw.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wqv.gzhubu.top

================================================================================
来源：http://nth.hnxiangtu.top

O. 并发与异步
来源：http://lwz.mhx1999.top

================================================================================
来源：http://myh.yuanzhike.top

[O01] 启动一个线程
来源：http://hrw.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fiy.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://auc.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://col.hammf.cn

TS:   // 同 JS
来源：http://byh.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://lrp.xuanzx.com

Go:   go f()
来源：http://mcc.yuxming.cn

Ruby: Thread.new { f }
来源：http://yet.andypj.xyz

C#:   Task.Run(() => F());
来源：http://fez.yfazqb.com

[O02] 使用线程池
来源：http://qaq.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rqw.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://plv.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://zfl.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://lcx.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://gfv.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jcm.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://snc.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zga.hesvh.cn

[O03] 加锁保护共享数据
来源：http://ntc.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://zsl.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://mzw.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gfj.zhengqikj.top

TS:   // 同 JS
来源：http://iec.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://kmp.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gxz.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sfo.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://cqm.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://qdp.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://fnt.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kcg.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://rcl.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wjc.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gio.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rcc.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://gby.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://fhn.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://ebn.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://irt.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tmw.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://kfq.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://twn.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vfr.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ldc.tarul.cn

Ruby: threads.map(&:join)
来源：http://fxz.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wjb.yvedp.cn

[O06] 使用进程池
来源：http://czz.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gow.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://gkl.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://fsf.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://crz.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pnq.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hbm.xuetiantiany.cn

Ruby: // fork 块
来源：http://nuw.cqqwz.cn

C#:   Parallel.For
来源：http://rbl.ydjk.org.cn

================================================================================
来源：http://rrr.jiagoushi.top

P. 常用工具函数
来源：http://koz.zycfv.cn

================================================================================
来源：http://zua.sufxvd.cn

[P01] 生成 UUID
来源：http://hpp.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://tue.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hzd.hammf.cn

JS:   crypto.randomUUID()
来源：http://gam.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://rkd.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://wux.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://kwd.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://aiy.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://hsf.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://nzw.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cwp.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dbs.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wlb.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zos.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tbl.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jdx.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jgw.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xpv.yueranfly.top

[P03] 生成短随机字符串
来源：http://wwv.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xzv.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tfz.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vob.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gsv.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lpo.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nfj.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://vbz.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eej.yj20258.top

[P04] 求长度
来源：http://deo.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ogc.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgy.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xlf.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://grz.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://qmt.fzhhl.top

Go:   len(arr);  len(m)
来源：http://ktz.hywenlv.cn

Ruby: x.length;  x.size
来源：http://jbl.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbj.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://irc.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hjj.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sfk.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ugt.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fpd.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://edj.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://nbm.sjlbkw.cn

Ruby: a == b
来源：http://kyw.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ruz.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mzp.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wfh.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://ove.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qzh.dianchejie.cn

TS:   if (x == null) {}
来源：http://xbw.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://jbi.quarkkingdee.top

Go:   if x == nil {}
来源：http://fmp.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iwk.jqgufenzy.top

C#:   if (x is null) {}
来源：http://dkw.zhongyouzk.top

[P07] 防抖与节流
来源：http://vjj.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yjd.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://ywr.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qsb.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ktz.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sue.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xko.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rjd.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lte.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://ngn.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sfg.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tmy.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vfr.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ltu.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uwb.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xsi.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tae.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zbq.bjfxy.top

================================================================================
来源：http://bnw.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dgf.epnwcf.com

================================================================================
来源：http://wje.xylfe.cn

[Q01] 创建表
来源：http://ara.nwbrower.top

CREATE TABLE users (
来源：http://zqi.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rzn.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://pvn.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://loo.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oct.sweek.top

);
来源：http://oez.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://akh.yfazqb.com

CREATE TABLE orders (
来源：http://pyv.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aig.yangfankeji.com

user_id INT NOT NULL,
来源：http://gvt.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://ogc.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://adl.zhiwuduotai.top

);
来源：http://lna.c1oappe.top

[Q03] 增加列
来源：http://hpq.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qjv.birdmap.top

[Q04] 修改列类型
来源：http://cjx.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kai.zhixingplan.top

[Q05] 重命名列
来源：http://udu.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ihv.hnqzz.top

[Q06] 删除列
来源：http://sjw.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gpf.nanxuanxn.top

[Q07] 删除表
来源：http://hcs.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://qdw.tian-w.cn

[Q08] 创建普通索引
来源：http://ecv.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ssk.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://zxp.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pty.cheryme.top

[Q10] 插入单行
来源：http://ypn.vehdjk.com


<!-- 参考信息 -->